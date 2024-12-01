# 目录

[TOC]


# 自学计算机科学
[TeachYourselfCS](https://teachyourselfcs.com)

* 你应当学习 **哪些科目**，为什么？
* 对于这些科目，**最好的书籍或者视频课程** 是什么？

## 简而言之

大致按照列出的顺序，借助我们所建议的教材或者视频课程（但是最好二者兼用），学习如下的九门科目。目标是先花 100 到 200 个小时学习完每一个科目，然后在你职业生涯中，不时温习其中的精髓🚀。

| 科目 | 为何要学？ | 最佳书籍 | 最佳视频 |
|-|-|-|-|
| [编程](#编程) | 不要做一个「永远没彻底搞懂」诸如递归等概念的程序员。 | [《计算机程序的构造和解释》](https://book.douban.com/subject/1148282/) | Brian Harvey’s Berkeley CS 61A |
| [计算机系统结构](#计算机系统结构) | 如果你对于计算机如何工作没有具体的概念，那么你所做出的所有高级抽象都是空中楼阁。 | [《深入理解计算机系统》](https://book.douban.com/subject/26912767/) | Berkeley CS 61C |
| [算法与数据结构](#算法和数据结构) | 如果你不懂得如何使用栈、队列、树、图等常见数据结构，遇到有难度的问题时，你将束手无策。 | [《算法设计手册》](https://book.douban.com/subject/4048566/) | Steven Skiena’s lectures |
| [数学知识](#数学知识) | 计算机科学基本上是应用数学的一个「跑偏的」分支，因此学习数学将会给你带来竞争优势。 | [《计算机科学中的数学》](https://book.douban.com/subject/33396340/) | Tom Leighton’s MIT 6.042J |
| [操作系统](#操作系统) | 你所写的代码，基本上都由操作系统来运行，因此你应当了解其运作的原理。 | [《操作系统导论》](https://book.douban.com/subject/33463930/) | Berkeley CS 162 |
| [计算机网络](#计算机网络) | 互联网已然势不可挡：理解工作原理才能解锁全部潜力。 | [《计算机网络：自顶向下方法》](https://book.douban.com/subject/30280001/) | Stanford CS 144 |
| [数据库](#数据库) | 对于多数重要程序，数据是其核心，然而很少人理解数据库系统的工作原理。 | *[Readings in Database Systems](https://book.douban.com/subject/2256069/)* （暂无中译本） | Joe Hellerstein’s Berkeley CS 186 |
| [编程语言与编译器](#编程语言与编译器) | 若你懂得编程语言和编译器如何工作，你就能写出更好的代码，更轻松地学习新的编程语言。 | *[Crafting Interpreters](https://craftinginterpreters.com/)* | Alex Aiken’s course on Lagunita   |
| [分布式系统](#分布式系统) | 如今，**多数** 系统都是分布式的。 | [《数据密集型应用系统设计》](https://book.douban.com/subject/30329536/) | MIT 6.824 |

## 还是太多？

如果花几年时间自学 9 门科目让人望而却步，我们建议你只专注于两本书：**《深入理解计算机系统》** 和 **《数据密集型应用系统设计》**。根据我们的经验，投入到这两本书的时间可以获得极高的回报率，特别适合从事网络应用开发的自学工程师。这两本书也可以作为上面表格中其他科目的纲领。

## 为什么要学习计算机科学？

软件工程师分为两种：一种充分理解了计算机科学，从而有能力应对充满挑战的创造性工作；另一种仅仅凭着对一些高级工具的熟悉而勉强应付。

这两种人都自称软件工程师，都能在职业生涯早期挣到差不多的工资。然而，随着时间流逝，第一种工程师不断成长，所做的事情将会越来越有意义且更为高薪，不论是有价值的商业工作、突破性的开源项目、技术上的领导力或者高质量的个人贡献。

> 全球短信系统每日收发约 200 亿条信息，而仅仅靠 57 名工程师，现在的 WhatsApp 每日收发 420 亿条。
>
> — Benedict Evans (@BenedictEvans) [2016 年 2 月 2 日](https://twitter.com/BenedictEvans/status/694342874729545729)

第一种工程师总是寻求深入学习计算机科学的方法，或是通过传统的方法学习，或是在职业生涯中永无止息地学习；第二种工程师
通常浮于表面，只学习某些特定的工具和技术，而不研究其底层的基本原理，仅仅在技术潮流的风向改变时学习新的技能。

如今，涌入计算机行业的人数激增，然而计算机专业的毕业生数量基本上未曾改变。第二种工程师的供过于求正在开始减少他们的工作机会，使他们无法涉足行业内更加有意义的工作。对你而言，不论正在努力成为第一种工程师，还是只想让自己的职业生涯更加安全，学习计算机科学是唯一可靠的途径。

> 23333 然而他们……[pic.twitter.com/XVNYlXAHar](https://web.archive.org/web/20170528095858/https://twitter.com/jenna/status/838161631662092289)
>
> — Jenna Bilotta (@jenna) [2017 年 3 月 4 日](https://web.archive.org/web/20170528095858/https://twitter.com/jenna/status/838161631662092289)

## 分科目指引

### 编程

大多数计算机专业本科教学以程序设计「导论」作为开始。这类课程的最佳版本不仅能满足初学者的需要，还适用于那些在初学编程阶段遗漏了某些有益的概念和程序设计模式的人。

对于这部分内容，我们的标准推荐是这部经典著作：[《计算机程序的构造和解释》](https://book.douban.com/subject/1148282/)。在网络上，这本书既可供 [免费阅读（英文版）](https://mitpress.mit.edu/sites/default/files/sicp/full-text/book/book.html)，也作为 [MIT 的免费视频课程](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-001-structure-and-interpretation-of-computer-programs-spring-2005/video-lectures/)。不过尽管这些视频课程很不错，我们对于视频课程的推荐实际上是 [Brian Harvey 开设的 SICP 课程](https://archive.org/details/ucberkeley-webcast-PL3E89002AA9B9879E?sort=titleSorter)（即 Berkeley 的 61A 课程）。比起 MIT 的课程，它更加完善，更适用于初学者。

我们建议至少学完 SICP 的前三章，并完成配套的习题。如果需要额外的练习，可以去解决一些小的程序设计问题，比如 [exercism](http://exercism.io)。

> **中文翻译新增：**
>
> * 关于 SICP 国内视频观看地址
>   * [MIT 的免费视频课程（中英字幕）](https://www.bilibili.com/video/av8515129/)
>   * [Brian Harvey 开设的 SICP 课程（英文字幕）](https://www.bilibili.com/video/av40460492/)
> * Scheme 学习的相关资源参见：<https://github.com/DeathKing/Learning-SICP>
> * 更详细的补充说明：[#3](https://github.com/izackwu/TeachYourselfCS-CN/issues/3)

自从 2016 年首次发布这份指南以来，最常被问到的一个问题是，我们是否推荐由 John DeNero 讲授的更新的 CS 61A 课程，以及配套的书籍 [*Composing Programs*](https://composingprograms.com/)，这本书「继承自 SICP」 但使用 Python 讲解。我们认为 DeNero 的课程也很不错，有的学生可能更喜欢，但我们还是建议把 SICP、Scheme 和 Brian Harvey 的视频课程作为首选。

为什么这么说呢？因为 SICP 是独一无二的，它可以——至少很有可能——改变你对计算机和编程的基本认识。不是每个人都有这样的体验。有的人讨厌这本书，有的人看了前几页就放弃了。但潜在的回报让它值得一读。

如果你觉得 SICP 过于难，试试 *Composing Programs*。如果还是不合适，那我们推荐 《程序设计方法》（[中文版](https://book.douban.com/subject/1140942/)，[英文版](http://www.htdp.org/)） ；如果你觉得 SICP 过于简单，那我们推荐 [*Concepts, Techniques, and Models of Computer Programming*](https://book.douban.com/subject/1782316/)。如果读这些书让你觉得没有收获，也许你应该先学习其他科目，一两年后再重新审视编程的理念。

> 新版原文删除了对 *Concepts, Techniques, and Models of Computer Programming* 一书的推荐，但这本书对各种编程模型有深入的见解，值得一读。所以译文中依然保留。
> — 译者注

最后，有一点要说明的是：本指南 **不适用** 于完全不懂编程的新手。我们假定你是一个没有计算机专业背景的程序员，希望填补一些知识空白。事实上，我们把「编程」章节包括进来只是提醒你还有更多知识需要学习。对于那些从来没有学过编程，但又想学的人来说，这份 [指南](https://www.reddit.com/r/learnprogramming/wiki/faq#wiki_getting_started) 更合适。

[![计算机程序的构造和解释](https://user-images.githubusercontent.com/20233656/66758473-ef7bff80-eed0-11e9-944a-15ae5c8542ca.jpg)](https://book.douban.com/subject/1148282/)

### 计算机系统结构

计算机系统结构——有时候又被称为「计算机系统」或者「计算机组成」——是了解软件底层的的重要视角。根据我们的经验，这是自学的软件工程师最容易忽视的领域。

我们最喜欢的入门书是 [《深入理解计算机系统》](https://book.douban.com/subject/26912767/)。典型的 [计算机体系结构导论课程](http://csapp.cs.cmu.edu/3e/courses.html) 会涵盖本书的 1-6 章。

我们喜爱《深入理解计算机系统》，因为它的实用性，并且站在程序员的视角。虽然计算机体系结构的内容比本书所涉及的内容多得多，但对于那些想了解计算机系统以求编写更快、更高效、更可靠的软件的人来说，这本书是很好的起点。

对于那些既想了解这个主题又想兼顾硬件和软件的知识的人来说，我们推荐 [《计算机系统要素》](https://book.douban.com/subject/1998341/)，又名「从与非门到俄罗斯方块」（Nand2Tetris），这本书规模宏大，让读者对计算机内的所有部分如何协同工作有完全的认识。这本书的每一章节对应如何构建计算机整体系统中的一小部分，从用 HDL（硬件描述语言）写基本的逻辑门电路出发，途经 CPU 和汇编，最终抵达诸如俄罗斯方块这般规模的应用程序。

我们推荐把此书的前六章读完，并完成对应的项目练习。这么做，你将更加深入地理解，计算机体系结构和运行其上的软件之间的关系。

这本书的前半部分（包括所有对应的项目）均可从 [Nand2Tetris 的网站上](http://www.nand2tetris.org) 免费获得。同时，在 Coursera 上，这是一门 [视频课程](https://www.coursera.org/learn/build-a-computer)。

为了追求简洁和紧凑，这本书牺牲了内容上的深度。尤其值得注意的是，流水线和存储层次结构是现代计算机体系结构中极其重要的两个概念，然而这本书对此几乎毫无涉及。

当你掌握了 Nand2Tetris 的内容后，我们推荐要么回到《深入理解计算机系统》，或者考虑 Patterson 和 Hennessy 二人所著的 [《计算机组成与设计》](https://book.douban.com/subject/26604008/)，一本优秀的经典著作。这本书中的不同章节重要程度不一，因此我们建议根据 Berkeley 的 [CS61C 课程](http://inst.eecs.berkeley.edu/~cs61c/sp15/) 「计算机体系结构中的伟大思想」来着重阅读一些章节。这门课的笔记和实验在网络上可以免费获得，并且在 [互联网档案](https://archive.org/details/ucberkeley-webcast-PL-XXv-cvA_iCl2-D-FS5mk0jFF6cYSJs_) 中有这门课程的过往资料。

[![深入理解计算机系统](https://user-images.githubusercontent.com/20510068/82109944-12270d00-976d-11ea-85a9-774e4f762ec9.png)](https://book.douban.com/subject/26912767/) [![计算机系统要素](https://user-images.githubusercontent.com/20233656/66758695-60231c00-eed1-11e9-8422-a4acfb10a390.jpg)](http://www.nand2tetris.org)

> 硬件是平台。
>
> — Mike Acton, Engine Director at Insomniac Games
> （[观看他在 CppCon 上的演说](https://www.youtube.com/watch?v=rX0ItVEVjHc)）

### 算法与数据结构

正如几十年来的共识，我们认为，计算机科学教育所赋予人们的最大能量在于对常见算法和数据结构的熟悉。此外，这也可以训练一个人对于各种问题的解决能力，有助于其他领域的学习。

关于算法与数据结构，有成百上千的书可供使用，但是我们的最爱是 Steven Skiena 编写的 [《算法设计手册》](https://book.douban.com/subject/4048566/) 。显而易见，他对此充满热爱，迫不及待地想要帮助其他人理解。在我们看来，这本书给人一种焕然一新的体验，完全不同于那些更加经常被推荐的书（比如 Cormen、Leiserson、Rivest、Stein 或 Sedgewick 的书，后两者充斥着过多的证明，不适合以 **解决问题** 为导向的学习）。

如果你更喜欢视频课程，[Skiena 慷慨地提供了他的课程](https://www.youtube.com/watch?v=A2bFN3MyNDA&list=PLOtl7M3yp-DX32N0fVIyvn7ipWKNGmwpp)。此外，Tim Roughgarden 的课程也很不错，
在 Stanford 的 MOOC 平台 Lagunita，或者 [Coursera](https://www.coursera.org/specializations/algorithms) 上均可获得。Skiena 和 Roughgarden 的这两门课程没有优劣之分，选择何者取决于个人品味。

至于练习，我们推荐学生在 [Leetcode](https://leetcode.com) 上解决问题。Leetcode 上的问题往往有趣且带有良好的解法和讨论。此外，在竞争日益激烈的软件行业，这些问题可以帮助你评估自己应对技术面试中常见问题的能力。我们建议解决大约 100 道随机挑选的 Leetcode 问题，作为学习的一部分。

最后，我们强烈推荐 [《怎样解题》](https://book.douban.com/subject/2124114/)。这本书极为优秀且独特，指导人们解决广义上的问题，因而一如其适用于数学，它适用于计算机科学。

[![算法设计手册](https://user-images.githubusercontent.com/20233656/66759121-361e2980-eed2-11e9-913c-8fc48c67122a.jpg)](https://book.douban.com/subject/4048566/) [![怎样解题](https://user-images.githubusercontent.com/20233656/66759282-8e552b80-eed2-11e9-89de-16b1f8d82e78.jpg)](https://book.douban.com/subject/2124114/)

> 我可以广泛推荐的方法只有一个： 写之前先思考。
>
>— Richard Hamming

### 数学知识

从某个角度说，计算机科学是应用数学的一个「发育过度」的分支。尽管许多软件工程师试图——并且在不同程度上成功做到——忽视这一点，我们鼓励你用学习来拥抱数学。如若成功，比起那些没有掌握数学的人，你将获得巨大的竞争优势。

对于计算机科学，数学中最相关的领域是「离散数学」，其中的「离散」与「连续」相对立，大致上指的是应用数学中那些有趣的主题，而不是微积分之类的。由于定义比较含糊，试图掌握离散数学的全部内容是没有意义的。较为现实的学习目标是，了解逻辑、排列组合、概率论、集合论、图论以及密码学相关的一些数论知识。考虑到线性代数在计算机图形学和机器学习中的重要性，该领域同样值得学习。

学习离散数学，我们建议从 [László Lovász 的课程笔记](http://www.cs.elte.hu/~lovasz/dmbook.ps) 开始。Lovász 教授成功地让这些内容浅显易懂且符合直觉，因此，比起正式的教材，这更适合初学者。

对于更加高阶的学习，我们推荐 [《计算机科学中的数学》](https://book.douban.com/subject/33396340/)，MIT 同名课程的课程笔记，篇幅与书籍相当（事实上，现已出版）。这门课程的视频同样 [可免费获得](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-042j-mathematics-for-computer-science-fall-2010/video-lectures/)，是我们所推荐的学习视频。

对于线性代数，我们建议从 [Essence of linear algebra](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab) 系列视频开始，然后再去学习 Gilbert Strang 的 [《线性代数导论》](https://book.douban.com/subject/34820335/) 和 [视频课程](https://ocw.mit.edu/courses/mathematics/18-06-linear-algebra-spring-2010/video-lectures/)。

[![计算机科学中的数学](https://user-images.githubusercontent.com/20233656/66759673-4387e380-eed3-11e9-8469-3e677d108e91.jpg)](https://book.douban.com/subject/33396340/)

> 如果人们不相信数学是简单的，那么只能是因为他们没有意识到生活有多么复杂。
>
>— John von Neumann

### 操作系统

[《操作系统概念》](https://book.douban.com/subject/30297919/)（「恐龙书」）和 [《现代操作系统》](https://book.douban.com/subject/27096665/) 是操作系统领域的经典书籍。二者都因为写作风格和对学生不友好而招致了一些批评。

[《操作系统导论》（*Operating Systems: Three Easy Pieces*）](https://book.douban.com/subject/33463930/) 是一个不错的替代品，并且 [可在网上免费获得（英文版）](http://pages.cs.wisc.edu/~remzi/OSTEP/)。我们格外喜欢这本书的结构，并且认为这本书的习题很值得一做。

在读完《操作系统导论》后，我们鼓励你探索特定操作系统的设计。可以借助「{OS name} Internals」风格的书籍，比如 [*Lion's commentary on Unix*](https://www.amazon.com/Lions-Commentary-Unix-John/dp/1573980137/)， [*The Design and Implementation of the FreeBSD Operating System*](https://www.amazon.com/Design-Implementation-FreeBSD-Operating-System/dp/0321968972/)，以及 [*Mac OS X Internals*](https://www.amazon.com/Mac-OS-Internals-Systems-Approach/dp/0321278542/)。对于 Linux ，我们推荐 Robert Love 的 [《Linux 内核设计与实现》](https://book.douban.com/subject/6097773/)。

为了巩固对操作系统的理解，阅读小型系统内核的代码并且为其增加特性是一个很不错的方法。比如，[xv6](https://pdos.csail.mit.edu/6.828/2016/xv6.html)，由 MIT 的一门课程所维护的从 Unix V6 到 ANSI C 和 x86 的移植，就是一个很棒的选择。《操作系统导论》有一个附录，记载了一些可能的 [xv6 实验项目](http://pages.cs.wisc.edu/~remzi/OSTEP/lab-projects-xv6.pdf)，其中充满了关于潜在项目的很棒想法。

[![操作系统导论](https://user-images.githubusercontent.com/20233656/66759780-78943600-eed3-11e9-8eb5-6472c318c265.jpg)](https://book.douban.com/subject/33463930/)

### 计算机网络

鉴于有那么多关于网络服务端和客户端的软件工程，计算机网络是计算机科学中价值最为「立竿见影」的领域之一。我们的学生，系统性地学习了计算机网络，最终能够理解那些曾困扰他们多年的术语、概念和协议。

在这一主题上，我们最爱的书籍是 [《计算机网络：自顶向下方法》](https://book.douban.com/subject/30280001/)。书中的小项目和习题相当值得练习，尤其是其中的「Wireshark labs」（[这部分在网上可以获得](http://www-net.cs.umass.edu/wireshark-labs/)）。

如果更喜欢视频课程，我们推荐 Stanford 的 [*Introduction to Computer Networking*](https://lagunita.stanford.edu/courses/Engineering/Networking-SP/SelfPaced/about)，可在他们的 MOOC 平台 Lagunita 上免费观看。

对于计算机网络的学习，做项目比完成小的习题更有益。一些可能的项目有：HTTP 服务器，基于 UDP 的聊天 APP，[迷你 TCP 栈](http://jvns.ca/blog/2014/08/12/what-happens-if-you-write-a-tcp-stack-in-python/)，代理，负载均衡器，或者分布式哈希表。

[![《计算机网络：自顶向下方法》](https://user-images.githubusercontent.com/20233656/66760004-d9bc0980-eed3-11e9-9b3f-74bf54b9571f.jpg)](https://book.douban.com/subject/30280001/)

> 你无法盯着水晶球预见未来，未来的互联网何去何从取决于社会。
>
>— Bob Kahn

### 数据库

比起其他主题，自学数据库系统需要更多的付出。这是一个相对年轻的研究领域，并且出于很强的商业动机，研究者把想法藏在紧闭的门后。此外，许多原本有潜力写出优秀教材的作者反而选择了加入或创立公司。

鉴于如上情况，我们鼓励自学者大体上抛弃教材，而是从 [2015 年春季学期的 CS 186 课程](https://archive.org/details/UCBerkeley_Course_Computer_Science_186)（Joe Hellerstein 在 Berkeley 的数据库课程）开始，然后前往阅读论文。

对于初学者，有一篇格外值得提及的论文：[*Architecture of a Database System*](http://db.cs.berkeley.edu/papers/fntdb07-architecture.pdf)。这篇论文提供了独特的对关系型数据库管理系统（RDBMS）如何工作的高层次观点，是后续学习的实用梗概。

[*Readings in Database Systems*](https://book.douban.com/subject/2256069/)，或者以 [数据库「红书」](http://www.redbook.io/) 更为人知，是由 Peter Bailis、Joe Hellerstein 和 Michael Stonebraker 编纂的论文合集。对于那些想要在 CS 186 课程的水平更进一步的学习者，「红书」应当是下一步。

如果你坚持一定要一本导论教材，那我们推荐 Ramakrishnan 和 Gehrke 所著的 [《数据库管理系统：原理与设计》](https://book.douban.com/subject/1155934/)。如需更深一步，Jim Gray 的经典著作 [*Transaction Processing: Concepts and Techniques*](https://book.douban.com/subject/2586390/) 值得一读，不过我们不建议把这本书当作首要资源。

如果没有编写足够数量的代码，很难巩固数据库理论。CS 186 课程的学生给 Spark 添加特性，倒是不错的项目，不过我们仅仅建议从零实现一个简单的关系型数据库管理系统。自然，它将不会有太多的特性，但是即便只实现典型的关系型数据库管理系统每个方面最基础的功能，也是相当有启发的。

最后，数据模型往往是数据库中一个被忽视的、教学不充分的方面。关于这个主题，我们推荐的书籍是 [*Data and Reality: A Timeless Perspective on Perceiving and Managing Information in Our Imprecise World*](https://book.douban.com/subject/17915870/)。

[![Readings in Database Systems](https://user-images.githubusercontent.com/20233656/66760126-08d27b00-eed4-11e9-82c6-46c571036aa1.jpg)](https://book.douban.com/subject/2256069/) [![数据库管理系统：原理与设计](https://user-images.githubusercontent.com/20233656/66760358-85655980-eed4-11e9-9130-66d2ecea5700.jpg)](https://book.douban.com/subject/1155934/)

### 编程语言与编译器

多数程序员学习编程语言的知识，而多数计算机科学家学习编程语言 **相关** 的知识。这使得计算机科学家比起程序员拥有显著的优势，即便在编程领域！因为他们的知识可以推而广之：相较只学习过特定编程语言的人，他们可以更深入更快速地理解新的编程语言。

我们推荐的入门书是 Bob Nystrom 所著的优秀的 [*Crafting Interpreters*](https://craftinginterpreters.com/contents.html)，可在网上免费获取。这本书条理清晰，富有趣味性，非常适合那些想要更好地理解语言和语言工具的人。我们建议你花时间读完整本书，并尝试任何一个感兴趣的「挑战」。

另一本更为传统的推荐书籍是 [《编译原理》](https://book.douban.com/subject/3296317/)，通常称为「龙书」。不幸的是，这本书不是为自学者而设计的，而是供教师从中挑选一些主题用于 1-2 学期的教学。

如果你选择使用龙书进行自学，你需要从中甄选主题，而且最好是在导师的帮助下。我们建议依据某个视频课程来设定学习的结构，然后按需从龙书中获取深入的内容。我们推荐的在线课程是 [Alex Aiken 在 MOOC 平台 edX 所开设的](https://www.edx.org/course/compilers)。

[![编译原理](https://user-images.githubusercontent.com/20233656/66760486-ca898b80-eed4-11e9-80ba-df298ac8d5da.jpg)](https://book.douban.com/subject/3296317/)

> 不要做一个只写样板代码的程序员。相反，给用户和其他程序员创造工具。从纺织工业和钢铁工业中学习历史教训：你想制造机器和工具，还是操作这些机器？
>
>— Ras Bodik 在他的编译器课程伊始

### 分布式系统

随着计算机在数量上的增加，计算机同样开始 **分散**。尽管商业公司过去愿意购买越来越大的大型机，现在的典型情况是，甚至很小的应用程序都同时在多台机器上运行。思考这样做的利弊权衡，即是分布式系统的研究所在，也是越来越重要的一项技能。

我们推荐的自学参考书是 Martin Kleppmann 的 [《数据密集型应用系统设计》](https://book.douban.com/subject/30329536/)。与传统的教科书相比，它是一本为实践者设计的具有很高的可读性的书，并且保持了深度和严谨性。

对于那些偏爱传统教材，或者希望可以从网上免费获取的人，我们推荐的教材是 Maarten van Steen 和 Andrew Tanenbaum 所著的 《分布式系统原理与范型》（[中文第二版](https://book.douban.com/subject/3108801/)，[英文第三版](https://book.douban.com/subject/26979326/)）。

对于喜欢视频课程的人，[MIT 的 6.824](https://www.youtube.com/watch?v=cQP8WApzIQQ&list=PLrw6a1wE39_tb2fErI4-WkMbsvGQk9_UB) 是一门很好的在线视频课程，由 Robert Morris 教授的研究生课程，在 [这里](https://pdos.csail.mit.edu/6.824/schedule.html) 可以看到课程安排。

不管选择怎样的教材或者其他辅助资料，学习分布式系统必然要求阅读论文。[这里](http://dsrg.pdos.csail.mit.edu/papers/) 有一个不错的论文清单，而且我们强烈建议你出席你当地的 [Papers We Love](http://paperswelove.org/)（仅限美国）。

[![数据密集型应用系统设计](https://user-images.githubusercontent.com/20510068/82111034-94ff9600-9774-11ea-9d49-90b00f746659.png)](https://book.douban.com/subject/30329536/)

## 常见问题解答

### 这份指引的目标受众是？

我们面向自学的软件工程师、培训班学生、「早熟的」高中生或者想要通过自学补充正式教育的大学生。关于何时开启这段自学旅程，完全取决于个人，不过多数人在有一定的职业经历后深入学习计算机科学理论会获益匪浅。比如，我们注意到，如果学生在工作中曾经使用过数据库，他们会 **喜爱** 学习数据库系统课程；如果学生从事过一两个 Web 项目，他们会 **喜爱** 学习计算机网络。

### 人工智能/计算机图形学/XX怎么样？

我们试图把计算机科学主题清单限制到那些我们认为 **每一个软件工程师** 都应该了解的内容，不限于专业或行业。拥有了这些基础，你将能更加轻松地挑选教材或论文，然而无需指引地学习核心概念。在这里，我们给出一些其他常见主题的自学起点：

* 人工智能：通过观看视频并完成 Pacman 项目来学习 [Berkeley 的 AI 课程](http://ai.berkeley.edu/)。至于教材，使用 Russell 和 Norvig 编写的 [《人工智能：一种现代方法》](https://book.douban.com/subject/25796281/)。
* 机器学习：学习吴恩达在 Coursera 上的课程。耐心学习，先确保理解了基础概念再奔向类如深度学习的诱人新主题。
* 计算机图形学：学习 [Berkeley CS 184 课程](http://inst.eecs.berkeley.edu/~cs184/fa12/onlinelectures.html) 的材料，使用 [《计算机图形学：原理及实践》](https://book.douban.com/subject/30402778/) 作为教材。

### 一定要严格遵守推荐次序吗？

事实上，所有主题之间都有一定程度的重叠，彼此循环引用。以离散数学和算法的关系为例：先学习数学可以帮助你更深入地分析和理解算法，然而先学习算法可以为学习离散数学提供更大的动力和应用背景。理想情况下，你将在你的职业生涯多次重温二者。

因此，我们所推荐的次序主要是为了帮助你 **起步**……如果你出于某种强烈的原因而倾向以不同的顺序学习，那也没有关系，勇敢开始吧！不过在我们看来，最重要的「先决条件」是：先学计算机体系结构再学操作系统或数据库，先学计算机网络和操作系统再学分布式系统。

### 对比OSS、freeCodeCamp

[OSS 指引](https://github.com/open-source-society/computer-science) 涵盖太多主题，在许多主题中推荐劣质资源，没有就特定课程哪些方面有价值提供原因或指引。我们努力对这份指引中的课程加以限制，仅仅包括那些你作为软件工程师 **确实需要了解的**，不论你的专业方向，并且对每门课程为何必要做出了解释以帮助你理解。

FreeCodeCamp 主要关注编程，而不是计算机科学。至于你为什么要学习计算机科学，参见 [上文](#为什么要学习计算机科学)。如果你是个新手，我们建议先学 freeCodeCamp 的课程，一两年后再回归本指南。

### XX 编程语言怎么样？

学习一门特定的编程语言和学习计算机科学的一个领域完全不在一个维度——相比之下，学习语言 **容易** 且 **缺乏价值**。如果你已经了解了一些语言，我们强烈建议遵照我们的指引，然后在学习的空当中习得语言，或者暂且不管以后再说。如果你已经把编程学得不错了（比如学完了 **《计算机程序的构造和解释》**），尤其是如果你学习过编译器，那么面对一门新的语言，你只需要花一个周末稍多的时间即可基本掌握，之后你可以在工作中学习相关的类库/工具/生态。

### XX 流行技术怎么样？

没有任何一种技术的重要程度可以达到学习其使用足以成为计算机科学教学的核心部分。不过，你对学习那门技术充满热情，这很不错。诀窍是先从特定的技术回退到基本的领域或概念，判断这门流行技术在技术的宏观大局中位于何处，然后才深入学习这门技术。

### 为什么你们还在推荐 SICP?

先尝试读一下，有些人觉得 SICP 让人神魂颠倒，这在其他书很少见。如果你不喜欢，你可以尝试其他的东西，也许以后再回到 SICP。

### 为什么你们还在推荐龙书？

龙书依旧是内容最为完整的编译器单本书籍。由于过分强调一些如今不够时新的主题的细节，比如解析，这本书招致了恶评。然而事实上，这本书从未打算供人一页一页的学习，而仅仅是为了给教师准备一门课程提供足够的材料。类似地，自学者可以从书中量身按需挑选主题，或者最好依照公开课授课教师在课程大纲中的建议。
# CS学习规划
[CS学习规划]https://csdiy.wiki/CS%E5%AD%A6%E4%B9%A0%E8%A7%84%E5%88%92/）

计算机领域方向庞杂，知识浩如烟海，每个细分领域如果深究下去都可以说学无止境。因此，一个清晰明确的学习规划是非常重要的。我在多年自学的尝试中也走过不少弯路，最终提炼出了下面的内容，供大家参考。

不过，在开始学习之前，先向小白们强烈推荐一个科普向系列视频 [Crash Course: Computer Science](https://www.bilibili.com/video/BV1EW411u7th)，在短短 8 个小时里非常生动且全面地科普了关于计算机科学的方方面面：计算机的历史、计算机是如何运作的、组成计算机的各个重要模块、计算机科学中的重要思想等等等等。正如它的口号所说的 _Computers are not magic!_，希望看完这个视频之后，大家能对计算机科学有个全貌性地感知，从而怀着兴趣去面对下面浩如烟海的更为细致且深入的学习内容。

## 必学工具

> 俗话说：磨刀不误砍柴工。如果你是一个刚刚接触计算机的24k纯小白，学会一些工具将会让你事半功倍。

学会提问：也许你会惊讶，提问也算计算机必备技能吗，还放在第一条？我觉得在开源社区中，学会提问是一项非常重要的能力，它包含两方面的事情。其一是会变相地培养你自主解决问题的能力，因为从形成问题、描述问题并发布、他人回答、最后再到理解回答这个周期是非常长的，如果遇到什么鸡毛蒜皮的事情都希望别人最好远程桌面手把手帮你完成，那计算机的世界基本与你无缘了。其二，如果真的经过尝试还无法解决，可以借助开源社区的帮助，但这时候如何通过简洁的文字让别人瞬间理解你的处境以及目的，就显得尤为重要。推荐阅读[提问的智慧](https://github.com/ryanhanwu/How-To-Ask-Questions-The-Smart-Way/blob/main/README-zh_CN.md)这篇文章，这不仅能提高你解决问题的概率和效率，也能让开源社区里无偿提供解答的人们拥有一个好心情。

[MIT-Missing-Semester](https://csdiy.wiki/%E7%BC%96%E7%A8%8B%E5%85%A5%E9%97%A8/MIT-Missing-Semester/) 这门课覆盖了这些工具中绝大部分，而且有相当详细的使用指导，强烈建议小白学习。不过需要注意的一点是，在课程中会不时提到一些与开发流程相关的术语。因此推荐至少在学完计算机导论级别的课程之后进行学习。

[翻墙](https://csdiy.wiki/%E5%BF%85%E5%AD%A6%E5%B7%A5%E5%85%B7/%E7%BF%BB%E5%A2%99/)：由于一些众所周知的原因，谷歌、GitHub 等网站在大陆无法访问。然而很多时候，谷歌和 StackOverflow 可以解决你在开发过程中遇到的 99% 的问题。因此，学会翻墙几乎是一个内地 CSer 的必备技能。（考虑到法律问题，这个文档提供的翻墙方式仅对拥有北大邮箱的用户适用）。

命令行：熟练使用命令行是一种常常被忽视，或被认为难以掌握的技能，但实际上，它会极大地提高你作为工程师的灵活性以及生产力。[命令行的艺术](https://github.com/jlevy/the-art-of-command-line/blob/master/README-zh.md)是一份非常经典的教程，它源于 Quora 的一个提问，但在各路大神的贡献努力下已经成为了一个 GitHub 十万 stars 的顶流项目，被翻译成了十几种语言。教程不长，非常建议大家反复通读，在实践中内化吸收。同时，掌握 Shell 脚本编程也是一项不容忽视的技术，可以参考这个[教程](https://www.shellscript.sh/)。

IDE (Integrated Development Environment)：集成开发环境，说白了就是你写代码的地方。作为一个码农，IDE 的重要性不言而喻，但由于很多 IDE 是为大型工程项目设计的，体量较大，功能也过于丰富。其实如今一些轻便的文本编辑器配合丰富的插件生态基本可以满足日常的轻量编程需求。个人常用的编辑器是 VS Code 和 Sublime（前者的插件配置非常简单，后者略显复杂但颜值很高）。当然对于大型项目我还是会采用略重型的 IDE，例如 Pycharm (Python)，IDEA (Java) 等等（免责申明：所有的 IDE 都是世界上最好的 IDE）。

[Vim](https://csdiy.wiki/%E5%BF%85%E5%AD%A6%E5%B7%A5%E5%85%B7/Vim/)：一款命令行编辑工具。这是一个学习曲线有些陡峭的编辑器，不过学会它我觉得是非常有必要的，因为它将极大地提高你的开发效率。现在绝大多数 IDE 也都支持 Vim 插件，让你在享受现代开发环境的同时保留极客的炫酷（yue）。

[Git](https://csdiy.wiki/%E5%BF%85%E5%AD%A6%E5%B7%A5%E5%85%B7/Git/)：一款代码版本控制工具。Git的学习曲线可能更为陡峭，但出自 Linux 之父 Linus 之手的 Git 绝对是每个学 CS 的童鞋必须掌握的神器之一。

[GitHub](https://csdiy.wiki/%E5%BF%85%E5%AD%A6%E5%B7%A5%E5%85%B7/GitHub/)：基于 Git 的代码托管平台。全世界最大的代码开源社区，大佬集聚地。

[GNU Make](https://csdiy.wiki/%E5%BF%85%E5%AD%A6%E5%B7%A5%E5%85%B7/GNU_Make/)：一款工程构建工具。善用 GNU Make 会让你养成代码模块化的习惯，同时也能让你熟悉一些大型工程的编译链接流程。

[CMake](https://csdiy.wiki/%E5%BF%85%E5%AD%A6%E5%B7%A5%E5%85%B7/CMake/)：一款功能比 GNU Make 更为强大的构建工具，建议掌握 GNU Make 之后再加以学习。

[LaTex](https://csdiy.wiki/%E5%BF%85%E5%AD%A6%E5%B7%A5%E5%85%B7/LaTeX/)：~逼格提升~ 论文排版工具。

[Docker](https://csdiy.wiki/%E5%BF%85%E5%AD%A6%E5%B7%A5%E5%85%B7/Docker/)：一款相较于虚拟机更轻量级的软件打包与环境部署工具。

[实用工具箱](https://csdiy.wiki/%E5%BF%85%E5%AD%A6%E5%B7%A5%E5%85%B7/tools/)：除了上面提到的这些在开发中使用频率极高的工具之外，我还收集了很多实用有趣的免费工具，例如一些下载工具、设计工具、学习网站等等。

[Thesis](https://csdiy.wiki/%E5%BF%85%E5%AD%A6%E5%B7%A5%E5%85%B7/thesis/)：毕业论文 Word 写作教程。

## 好书推荐

> 私以为一本好的教材应当是以人为本的，而不是炫技式的理论堆砌。告诉读者“是什么”固然重要，但更好的应当是教材作者将其在这个领域深耕几十年的经验融汇进书中，向读者娓娓道来“为什么”以及未来应该“怎么做”。

[链接戳这里](https://csdiy.wiki/%E5%A5%BD%E4%B9%A6%E6%8E%A8%E8%8D%90/)

## 环境配置

> 你以为的开发 —— 在 IDE 里疯狂码代码数小时。
>
> 实际上的开发 —— 配环境配几天还没开始写代码。

### PC 端环境配置

如果你是 Mac 用户，那么你很幸运，这份[指南](https://sourabhbajaj.com/mac-setup/) 将会手把手地带你搭建起整套开发环境。如果你是 Windows 用户，在开源社区的努力下，你同样可以获得与其他平台类似的体验：[Scoop](https://csdiy.wiki/%E5%BF%85%E5%AD%A6%E5%B7%A5%E5%85%B7/Scoop)。

另外大家可以参考一份灵感来自 [6.NULL MIT-Missing-Semester](https://csdiy.wiki/%E7%BC%96%E7%A8%8B%E5%85%A5%E9%97%A8/MIT-Missing-Semester/) 的 [环境配置指南](https://taylover2016.github.io/%E6%96%B0%E6%9C%BA%E5%99%A8%E4%B8%8A%E6%89%8B%E6%8C%87%E5%8D%97%EF%BC%88%E6%96%B0%E6%89%8B%E5%90%91%EF%BC%89/index.html)，重点在于终端的美化配置。此外还包括常用软件源（如 GitHub, Anaconda, PyPI 等）的加速与替换以及一些 IDE 的配置与激活教程。

### 服务器端环境配置

服务器端的运维需要掌握 Linux（或者其他类 Unix 系统）的基本使用以及进程、设备、网络等系统相关的基本概念，小白可以参考中国科学技术大学 Linux 用户协会编写的[《Linux 101》在线讲义](https://101.lug.ustc.edu.cn/)。如果想深入学习系统运维相关的知识，可以参考 [Aspects of System Administration](https://stevens.netmeister.org/615/) 这门课程。

另外，如果需要学习某个具体的概念或工具，推荐一个非常不错的 GitHub 项目 [DevOps-Guide](https://github.com/Tikam02/DevOps-Guide)，其中涵盖了非常多的运维方面的基础知识和教程，例如 Docker, Kubernetes, Linux, CI-CD, GitHub Actions 等等。

## 课程地图

> 正如这章开头提到的，这份课程地图仅仅是一个**仅供参考**的课程规划，我作为一个临近毕业的本科生。深感自己没有权利也没有能力向别人宣扬“应该怎么学”。因此如果你觉得以下的课程分类与选择有不合理之处，我全盘接受，并深感抱歉。你可以在下一节[定制属于你的课程地图](https://csdiy.wiki/CS%E5%AD%A6%E4%B9%A0%E8%A7%84%E5%88%92/#yourmap)

以下课程类别中除了含有 _基础_ 和 _入门_ 字眼的以外，并无明确的先后次序，大家只要满足某个课程的先修要求，完全可以根据自己的需要和喜好选择想要学习的课程。

### 数学基础

#### 微积分与线性代数

作为大一新生，学好微积分线代是和写代码至少同等重要的事情，相信已经有无数的前人经验提到过这一点，但我还是要不厌其烦地再强调一遍：学好微积分线代真的很重要！你也许会吐槽这些东西岂不是考完就忘，那我觉得你是并没有把握住它们本质，对它们的理解还没有达到刻骨铭心的程度。如果觉得老师课上讲的内容晦涩难懂，不妨参考 MIT 的 [Calculus Course](https://csdiy.wiki/%E6%95%B0%E5%AD%A6%E5%9F%BA%E7%A1%80/MITmaths/) 和 [18.06: Linear Algebra](https://csdiy.wiki/%E6%95%B0%E5%AD%A6%E5%9F%BA%E7%A1%80/MITLA/) 的课程 notes，至少于我而言，它帮助我深刻理解了微积分和线性代数的许多本质。顺道再安利一个油管数学网红 [**3Blue1Brown**](https://www.youtube.com/c/3blue1brown)，他的频道有很多用生动形象的动画阐释数学本质内核的视频，兼具深度和广度，质量非常高。

#### 信息论入门

作为计算机系的学生，及早了解一些信息论的基础知识，我觉得是大有裨益的。但大多信息论课程都面向高年级本科生甚至研究生，对新手极不友好。而 MIT 的 [6.050J: Information theory and Entropy](https://csdiy.wiki/%E6%95%B0%E5%AD%A6%E5%9F%BA%E7%A1%80/information/) 这门课正是为大一新生量身定制的，几乎没有先修要求，涵盖了编码、压缩、通信、信息熵等等内容，非常有趣。

### 数学进阶

#### 离散数学与概率论

集合论、图论、概率论等等是算法推导与证明的重要工具，也是后续高阶数学课程的基础。但我觉得这类课程的讲授很容易落入理论化与形式化的窠臼，让课堂成为定理结论的堆砌，而无法使学生深刻把握理论的本质，进而造成学了就背，考了就忘的怪圈。如果能在理论教学中穿插算法运用实例，学生在拓展算法知识的同时也能窥见理论的力量和魅力。

[UCB CS70 : discrete Math and probability theory](https://csdiy.wiki/%E6%95%B0%E5%AD%A6%E8%BF%9B%E9%98%B6/CS70/) 和 [UCB CS126 : Probability theory](https://csdiy.wiki/%E6%95%B0%E5%AD%A6%E8%BF%9B%E9%98%B6/CS126/) 是 UC Berkeley 的概率论课程，前者覆盖了离散数学和概率论基础，后者则涉及随机过程以及深入的理论内容。两者都非常注重理论和实践的结合，有丰富的算法实际运用实例，后者还有大量的 Python 编程作业来让学生运用概率论的知识解决实际问题。

#### 数值分析

作为计算机系的学生，培养计算思维是很重要的，实际问题的建模、离散化，计算机的模拟、分析，是一项很重要的能力。而这两年开始风靡的，由 MIT 打造的 [Julia](https://julialang.org/) 编程语言以其 C 一样的速度和 Python 一样友好的语法在数值计算领域有一统天下之势，MIT 的许多数学课程也开始用 Julia 作为教学工具，把艰深的数学理论用直观清晰的代码展示出来。

[ComputationalThinking](https://computationalthinking.mit.edu/Spring21/) 是 MIT 开设的一门计算思维入门课，所有课程内容全部开源，可以在课程网站直接访问。这门课利用 Julia 编程语言，在图像处理、社会科学与数据科学、气候学建模三个 topic 下带领学生理解算法、数学建模、数据分析、交互设计、图例展示，让学生体验计算与科学的美妙结合。内容虽然不难，但给我最深刻的感受就是，科学的魅力并不是故弄玄虚的艰深理论，不是诘屈聱牙的术语行话，而是用直观生动的案例，用简练深刻的语言，让每个普通人都能理解。

上完上面的体验课之后，如果意犹未尽的话，不妨试试 MIT 的 [18.330 : Introduction to numerical analysis](https://csdiy.wiki/%E6%95%B0%E5%AD%A6%E8%BF%9B%E9%98%B6/numerical/)，这门课的编程作业同样会用 Julia 编程语言，不过难度和深度上都上了一个台阶。内容涉及了浮点编码、Root finding、线性系统、微分方程等等方面，整门课的主旨就是让你利用离散化的计算机表示去估计和逼近一个数学上连续的概念。这门课的教授还专门撰写了一本配套的开源教材 [Fundamentals of Numerical Computation](https://fncbook.github.io/fnc/frontmatter.html)，里面附有丰富的 Julia 代码实例和严谨的公式推导。

如果你还意犹未尽的话，还有 MIT 的数值分析研究生课程 [18.335: Introduction to numerical method](https://ocw.mit.edu/courses/mathematics/18-335j-introduction-to-numerical-methods-spring-2019/index.htm) 供你参考。

#### 微分方程

如果世间万物的运动发展都能用方程来刻画和描述，这是一件多么酷的事情呀！虽然几乎任何一所学校的 CS 培养方案中都没有微分方程相关的必修课程，但我还是觉得掌握它会赋予你一个新的视角来审视这个世界。

由于微分方程中往往会用到很多复变函数的知识，所以大家可以参考 [MIT18.04: Complex variables functions](https://ocw.mit.edu/courses/mathematics/18-04-complex-variables-with-applications-spring-2018/) 的课程 notes 来补齐先修知识。

[MIT18.03: differential equations](https://ocw.mit.edu/courses/mathematics/18-03sc-differential-equations-fall-2011/unit-i-first-order-differential-equations/) 主要覆盖了常微分方程的求解，在此基础之上 [MIT18.152: Partial differential equations](https://ocw.mit.edu/courses/mathematics/18-152-introduction-to-partial-differential-equations-fall-2011/index.htm) 则会深入偏微分方程的建模与求解。掌握了微分方程这一有力工具，相信对于你的实际问题的建模能力以及从众多噪声变量中把握本质的直觉都会有很大帮助。

### 数学高阶

作为计算机系的学生，我经常听到数学无用论的论断，对此我不敢苟同但也无权反对，但若凡事都硬要争出个有用和无用的区别来，倒也着实无趣，因此下面这些面向高年级甚至研究生的数学课程，大家按兴趣自取所需。

#### 凸优化

[Standford EE364A: Convex Optimization](https://csdiy.wiki/%E6%95%B0%E5%AD%A6%E8%BF%9B%E9%98%B6/convex/)

#### 信息论

[MIT6.441: Information Theory](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-441-information-theory-spring-2016/syllabus/)

#### 应用统计学

[MIT18.650: Statistics for Applications](https://ocw.mit.edu/courses/mathematics/18-443-statistics-for-applications-spring-2015/index.htm)

#### 初等数论

[MIT18.781: Theory of Numbers](https://ocw.mit.edu/courses/mathematics/18-781-theory-of-numbers-spring-2012/index.htm)

#### 密码学

[Standford CS255: Cryptography](http://crypto.stanford.edu/~dabo/cs255/)

### 编程入门

> Languages are tools, you choose the right tool to do the right thing. Since there's no universally perfect tool, there's no universally perfect language.

#### Shell

-   [MIT-Missing-Semester](https://csdiy.wiki/%E7%BC%96%E7%A8%8B%E5%85%A5%E9%97%A8/MIT-Missing-Semester/)

#### Python

-   [CS50P: CS50's Introduction to Programming with Python](https://csdiy.wiki/%E7%BC%96%E7%A8%8B%E5%85%A5%E9%97%A8/CS50P/)
-   [Harvard CS50: This is CS50x](https://csdiy.wiki/%E7%BC%96%E7%A8%8B%E5%85%A5%E9%97%A8/CS50/)
-   [UCB CS61A: Structure and Interpretation of Computer Programs](https://csdiy.wiki/%E7%BC%96%E7%A8%8B%E5%85%A5%E9%97%A8/CS61A/)

#### C++

-   [Stanford CS106B/X: Programming Abstractions](https://csdiy.wiki/%E7%BC%96%E7%A8%8B%E5%85%A5%E9%97%A8/CS106B_CS106X/)
-   [Stanford CS106L: Standard C++ Programming](https://csdiy.wiki/%E7%BC%96%E7%A8%8B%E5%85%A5%E9%97%A8/CS106L/)

#### Rust

-   [Stanford CS110L: Safety in Systems Programming](https://csdiy.wiki/%E7%BC%96%E7%A8%8B%E5%85%A5%E9%97%A8/CS110L/)

#### OCaml

-   [Cornell CS3110 textbook: Functional Programming in OCaml](https://cs3110.github.io/textbook/cover.html)

### 电子基础

#### 电路基础

作为计算机系的学生，了解一些基础的电路知识，感受从传感器收集数据到数据分析再到算法预测整条流水线，对于后续知识的学习以及计算思维的培养还是很有帮助的。[EE16A&B: Designing Information Devices and Systems I&II](https://csdiy.wiki/%E7%94%B5%E5%AD%90%E5%9F%BA%E7%A1%80/EE16/) 是伯克利 EE 学生的大一入门课，其中 EE16A 注重通过电路从实际环境中收集和分析数据，而 EE16B 则侧重从这些收集到的数据进行分析并做出预测行为。

#### 信号与系统

信号与系统是一门我觉得非常值得一上的课，最初学它只是为了满足我对傅里叶变换的好奇，但学完之后我才不禁感叹，傅立叶变换给我提供了一个全新的视角去看待这个世界，就如同微分方程一样，让你沉浸在用数学去精确描绘和刻画这个世界的优雅与神奇之中。

[MIT 6.003: signal and systems](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-003-signals-and-systems-fall-2011/lecture-videos/lecture-1-signals-and-systems/) 提供了全部的课程录影、书面作业以及答案。也可以去看这门课的[远古版本](https://csdiy.wiki/%E7%94%B5%E5%AD%90%E5%9F%BA%E7%A1%80/Signals_and_Systems_AVO/)

而 [UCB EE120: Signal and Systems](https://csdiy.wiki/%E7%94%B5%E5%AD%90%E5%9F%BA%E7%A1%80/signal/) 关于傅立叶变换的 notes 写得非常好，并且提供了6 个非常有趣的 Python 编程作业，让你实践中运用信号与系统的理论与算法。

### 数据结构与算法

算法是计算机科学的核心，也是几乎一切专业课程的基础。如何将实际问题通过数学抽象转化为算法问题，并选用合适的数据结构在时间和内存大小的限制下将其解决是算法课的永恒主题。如果你受够了老师的照本宣科，那么我强烈推荐伯克利的 [UCB CS61B: Data Structures and Algorithms](https://csdiy.wiki/%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%E4%B8%8E%E7%AE%97%E6%B3%95/CS61B/) 和普林斯顿的 [Coursera: Algorithms I & II](https://csdiy.wiki/%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%E4%B8%8E%E7%AE%97%E6%B3%95/Algo/)，这两门课的都讲得深入浅出并且会有丰富且有趣的编程实验将理论与知识结合起来。

以上两门课程都是基于 Java 语言，如果你想学习 C/C++ 描述的版本，可以参考斯坦福的数据结构与基础算法课程 [Stanford CS106B/X: Programming Abstractions](https://csdiy.wiki/%E7%BC%96%E7%A8%8B%E5%85%A5%E9%97%A8/CS106B_CS106X/)。偏好 Python 的同学可以学习 MIT 的算法入门课 [MIT 6.006: Introduction to Algorithms](https://csdiy.wiki/%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%E4%B8%8E%E7%AE%97%E6%B3%95/6.006/)

对一些更高级的算法以及 NP 问题感兴趣的同学可以学习伯克利的算法设计与分析课程 [UCB CS170: Efficient Algorithms and Intractable Problems](https://csdiy.wiki/%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%E4%B8%8E%E7%AE%97%E6%B3%95/CS170/) 或者 MIT 的高阶算法 [MIT 6.046: Design and Analysis of Algorithms](https://csdiy.wiki/%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%E4%B8%8E%E7%AE%97%E6%B3%95/6.046/)。

### 软件工程

#### 入门课

一份“能跑”的代码，和一份高质量的工业级代码是有本质区别的。因此我非常推荐低年级的同学学习一下 [MIT 6.031: Software Construction](https://csdiy.wiki/%E8%BD%AF%E4%BB%B6%E5%B7%A5%E7%A8%8B/6031/) 这门课，它会以 Java 语言为基础，以丰富细致的阅读材料和精心设计的编程练习传授如何编写**不易出 bug、简明易懂、易于维护修改**的高质量代码。大到宏观数据结构设计，小到如何写注释，遵循这些前人总结的细节和经验，对于你此后的编程生涯大有裨益。

#### 专业课

当然，如果你想系统性地上一门软件工程的课程，那我推荐的是伯克利的 [UCB CS169: software engineering](https://csdiy.wiki/%E8%BD%AF%E4%BB%B6%E5%B7%A5%E7%A8%8B/CS169/)。但需要提醒的是，和大多学校（包括贵校）的软件工程课程不同，这门课不会涉及传统的 **design and document** 模式，即强调各种类图、流程图及文档设计，而是采用近些年流行起来的小团队快速迭代 **Agile Develepment** 开发模式以及利用云平台的 **Software as a service** 服务模式。

### 体系结构

#### 入门课

从小我就一直听说，计算机的世界是由 01 构成的，我不理解但大受震撼。如果你的内心也怀有这份好奇，不妨花一到两个月的时间学习 [Coursera: Nand2Tetris](https://csdiy.wiki/%E4%BD%93%E7%B3%BB%E7%BB%93%E6%9E%84/N2T/) 这门无门槛的计算机课程。这门麻雀虽小五脏俱全的课程会从 01 开始让你亲手造出一台计算机，并在上面运行俄罗斯方块小游戏。一门课里涵盖了编译、虚拟机、汇编、体系结构、数字电路、逻辑门等等从上至下、从软至硬的各类知识，非常全面。难度上也是通过精心的设计，略去了众多现代计算机复杂的细节，提取出了最核心本质的东西，力图让每个人都能理解。在低年级，如果就能从宏观上建立对整个计算机体系的鸟瞰图，是大有裨益的。

#### 专业课

当然，如果想深入现代计算机体系结构的复杂细节，还得上一门大学本科难度的课程 [UCB CS61C: Great Ideas in Computer Architecture](https://csdiy.wiki/%E4%BD%93%E7%B3%BB%E7%BB%93%E6%9E%84/CS61C/)。UC Berkeley 作为 RISC-V 架构的发源地，在体系结构领域算得上首屈一指。其课程非常注重实践，你会在 Project 中手写汇编构造神经网络，从零开始搭建一个 CPU，这些实践都会让你对计算机体系结构有更为深入的理解，而不是仅停留于“取指译码执行访存写回”的单调背诵里。

### 系统入门

计算机系统是一个庞杂而深刻的主题，在深入学习某个细分领域之前，对各个领域有一个宏观概念性的理解，对一些通用性的设计原则有所知晓，会让你在之后的深入学习中不断强化一些最为核心乃至哲学的概念，而不会桎梏于复杂的内部细节和各种 trick。因为在我看来，学习系统最关键的还是想让你领悟到这些最核心的东西，从而能够设计和实现出属于自己的系统。

[MIT6.033: System Engineering](http://web.mit.edu/6.033/www/) 是 MIT 的系统入门课，主题涉及了操作系统、网络、分布式和系统安全，除了知识点的传授外，这门课还会讲授一些写作和表达上的技巧，让你学会如何设计并向别人介绍和分析自己的系统。这本书配套的教材 _Principles of Computer System Design: An Introduction_ 也写得非常好，推荐大家阅读。

[CMU 15-213: Introduction to Computer System](https://csdiy.wiki/%E4%BD%93%E7%B3%BB%E7%BB%93%E6%9E%84/CSAPP/) 是 CMU 的系统入门课，内容覆盖了体系结构、操作系统、链接、并行、网络等等，兼具广度和深度，配套的教材 _Computer Systems: A Programmer's Perspective_ 也是质量极高，强烈建议阅读。

### 操作系统

> 没有什么能比自己写个内核更能加深对操作系统的理解了。

操作系统作为各类纷繁复杂的底层硬件虚拟化出一套规范优雅的抽象，给所有应用软件提供丰富的功能支持。了解操作系统的设计原则和内部原理对于一个不满足于当调包侠的程序员来说是大有裨益的。出于对操作系统的热爱，我上过国内外很多操作系统课程，它们各有侧重和优劣，大家可以根据兴趣各取所需。

[MIT 6.S081: Operating System Engineering](https://csdiy.wiki/%E6%93%8D%E4%BD%9C%E7%B3%BB%E7%BB%9F/MIT6.S081/)，MIT 著名 PDOS 实验室出品，11 个 Project 让你在一个实现非常优雅的类Unix操作系统xv6上增加各类功能模块。这门课也让我深刻认识到，做系统不是靠 PPT 念出来的，是得几万行代码一点点累起来的。

[UCB CS162: Operating System](https://csdiy.wiki/%E6%93%8D%E4%BD%9C%E7%B3%BB%E7%BB%9F/CS162/)，伯克利的操作系统课，采用和 Stanford 同样的 Project —— 一个教学用操作系统 Pintos。我作为北京大学2022年春季学期操作系统实验班的助教，引入并改善了这个 Project，课程资源也会全部开源，具体参见[课程网站](https://https//pku-os.github.io/sp22/)。

[NJU: Operating System Design and Implementation](https://csdiy.wiki/%E6%93%8D%E4%BD%9C%E7%B3%BB%E7%BB%9F/NJUOS/)，南京大学的蒋炎岩老师开设的操作系统课程。蒋老师以其独到的系统视角结合丰富的代码示例将众多操作系统的概念讲得深入浅出，此外这门课的全部课程内容都是中文的，非常方便大家学习。

### 并行与分布式系统

想必这两年各类 CS 讲座里最常听到的话就是“摩尔定律正在走向终结”，此话不假，当单核能力达到上限时，多核乃至众核架构如日中天。硬件的变化带来的是上层编程逻辑的适应与改变，要想充分利用硬件性能，编写并行程序几乎成了程序员的必备技能。与此同时，深度学习的兴起对计算机算力与存储的要求都达到了前所未有的高度，大规模集群的部署和优化也成为热门技术话题。

#### 并行计算

[CMU 15-418/Stanford CS149: Parallel Computing](https://csdiy.wiki/%E5%B9%B6%E8%A1%8C%E4%B8%8E%E5%88%86%E5%B8%83%E5%BC%8F%E7%B3%BB%E7%BB%9F/CS149/)

#### 分布式系统

[MIT 6.824: Distributed System](https://csdiy.wiki/%E5%B9%B6%E8%A1%8C%E4%B8%8E%E5%88%86%E5%B8%83%E5%BC%8F%E7%B3%BB%E7%BB%9F/MIT6.824/)

### 系统安全

不知道你当年选择计算机是不是因为怀着一个中二的黑客梦想，但现实却是成为黑客道阻且长。

#### 理论课程

[UCB CS161: Computer Security](https://csdiy.wiki/%E7%B3%BB%E7%BB%9F%E5%AE%89%E5%85%A8/CS161/) 是伯克利的系统安全课程，会涵盖栈攻击、密码学、网站安全、网络安全等等内容。

[ASU CSE365: Introduction to Cybersecurity](https://csdiy.wiki/%E7%B3%BB%E7%BB%9F%E5%AE%89%E5%85%A8/CSE365/) 亚利桑那州立大学的 Web 安全课程，主要涉及注入、汇编与密码学的内容。

[ASU CSE466: Computer Systems Security](https://csdiy.wiki/%E7%B3%BB%E7%BB%9F%E5%AE%89%E5%85%A8/CSE466/) 亚利桑那州立大学的系统安全课程，涉及内容全面。门槛较高，需要对 Linux, C 与 Python 充分熟悉。

#### 实践课程

掌握这些理论知识之后，还需要在实践中培养和锻炼这些“黑客素养”。[CTF 夺旗赛](https://ctf-wiki.org/)是一项比较热门的系统安全比赛，赛题中会融会贯通地考察你对计算机各个领域知识的理解和运用。北大今年也成功举办了[第 0 届和第 1 届](https://geekgame.pku.edu.cn/)，鼓励大家后期踊跃参与，在实践中提高自己。下面列举一些我平时学习（摸鱼）用到的资源：

-   [CTF-wiki](https://ctf-wiki.org/)
-   [CTF-101](https://ctf101.org/)
-   [Hacker-101](https://ctf.hacker101.com/)

### 计算机网络

> 没有什么能比自己写个 TCP/IP 协议栈更能加深对计算机网络的理解了。

大名鼎鼎的 [Stanford CS144: Computer Network](https://csdiy.wiki/%E8%AE%A1%E7%AE%97%E6%9C%BA%E7%BD%91%E7%BB%9C/CS144/)，8 个 Project 带你实现整个 TCP/IP 协议栈。

如果你只是想在理论上对计算机网络有所了解，那么推荐计网著名教材《自顶向下方法》的配套学习资源 [Computer Networking: A Top-Down Approach](https://csdiy.wiki/%E8%AE%A1%E7%AE%97%E6%9C%BA%E7%BD%91%E7%BB%9C/topdown/)。

### 数据库系统

> 没有什么能比自己写个关系型数据库更能加深对数据库系统的理解了。

CMU 的著名数据库神课 [CMU 15-445: Introduction to Database System](https://csdiy.wiki/%E6%95%B0%E6%8D%AE%E5%BA%93%E7%B3%BB%E7%BB%9F/15445/) 会通过 4 个 Project 带你为一个用于教学的关系型数据库 [bustub](https://github.com/cmu-db/bustub) 添加各种功能。实验的评测框架也免费开源了，非常适合大家自学。此外课程实验会用到 C++11 的众多新特性，也是一个锻炼 C++ 代码能力的好机会。

Berkeley 作为著名开源数据库 postgres 的发源地也不遑多让，[UCB CS186: Introduction to Database System](https://csdiy.wiki/%E6%95%B0%E6%8D%AE%E5%BA%93%E7%B3%BB%E7%BB%9F/CS186/) 会让你用 Java 语言实现一个支持 SQL 并发查询、B+ 树索引和故障恢复的关系型数据库。

### 编译原理

> 没有什么能比自己写个编译器更能加深对编译器的理解了。

[Stanford CS143: Compilers](https://csdiy.wiki/%E7%BC%96%E8%AF%91%E5%8E%9F%E7%90%86/CS143/) 带你手写编译器。

### Web开发

前后端开发很少在计算机的培养方案里被重视，但其实掌握这项技能还是好处多多的，例如搭建自己的个人主页，抑或是给自己的课程项目做一个精彩的展示网页。

#### 两周速成版

[MIT web development course](https://csdiy.wiki/Web%E5%BC%80%E5%8F%91/mitweb/)

#### 系统学习版

[Stanford CS142: Web Applications](https://csdiy.wiki/Web%E5%BC%80%E5%8F%91/CS142/)

### 计算机图形学

-   [Stanford CS148](https://csdiy.wiki/%E8%AE%A1%E7%AE%97%E6%9C%BA%E5%9B%BE%E5%BD%A2%E5%AD%A6/CS148/)
-   [Games101](https://csdiy.wiki/%E8%AE%A1%E7%AE%97%E6%9C%BA%E5%9B%BE%E5%BD%A2%E5%AD%A6/GAMES101/)
-   [Games103](https://csdiy.wiki/%E8%AE%A1%E7%AE%97%E6%9C%BA%E5%9B%BE%E5%BD%A2%E5%AD%A6/GAMES103/)
-   [Games202](https://csdiy.wiki/%E8%AE%A1%E7%AE%97%E6%9C%BA%E5%9B%BE%E5%BD%A2%E5%AD%A6/GAMES202/)

### 数据科学

其实数据科学和机器学习与深度学习有着很紧密的联系，但可能更侧重于实践。Berkeley 的 [UCB Data100: Principles and Techniques of Data Science](https://csdiy.wiki/%E6%95%B0%E6%8D%AE%E7%A7%91%E5%AD%A6/Data100/) 通过丰富的编程练习让你在实践中掌握各类数据分析工具和算法，并带领你体验从海量的数据集中提取出想要的结果，并对未来的数据或用户的行为做出相应的预测。但这只是一门基础课，如果想学习工业级别的数据挖掘与分析技术，可以尝试 Stanford 的大数据挖掘课程 [CS246: Mining Massive Data Sets](https://web.stanford.edu/class/cs246/)。

### 人工智能

近十年人工智能应该算是计算机界最火爆的领域。如果你不满足于整日听各路媒体争相报道人工智能相关的进展，而想真正一探究竟，那么非常推荐学习 Harvard 神课 CS50 系列的人工智能课程 [Harvard CS50: Introduction to AI with Python](https://csdiy.wiki/%E4%BA%BA%E5%B7%A5%E6%99%BA%E8%83%BD/CS50/)。课程短小精悍，覆盖了传统人工智能领域的几大分支，并配有丰富有趣的 Python 编程练习来巩固你对人工智能算法的理解。美中不足的是这门课因为面向在线自学者的缘故内容较为精简，并且不会涉及特别深入的数学理论，如果想要系统深入地学习还需要一门本科生难度的课程，例如 Berkeley 的 [UCB CS188: Introduction to Artificial Intelligence](https://csdiy.wiki/%E4%BA%BA%E5%B7%A5%E6%99%BA%E8%83%BD/CS188/)。这门课的 Project 复刻了经典游戏糖豆人，让你运用人工智能算法玩游戏，非常有趣。

### 机器学习

机器学习领域近些年最重要的进展就是发展出了基于神经网络的深度学习分支，但其实很多基于统计学习的算法依然在数据分析领域有着广泛的应用。如果你之前从未接触过机器学习的相关知识，而且不想一开始就陷入艰深晦涩的数学证明，那么不妨先从 Andrew Ng （吴恩达）的 [Coursera: Machine Learning](https://csdiy.wiki/%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0/ML/) 学起。这门课在机器学习领域基本无人不晓，吴恩达以其深厚的理论功底和出色的表达能力把很多艰深的算法讲得深入浅出，并且非常实用。其配套的作业也是质量相当上乘，可以帮助你快速入门。

但上过这门课只能让你从宏观上对机器学习这一领域有一定了解，如果想真正理解那些“神奇”算法背后的数学原理甚至从事相关领域的科研工作，那么还需要一门更“数学”的课程，例如 [Stanford CS229: Machine Learning](https://csdiy.wiki/%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0/CS229/) 或者 [UCB CS189: Introduction to Machine Learning](https://csdiy.wiki/%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0/CS189/)。

### 深度学习

前几年 AlphaGo 的大热让深度学习进入了大众的视野，不少大学甚至专门成立了相关专业。很多计算机的其他领域也会借助深度学习的技术来做研究，因此基本不管你干啥多少都会接触到一些神经网络、深度学习相关的技术需求。如果想快速入门，同样推荐 Andrew Ng （吴恩达）的 [Coursera: Deep Learning](https://csdiy.wiki/%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0/CS230/)，质量无需多言，Coursera 上罕见的满分课程。此外如果你觉得英文课程学习起来有难度，推荐李宏毅老师的 [国立台湾大学：机器学习](https://csdiy.wiki/%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0/LHY/) 课程。这门课打着机器学习的名号，却囊括了深度学习领域的几乎所有方向，非常全面，很适合你从宏观上对这个领域有一个大致的了解。而且老师本人也非常幽默，课堂金句频出。

当然因为深度学习领域发展非常迅速，已经拥有了众多研究分支，如果想要进一步深入，可以按需学习下面罗列的代表课程，

#### 计算机视觉

[Stanford CS231n: CNN for Visual Recognition](https://csdiy.wiki/%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0/CS231/)

#### 自然语言处理

[Stanford CS224n: Natural Language Processing](https://csdiy.wiki/%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0/CS224n/)

#### 图神经网络

[Stanford CS224w: Machine Learning with Graphs](https://csdiy.wiki/%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0/CS224w/)

#### 强化学习

[UCB CS285: Deep Reinforcement Learning](https://csdiy.wiki/%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0/CS285/)

## 定制属于你的课程地图

> 授人以鱼不如授人以渔。

以上的课程规划难免带有强烈的个人偏好，不一定适合所有人，更多是起到抛砖引玉的作用。如果你想挑选自己感兴趣的方向和内容加以学习，可以参考我在下面列出来的资源。

-   [MIT OpenCourseWare](https://ocw.mit.edu/): 麻省理工学院的课程资源开放共享项目，收录了数以千计的各科课程资源，其中计算机类的课号是 6.xxx。
-   [MIT CS Course List](http://student.mit.edu/catalog/m6a.html): 麻省理工学院的 CS 课程列表。
-   [UC Berkeley EECS Course Map](https://hkn.eecs.berkeley.edu/courseguides): UC Berkeley 的 EECS 培养方案，以课程地图的方式将各门课程的类别和先修关系一目了然地呈现，其中绝大多数课程本书中均有收录。
-   [UC Berkeley CS Course List](https://www2.eecs.berkeley.edu/Courses/CS/): UC Berkeley 的 CS 课程列表。
-   [Stanford CS Course List](https://blog.csdn.net/qq_41220023/article/details/81976967): 斯坦福的 CS 课程列表。

