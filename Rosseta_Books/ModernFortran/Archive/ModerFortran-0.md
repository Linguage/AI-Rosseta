
![封面](Archive/Figures_0/截屏2024-02-21%2016.25.34.png)

# 前言

得知米兰·库尔奇克将要写一本现代Fortran的书，我立刻感到兴奋。几乎每周，我都会遇到人们对于Fortran在其诞生60多年后仍然在使用感到惊讶，因此，任何对一个经常被认为已经死亡或濒临消亡的语言出现新生机的迹象都是值得庆祝的。我通常会解释说，Fortran在早期接受计算机的领域中占据着最强大的地位。我会继续告诉他们，当他们每天检查天气预报时，几乎肯定会使用Fortran程序的结果。米兰的工作之所以令人着迷，是因为它将长期以来Fortran占据主导地位的已建立领域与Fortran稀缺的新兴领域联系起来。这本书源于米兰独特的视角，他一直致力于弥合阻止许多学科写作Fortran的鸿沟，并阻止大多数Fortran程序员利用其他语言中已广泛使用的编程范式。

值得赞扬的是，这本书侧重于教授Fortran编程，而不是推广他所贡献的有趣的软件库和应用程序。那些跟随他的工作以及其他人的链接的幸运读者将获得的不仅仅是对Fortran编程的理解。这样的读者将踏上一段旅程，将数值天气预报（作为一门与计算同样古老的学科）与云计算（二十一世纪的创新）联系起来。这样的读者还将发现如何在Fortran中融入函数式编程的方面，这是一个整个语言都围绕着建立的编程范式，而Fortran则是所有高级编程语言的最终祖先。这样的读者还将暴露于神经网络的知识中，这是一个正在经历爆炸式增长并影响着诸如自动驾驶和癌症诊断等截然不同的技术的领域。

米兰在这些领域中领导或贡献了一些流行的软件，其中一些软件包源于这本书，或者反之亦然。例如，他与他人共同开发的服务Cloudrun[(https://cloudrun.co)](https://cloudrun.co)开创了使用云计算平台进行数值天气预报软件即服务（SaaS）的先河。开源的functional-fortran库[(http://mng.bz/vxy1)](http://mng.bz/vxy1)提供了支持一种编程范式的实用工具，这种编程范式在Fortran世界中的普及程度不如我所希望的那样高。开源的Fortran标准库[（https://github.com/fortran-lang/stdlib）](https://github.com/fortran-lang/stdlib)旨在使Fortran与其他语言更加平等，这些语言受益于被视为语言一部分的大型库。他的neural-fortran[（https://github.com/modern-fortran/neural-fortran）](https://github.com/modern-fortran/neural-fortran)是从他在本书的一章中的工作中发展而来的，它展示了Fortran可扩展并行编程模型在一个由缺乏内置并行编程模型以利用分布式内存平台的语言主导的领域中的应用。总的来说，这些项目被全球数百名开发人员使用，他在这本书上的工作与这些项目的工作相互影响和启发了书中对语言的覆盖。

对于寻求现代Fortran生机的读者，米兰的工作为这种语言在技术现代化中持续发挥作用提供了充分的证据。这本书是他工作中生长出的更有活力的芽之一，感兴趣的读者将学到在米兰的广泛项目组合中已被证明有用的语言特性。 

> ——DAMIAN ROUSON，
>
> 博士，P.E. 董事长，Sourcery Institute，加利福尼亚州奥克兰，美国

# 序言

2017年夏天，曼宁出版社的迈克·斯蒂芬斯（Mike Stephens）首次与我联系时写道：“我们看到了你的一些论坛帖子和GitHub仓库；你考虑过和曼宁一起写一本Fortran书吗？”写书从未在我的脑海中出现过，我也不认为自己适合这个工作。我闭上眼睛，做了一个信任的飞跃。“当然，我很愿意！我把提案发送到哪里呢？”夏天结束时，我们签订了合同，并制定了初步的目录。经过两名开发编辑、两名技术编辑、四次同行评审、三次章节重写、两次飓风的影响，以及将近三年的时间，我们完成了这本书。

欢迎来到《现代Fortran：构建高效的并行应用》！如果你拿着这本书，很可能你要么想要学习Fortran编程以应对学校或工作的需要，要么你是一位经验丰富的Fortran程序员，想要了解该语言的最新发展。无论哪种情况，你来对地方了。如果你刚开始学习，我希望这本书能为你提供一种简单、动手实践的实用Fortran编程方法。如果你已经有了使用该语言的经验，我希望这本书能成为你在Fortran世界中的实用指南。忘记如何编写既能操作标量又能操作数组的函数了吗？想知道如何为并行执行编写程序？这里有实用的项目和练习，以及解决方案，来帮助你理解。

我很高兴有机会与你分享我在过去14年里学到的东西。提前感谢你信任我，花费时间和金钱阅读这本书。《现代Fortran》是我回报给那些教导我、帮助过我的人的方式。我希望你能利用这本书来培养下一代Fortran程序员。


# 致谢

要完成一本优秀的书籍，需要整个团队的努力。迈克·斯蒂芬斯是采编编辑，他邀请我加入，并帮助制定了目录，确定了这本书的读者群。我的开发编辑克里斯汀·瓦特森（Kristen Watterson）和莱斯利·特里特斯（Lesley Trites）在整个过程中给予我指导，并不懈地推动我前进。克里斯汀与我一起起草了九章的初稿；然后莱斯利接手了剩下的工作，并将所有内容整合在一起。技术编辑米歇尔·特里姆普（Michiel Trimpe）和阿兰·库尼奥（Alain Couniot）确保指出了代码中的任何错误和令人困惑的段落。伯特·贝茨（Bert Bates）偶尔会加入，帮助我从抽象中提炼出具体内容。毛里齐奥·托马西（Maurizio Tomasi）是技术校对员，确保书中的所有代码都能正常运行。梅洛迪·多拉布（Melody Dolab）担任最终校对，洛里·韦德特（Lori Weidert）担任制作编辑。还要感谢曼宁其他与我合作的工作人员：坎迪斯·吉尔胡利（Candace Gillhoolley）、安娜·罗马克（Ana Romac）、雷哈娜·马尔卡诺维奇（Rejhana Markanovic）、亚历山大·德拉戈萨维里耶维奇（Aleksandar Dragosavljevic）、马特科·赫瓦汀（Matko Hrvatin）等等。谢谢你们，我从你们身上学到了很多。

我还要感谢所有的审阅者：安德斯·约翰松（Anders Johansson）、安东·门舒夫（Anton Menshov）、布里奇尔·豪威尔（Bridger Howell）、大卫·克莱门斯（David Celements）、达维德·卡达穆罗（Davide Cadamuro）、弗雷德里克·拉格纳（Fredric Ragnar）、简·皮特·赫韦尔（Jan Pieter Herweijer）、何塞·圣莱安德罗（Jose San Leandro）、约瑟夫·伊恩·沃克（Joseph Ian Walker）、卡纳克·克谢特里（Kanak Kshetri）、肯·W·阿尔杰（Ken W. Alger）、康拉德·欣森（Konrad Hinsen）、凯尔·曼德利（Kyle Mandli）、莱昂纳多·科斯塔·普劳奇纳（Leonardo Costa Prauchner）、洛蒂·格林伍德（Lottie Greenwood）、路易斯·穆·多明格斯（Luis MouxDomínguez）、马尔西奥·尼科劳（Marcio Nicolau）、马丁·比尔（Martin Beer）、马修·埃米特（Matthew Emmett）、毛里齐奥·托马西（Maurizio Tomasi）、迈克尔·詹森（Michael Jensen）、米哈尔·康拉德·奥维亚克（Michal Konrad Owsiak）、米克尔·阿伦托夫特（Mikkel Arentoft）、翁德雷·切尔蒂克（Ondrˇej Cˇertík）、帕特里克·西沃尔德（Patrick Seewald）、理查德·菲尔森德（Richard Fieldsend）、瑞安·B·哈维（Ryan B. Harvey）、斯尔德扬·桑蒂奇（Srdjan Santic）、斯蒂法诺·博里尼（Stefano Borini）、蒂齐亚诺·穆勒（Tiziano Müller）、汤姆·格思（Tom Gueth）、瓦尔米基·阿奎萨达斯（Valmiky Arquissandas）以及文森特·扎巴拉（Vincent Zaballa）。你们的建议帮助了这本书的完善。

阿尔扬·马库斯（Arjen Markus）在曼宁早期访问计划中，每当新章节发布时都提供了详尽的审阅和建议。伊萨克·比克曼（Izaak Beekman）、雅各布·威廉姆斯（Jacob Williams）、马库斯·范利尔-瓦尔奎（Marcus Van Lier-Walqui）和史蒂夫·利奥内尔（Steve Lionel）在书的初稿阶段提供了有益的评论。达米安·鲁森（Damian Rouson）及其自己的书籍给了我启发，并在我前进的道路上给予了进一步的鼓励。迈克尔·赫希（Michael Hirsch）帮助我持续集成了与本书相关的一些GitHub仓库。最后，感谢所有在书还在编写过程中就信任我并购买了这本书的读者们——你们帮助我坚持下去，完成了这项工作。最后但同样重要的是，感谢我的妻子、家人和朋友们的支持和鼓励——没有你们的爱和帮助，我无法完成这个任务。

# 关于本书

《现代Fortran》旨在填补现有Fortran文献中的一大空白：通过实际的动手示例，特别关注并行编程和语言最新发展，教授现代Fortran。这是一本为科学家和工程师准备的书籍，他们希望使用成熟、高性能、易于使用的技术解决明天的复杂计算问题。如果你对Fortran一无所知，但想要参与Fortran项目（新项目或现有项目），我相信这本书是让你快速上手的最简单、最快的方式。

《现代Fortran》并不是关于语言所有特性的完整参考资料。相反，它是一本直接、实用的Fortran编程课程，涵盖了你在工作中可能会使用到的最基本的特性。我还希望这本书能成为解决科学和工程中实际日常问题的有用参考文本。本书的示例涵盖了从一般性的，如记笔记应用和处理日期和时间；到专业化的，比如股票价格和天气数据分析；再到更复杂的，比如并行海啸模拟。你将在这本书中找到许多其他Fortran书籍通常不涵盖的示例和问题解决方案。

此外，与大多数其他Fortran书籍不同，本书还特别关注并行编程。自2008年发布以来，Fortran是一种本地并行编程语言，最近的2018年版本带来了更多新特性。特别是，本书将向你展示如何使用共组、团队、事件和集合编写并行Fortran程序，而不依赖于诸如消息传递接口（MPI）之类的外部库。

然而，并行编程是一个高级话题，本书的大多数章节都着重于温和地介绍非并行语言概念。一本书能涵盖的内容是有限的，因此重要的主题，比如并行算法和扩展性，都没有涵盖进来。消息传递接口（MPI）、OpenMP和OpenACC，虽然都是非常重要的技术，但它们超出了本书的范围。同样，调试、预处理器和处理遗留代码也没有涵盖进来。我会在适当的时候提供进一步阅读的参考资料。

## 适合阅读本书的人群

本书主要适合那些想要学习Fortran的新手读者。对于有经验的Fortran程序员来说，通过有趣的练习来了解Fortran的最新发展也会很有帮助。无论你是否接触过Fortran，我假设你至少具有一定的编程经验，并理解源代码、变量和函数的基本概念。也许你是一位熟练的Fortran程序员，希望提升自己的并行编程能力。也许你的公司正在将一个庞大的Fortran模拟代码库嵌入到现有的软件堆栈中，而这个项目就落在了你的手上。无论你的情况如何，我相信你会从本书中学到一些新东西。我相信以下专业人士将从本书中获益最多：

- 在科学或工程领域的学生和研究人员，特别是涉及计算流体动力学的学科；
- 气象学家、海洋学家和气候科学家，特别是那些从事数值预测问题研究的人员；
- 数据分析专业人士，如数据工程师和数据科学家；
- 机器学习研究人员和实践者；
- 量化金融分析师；
- 高性能计算系统管理员；
- 上述任何学科的教师和讲师，以及对编程语言和计算感兴趣的其他人。

## 一点Fortran历史

Fortran是一种编译型、静态类型、通用编程语言。它由John Backus及其IBM团队开发，首次发布于1957年，用于IBM 704计算机。最初称为FORTRAN（FORmula TRANslation），与当时的机器指令相比，它使程序员能够更轻松地编写程序。Fortran是历史上第一批高级编程语言之一，也是今天仍在积极使用和发展的最古老的编程语言。从这个意义上说，Fortran是我们今天实践的现代计算的开端。

该语言经历了十多次修订和几个ISO标准的制定。Fortran仍然是高性能计算（HPC）的主导语言，在这里许多相互连接的处理器共同解决巨大的问题。Fortran 2018是该语言的最新版本。目前正在开发中的下一个修订版本，暂时以Fortran 202x为工作名称，预计将在未来几年内发布。

如今，Fortran是许多物理科学和工程领域中主要使用的编程语言。这些领域包括计算流体动力学、数值天气预报、气候科学、空气动力学、天体物理学等等。Fortran还被用于评估世界上最快、最大的超级计算机[https://top500.org](https://top500.org)。
许多大学仍然在科学和工程专业中教授Fortran编程，因为Fortran在这些行业仍然具有重要性。在过去20年里，随着互联网和移动技术的爆炸性增长，Fortran生态系统显然已经从主流计算的角度进入了阴影之中。然而，从绝对意义上来说，它的重要性从未减弱过。事实上，Fortran编译器、Fortran库以及其开源社区比以往任何时候都更加强大。Fortran是唯一具有本地并行编程模型的标准化语言，使用直观的类数组语法表达。随着当前向多核架构的趋势发展，可以肯定地说，Fortran在未来很多年里都将保持重要性。

## 本书组织结构：路线图

《现代Fortran》分为四个部分和十二章节：

- 第一部分—入门现代Fortran
  - 第1章将让你领略Fortran的味道，以及它最擅长解决哪些问题。
  - 第2章将引导你完成一个基本但完整的Fortran程序。

- 第二部分—Fortran的核心要素
  - 第3章将教你如何使用过程来简化和重用你的Fortran程序。
  - 第4章解释了如何在模块中组织你的过程和变量。
  - 第5章涵盖了数组和整体数组运算。
  - 第6章解决了输入和输出，以及将数值数据格式化为文本的问题。

- 第三部分—Fortran的高级应用
  - 第7章将向你展示如何使用图像和共组进行并行编程。
  - 第8章介绍了用于处理抽象和复杂数据结构的派生类型。
  - 第9章解释了如何编写可以处理任何数据类型参数的通用过程。
  - 第10章涵盖了派生类型的用户定义运算符。

- 第四部分—最后的冲刺
  - 第11章将教你如何从Fortran与现有的C库进行接口交互。
  - 第12章涵盖了高级并行编程概念：团队、事件和集合。

第一部分将让你初步了解Fortran。如果你是Fortran的新手，可以开始学习这一部分。即使你有一些Fortran经验，如果你想要跟着示例（一个海啸模拟器）学习，它会在第2章介绍。在第一部分结束时，你将能够编写、编译和运行基本的Fortran程序。

在第二部分，我将介绍语言的核心要素：过程（函数和子程序）、模块、数组和输入/输出。这些是大多数Fortran项目中都会涉及到的特性，对于编写清晰、有组织、可重用的代码至关重要。在第二部分结束时，你将能够编写更复杂的Fortran程序和库来解决实际问题。如果你精通一种或多种其他编程语言，可以从这里开始学习。在完成这一部分并获得一些实际经验后，你将成为一个功能完备、独立的Fortran程序员。

第三部分介绍了使用共组（第7章）进行并行编程，以及派生类型（第8章）、通用过程（第9章）和自定义运算符（第10章）。在这里，你将编写你的第一个并行程序，使用类来建模复杂的数据结构，并编写可以处理任何数据类型的通用过程。这一部分依赖于第二部分介绍的概念。请先熟悉这些概念。在完成第三部分后，你将能够理解、重用和扩展大部分现有的Fortran代码，以及编写创新的并行Fortran解决方案。这是本书最深入的部分，需要耐心和开放的思维方式。

最后，第四部分涵盖了专业主题：从Fortran中与C代码进行接口交互（第11章），以及最近添加到语言中的高级并行功能——团队、事件和集合（第12章）。前者对于将Fortran用于系统编程、网络编程、与仪器接口交互，或者重用现有的C库来执行任何任务都很重要。后者是Fortran中并行编程的前沿。我建议在熟悉第二部分和第三部分中涵盖的概念后再学习这些章节。

在组织不同章节和主题的顺序时，我们发现没有明显的答案。根据你的经验和兴趣，你可能会发现一些更基础的主题在书中后面才被涵盖。如果是这样，随时跳过去，稍后再回来学习。就像任何新的创作一样，这本书是一个实验。选择你自己的冒险之旅，做自己觉得好的事情。

## 关于代码

本书开发了大量源代码，主要组织在一个大型的运行示例（海啸模拟器）和几个小型项目中。本书中的所有代码都组织在Git仓库中，地址为[https://github.com/modern-fortran](https://github.com/modern-fortran)。海啸模拟器和小型项目各自有其自己的GitHub仓库，因此你可以独立地探索和调试它们。不属于任何单一项目的杂项示例和源代码清单都组织在“listings”仓库中，地址为[https://github.com/modern-fortran/listings](https://github.com/modern-fortran/listings)。我将这些项目作为活跃项目进行维护，因此如果你发现任何问题或对代码有疑问，请随时在相应的仓库中提出问题。

尽管所有的代码都可以下载，但我建议你在阅读本书时手动输入源代码。这样做可以让你熟悉Fortran的语法，并帮助你形成肌肉记忆。然而，如果你仍然想要只下载代码并运行它，当然可以。如果你熟悉Git，获取代码的最简单方式是从命令行克隆每个项目仓库。如果你没有Git或不想使用它，只需从仓库页面下载源代码的zip压缩包。每个项目中的README文件将指导你如何构建它。

本书包含许多源代码示例，包括编号清单、代码片段和嵌入在正文中的代码。在所有情况下，除了代码注释之外，源代码都以固定宽度的字体进行格式化，以使其与普通文本分隔开来。在许多情况下，原始源代码已经重新格式化；我们添加了换行符并重新调整了缩进，以适应书中的可用页面空间。此外，在文本中描述代码时，源代码中的注释通常会被移除。许多清单都带有代码注释，突出显示重要的概念。

## 环境要求

要完成本书的学习，你需要一台计算机，最好是运行Linux或macOS操作系统。如果你使用的是Windows 10，你可能已经可以访问Windows子系统用于Linux（WSL），它提供了一个本地的Linux环境，我建议你使用它。如果你使用的是较旧版本的Windows，我建议在你的系统上设置一个Linux虚拟机。Linux操作系统的优势在于它们专为软件开发而设计。在撰写本书时，我使用了Ubuntu 18.10（桌面）和Fedora 28（笔记本）。它们都非常适合Fortran开发。

你还需要对带有语法突出显示功能的文本编辑器有一定了解，以便阅读和编写源代码，并且要知道如何使用Linux/UNIX命令行来编译程序。在选择文本编辑器时，我是一个极简主义者，更喜欢Vim（Vi IMproved）。如果你喜欢更复杂的编辑器，如Sublime、Atom或VS Code，那也可以。毕竟，编辑器只是一种工具。选择一个能让你专注于实际工作的工具。你可以在附录A中找到有关文本编辑器的更多信息。

## 参与其中

如果你喜欢Fortran，并且本书激发了你的兴趣，考虑加入Fortran开源社区和/或标准委员会：

- 在互联网上关于Fortran的主页：[https://fortran-lang.org](https://fortran-lang.org)
- 在GitHub上关于Fortran的主页：[https://github.com/fortran-lang](https://github.com/fortran-lang)
- Fortran标准库：[https://github.com/fortran-lang/stdlib](https://github.com/fortran-lang/stdlib)
- Fortran包管理器：[https://github.com/fortran-lang/fpm](https://github.com/fortran-lang/fpm)
- 提交给Fortran标准委员会的提案：[https://github.com/j3-fortran/fortran_proposals](https://github.com/j3-fortran/fortran_proposals)
- 美国Fortran标准委员会：[https://j3-fortran.org](https://j3-fortran.org)
- 国际Fortran标准委员会：[https://wg5-fortran.org](https://wg5-fortran.org)

社区对所有怀有善意的新人都非常友好和开放。我们需要你的帮助，加入我们吧！

## liveBook讨论论坛

购买《现代Fortran：构建高效并行应用》(Modern Fortran: Building Efficient Parallel Applications)将免费获得Manning Publications运营的私人网络论坛的访问权限，在这里你可以对书籍发表评论，提出技术问题，并从作者和其他用户那里得到帮助。要访问论坛，请转到[https://livebook.manning.com/#!/book/modernfortran/discussion](https://livebook.manning.com/#!/book/modernfortran/discussion)。你也可以在[https://livebook.manning.com/#!/discussion](https://livebook.manning.com/#!/discussion)了解有关Manning论坛以及行为规范的更多信息。Manning对我们的读者的承诺是提供一个场所，让个体读者之间以及读者与作者之间进行有意义的对话。这不是对作者参与的特定数量的承诺，作者对论坛的贡献是自愿的（且不收费）。我们建议你尝试向作者提出一些具有挑战性的问题，以免他失去兴趣！只要本书在印刷中，论坛和先前讨论的存档将可以从出版商的网站访问。

# 作者简介

**米兰·库尔奇克（Milan Curcic）** 是一名气象学家和海洋学家。他在迈阿密大学研究海洋波浪和湍流，以及它们对数值天气和海洋预测的重要性。他还致力于在可扩展的计算云中实现数值天气预测。作为一名自2006年以来的Fortran程序员，他曾与美国海军和NASA的团队合作开发和改进地球系统预测模型。他撰写了几个开源的Fortran库，并与Fortran标准委员会合作开发下一代Fortran发布版及其标准库。米兰与妻子伊芙琳（Evelyn）和儿子诺兰（Nolan）居住在佛罗里达州博卡拉顿。你可以通过[https://milancurcic.com](https://milancurcic.com)了解更多信息并与他取得联系。

# 关于封面插图

《现代Fortran：构建高效并行应用》封面上的图案标题为“Ingrienne”，指的是历史地理区域Ingria的女性，该地区位于芬兰湾的南岸。这幅插图取自雅克·格拉塞·德·圣索维尔（Jacques Grasset de Saint-Sauveur，1757–1810）的一部作品，标题为《各国现代民俗服饰》，于1788年在法国出版。每幅插图都是精细绘制和手工上色的。格拉塞·德·圣索维尔收集的丰富多样的作品让我们生动地回想起200年前世界各地的城镇和地区在文化上是多么独立。人们彼此隔绝，说着不同的方言和语言。在街上或乡间，仅凭着他们的着装就可以轻易地辨别出他们住在哪里，以及他们的贸易或社会地位。

自那时以来，我们的着装方式已经发生了变化，当时如此丰富多样的地区多样性已经消失了。现在很难区分不同大陆的居民，更不用说不同的城镇、地区或国家了。也许我们以文化多样性换取了更丰富多样的个人生活——当然还有更丰富多样和快节奏的技术生活。

在很难区分一本计算机书籍与另一本计算机书籍的时代，曼宁出版社通过基于两个世纪前地区生活丰富多样性的封面图案，借助格拉塞·德·圣索维尔的插图，庆祝计算机业的创造力和主动性。
