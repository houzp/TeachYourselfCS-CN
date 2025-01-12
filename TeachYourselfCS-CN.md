# 自学计算机科学

> 本文档是对[TeachYourselfCS](https://teachyourselfcs.com)内容的中文翻译，原作者为[Ozan Onay](https://twitter.com/oznova_)和[Myles Byrne](https://twitter.com/quackingduck)。如需了解翻译相关信息或帮助改进翻译，请参见[本文档结尾](#这份指引是谁翻译的)。
>
> This document is a Chinese translation of [TeachYourselfCS](https://teachyourselfcs.com), which is written by [Ozan Onay](https://twitter.com/oznova_) and [Myles Byrne](https://twitter.com/quackingduck). For more information about this translation, please refer to [the end of this document](#这份指引是谁翻译的).

如果你是一个自学成才的工程师，或者从编程培训班毕业，那么你很有必要学习计算机科学。幸运的是，不必为此花上数年光阴和不菲费用去攻读一个学位：仅仅依靠自己，你就可以获得世界一流水平的教育💸。

互联网上，到处都有许多的学习资源，然而精华与糟粕并存。你所需要的的，不是一个诸如“200+免费在线课程”的清单，而是以下问题的答案：

*   你应当学习**哪些科目**，为什么？
*   对于这些科目，**最好的书籍或者视频课程**是什么？

在这份指引中，我们尝试对这些问题做出确定的回答。

## 简而言之

大致按照列出的顺序，借助我们所建议的教材或者视频课程（但是最好二者兼用），学习如下的九门科目。目标是先花100到200个小时学习完每一个科目，然后在你职业生涯中，不时温习其中的精髓🚀。

| 科目 | 为何要学？ | 最佳书籍 | 最佳视频 |
| --- | --- | --- | --- |
| **[编程](#编程)** | 不要做一个“永远没彻底搞懂”诸如递归等概念的程序员。| _《计算机程序的构造和解释》_ | Brian Harvey’s Berkeley CS 61A |
| **[计算机架构](#计算机架构)** | 如果你对于计算机如何工作没有具体的概念，那么你所做出的所有高级抽象都是空中楼阁。 | _《计算机组成与设计》_ | Berkeley CS 61C |
| **[算法与数据结构](#算法和数据结构)** | 如果你不懂得如何使用栈、队列、树、图等常见数据结构，遇到有难度的问题时，你将束手无策。| _《算法设计手册》_ | Steven Skiena’s lectures |
| **[数学知识](#数学知识)** | 计算机科学基本上是应用数学的一个“失控的”分支，因此学习数学将会给你带来竞争优势。| _《计算机科学中的数学》_ | Tom Leighton’s MIT 6.042J |
| **[操作系统](#操作系统)** | 你所写的代码，基本上都由操作系统来运行，因此你应当了解其运作的原理。 | _《操作系统导论》_ | Berkeley CS 162 |
| **[计算机网络](#计算机网络)** | 互联网已然势不可挡：理解工作原理才能解锁全部潜力。 | _《计算机网络：自顶向下方法》_ | Stanford CS 144 |
| **[数据库](#数据库)** | 对于多数重要程序，数据是其核心，然而很少人理解数据库系统的工作原理。 | _Readings in Database Systems （暂无中译本）_ | Joe Hellerstein’s Berkeley CS 186 |
| **[编程语言与编译器](#编程语言与编译器)** | 若你懂得编程语言和编译器如何工作，你就能写出更好的代码，更轻松地学习新的编程语言。| _《编译原理》_ | Alex Aiken’s course on Lagunita |
| **[分布式系统](#分布式系统)** | 如今，_多数_ 系统都是分布式的。 | _《分布式系统原理与范型》，第三版_  Maarten van Steen著 | 🤷‍ |

## 为什么要学习计算机科学？

软件工程师分为两种：一种充分理解了计算机科学，从而有能力应对充满挑战的创造性工作；另一种仅仅凭着对一些高级工具的熟悉而勉强应付。

这两种人都自称软件工程师，都能在职业生涯早期挣到差不多的工资。然而，随着时间流逝，第一种工程师不断成长，所做的事情将会越来越有意义且更为高薪，不论是有价值的商业工作、突破性的开源项目、技术上的领导力或者高质量的个人贡献。

> 全球短信系统每日收发约200亿条信息，而仅仅靠57名工程师，现在的 WhatsApp 每日收发420亿条。 
>
> — Benedict Evans (@BenedictEvans) [2016年2月2日](https://twitter.com/BenedictEvans/status/694342874729545729)

第一种工程师总是寻求深入学习计算机科学的方法，或是通过传统的方法学习，或是在职业生涯中永无止息地学习；第二种工程师
通常浮于表面，只学习某些特定的工具和技术，而不研究其底层的基本原理，仅仅在技术潮流的风向改变时学习新的技能。

如今，涌入计算机行业的人数激增，然而计算机专业的毕业生数量基本上未曾改变。第二种工程师的供过于求正在开始减少他们的工作机会，使他们无法涉足行业内更加有意义的工作。对你而言，不论正在努力成为第一种工程师，还是只想让自己的职业生涯更加安全，学习计算机科学是唯一可靠的途径。

> 23333 然而他们... [pic.twitter.com/XVNYlXAHar](https://t.co/XVNYlXAHar)
>
> — Jenna Bilotta (@jenna) [2017年3月4日](https://twitter.com/jenna/status/838161631662092289)


## 分科目指引

### 编程

大多数计算机专业本科教学以程序设计“导论”作为开始。这类课程的最佳版本不仅能满足初学者的需要，还适用于那些在初学编程阶段遗漏了某些有益的概念和程序设计模式的人。

对于这部分内容，我们的标准推荐是这部经典著作：《计算机程序的构造和解释》。在网络上，这本书既可供[免费阅读（英文版）](https://mitpress.mit.edu/sites/default/files/sicp/full-text/book/book.html)，也作为[MIT的免费视频课程](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-001-structure-and-interpretation-of-computer-programs-spring-2005/video-lectures/)。不过尽管这些视频课程很不错，我们对于视频课程的推荐实际上是[Brian Harvey 开设的 SICP 课程](https://archive.org/details/ucberkeley-webcast-PL3E89002AA9B9879E?sort=titleSorter)（即 Berkeley 的 61A 课程）。比起MIT的课程，它更加完善，更适用于初学者。

我们建议至少学完SICP的前三章，并完成配套的习题。如果需要额外的练习，可以去解决一些小的程序设计问题，比如[exercism](http://exercism.io)。

如果你觉得SICP过于难，那我们推荐 _[How to Design Programs](http://www.htdp.org/)_ ；如果你觉得SICP过于简单，那我们推荐 _[Concepts, Techniques, and Models of Computer Programming](https://smile.amazon.com/Concepts-Techniques-Models-Computer-Programming/dp/0262220695/)_ 。

### 计算机架构

计算机架构——有时候又被称为“计算机系统”或者“计算机组成”——是了解软件底层的的重要视角。根据我们的经验，这是自学的软件工程师最容易忽视的领域。

_The Elements of Computing Systems_，又名“从与非门到俄罗斯方块”（“Nand2Tetris”），这本书规模宏大，让读者对计算机内的所有部分如何协同工作有完全的认识。这本书的每一章节对应如何构建计算机整体系统中的一小部分，
从用HDL（硬件描述语言）写基本的逻辑门电路出发，途经CPU和汇编，最终抵达诸如俄罗斯方块这般规模的应用程序。

我们推荐把此书的前六章读完，并完成对应的项目练习。这么做，你将更加深入地理解，计算机架构和运行其上的软件之间的关系。

这本书的前半部分（包括所有对应的项目）均可从[Nand2Tetris的网站上](http://www.nand2tetris.org)免费获得。同时，在Coursera上，这是一门[视频课程](https://www.coursera.org/learn/build-a-computer)。

为了追求简洁和紧凑，这本书牺牲了内容上的深度。尤其值得注意的是，流水线和存储层次结构是现代计算机架构中极其重要的两个概念，然而这本书对此几乎毫无涉及。

当你掌握了Nand2Tetris的内容后，我们接下来推荐Patterson和Hennessy二人所著的 _[《计算机组成与设计》](https://smile.amazon.com/Computer-Organization-Design-Fifth-Architecture/dp/0124077269)_，一本优秀的经典著作。这本书中的不同章节重要程度不一，因此我们建议根据Berkeley的[CS61C课程](http://inst.eecs.berkeley.edu/~cs61c/sp15/) “计算机架构中的伟大思想”来着重阅读一些章节。这门课的笔记和实验在网络上可以免费获得，并且在[互联网档案](https://archive.org/details/ucberkeley-webcast-PL-XXv-cvA_iCl2-D-FS5mk0jFF6cYSJs_)中有这门课程的过往资料。

[![Elements of Computing Systems](https://teachyourselfcs.com/elements-computing-systems.jpg)](http://www.nand2tetris.org) 

> 硬件是平台。
>
> — Mike Acton, Engine Director at Insomniac Games
([观看他在CppCon上的演说](https://www.youtube.com/watch?v=rX0ItVEVjHc))

### 算法与数据结构

正如几十年来的共识，我们认为，计算机科学教育所赋予人们的最大能量在于对常见算法和数据结构的熟悉。此外，这也可以训练一个人对于各种问题的解决能力，有助于其他领域的学习。

关于算法与数据结构，有成百上千的书可供使用，但是我们的最爱是Steven Skiena编写的 _[《算法设计手册》](https://smile.amazon.com/Algorithm-Design-Manual-Steven-Skiena/dp/1848000693/)_。显而易见，他对此充满热爱，迫不及待地想要帮助其他人理解。在我们看来，这本书给人一种焕然一新的体验，完全不同于那些更加经常被推荐的书（比如Cormen，Leiserson，Rivest 和 Stein，或者 Sedgewick的书，后两者充斥着过多的证明，不适合以 _解决问题_ 为导向的学习）。

如果你更喜欢视频课程，[Skiena慷慨地提供了他的课程](https://www.youtube.com/watch?v=A2bFN3MyNDA&list=PLOtl7M3yp-DX32N0fVIyvn7ipWKNGmwpp)。此外，Tim Roughgarden的课程也很不错，
在Stanford的MOOC平台Lagunita，或者[Coursera](https://www.coursera.org/specializations/algorithms)上均可获得。Skiena和Roughgarden的这两门课程没有优劣之分，选择何者取决于个人品味。

至于练习，我们推荐学生在[Leetcode](https://leetcode.com)上解决问题。Leetcode上的问题往往有趣且带有良好的解法和讨论。此外，在竞争日益激烈的软件行业，这些问题可以帮助你评估自己应对技术面试中常见问题的能力。我们建议解决大约100道随机挑选的Leetcode问题，作为学习的一部分。

最后，我们强烈推荐 _[How to Solve It](https://smile.amazon.com/How-Solve-Mathematical-Princeton-Science/dp/069116407X/)_。这本书极为优秀且独特，指导人们解决广义上的问题，因而一如其适用于数学，它适用于计算机科学。

[![算法设计手册](https://teachyourselfcs.com/skiena.jpg)](https://smile.amazon.com/Algorithm-Design-Manual-Steven-Skiena/dp/1848000693/) [![How to Solve It](https://teachyourselfcs.com/polya.jpg)](https://smile.amazon.com/How-Solve-Mathematical-Princeton-Science/dp/069116407X/) 

> 我可以广泛推荐的方法只有一个： 写之前先思考。
>
>— Richard Hamming

### 数学知识

从某个角度说，计算机科学是应用数学的一个“发育过度”的分支。尽管许多软件工程师试图——并且在不同程度上成功做到——忽视这一点，我们鼓励你用学习来拥抱数学。如若成功，比起那些没有掌握数学的人，你将获得巨大的竞争优势。

对于计算机科学，数学中最相关的领域是“离散数学”，其中的“离散”与“连续”相对立，大致上指的是应用数学中那些有趣的主题，而不是微积分之类的。由于定义比较含糊，试图掌握离散数学的全部内容是没有意义的。较为现实的学习目标是，了解逻辑、排列组合、概率论、集合论、图论以及密码学相关的一些数论知识。考虑到线性代数在计算机图形学和机器学习中的重要性，该领域同样值得学习。

学习离散数学，我们建议从[László Lovász的课程笔记](http://www.cs.elte.hu/~lovasz/dmbook.ps)开始。Lovász教授成功地让这些内容浅显易懂且符合直觉，因此，比起正式的教材，这更适合初学者。

对于更加高阶的学习，我们推荐 _[《计算机科学中的数学》](https://courses.csail.mit.edu/6.042/spring17/mcs.pdf)_，MIT同名课程的课程笔记，篇幅与书籍相当。这门课程的视频同样[可免费获得](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-042j-mathematics-for-computer-science-fall-2010/video-lectures/)，是我们所推荐的学习视频。

对于线性代数，我们建议从[Essence of linear algebra](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab)系列视频开始，然后再去学习Gilbert Strang的[著作](https://www.amazon.com/Introduction-Linear-Algebra-Gilbert-Strang/dp/0980232775/)和[视频课程](https://ocw.mit.edu/courses/mathematics/18-06-linear-algebra-spring-2010/video-lectures/)。

> 如果人们不相信数学是简单的，那么只能是因为他们没有意识到生活有多么复杂。
>
>— John von Neumann

### 操作系统

_[《操作系统概念》](https://www.amazon.com/dp/1118063333/)_ （“恐龙书”）和 _[《现代操作系统》](https://www.amazon.com/dp/013359162X/)_ 是操作系统领域的经典书籍。二者都因为写作风格，长达1000页的篇幅以及每隔几年就增加内容来鼓励人们购买“最新版本”招致了一些批评。

_《操作系统导论》（Operating Systems: Three Easy Pieces）_ 是一个不错的替代品，并且[可在网上免费获得](http://pages.cs.wisc.edu/~remzi/OSTEP/)。我们格外喜欢这本书的结构，并且认为这本书的习题很值得一做。

在读完《操作系统导论》后，我们鼓励你探索特定操作系统的设计。可以借助“{OS name} Internals”风格的书籍，比如 _[Lion's commentary on Unix](https://www.amazon.com/Lions-Commentary-Unix-John/dp/1573980137/)_， _[The Design and Implementation of the FreeBSD Operating System](https://www.amazon.com/Design-Implementation-FreeBSD-Operating-System/dp/0321968972/)_，以及 _[Mac OS X Internals](https://www.amazon.com/Mac-OS-Internals-Systems-Approach/dp/0321278542/)_。

为了巩固对操作系统的理解，阅读小型系统内核的代码并且为其增加特性是一个很不错的方法。比如，[xv6](https://pdos.csail.mit.edu/6.828/2016/xv6.html)，由MIT的一门课程所维护的从Unix V6到ANSI C和x86的移植，就是一个很棒的选择。《操作系统导论》有一个附录，记载了一些可能的[xv6实验项目](http://pages.cs.wisc.edu/~remzi/OSTEP/lab-projects-xv6.pdf)，其中充满了关于潜在项目的很棒想法。

### 计算机网络

鉴于有那么多关于网络服务端和客户端的软件工程，计算机网络是计算机科学中价值最为“立竿见影”的领域之一。我们的学生，系统性地学习了计算机网络，最终能够理解那些曾困扰他们多年的术语、概念和协议。

在这一主题上，我们最爱的书籍是 _[《计算机网络：自顶向下方法》](https://smile.amazon.com/Computer-Networking-Top-Down-Approach-7th/dp/0133594149/)_。书中的小项目和习题相当值得练习，尤其是其中的“Wireshark labs”（[这部分在网上可以获得](http://www-net.cs.umass.edu/wireshark-labs/)）。

如果更喜欢视频课程，我们推荐Stanford的[_Introduction to Computer Networking_](https://lagunita.stanford.edu/courses/Engineering/Networking-SP/SelfPaced/about)，可在他们的MOOC平台Lagunita上免费观看。

对于计算机网络的学习，做项目比完成小的习题更有益。一些可能的项目有：HTTP服务器，基于UDP的聊天APP，[迷你TCP栈](http://jvns.ca/blog/2014/08/12/what-happens-if-you-write-a-tcp-stack-in-python/)，代理，负载均衡器，或者分布式哈希表。

> 你无法盯着水晶球预见未来，未来的互联网何去何从取决于社会。
>
>— Bob Kahn

[![《计算机网络：自顶向下方法》](https://teachyourselfcs.com/top-down.jpg)](https://smile.amazon.com/Computer-Networking-Top-Down-Approach-7th/dp/0133594149/) 

### 数据库

比起其他主题，自学数据库系统需要更多的付出。这是一个相对年轻的研究领域，并且出于很强的商业动机，研究者把想法藏在紧闭的门后。此外，许多原本有潜力写出优秀教材的作者反而选择了加入或创立公司。

鉴于如上情况，我们鼓励自学者大体上抛弃教材，而是从[2015年春季学期的CS 186课程](https://archive.org/details/UCBerkeley_Course_Computer_Science_186)（Joe Hellerstein在Berkeley的数据库课程）开始，然后前往阅读论文。

对于初学者，有一篇格外值得提及的论文：“[Architecture of a Database System](http://db.cs.berkeley.edu/papers/fntdb07-architecture.pdf)”。这篇论文提供了独特的对关系型数据库管理系统（RDBMS）如何工作的高层次观点，是后续学习的实用梗概。

_Readings in Database Systems_，或者以[数据库“红书”](http://www.redbook.io/)更为人知，是由Peter Bailis，Joe Hellerstein和Michael Stonebraker编纂的论文合集。对于那些想要在CS 186课程的水平更进一步的学习者，“红书”应当是下一步。

如果你坚持一定要一本导论教材，那我们推荐Ramakrishnan和Gehrke所著的 _[Database Management Systems](https://smile.amazon.com/Database-Management-Systems-Raghu-Ramakrishnan/dp/0072465638/)_。如需更深一步，Jim Gray的经典著作 _[Transaction Processing: Concepts and Techniques](https://www.amazon.com/Transaction-Processing-Concepts-Techniques-Management/dp/1558601902)_ 值得一读，不过我们不建议把这本书当作首要资源。

如果没有编写足够数量的代码，很难巩固数据库理论。CS 186课程的学生给Spark添加特性，倒是不错的项目，不过我们仅仅建议从零实现一个简单的关系型数据库管理系统。自然，它将不会有太多的特性，但是即便只实现典型的关系型数据库管理系统每个方面最基础的功能，也是相当有启发的。

最后，数据模型往往是数据库中一个被忽视的、教学不充分的方面。关于这个主题，我们推荐的书籍是 _[Data and Reality: A Timeless Perspective on Perceiving and Managing Information in Our Imprecise World](https://www.amazon.com/Data-Reality-Perspective-Perceiving-Information/dp/1935504215)_。

### 编程语言与编译器

多数程序员学习编程语言的知识，而多数计算机科学家学习编程语言 _相关_ 的知识。这使得计算机科学家比起程序员拥有显著的优势，即便在编程领域！因为他们的知识可以推而广之：相较只学习过特定编程语言的人，他们可以更深入更快速地理解新的编程语言。

权威的导论书籍是 _[《编译原理》](https://smile.amazon.com/Compilers-Principles-Techniques-Tools-2nd/dp/0321486811)_，通常称为“龙书”。不幸的是，这本书不是为自学者而设计的，而是供教师从中挑选一些主题用于1-2学期的教学。因此十分重要的是，你需要从中甄选主题，而且最好是在导师的帮助下。

如果你选择使用龙书进行自学，我们建议依据某个视频课程来设定学习的结构，然后按需从龙书中获取深入的内容。我们推荐的在线课程是[Alex Aiken在Stanford的MOOC平台Lagunita所开设的](https://lagunita.stanford.edu/courses/Engineering/Compilers/Fall2014/about)。

我们所推荐的龙书替代品是Terence Parr所著的 _[Language Implementation Patterns](https://smile.amazon.com/Language-Implementation-Patterns-Domain-Specific-Programming/dp/193435645X/)_。这本书更加直接地面向那些想要着手于诸如DSL的小型编程语言项目的软件工程师，因此从你的角度来看可能会更加实用。当然，这样做牺牲了一些有价值的理论内容。

对于项目练习，我们建议为诸如COOL的简单教学语言或者你所感兴趣的某个语言的一个子集写一个编译器。如果感觉这样的项目让人生畏，可以先从[Make a Lisp](https://github.com/kanaka/mal)开始，在一步步的指引下完成项目。

[![《编译原理》](https://teachyourselfcs.com/dragon.jpg) ](https://smile.amazon.com/Compilers-Principles-Techniques-Tools-2nd/dp/0321486811) [![Language Implementation Patterns](https://teachyourselfcs.com/parr.jpg)](https://smile.amazon.com/Language-Implementation-Patterns-Domain-Specific-Programming/dp/193435645X/) 

> 不要做一个只写样板代码的程序员。相反，给用户和其他程序员创造工具。从纺织工业和钢铁工业中学习历史教训：你想制造机器和工具，还是操作这些机器？
>
>— Ras Bodik 在他的编译器课程伊始

### 分布式系统

随着计算机在数量上的增加，计算机同样开始 _分散_。尽管商业公司过去愿意购买越来越大的大型机，现在的典型情况是，甚至很小的应用程序都同时在多台机器上运行。思考这样做的利弊权衡，即是分布式系统的研究所在，也是越来越重要的一项技能。

对于自学者，我们推荐的教材是Maarten van Steen和Andrew Tanenbaum所著的 _[《分布式系统原理与范型》（第三版）](https://www.distributed-systems.net/index.php/books/distributed-systems-3rd-edition-2017/)_。相较之前的版本，第三版有巨大的改进，并且多亏了其作者的慷慨，这本书在网上可以免费获得。考虑到分布式系统是一个迅速变化的领域，没有教材可以完全作为路标指引，不过就我们所见，这本书是基础扎实的最佳总览。

[MIT的6.824](https://www.youtube.com/watch?v=hBWfjkGKRas&list=PLkcQbKbegkMqiWf7nF8apfMRL4P4sw8UL)（研究生课程）是一门在网络有部分视频的优秀课程，不过不幸的是，录像中的声音质量很差，并且不确定这些录像是否经过许可。

不管选择怎样的教材或者其他辅助资料，学习分布式系统必然要求阅读论文。[这里](http://dsrg.pdos.csail.mit.edu/papers/)有一个不错的论文清单，而且我们强烈建议你出席你当地的[Papers We Love](http://paperswelove.org/)（仅限美国）。

## 常见问题解答

### 人工智能/计算机图形学/XX主题怎么样？

我们试图把计算机科学主题清单限制到那些我们认为 _每一个软件工程师_ 都应该了解的内容，不限于专业或行业。拥有了这些基础，你将能更加轻松地挑选教材或论文，然而无需指引地学习核心概念。在这里，我们给出一些其他常见主题的自学起点：

*   人工智能：通过观看视频并完成Pacman项目来学习[Berkeley的AI课程](http://ai.berkeley.edu/)。至于教材，使用Russell和Norvig编写的 _《人工智能：一种现代方法》_。
*   机器学习：学习吴恩达在Coursera上的课程。耐心学习，先确保理解了基础概念再奔向类如深度学习的诱人新主题。
*   计算机图形学：学习[Berkeley CS 184课程](http://inst.eecs.berkeley.edu/~cs184/fa12/onlinelectures.html)的材料，使用[Computer Graphics: Principles and Practice](https://www.amazon.com/Computer-Graphics-Principles-Practice-3rd/dp/0321399528)作为教材。

### 一定要严格遵守推荐的学习次序吗？

事实上，所有主题之间都有一定程度的重叠，彼此循环引用。以离散数学和算法的关系为例：先学习数学可以帮助你更深入地分析和理解算法，然而先学习算法可以为学习离散数学提供更大的动力和应用背景。理想情况下，你将在你的职业生涯多次重温二者。

因此，我们所推荐的次序主要是为了帮助你 _起步_……如果你出于某种强烈的原因而倾向以不同的顺序学习，那也没有关系，勇敢开始吧！不过在我们看来，最重要的“先决条件”是：先学计算机架构再学操作系统或数据库，先学计算机网络和操作系统再学分布式系统。

### 这份指引的目标受众是？

我们面向自学的软件工程师、培训班学生、“早熟的”高中生或者想要通过自学补充正式教育的大学生。关于何时开启这段自学旅程，完全取决于个人，不过多数人在有一定的职业经历后深入学习计算机科学理论会获益匪浅。比如，我们注意到，如果学生在工作中曾经使用过数据库，他们会 _喜爱_ 学习数据库系统课程；如果学生从事过一两个Web项目，他们会 _喜爱_ 学习计算机网络。

### 和Open Source Society、freeCodeCamp curricula等比起来，这份指引?

[OSS指引](https://github.com/open-source-society/computer-science)涵盖太多主题，在许多主题中推荐劣质资源，没有就特定课程哪些方面有价值提供原因或指引。我们努力对这份指引中的课程加以限制，仅仅包括那些你作为软件工程师 _确实需要了解的_，不论你的专业方向，并且对每门课程为何必要做出了解释以帮助你理解。

FreeCodeCamp主要关注编程，而不是计算机科学。至于你为什么要学习计算机科学，参见[上文](#为什么要学习计算机科学？)。

### XX编程语言怎么样?

学习一门特定的编程语言和学习计算机科学的一个领域完全不在一个维度——相比之下，学习语言 _容易_ 且 _缺乏价值_。如果你已经了解了一些语言，我们强烈建议遵照我们的指引，然后在学习的空当中习得语言，或者暂且不管以后再说。如果你已经把编程学得不错了（比如学完了 _《计算机程序的构造和解释》_），尤其是如果你学习过编译器，那么面对一门新的语言，你只需要花一个周末稍多的时间即可基本掌握。

### XX流行技术怎么样?

没有任何一种技术的重要程度可以达到学习其使用足以成为计算机科学教学的核心部分。不过，你对学习那门技术充满热情，这很不错。诀窍是先从特定的技术回退到基本的领域或概念，判断这门流行技术在技术的宏观大局中位于何处，然后才深入学习这门技术。

### 为什么你们还在推荐龙书?

龙书依旧是内容最为完整的编译器单本书籍。由于过分强调一些如今不够时新的主题的细节，比如解析，这本书招致了恶评。然而事实上，这本书从未打算供人一页一页的学习，而仅仅是为了给教师准备一门课程提供足够的材料。类似地，自学者可以从书中量身按需挑选主题，或者最好依照公开课授课教师在课程大纲中的建议。

### 如何便宜获取教材?

我们所建议的许多教材在网上都可以免费获得，这多亏了作者们的慷慨。对于那些不免费的书籍，我们建议购买旧版本的二手书籍。广而言之，如果一本教材有多个版本，旧版本大概率是完全足够使用的。即便新版本的价格是旧版本的10倍，新版本也绝不可能比旧版本好10倍！

### 这份指引是谁写的?

这份指引由[Bradfield School of Computer Science](https://bradfieldcs.com)（旧金山）的两位教员：[Ozan Onay](https://twitter.com/oznova_)和[Myles Byrne](https://twitter.com/quackingduck)编写。这份指引基于我们对数百名自学成才的工程师和培训班学生教授计算机科学基础的经验。感谢我们所有学生对自学资源的持续反馈。同样感谢Alek Sharma，Omar Rayward，Ammar Mian和Tyler Bettilyon对这份指引的反馈。

### 这份指引是谁翻译的？

这份指引的中文翻译是[社区共同贡献的成果](https://github.com/keithnull/TeachYourselfCS-CN/)，我们欢迎任何反馈和改进！
