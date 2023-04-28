# 目录
[TOC]


# 基础知识
## 新建程序

[官网——手动GCC调试](https://mooseframework.inl.gov/getting_started/installation/manual_installation_gcc.html)


```bash
# 创建程序，取名
cd ~/projects
./moose/scripts/stork.sh 程序名

# 先去GitHub新建同名仓库
# 继续
cd 程序名
git remote add origin https://github.com/xxx/仓库名.git
git commit -m "initial commit"
git push -u origin main

# 自动化保存为MOOSE代码格式
./scripts/install-format-hook.sh

## 提交
git add -A
git commit -a -m "." -- no-verify
git push


```



## 编译测试运行

```bash
# 常用
clear && make -j4 METHOD=dbg && mpiexec -n84 ./phase2eq5-dbg -i problems/1.i  -pc_type svd -snes_type vinewtonssls

# 基础
make -j4 METHOD=dbg
./run_tests -j4

# 并行
mpiexec -n 4 xxx-opt -i xx.i
# 注意，C++使用多线程在输出的时候信息可能会覆盖。比如40个网格4线程输出残差，最后控制台只能看到最后的10个网格的残差。
# opt 模式比 dbg 快近 5 倍

# 调试 + 限制变量值
# break libmesh_handleFPE
gdb --args ./phase2eq4-dbg -i problems/liquid2vapor.i  -pc_type svd -snes_type vinewtonssls


# 不计算，只后处理
# 在输入卡[Problem]块中填入solve = false


```

# 使用技巧

## kernel 编写
变量是谁
变量 = 标量 / 矢量
需要耦合哪些变量、物性、辅助变量

## 输入文件启用禁用块
启用禁用块: `active = [blockname]`，`inactive = [blockname]`


## 重装 MOOSE
[官网——手动GCC调试](https://mooseframework.inl.gov/getting_started/installation/install_moose.html)


```bash
# 克隆 MOOSE 官方仓库
mkdir ~/projects
cd ~/projects
git clone https://github.com/idaholab/moose.git
cd moose
git checkout master

# 编译 PETSc
cd ~/projects/moose
unset PETSC_DIR PETSC_ARCH
./scripts/update_and_rebuild_petsc.sh --prefix=/home/lee/software/petsc
export PETSC_DIR=/home/lee/software/petsc

# 测试 PETCs
cd ./petsc
make PETSC_DIR=/home/lee/projects/moose/scripts/../petsc PETSC_ARCH=arch-moose check

# 编译 libMesh
cd ~/projects/moose
./scripts/update_and_rebuild_libmesh.sh

# 编译、测试 MOOSE(8G时-j4初次编译会死机！每个处理器都要占用2G内存)
cd ~/projects/moose/test
make -j 3
./run_tests -j 3

```

## 限制变量值
[限制变量值](https://mooseframework.inl.gov/source/auxkernels/ConstantBoundsAux.html)

```bash
[Bounds]
  [./u_upper_bound]
    type = ConstantBoundsAux
    variable = bounds_dummy
    bounded_variable = alpha
    bound_type = upper
    bound_value = 1
  [../]
  [./u_lower_bound]
    type = ConstantBoundsAux
    variable = bounds_dummy
    bounded_variable = alpha
    bound_type = lower
    bound_value = 0
  [../]
[]

[AuxVariables]
  [./bounds_dummy]
    order = FIRST
    family = LAGRANGE
  [../]
[]
# 一定要运行时加-snes_type vinewtonssls才能生效
./phase2eq4-dbg -i problems/liquidvapor.i -snes_type vinewtonssls

```

## vscode 配置文件
https://mooseframework.inl.gov/help/development/VSCode.html

应该是ctrl shift p-> settings.json->open user settings (~/.config/Code/User/settings.json)

## moose输出残差
不同kernel的precomputeQpResidual()函数有时候输出的数量不一致,例如最常见的是每次输出4个/2个, 一般2个输出的是正确的值,4个则需要分别两两相加
例如 v2rhoudalphadz 出现两次: -1.43717与1.27698* 35.9669* -0.031291相等
v2alpharhodudz  (-0.0804875出现4次, -0.0804875+ -0.0215666= -0.102054256 才等于0.000960171*35.9669*-2.95515


v2rhoudalphadz  (-1.43717,{})
v2rhoudalphadz__u_v  (1.27698,{})
v2rhoudalphadz__rho_v  (35.9669,{})
v2rhoudalphadz__grad_u_v  (-0.031291,{})
v2rhoudalphadz  (-1.37953,{})
v2rhoudalphadz__u_v  (1.2258,{})
v2rhoudalphadz__rho_v  (35.9659,{})
v2rhoudalphadz__grad_u_v  (-0.031291,{})
v2alphaudrhodpdpdz  (-7.59565e-05,{})
v2alphaudrhodpdpdz  (-2.03525e-05,{})
v2alphaudrhodpdpdz  (-8.50894e-06,{})
v2alphaudrhodpdpdz  (-3.17558e-05,{})
v2alpharhodudz  (-0.0804875,{})
v2alpharhodudz__alpha  (0.000960171,{})
v2alpharhodudz__rho_v  (35.9669,{})
v2alpharhodudz__grad_u_v  (-2.95515,{})
v2alpharhodudz  (-0.0215666,{})
v2alpharhodudz__alpha  (0.000960171,{})
v2alpharhodudz__rho_v  (35.9669,{})
v2alpharhodudz__grad_u_v  (-2.95515,{})
v2alpharhodudz  (-0.00939288,{})
v2alpharhodudz__alpha  (0.000418194,{})
v2alpharhodudz__rho_v  (35.9659,{})
v2alpharhodudz__grad_u_v  (-2.95515,{})
v2alpharhodudz  (-0.0350547,{})
v2alpharhodudz__alpha  (0.000418194,{})
v2alpharhodudz__rho_v  (35.9659,{})
v2alpharhodudz__grad_u_v  (-2.95515,{})

## 自定义后处理的先后顺序
(没用过)参数 execution_order_group

https://mooseframework.inl.gov/moose/syntax/UserObjects/index.html

# 未整理
## 矢量速度
  ADReal j_g = (1 - alpha_g) * _u[_qp] * ADRealVectorValue(1, 0, 0);

### min,`max`函数不匹配
min(170 * (Re / Re), -Re / 6e4)

### ADReal就是（double，偏导）
```cpp
typedef double libMesh::Real
typedef DualNumber<Real, DNDerivativeType, /*allow_skiping_derivatives=*/true> DualReal;
typedef DualReal ADReal;

```

