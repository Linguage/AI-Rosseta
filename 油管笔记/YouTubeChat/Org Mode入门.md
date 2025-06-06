
- [Getting Started With Org Mode](https://www.youtube.com/watch?v=SzA2YODtgK4&t=1017s)
- [博主链接](https://www.youtube.com/@thoughtbot)


## 概述

这份文档是 Harry Schwarz（来自 thoughtbot）关于 Emacs Org mode 的入门讲座实录。Org mode 是 Emacs 环境下一个功能极其丰富的模式，以其纯文本、高度可定制的特性，在笔记、写作、任务管理和文学编程等领域备受推崇。

在本次讲座中，Harry Schwarz 从 Org mode 的基本概念入手，介绍了其作为大纲编辑器的核心功能，以及常用的标记语法，包括文本格式化、列表和强大的链接系统。随后，他演示了 Org mode 在处理表格方面的优势，并重点介绍了其灵活强大的导出功能，能够将 Org 文档转换为 HTML、PDF（通过 LaTeX）、Markdown 等多种格式。

讲座深入探讨了 Org mode 的高级特性。通过 Babel，Org mode 实现了文学编程，允许在文档中嵌入、执行代码块，并将结果整合其中——讲者以自己的 Emacs 配置为例进行了说明。此外，内容还涵盖了对 LaTeX 数学公式的良好支持。作为 Org mode 的热门应用，任务管理（GTD）方面也得到了详细介绍，包括 TODO 状态切换、时间戳、截止日期、日程视图（Agenda）和归档机制。讲座中还穿插了关于文学编程理念、任务管理哲学的讨论，以及对 Org Capture、Org Publish 等扩展功能的提及。

### 3. 视频内容纲要

```
主讲：Harry Schwarz (thoughtbot 开发者) - Emacs Org mode 介绍
├── 引言
│   ├── 讲者与 Org mode 使用背景
│   ├── Org mode 的多功能性 (文档, 日历, 待办, 文章)
│   ├── 现场听众互动 (用户比例)
│   └── 使用环境 (Emacs 与 Org 版本)
│
├── Org mode 基础与标记语言
│   ├── 大纲结构 (Outliner)
│   │   ├── 标题层级 (*)
│   │   ├── 文本块与折叠/展开 (Tab)
│   │   ├── 快速创建与排序 (Meta+Enter, Meta+Up/Down)
│   │   └── 纯文本本质
│   └── 标记语法 (Markup)
│       ├── 文本格式 (粗体, 斜体, 等宽, 删除线)
│       ├── 列表 (无序, 有序)
│       └── 链接 (C-c C-l, C-c C-o)
│           ├── 格式: [[地址][描述]]
│           └── 类型: 网页, 文件, 邮件, 待办事项
│
├── 表格处理
│   ├── 创建与自动对齐 (|, Tab, |-)
│   ├── 编辑与导航 (Tab, Enter)
│   ├── 行列操作 (Meta+方向键)
│   └── 高级功能提及 (公式计算, elisp, 格式化)
│
├── 导出功能
│   ├── 核心命令 (C-c C-e)
│   ├── 支持格式 (HTML, LaTeX/PDF, Markdown, iCal, Beamer, TWBS 等)
│   ├── 导出范围控制 (Buffer, Subtree)
│   └── 适用场景 (学术论文等)
│
├── 元数据与文档选项
│   ├── 格式: #+KEY: VALUE
│   ├── 常用元数据 (TITLE, AUTHOR, DATE)
│   └── 常用选项 (#+OPTIONS: toc, num 等)
│
├── 代码块处理 (Babel)
│   ├── 插入与编辑
│   │   ├── 结构: #+BEGIN_SRC ... #+END_SRC
│   │   ├── 快捷键: <s + Tab
│   │   └── 特定语言模式编辑 (C-c ')
│   ├── 代码块导出 (语法高亮)
│   └── 代码执行 (C-c C-c)
│       ├── 结果插入 (#+RESULTS:)
│       ├── 块间数据传递 (提及)
│       └── 示例: Ruby 阶乘函数
│
├── 数学与公式
│   ├── LaTeX 语法支持
│   ├── 特殊字符 (\alpha, \beta 等) => $\alpha, \beta$
│   ├── 行内公式 ($...$) => $E=mc^2$
│   ├── 块级公式 ($$..., \begin{env}...\end{env}$)
│   └── 导出处理 (MathJax for HTML, LaTeX native for PDF)
│
├── 文学编程 (Literate Programming)
│   ├── Babel 作为工具核心
│   ├── 核心思想: 代码、文档、结果整合
│   ├── 讲者实例: Emacs 配置文件 (init.el -> configuration.org)
│   └── 适用性讨论 (配置文件, 书籍, 论文 vs. 快速迭代项目)
│
├── 任务管理 (To-Do / GTD)
│   ├── 创建与标记 (TODO 关键字, Shift+Meta+Enter)
│   ├── 状态切换 (C-c C-t, 自定义状态)
│   │   └── 完成标记与时间戳 (CLOSED:)
│   ├── 时间管理
│   │   ├── 截止日期 (Deadline, C-c C-d)
│   │   ├── 计划日期 (Scheduled, C-c C-s)
│   │   └── 日期调整 (Shift+方向键)
│   ├── Agenda 视图 (C-c a)
│   │   ├── 功能: 聚合, 多视图, 过滤, 提醒
│   ├── 归档 (Archiving, C-c C-x C-a / C-c $)
│   └── 任务管理哲学讨论 (vs. "每天三件事", Deadline 使用, 嵌套与梳理)
│
├── 高级功能与扩展
│   ├── Org Capture (C-c c, 快速捕捉)
│   ├── Org Publish (网站/项目发布)
│   ├── org-drill (间隔重复/抽认卡)
│   └── 移动端支持提及 (Orgzly, Drafts)
│
├── 同步与外部工具
│   ├── 同步方案: ownCloud (文件, 日历, 联系人)
│   └── 版本控制讨论 (未直接使用 Git, 考虑中)
│
└── 总结与问答
    └── 进一步讨论 (Beamer 配置, Google Calendar 集成等)

```

## 引言

我是 Harry Schwarz，thoughtbot 的一名开发者。我非常喜欢 Emacs，并用它来做各种各样的事情。特别有一种叫做 Org mode 的模式，它基本上接管了我的生活。我用它来写文档，用它来组织日历事件，有时我用它来管理待办事项，我用它写各种文章，偶尔也写博客文章。它就是一个……一个庞大的混合体。嗯，我的意思是它是有史以来最好的东西，但它确实接管了我的生活。今天，我将通过实例和一些概念性的东西，带大家入门 Org mode。

首先，这里有谁在某种程度上使用 Org mode？好的，大概有一半人。太好了，这会很有趣。你们会问我一些我可能答不上来的难题。

我喜欢以一种比较轻松的方式进行，所以如果你有任何问题，尽管喊出来就行。


**问：** 你能给我们介绍一下你现在使用的版本背景吗？

**答：** 当然，我使用的版本。是的，我用的是 Emacs 24.5，并且我用的是 Org 版本 8。我相信我用的是当前的版本，是的。我不确定具体是哪个小版本，但肯定是 8 点几。我认为我接下来要演示的内容不会有很强的版本特定性。如果你使用的是过去几年内发布的任何版本，这些应该都能正常工作。

## Org mode 基础与标记语言

Org mode 最初是作为一个大纲编辑器出现的。你可以用一个星号开始大纲中的条目。

（调整字体大小）

是的。在这样的标题下面，你可以添加任意的文本块，文本、文本、文本。你可以随心所欲地展开或收缩这些，这相当方便。在标题下面，你可以添加更多的条目。在这一行的末尾，你可以按 `Meta+Enter`（Alt+Enter）来创建一个同类型的新条目，又一个。你也可以用 `Meta+Up/Down`（Alt+Up/Down）来重新排序它们，这非常方便。

Org mode 基本上是一种标记语言。如果你用过像 Markdown 之类的东西，它很像，但在上千个方面要好得多，我们稍后会深入探讨。它也类似于 reStructuredText 和所有其他类似的东西。

那么，我们来谈谈标记。你可以做很多不同种类的标记操作。你可以用星号使文本 **加粗**。你可以用斜杠使它们 *倾斜*。你可以用等号使它们 `等宽`（verbatim）。你会注意到，随着我们的操作，样式会有一点变化。如果你真的想，你也可以 ~~划掉~~ 文本，我觉得这看起来很糟糕，但没关系。

就像任何标记语言一样，你可以有：

-   项目符号
-   列表项

你也可以插入链接。这里有个例子。假设我想链接到那个很棒的 orgmode.org 页面。我可以按 `Ctrl+C Ctrl+L` 来插入一个链接。（屏幕底部提示有点小）它提示输入“Link:”，我就粘贴 Org mode 的网址进去。然后它提示“Description:”，我就输入“Org mode”。它就为我添加了这个链接。我可以用 `Ctrl+C Ctrl+O` 来访问这个链接，它会在我的浏览器中打开那个页面。这很酷。

从内部来看，如果我在这里按退格键，它实际上是用一对括号来表示的。一对括号里是地址，另一对括号里是文本，最后还有一对括号把它们都包起来。所以，它就是纯文本。所有这些 Org mode 的东西，都只是纯文本。如果你愿意，你可以在 Vim 里打开它并编辑，我不知道为什么会有人想这么做，但你可以。

关于链接的另一个好处是，你可以链接到任意其他东西，不仅仅是网站，还可以是文件、邮件或待办事项。这非常酷。我把这个功能绑定到了 `Ctrl+C l`。它在底部显示“Stored display preferences”，这是我配置中的一个项目。如果我切换回那个缓冲区，我可以按 `Ctrl+C Ctrl+L`，然后按向上键，它会提示“File:”，然后显示那个文件名，接着是“::display preferences”。我就把它命名为“display preferences”，这是默认的。当我在这里按 `Ctrl+C Ctrl+O` 来访问它时，它会弹开那个缓冲区。这超级方便。有时候我编辑代码，知道源文件里有一堆东西需要修改时，我会为自己创建一个小的待办列表，里面包含指向那些位置的链接。这在这方面非常方便。

它也很方便，因为你可以链接到像待办列表这样的东西，正如我所说，或者电子邮件地址——嗯，应该是电子邮件消息，如果你在 Emacs 里读邮件的话，我知道这里至少有一个人是这么做的，但不是我。嗯，总有一天，总有一天。也许，也许下个月吧，我们看看。或者再下下个月。


**问：** 你是怎么弄出这些漂亮的圆点符号的？

**答：** 哦，美化过的？我快速在我的配置里展示一下，但这其实就是一行代码。有人写了一个包，你可以添加进去，叫做…嗯…类似“pretty bullets”或者“formatted bullets”的东西。我稍后会看一下。顺便说一下，那些（标题的星号）只是星号。我想我说过了，但忘了是否说清楚了。星号的数量就像在 HTML 里一样，一个星号是 H1，两个星号是 H2，依此类推。

## 表格处理

所以，这都很酷。另一件你可以做的事情，是其他一些 Markdown 格式真的做得不好的，那就是表格。特别是 Markdown 的表格处理非常糟糕。但 Org 就很擅长。如果我在这里放一个竖线 `|`，假设我想输入一些数据。我输入内容，竖线，换行，再输入 `|-`，然后按 `Tab` 键，它就自动补全了表格线，非常高级，对吧？现在我可以用 `Tab` 在这些单元格之间切换。我们来加点数据：

| One   | Two          |
|-------|--------------|
| Three | Four         |
| Buckle my shoe | Shut the door |

就这样。我们有了这些数据，只需用 `Tab` 键输入，它就创建好了。这很酷。

不过，一个真正酷的功能是，我们可以用 `Meta+上/下/左/右`（Alt+方向键）来重新排列内容。假设我决定要把“Three Four Shut the door”这一行放到最上面，我只需拖动它们就行。我也可以用同样的方式重新排列列。这非常高级。

我不会在这里深入探讨这个，因为它极其复杂，但是 Org mode 表格比我在这里展示的要强大得多。它们是电子表格。你可以放入任意的 elisp 代码，可以让单元格包含各种其他东西。这太疯狂了，太不可思议了。还有格式化功能。超级酷。不过，请自行探索，因为那完全是另一个演讲的主题了。顺便说一句，如果有人想做那个演讲，请告诉我。

## 导出功能

编写任何类型的标记语言的好处之一是你可以导出到其他格式。这是通过 `Ctrl+C Ctrl+E` 命令完成的。假设我想导出这个文件，按 `Ctrl+C Ctrl+E`，会弹出一个缓冲区，列出了所有我可以导出的不同格式。让我放大一点…我放大不了这个，真尴尬。但是，我可以导出到 iCalendar 格式，因为你可以给条目附加日期，我稍后会讨论。你可以导出到 HTML、LaTeX、Markdown、纯文本。我还有一个可以导出到 Twitter Bootstrap 格式化网站的设置，非常漂亮。所以，所有这些以及更多。你可以…有各种人们编写的任意导出器。实际上编写一个导出器非常容易。

假设我想把这个导出为 HTML。我按 `H` 进入这个选项，然后按 `O` 选择“as HTML file and open”。然后瞧，它就在这里了。这是那个表格，看起来甚至很漂亮。所以，这很酷。


**问：** 你能导出 Org 文件的一部分，比如一个区域吗？

**答：** 可能可以。是的。没错。酷。我没这么做过…
**有人提示：** `Ctrl+E` 然后按 `Ctrl+S`，它会提示你可以导出子树…

**答：** 无论如何。`Ctrl+C Ctrl+E`？
**有人提示：** `Ctrl+C Ctrl+E`，然后在顶部，你应该看到“Export scope”。

**答：** 哦，“Export scope”，太酷了！可以选择“Buffer”或“Subtree”。所以你可以在整个缓冲区或你当前所在的子树之间切换。如果我选择“Subtree”然后按回车…当然我不想按这个，我想按 `H` 然后 `O`。好了，它只显示了我刚才所在位置的那部分内容。漂亮！啊，谢谢你！我之前不知道这个。

所以这就是诀窍：你做一个演讲，然后你就能学到东西。

哦，我没提到这个，但你也可以导出为许多其他格式。我只展示了 HTML，但让我们展示一个通过 LaTeX 生成的 PDF。LaTeX 是一种中间格式，我的意思是，它本身就是一种非常好的写作格式，但你可以用它来生成非常漂亮的 PDF。

（等待 PDF 生成）

真漂亮！这是来自同一个源文件的，超级方便。很多人喜欢…很多在学术领域写论文的人会用 Org mode 来做这个，因为它提供了 LaTeX 的大部分好处，而又不必完全用 LaTeX 来写，因为有时用 LaTeX 写作有点痛苦。它超级强大，但我个人在可能的情况下更愿意用这种方式写。

## 元数据与文档选项

你会注意到，在这个导出的文件里，我有一个叫做 `example.org` 的文件，它自动把标题设为了 “example”。这对一个文档来说不是个好标题。我可以给 Org 文档添加各种元数据。格式是 `#+` 加上各种不同的键。在这种情况下是 `TITLE`。哦天，这对比度太糟糕了。是大写的 `TITLE`，然后一个冒号，然后我把它叫做“Org mode 温柔入门”。要是我打字能快点就好了。现在我保存这个，当我再次尝试导出它…好了，标题改过来了。这很好。

我还可以做类似…有一个选项叫做 `OPTIONS`，非常贴切的名字。它有一大堆键值对，让你修改文档的外观。假设我不喜欢这个目录（Table of Contents）的东西…我真的不喜欢。我可以把 `toc` 设置为 `nil`。保存，再次导出，它就消失了。还有一大堆其他选项可以设置，比如也许我们不想要编号，也许我们…你知道…想在底部显示一个小页脚，也许我们不想显示页脚，也许我们想…各种各样的事情，可以做的事情太多了。但这是一个简单的例子。

## 代码块处理 (Babel)

Org mode 的一个好处是你可以非常容易地包含源代码。我们来谈谈源代码。

你可以插入形如 `#+BEGIN_SRC` 然后是你想用的代码类型，比如这里是 Ruby，然后是 `#+END_SRC` 的块。Org mode 中也内置了一些快捷方式。如果你输入 `<s` 然后按 `Tab`，你也会得到一个展开的小源码块。这很有帮助，没人想把那些都打出来。

我们可以用 `Ctrl+C '`（Ctrl+C 单引号）在代码块对应的语言模式下编辑它。

我们来写一个非常小的阶乘函数。假设我们是函数式程序员，我们整天做的事情就是写阶乘函数。

```ruby
def factorial(n)
  if n == 1 # 原视频此处为 n==0，但阶乘通常定义1为基准，且后续计算5!时120结果是基于n==1
    1
  else
    n * factorial(n - 1)
  end
end
```

对你来说看起来对吗？对我来说似乎是对的。好了，它现在就在那里了。我可以保存它，当我把它导出到 HTML…它现在会声称我不在一个项目里，之前没有这样。真令人沮丧。我想这是 projectile 包的问题。我想这是因为它希望我在一个 Git 项目里。所以我快速操作一下来满足它。好了。非常好。然后我们有了这个源码块，这里不太清楚，但它是语法高亮的。因为我用一个叫做 `minted` 的包设置了它，非常漂亮。


**问：** 那边的那个源代码块，有没有办法让 Org mode 运行那段代码？

**答：** 的确有。我们稍后会谈到这个。是的。

如果我们给它命名…嗯，实际上一个非常简单的方法是按 `Ctrl+C Ctrl+C`，它会就地评估它。这些是结果。（指屏幕上可能出现的 `#+RESULTS:` 块）假设我们想调用 `factorial(5)`。我没试过这个，所以我真的是在冒险。好了，120。所以它用合适的解释器评估了它，并把结果粘贴了进去。这有多疯狂？答案是：非常疯狂。太棒了！光荣！我知道，这太棒了。

我应该提到，当你谈论评估代码块时，如果你有一个代码块并且它有一些结果，你可以将这些结果输出到屏幕，输出到编译后的文档中，但你也可以将它们作为输入传递给另一个代码块。所以有时候人们会编写代码生成一些信息，然后将其传递给像 gnuplot 块来生成图表。哦，这简直是魔法！我觉得这超级酷。


**问：** 关于源代码块的导航快捷键你熟悉吗？

**答：** 源代码块的导航快捷键？我知道它们存在。

**问：** 好的，你具体指的是哪个？

**答：** 有一个用于“移动到上一个/下一个源代码块”的，它会将你的光标带到 `BEGIN_SRC` 指令处。我在想是否有一个可以将你带到 `END_SRC` 指令或 `RESULTS` 指令处？

**答：** 当然。所以问题是，有没有一个键命令可以把你从源代码带到结果指令或结束指令？嗯……我会说“有”，因为对于“有没有一个键命令可以做某事？”这类问题，答案通常是“是的，是的，有人做过那个”。但我不知道具体是哪个。

实际上我用的是 evil mode（Vim 模拟），我用花括号 `{}` 来按段落上下跳转，实践中这大概也就多按一两次键，所以我还没费心去研究那个优化。但我打赌肯定有东西能帮你做到。我非常有信心，事实上，这看起来就是那种必须存在的东西。

还有其他关于代码块或代码的问题吗？

## 数学与公式

我提到过你可以用它作为 LaTeX 的替代品，你完全可以。所以你可以得到像 `\alpha` 这样的字符。

（屏幕显示输入 `\alpha` 后变成 α）

我们把这些放进去，然后，嘣！`\alpha` 到 `\beta`。太棒了。那个有点靠下，让我放大一点。是的。所以你可以在 Org 文档中直接包含 LaTeX 命令。如果你想更高级一点，你可以包含数学块。比如假设我们想说类似 `$O(n \log n)$ 这样的东西，这是我们经常会说的，对吧？我们把它展开，好了，格式正确。太好了。

如果我们想，我们甚至可以说更复杂的东西，比如我们可以使用 LaTeX 提供的 `align*` 环境。

（输入 LaTeX 公式环境）

哦是的，别介意我，我记得 LaTeX，我真的记得，我发誓。我们把那些改成这些，再来一次。好了。然后我可以说类似 $3 \times 2 \times 1$ 等于…我这里有个例子…但是我们可以对齐一些东西，说它等于 $6+1$，然后换行，然后对齐这些，它等于 7。嘿， presto！当我们创建它时，它会正确地把它放进去。这只是 HTML，但它使用了一个叫做 MathJax 的 JavaScript 包，默认情况下，Org 编译时就会包含它。如果你真的想，你可以禁用它，但这非常酷。而且不出所料，当你导出到 PDF 时，它也同样正确地显示出来，毕竟我们这里写的是 LaTeX。所以这更精炼了，我想。

## 文学编程 (Literate Programming)

我们展示了你可以在你的 Org 文件中评估源代码块。另一个你可以做的很酷的事情是评估一个 Org 文件中所有的源代码块。我有一个非常非常简单的 `init.el` 文件。让我在这里打开它。`emacs/init.el`。它只有一行。我运行这个命令 `org-babel-load-file`，它加载了一个 Org 文档，也就是我的 `configuration.org`。它的作用是遍历这个文件，找到所有标记为 Emacs Lisp 的源代码块，并按顺序评估它们。

所以如果我们看一下实际的配置文件，它…我的意思是，它就是一个 Org 文档。我用了一个叫做 `sensible-defaults` 的包来设置一些东西。我在这里设置了我的个人信息。让我想想…哦，这是我的 Org 相关设置。我有一些显示偏好。哦，就是这个：`org-bullets-mode`。我把它设置成了 true。我相信你还需要安装一个叫做 `org-bullets` 的包。你也可以做一些事情，比如隐藏前导星号，就是如果你有比如三个星号，它只会显示第三个，并且会正确缩进。

总之，发生的事情是，有一个叫做 Babel 的系统，它与 Org 相关联，它会遍历你的文档，找到所有用适当语言编写的源代码，并从中生成一段新的源代码，一个新的文档。这就是我正在做的。

关于这部分有什么问题吗？这有点神奇。

我对文学编程有很多看法。我认为它在大多数情况下是个相当糟糕的主意。但对于像这样不怎么变化，并且有点意在教学——就是人们应该从中学习的东西——我认为这是一种非常有用的方式。而且，当我把我的配置转换成 Org mode 时，我发现了各种疯狂的重复、奇怪的不一致等等。所以这是一次非常好的练习。


**问：** 这就是你整个的配置文件吗？

**答：** 这是我整个的配置文件。公平地说，它差不多有 1200 行长。所以，你知道，我们可以把它展开，它变得相当…相当疯狂。但是，你知道，其中很多也是散文（prose），这有点…哦嘿，我甚至链接了散文。无论如何，好东西。

我也可以导出这个，例如，导出。好了。这是目录。是的，这挺酷的。我有很多代码。我做了各种疯狂的事情。就像我说的，这些都在网上。作为一个好处，它托管在 GitHub 上，而 GitHub 现在能正确解析 Org 文档并显示它们，效果和它们显示 Markdown 差不多。它们不会做一些聪明的事情，比如评估代码块并把结果放进去，但是，是的。


**问：** 在配置文件里，那是一个大文件还是…？

**答：** 哦，我的配置文件？它就是一个庞大的文件，是的。

**问：** 有没有可能把这些分成不同的文件，但是像…组织成…？

**答：** 我可以把它们分成不同的文件。我不知道那样会有什么好处。就像现在，我可以展开和折叠它们，搜索起来也非常容易。只有一个文件，我用 grep 就行。我在这方面比较懒。这挺好的。对于…我的意思是，通常我非常倾向于“是的，让我们把所有东西都分成独立的文件”，你知道，“每个地方一个职责”以及所有那些好东西。但对于这个，我完全走向了相反的方向。


**问：** 你有没有尝试过将文学编程用于 Emacs Lisp 之外的其他东西？

**答：** 我有没有尝试过将文学编程用于 Emacs Lisp 之外的其他东西？我有。我尝试过将代码结果通过管道传递给其他块，比如生成图表之类的，或多或少是为了好玩。我用 Ruby 成功做到了这一点。我还没怎么尝试过用其他语言。

我实际上认为文学编程几乎总是一个糟糕的主意。如果你有一个项目，我认为好的软件工程实践是关于确保该项目在未来能够轻松地进行更改。我认为，当代码更改时，大量需要同时更改的注释也会使更改变得更加困难，并最终会变得具有欺骗性，因为人们不会总是更改那些注释。等等等等。关于这个话题，我准备了一个半小时的长篇大论，如果你想听，之后可以让我释放出来。但是，是的，除了这种东西，我还没怎么用过文学编程。

我认为它对于论文也很好。比如，如果我在写一篇论文，特别是如果我对可重复研究感兴趣，我认为那将是一种很好的方式。任何更像是文档——像文档驱动的，或者旨在教学的东西，我认为文学编程是一个非常棒的模型。对于不像那样的东西，我认为它不是一个好模型。我认为如果你是 Donald Knuth，并且你在写《计算机程序设计艺术》，那是绝佳的选择。如果你不是…但配置文件，我认为是它的一个很好的应用场景。它们不怎么改变，它们需要有良好的文档，人们会从中学习。所以对我来说，这似乎是文学编程的一个绝佳案例。是的。

酷。是的，我实际上在这个问题上来了个 180 度大转弯。我以前完全不那样做。我有一大堆微小的 elisp 函数，并且我主动不给它们写注释，因为我希望函数名本身就是文档。后来我意识到那是愚蠢的。对于这个特定的用例来说，这根本不是一个好的选择。

## 任务管理 (To-Do / GTD)

好了，关于那些我要谈的待办事项。最初吸引我进入 Org mode 的，并非所有这些你可以做的整洁的发布功能，而是待办事项管理。我读了《搞定》（Getting Things Done），那是一本关于将你所有生活都放入待办列表的花哨的书。我想，是的，我想那么做。但我也喜欢纯文本，并且我喜欢这个来自 70 年代的笨重的老编辑器。我该如何将我所有的热情结合在一起呢？

事实证明，Org 非常适合这个。如果你有一些项目符号项，并且你在它前面加上单词 `TODO`，你会注意到它变成了奇怪的颜色。TODO，让我想想…“解释待办列表”。如果我按 `Shift+Meta+Enter`（Shift+Alt+Enter），它会在下面创建另一个同级条目。

你可以做的一件事是，你可以循环切换状态。如果我有这个家伙在这里，我可以按 `Ctrl+C Ctrl+T`，它就会被标记为 `DONE`（完成）。多么高级！我可以再按一次 `Ctrl+C Ctrl+T`，它会移除 TODO 标记。如果我再按一次 `Ctrl+C Ctrl+T`，它会循环回到 `TODO`。如果我愿意，我可以更改该文件的一些元数据，来说明我想要在那个循环中插入额外的状态，甚至可以有多个循环。就我个人而言，我使用 `TODO`、`WAITING` 和 `DONE`。`WAITING` 用于那些我被阻塞、等待别人的事情。所以，这都很酷。

请注意，当我这样做时（标记为 DONE），它在末尾添加了这个小时间戳，这相当高级。顺便说一句，关于 Org 时间戳的一个很酷的事情是，你可以用 `Shift+左/右` 来修改它们。所以我可以像是，“哦，让我们换到另一天”。这挺酷的。

我可以给事情附加截止日期（deadlines）。假设我今天真的需要解释待办列表。我可以按 `Ctrl+C Ctrl+D`，这会在我的文本编辑器里调出这个神奇的日历，这太疯狂了。它会让我选择一天。假设我早该完成那个了。现在这个被分配了一个截止日期。我可以用 `Shift+左/右` 来切换日期，用 `Shift+上/下` 按月份切换，如果我愿意的话。我觉得这很酷。


**问：** 你能按截止日期排序吗？我能做到吗？

**答：** 哦天哪，哦天哪。如果我按 `Ctrl+C a`，它会召唤出 Agenda（议程）。这也是一个我放大不了的东西，该死。然而，这里有一个字母列表以及它们的作用。在这些功能中，我可以看到当前周或天的议程，一个包含我所有待办事项条目的列表——如果我配置了，可以跨多个文件。你需要写一点点 elisp 来设置这些，但这相当直接。我可以基于特定的标签进行搜索。有标签功能。嗯…我可以做各种疯狂的事情。所以，是的，我完全可以按东西排序。

但我实际做的，然而，是当我完成某件事时，我按 `Ctrl+C Ctrl+X Ctrl+A`（或 `Ctrl+C $`）来归档它。它的作用是，它拿到那个条目，将它标记为完成，设置那个 `CLOSED:` 时间戳，将它从当前所在的文件中移除，并将其附加到我别处的一个 `archive.org` 文件的末尾。所以我有一个列表，记录了我在过去五年里做过的所有事情，这挺不错的，还有我做它们的时间，所有这些好东西。所以在实践中，我不需要按“完成”来排序，因为它们已经被“完成”排序了——我有了这个（指归档文件）。


**问：** 这个问题跟 Org mode 或 Emacs 关系不大，但是作为一个可能读 Jeff Atwood 博客的人…

**答：** 哦是的。

**问：** 你看到他…我怀疑你看到了他大概六个月前关于待办列表的长篇大论…

**答：** Jeff Atwood 关于待办列表的长篇大论？那篇文章的论点是什么？

**问：** 是说你应该把它们都扔掉。扔掉你所有的包、约定，等等，然后就每天做三件事。因为你能记住事情，这很简单，你不需要写下来，你不需要把它放进 Emacs，你不需要跟踪它，你会知道你是否完成了它们。

**答：** 酷。

**问：** 我看到了那个，而且我做过这么多这方面的事情，有这么多历史，可能至少可以追溯到 1992 年。我看到那个之后，对于工作来说，我立刻就信了。当然。但我很好奇你是否遇到过它，以及你的反应会是什么？

**答：** 现在你提到了，我听说过。录音提示：那是 Jeff Atwood 关于扔掉你的待办列表，每天只写下你需要做的三件最重要的事情的帖子。我的回应是：Jeff Atwood 怎么会记得他什么时候需要去看牙医？如果我没有东西告诉我，我永远不会记得。对我来说那是日历条目，但是，我有远不止三件事情需要做，而且它们大多是我不想记住的事情。所以我真的需要某种积压列表（backlog）。

我觉得，如果你把所有事情都放在一个待办列表里，并且你非常勤奋地维护它，从中移除事情，并在有新需要做的事情进来时追加到里面，那会工作得相当好。如果你只是半途而废，有一个待办列表，里面的东西你不定期更新，它就那么笼罩着你，与你脑子里一个未写下的、让你担忧的事情列表同时存在，那么你会过得很糟糕，而且它不会起作用。根据我的经验，是这样的。所以我认为，“没有待办列表”是一个选项。我认为那样很难跟踪事情，因为我有超过三件事情需要做，而且其中一些我明天就需要做。


**问：** 这也基于一个前提，就是你并不一定想记住你做过什么。

**答：** 是的，那也是。我在这里的做法是，我现在有了我做过的所有事情的记录。这有时候挺方便的。我偶尔需要知道，“我什么时候付了那张账单？”或者，你知道，“我上次去看牙医是什么时候？”之类的，我可以很容易地查到。这有点用。是的。所以如果你喜欢那样，我认为这是一种很好的做事方式。如果你有不同的系统，尽管不用这个。

我偶尔会为工作建立一个这样的小列表。你知道，比如我知道我今天有四五件小事要做，我就会建一个单独的小列表，这只是帮助我记住它们。或者有时候我直接在纸上做。

我没有展示日程安排（schedule）。我没有。让我给你看看议程。哦天哪，我希望我的生活中没有什么尴尬的事情正在发生。不，还好。不多。这会发布到互联网上。我正在写一些…该死的…代码示例。我有一个绩效评估需要填写。让我想想…我需要读一本关于 Haskell 的书，这对我来说很重要。其中一件事我有一个截止日期。所以这就是…这就是我接下来一周的总结。我不太常用日期相关的功能。我大部分的日程安排使用更传统的日历，但有些人非常喜欢这样做。


**问：** 我使用 Org mode 的问题之一是，你知道，我捕捉了成堆成堆成堆的待办事项，但我总是给它们分配一个截止日期，但实际上搜索那些没有截止日期的待办事项我发现有点棘手。所以我不知道…

**答：** 是的。

**问：** 所以我希望所有事情都有一个应该完成的日期，你知道，只是为了它最终能出现。

**答：** 是的。所以，问题是，没有截止日期的事情怎么完成，有点这个意思。

**问：** 确切地说。

**答：** 哎，我人生的写照。嗯…所以我只给那些有非常确定完成时间的事情分配截止日期。比如，你知道，我真的应该读那本 Haskell 书，但那没有截止日期。我可以说我需要在周六之前完成那一章。但我并不需要在周六之前完成。既然那是一个编造的截止日期，那会让我不尊重任何截止日期，最终事情就会从缝隙中溜走。所以我倾向于不那样做。

因为 Org 是层级化的，我的意思是，我可以把待办事项嵌套在其他待办事项里。所以我可以说，“哦，你知道，我有所有这些事情…”因为我可以嵌套待办事项，我可以创建项目，它们会有一系列我可以划掉的任务。所以我认为每隔一段时间，过一遍你的待办列表，稍微“整理”（grooming）一下，只是为了用一种合理的方式组织事情，是非常有用的。所以我倾向于经常这样做。我的意思是，不是非常频繁，但你知道，每隔几天我会看看，“这里到底发生了什么？”然后清理一下，用更合理的方式组织一下。这通常能让事情得以完成。

不必在这里再次完全 GTD 化，关于《搞定》的哲学，但是，对于每个项目，有一个“下一步行动”（Next Step）任务是非常有用的。我发现这种方式对此非常有利。是的。

## 高级功能与扩展


**问：** 你打算谈谈联系人列表吗？

**答：** 我谈联系人列表吗？我不谈。因为我还没有找到一个在 Org 中处理联系人列表的好方案。我知道有一个叫做 `org-contacts` 的包，而且我确定有人用它。我没有发现它特别好用。我处理联系人的方法是使用一个叫做 `abook` 的 Unix 程序，它就像一个地址簿，是一个 curses 工具，它与 Mutt 集成得非常好，我用 Mutt 处理我的邮件。我认为如果你想在 Emacs 中管理联系人，一个很棒的老工具仍然是 `bbdb`，也就是 Big Brother Database，它会监控你所有的邮件并将它们添加到地址簿中。管理联系人的一种超级好的方式，很多人这样做。我的意思是，你知道，相对于用 Emacs 处理邮件的人数来说是很多人，还是有一些的。它是一个很好的工具。


**问：** 我之前深度使用 Org mode 时有过一次经历，当时我在做一些账户管理…那是什么来着…会计方面的事情，用来生成发票之类的。

**答：** 是的，会计，时间追踪。

**问：** 是的，并且深入到通过编程生成数据、表格和报告。我遇到了一些情况，我需要的 Org mode 功能…那个词…不存在，但在下一个版本里才有。所以我陷入了一个我自己造成的陷阱，你知道，当然，罪有应得。但我用了 Emacs 的开发版源码，然后我又试图用 Org mode 的开发版源码，两者冲突了，最后到了我抓狂的地步，我有点和 Org mode 脱离关系了。但我确实记得它极其强大。我也更多地转向了 Google 的思维模式，使用 Gmail、日历以及其他各种东西。但对于其他所有事情，我还是用…

**答：** 当然，明白了。这是个问题吗？

**问：** 所以问题是，你是否也被卷入了使用新功能的诱惑中？Org mode 开发者以令人难以置信的速度推出新功能。

**答：** 是的。

**问：** 而且，我的意思是，Org mode 的发展…Org mode 独立于 Emacs 发展的事实…如果它是在 Emacs 内部开发的，那会容易得多，我认为。

**答：** 当然。

**问：** 然后是关于这点的争论，优点和缺点。但我想知道你是否也被卷入了那种模式，因为你是一个重度用户？

**答：** 没有。所以…所以，是的。所以问题大致是，因为 Org 和 Emacs 是分开开发的，而且 Org 中有一些前沿功能可能与某个版本的 Emacs 不兼容，你最终会陷入这种让两者都保持前沿的竞赛中，有时东西会坏掉。但是新版本的 Org 中有很酷的东西。我是否会陷入那样的困境？我并没有真正…我并没有真正使用那么多 Org 中真正酷的功能。我的意思是，我认为我做的事情是惊人地酷的功能，比如，嗯，你知道，我正在用 Org mode 写一本书，这太棒了。但肯定有更酷的事情你可以做，比如时间追踪之类的。还有各种各样非常花哨的新功能，我真的不用它们。抱歉，这是一个 Org mode 的入门讲座。

不过，说到可以用 Emacs…嗯…用 Org mode 做的酷事。有一个叫做 `org-t-…` `org2blog` 的包。（看着屏幕）在我面前的编辑器里。它叫做 `org2blog`。它可以用来获取一个 Org 文档并将其发布到一个 WordPress 站点。所以如果你有一个 WordPress 博客，你可以在你的编辑器里舒适地编写所有帖子并在 Org mode 中发布它们，而无需访问那个网站，这相当高级。如果你甚至不想要那么多开销，我可能就不会，你可以使用一个叫做 `org-publish` 的工具。你可以用 Org mode 定义一个网站的布局，或者实际上是任何类型的项目，然后有一个文件目录，在 Emacs 内部调用 `org-publish`，它会获取整个目录结构，通过 Org mode 处理所有内容，然后生成一个网站。这很疯狂，但有很多人这样做，而且超级酷。希望有一天我也能加入他们。

让我想想…还有一些其他很酷的事情。你可以导出到…我提到了 Beamer。我没给你们看 Twitter Bootstrap，对吧？让我给你们展示一下 Twitter Bootstrap。这个有点酷。让我用这个导出我的配置。所以，Twitter Bootstrap，或者他们现在更愿意称之为 Bootstrap，它是一种…嗯…设计静态网站并让它们看起来很漂亮的框架。基本上现在每个创业公司的网站看起来都像那样。几乎每个人都用 Twitter Bootstrap 来做那个页面。所以有一个叫做 `ox-twbs` 的导出器。我应该把它写下来。`o-x-dash-t-w-b-s`。我安装了那个。所以当我按 `Ctrl+C Ctrl+E` 时，我可以按 `w` `o`，它会处理它，然后瞧！就是这个东西。多酷啊！它旁边有这个古怪的 JavaScript 菜单。它完全…字间距，你知道，很棒。这真的很漂亮。所以，这很酷。你可以就这样到处跳转之类的。这里有我所有的定制。所以这是一个花哨的功能。

另一个导出器是 `ox-gfm`，用于 GitHub Flavored Markdown，如果你喜欢用那个的话。如果你写很多那个，这可能挺方便的。老实说，我直接在里面写，我懒得导出到那个格式，但有些人可能会。

让我想想…我提到过你可以在 Org 表格里做各种可怕的电子表格操作。你能在里面做的事情太疯狂了。你应该去看看。太疯狂了。

嗯…我能想到的最后一个很酷的东西是一个叫做 `org-drill` 的工具。它让你定义一个信息的层级结构，它会在 Emacs 内部将它们结构化为抽认卡（flashcards）。所以你可以有一个问题，然后一个答案，它会先显示问题，然后显示答案。但你可以拥有这整个层级的抽认卡，然后运行 `org-drill`，它会对你进行抽认测试。


**问：** 听起来像是做你的 GTD 回顾的好方法。

**答：** 是啊，对吧？必要的？是？不？是的。所以那相当高级。

Org mode 里有大量很酷的事情可以做。这就是我这里准备的全部内容了。但是你们有什么问题吗？我很乐意回答。


**问：** 你用 org-publish 功能吗？

**答：** 我最近一直在玩那个。我有点…所以我现在的博客是用 Jekyll 构建的。我喜欢它，它很好，别误会，Jekyll 是高质量的东西。但是，你知道，我宁愿写 Org mode 而不是 Markdown。而且我把它托管在 GitHub Pages 上，它需要恰好是那种特定的 Markdown 格式。我宁愿不那样做。所以我正在考虑切换过去。我一直在玩那个。对我来说主要的问题是试图弄清楚如何让我旧的 Jekyll 链接工作。因为 Jekyll 是按目录结构组织的，比如，你知道 `2014/07/15/`…当然是 7 月 15 日，该死的聪明天气…然后是文章的名字。而且，你知道，我需要弄清楚如何让那个结构工作。我还没弄明白，但我想弄明白。所以那是未来的某个计划。从我目前玩过的情况来看，它似乎真的很酷。如果你没有一个需要匹配的现有结构，哦天哪，我绝对会立刻就用它。它很好。

还有什么你们想问的？


**问：** 你用过 `org-mobile` 吗？

**答：** 我几年前玩过 `org-mobile`，我不喜欢它。它非常笨重。我想它有一段时间没有维护了。我听说有人试图重新激活 `org-mobile`，但我还没试过。我希望他们成功了。移动端的 Org 功能会非常棒。
**有人提示：** Android 上的 Orgzly 实际上相当不错。

**答：** Android 上的 Orgzly？酷。听起来…
**有人提示：** 是的，就像有人走了自己的路，把旧的放一边了，它实际上…我的意思是，你不能在里面做任何重活，但如果你只是想同步，能够添加和查看东西，我觉得它…

**答：** O-R-G-Z-L-Y？
**有人提示：** Z-L-Y。O-R-G-Z-L-Y。

**答：** Orgzly。当然。看，有这么个东西叫 Orgzly，而且显然它很好。是的。org-z-l-y。酷。酷。我不知道 iPhone 上有没有。
**有人提示：** iOS 上可以看看。

**答：** iOS 上有一个叫做 Drafts 的程序，D-R-A-F-T-S。它让你写…它有点难解释，但你在一个窗口里写一小段文本，然后你可以让它通过某个模板，那会以某种方式处理它，比如也许添加一个时间戳，或者例如，在前面加上 `* TODO `，然后把它追加到某个文件，或者创建一个新文件，或者把它发送到某种其他外部服务。那是一个超级强大的工具，没多少人在谈论它。他们都应该谈论，因为它太棒了。如果你用 iOS，Drafts 很不错。

还有其他与 Org 相关的问题吗？

## 同步与外部工具


**问：** 你提到同步，你在你的电脑上同步它吗？

**答：** 是的。所以我把这个同步在一个文件夹里。我有一个包含多个文档的目录，我通过一个叫做 ownCloud 的工具将它们同步到一个我控制的服务器上。提醒我最后回来谈谈 ownCloud，因为那是我可以聊一会儿的东西之一。但 ownCloud 是一个我非常喜欢的、很棒的软件。它就像是 Dropbox 的替代品，但在很多方面也是 Google 的替代品，这相当不错。


**问：** ownCloud？

**答：** ownCloud。哦是的。我们先有 Org mode 的问题吗？

ownCloud 很神奇。如果你有一台服务器，可以是物理服务器，也可以是像 DigitalOcean 的实例或其他你喜欢的。它是一个…它是一个 LAMP 类型的程序。它是一个 PHP 应用程序，运行在 MySQL 上。它提供给你的是…某种同步工具，有点像你通过 Dropbox 得到的那种，它有适用于所有你期望平台（Windows, macOS, Linux）的桌面客户端，也有移动客户端。我用它来同步日历。所以，我不用 Google。所以我需要某种能和那边那位女士共享日历的东西，而且不是 Google 的。所以我一直使用…我桌子旁边运行着一台服务器，上面跑着 ownCloud，它就做这个。它工作得非常好。你可以用它管理联系人并同步它们。日历功能运行的是 CalDAV。联系人功能运行的是…对应的联系人协议…CardDAV。就是它，是的。所以这很酷。

你还可以用它做很多其他事情。还有一大堆我没有利用到的其他包。如果你在一台物理服务器上运行它，一个优势是，在文件同步方面，你唯一的限制是你硬盘的大小。所以我大概有 1TB 的同步空间，这要是从 Dropbox 买会花我很多钱，这很棒。所以这挺酷的。我是 ownCloud 的忠实粉丝。


**问：** 在与 ownCloud 同步方面，你对你的 Org 文件使用任何版本控制吗？比如 Git Annex？

**答：** 没有。我玩过 Git Annex，也考虑过那么做，但我还没做。Git Annex 看起来超级酷。我也考虑过在我的服务器上设置一个…像…像一个通知系统，当那些文件改变时，它会自动创建一个提交。有一个非常酷的工具叫做 `entr`，我想是这个名字，没多少人知道。它就像一个通用的 inotify 工具。这有点跑题了，但我认为 `entr` 太神奇了，所以我必须告诉你它的存在。但我不知道我是否会用它来做那个，但它超级酷。但如果，例如，你想一直重新生成 ctags 之类的，`entr` 会是一个很棒的工具。


**问：** 所以这个 ownCloud 的事情是，你有一台服务器，上面有大量数据，然后你管理备份之类的事情，你做所有的维护？

**答：** 是的，它就在我桌子旁边。这没那么难。它不怎么变。我…你知道，每六个月我登录一次，更新所有软件包，然后就不管它了。它就是一个 Debian Stable 在那里运行，不怎么变。

**问：** 所以你的 ownCloud 日历信息和你的 Org 日历信息是分开的？

**答：** 完全分开。我没有让它们互通。我还没有将我的日历功能与 Org 集成。还不确定是否会。我们再看。是的。

ownCloud 超级酷。它全是 GPL 的，是自由软件。所以你可以把它安装在任何你喜欢的地方。我想你也可以通过它处理邮件，我没有。我用不同的服务处理邮件。但是，超级酷。你也可以…我想你也可以通过他们购买共享主机来托管一个 ownCloud 实例。我不知道你为什么要那样做，感觉有点违背初衷，但无所谓。那可能也挺好的。


**问：** 说到日历，把 Org 的东西导出到 iCal 非常容易，然后你可以比如推送到服务器，导入到你的日历应用里。但反过来就天知道会怎样了。

**答：** 是的。

**问：** 像我…回到 Org 里。那部分我还在试图解决。

**答：** 是的，双向同步对我来说似乎超级难。就像我有一个桌面日历应用程序，它都几乎不能可靠地进行双向同步。所以我对用 Org 做那个没有抱太大希望。但我确定这是可以做到的。
**有人提示：** 有一个 `org-gcal`…如果我不用 Google Calendar 的话…

**答：** 是的。
**有人提示：** 是的。所以评论是…是的。很难取代 Google Calendar，该死。

**答：** 评论是说有一个 `org-gcal` 包，可以和 Google Calendar 很好地同步。这很酷。我很高兴。

## 总结

还有其他问题吗？关于 Org 或 ownCloud 或其他的？

好了。那边还有很多希腊食物可以吃，所以大家去吃吧。非常感谢！

---

## 内容回顾

**引言**

-   演讲者 Harry Schwarz (thoughtbot 开发者) 介绍自己是 Emacs 和 Org mode 的重度用户。
-   Org mode 已深度融入其工作与生活，用于：
    -   文档写作
    -   日历事件组织
    -   待办事项 (To-do) 管理
    -   文章与博客撰写
-   现场听众中约有一半使用 Org mode。
-   使用的版本：Emacs 24.5, Org mode 8.x (内容基本与近几年的版本兼容)。

**Org mode 基础与标记语言**

-   **大纲结构 (Outliner)**
    -   Org mode 最初是一个大纲编辑器。
    -   使用星号 (`*`) 创建层级标题 (一个 `*` 为一级，两个 `**` 为二级，以此类推)。
    -   标题下可添加任意文本块。
    -   可使用 `Tab` 键方便地折叠和展开各级标题下的内容。
    -   `Meta+Enter` (Alt+Enter) 可快速创建同级标题。
    -   `Meta+Up/Down` (Alt+Up/Down) 可调整标题及其内容的顺序。
-   **标记语法 (Markup)**
    -   Org mode 是一种标记语言，类似 Markdown、reStructuredText，但功能更强大。
    -   文本格式化：
        -   `*粗体*`
        -   `/斜体/`
        -   `_下划线_` (视频中未明确演示，但为标准语法)
        -   =等宽代码=(verbatim)
        -   `+删除线+`
    -   列表：
        -   使用 `-`, `+` 或 `*` (在非标题行首) 创建无序列表。
        -   使用 `1.` 或 `1)` 创建有序列表。
    -   链接：
        -   使用 `C-c C-l` (Ctrl+C Ctrl+L) 插入链接。
        -   格式：`[[链接地址][显示文本]]`。
        -   支持多种链接类型：
            -   网页链接 (e.g., `[[http://orgmode.org][Org mode 官网]]`)
            -   本地文件链接 (e.g., `[[file:path/to/your/file.org::*可选标题或行号][文件描述]]`)，非常适合项目内跳转或引用。
            -   邮件链接 (需配置邮件客户端)。
            -   待办事项链接。
        -   使用 `C-c C-o` (Ctrl+C Ctrl+O) 打开光标处的链接。

**表格处理**

-   Org mode 的表格功能远胜于 Markdown。
-   创建表格：
    -   输入 `|` 开始一行，然后输入表头或内容，用 `|` 分隔。
    -   按 `Tab` 或 `Enter` 键，Org mode 会自动对齐表格。
    -   输入 `|-` 后按 `Tab` 可快速生成分隔线。
-   编辑与导航：
    -   `Tab` 键在单元格间移动。
    -   `Enter` 键移动到下一行。
-   行列操作：
    -   `Meta+方向键` (Alt+方向键) 可快速移动行或列，重排表格结构。
-   高级功能 (提及但未深入)：
    -   表格内支持公式计算，使其成为一个简单的电子表格。
    -   可以嵌入 Emacs Lisp 代码进行复杂计算。
    -   支持丰富的格式化选项。

**导出功能**

-   强大的导出能力是 Org mode 的核心优势之一。
-   `C-c C-e` (Ctrl+C Ctrl+E) 打开导出调度器 (Export Dispatcher)。
-   支持导出为多种格式：
    -   HTML
    -   LaTeX (进而生成 PDF，效果精美)
    -   Markdown (包括 GFM - GitHub Flavored Markdown，需 `ox-gfm` 包)
    -   纯文本 (Plain Text)
    -   iCalendar (用于日历事件)
    -   Beamer (基于 LaTeX 的演示文稿，需 `ox-beamer` 包)
    -   Twitter Bootstrap 样式的 HTML (需 `ox-twbs` 包)
    -   以及更多其他格式，可通过扩展添加。
-   导出范围：
    -   可导出整个缓冲区 (Buffer)。
    -   可仅导出当前子树 (Subtree)。
    -   可在导出菜单 (`C-c C-e`) 后按 `Ctrl+s` 切换导出范围。
-   非常适合撰写学术论文 (利用 LaTeX 的排版优势，但使用更友好的 Org 语法)。

**元数据与文档选项**

-   使用 `#+KEY: VALUE` 格式在文件开头定义元数据和选项。
-   常用元数据：
    -   `#+TITLE: 文档标题`
    -   `#+AUTHOR: 作者名`
    -   `#+DATE: 日期`
-   常用选项 (`#+OPTIONS`)：
    -   `toc:nil` 或 `toc:t` 控制是否生成目录 (Table of Contents)。
    -   `num:nil` 或 `num:t` 控制章节是否自动编号。
    -   还有许多其他选项用于控制导出时的各种行为和外观。

**代码块处理 (Babel)**

-   **插入与编辑代码块**
    -   使用 `#+BEGIN_SRC <language> ... #+END_SRC` 结构包裹代码。
    -   快捷方式：输入 `<s` 后按 `Tab` 可快速插入代码块结构。
    -   `<language>` 指定代码块的语言 (e.g., `ruby`, `python`, `emacs-lisp`, `shell`)。
    -   `C-c '` (Ctrl+C 单引号) 可在对应语言的主模式 (Major Mode) 下编辑当前代码块，提供语法高亮、补全等支持。
-   **代码块导出**
    -   导出时，代码块通常会进行语法高亮 (可配置，演讲者提到使用 `minted` 包获得更好看的 LaTeX 输出)。
-   **代码执行 (Literate Programming 核心)**
    -   `C-c C-c` (Ctrl+C Ctrl+C) 在代码块内可执行该代码块。
    -   执行结果可以：
        -   直接插入到 Org 文档中 (在代码块下方生成 `#+RESULTS:` 块)。
        -   被后续的代码块作为输入使用 (通过设置代码块头参数 `:var` 等)。
        -   用于生成图表 (e.g., 将数据传递给 `gnuplot` 代码块)。
    -   演示了执行 Ruby 阶乘函数并计算 `$factorial(5)$`。

**数学与公式**

-   Org mode 内建对 LaTeX 数学语法的支持。
-   特殊字符：可以直接输入 LaTeX 命令，如 `\alpha`, `\beta`, `\sum` 等，Org mode 会尝试实时预览或在导出时正确处理 ($\alpha$, $\beta$, $\sum$)。
-   行内公式：使用 `$...$` 包裹 LaTeX 公式，例如 `$E=mc^2$`。
-   块级公式：
    -   使用 `$$...$$` 包裹单行居中公式。
    -   使用 `\begin{equation} ... \end{equation}` 或 `\begin{align*} ... \end{align*}` 等标准 LaTeX 环境书写多行或对齐的公式。
-   导出处理：
    -   导出为 HTML 时，通常使用 MathJax 库在浏览器端渲染 LaTeX 公式。
    -   导出为 PDF (通过 LaTeX) 时，公式由 LaTeX 原生处理。

**文学编程 (Literate Programming)**

-   Babel 功能使得 Org mode 成为优秀的文学编程工具。
-   核心思想：将代码、代码的说明文档、执行结果有机地组织在同一个 Org 文件中。
-   演讲者案例：其 Emacs 配置文件 (`init.el`) 极简，只包含一行 `(org-babel-load-file "path/to/configuration.org")`。
-   实际的配置逻辑和说明都在 `configuration.org` 文件中，通过带有 `:tangle yes` (视频未明确提，但这是标准做法) 或直接执行的方式生效。
-   优点：
    -   配置文档化、易于理解和维护。
    -   适合教程、报告、可复现研究等场景。
-   观点：文学编程不一定适用于所有软件开发场景 (特别是快速迭代的项目，维护成本可能较高)，但非常适合配置文件、书籍、论文等相对稳定或以教学为目的的内容。

**任务管理 (To-Do / GTD)**

-   Org mode 是强大的个人任务管理系统，支持 GTD (Getting Things Done) 方法论。
-   **创建与标记任务**
    -   在标题前加上 `TODO` 关键字即可将其标记为待办任务 (关键字可自定义)。
    -   `Shift+Meta+Enter` (Shift+Alt+Enter) 可快速创建新的同级 TODO 项。
-   **任务状态切换**
    -   `C-c C-t` (Ctrl+C Ctrl+T) 可按预设流程循环切换任务状态 (e.g., `TODO` -> `DONE` -> 无状态)。
    -   可以自定义状态关键字和转换流程 (e.g., 添加 `WAITING`, `CANCELLED` 等状态)。
    -   任务完成 (切换到 `DONE` 状态) 时，会自动添加 `CLOSED:` 时间戳。
-   **时间管理**
    -   `C-c C-d` (Ctrl+C Ctrl+D) 为任务设置截止日期 (Deadline)，会弹出日历供选择。
    -   `C-c C-s` (Ctrl+C Ctrl+S) 为任务设置计划开始日期 (Scheduled)。
    -   `Shift+方向键` 可在日期上快速调整年/月/日。
-   **Agenda 视图**
    -   `C-c a` (Ctrl+C a) 打开强大的 Agenda 视图。
    -   可以聚合来自多个 Org 文件的任务和日程信息。
    -   提供日视图、周视图、全局 TODO 列表、按标签/优先级/类别过滤等多种视图。
    -   显示即将到期或已过期的任务。
-   **归档 (Archiving)**
    -   `C-c C-x C-a` (或 `C-c $`) 将已完成的任务移动到指定的归档文件中 (通常是同目录下或指定路径下的 `*.org_archive` 文件)。
    -   保持主 Org 文件整洁，同时保留完整的任务历史记录。
-   **任务管理哲学讨论**
    -   回应 Jeff Atwood 的 "每天只做三件事" 观点：演讲者认为对于需要长期跟踪或有明确时间点的事情 (如看牙医)，任务列表和提醒是必要的。
    -   强调仅对“硬性”截止日期使用 Deadline，避免虚假 Deadline 降低其约束力。
    -   提倡通过层级结构组织项目、定期“梳理”(grooming) 任务列表、明确“下一步行动”(next action) 来管理任务。

**高级功能与扩展**

-   **Org Capture**
    -   `C-c c` (Ctrl+C c) 触发 Capture 功能。
    -   允许通过预设模板快速捕捉笔记、任务、想法等，并自动存入指定 Org 文件的预定位置。
    -   演讲者绑定了 `Meta+n` (Alt+n) 作为快捷键。
-   **Org Publish**
    -   用于将一系列 Org 文件组成的“项目”发布为网站、文档集等。
    -   可以定义项目结构、应用模板、处理链接和资源文件。
    -   演讲者正在考虑用其替代 Jekyll 来构建个人博客。
-   **`org-drill`**
    -   一个基于 Org 文件内容的间隔重复学习 (Spaced Repetition) / 抽认卡 (Flashcard) 工具。
-   **移动端支持**
    -   `org-mobile` (官方，早期体验不佳)。
    -   `Orgzly` (Android 应用，社区推荐，功能较完善)。
    -   `Drafts` (iOS 应用，可通过动作将文本处理后发送到 Org 文件，适合快速捕捉)。

**同步与外部工具**

-   **同步方案**
    -   演讲者使用 `ownCloud` (一个开源、自托管的云存储和协作平台) 在电脑和可能存在的移动设备间同步包含 Org 文件的目录。
-   **ownCloud 简介**
    -   提供类似 Dropbox 的文件同步功能。
    -   提供日历 (CalDAV) 和联系人 (CardDAV) 服务。
    -   演讲者用它替代 Google Calendar 等服务。
    -   可在自己的服务器上部署，掌控数据。
-   **版本控制**
    -   目前演讲者未对其 Org 文件直接使用 Git 等版本控制系统进行管理，但有考虑过。

**总结**

-   Org mode 是一个极其强大和灵活的 Emacs 模式，集大纲编辑、标记语言、任务管理、文学编程、导出发布等多种功能于一身。
-   虽然初看起来可能复杂，但其纯文本、可扩展的特性使其深受许多用户喜爱。