## Workflow

Nicholas J. Higham

Workflow refers to everything involved in producing a mathematical paper other than the actual research. It is about the practicalities of how to do things, including how best to use different kinds of software for differ- ent tasks. The characteristics of a good workflow are that it allows the end result to be achieved efficiently, repeatably, and in a way that allows easy recovery from mistakes.

"Workflow" 指的是生成数学论文时除了实际研究外的所有内容。它涉及到如何实际操作的实用性，包括如何最好地使用不同类型的软件来完成不同的任务。一个良好的工作流的特征在于它能够高效、可重复地实现最终结果，并且能够轻松纠正错误。

### 1 Typesetting: TEX and LATEX

 1 排版：TEX 和 LATEX


In the days before personal computers, articles would be handwritten, then typed on a typewriter by a secre- tary, and ultimately typeset by a publisher. Nowadays, almost every author prepares the article herself or him- self on a computer, and the publisher works from the author’s files. In many areas of academia it is the cus- tom to use Microsoft Word, or an open-source equiv- alent. In mathematics, computer science, and physics LATEX has become the de facto standard.

在个人计算机出现之前，文章通常是手写的，然后由秘书使用打字机打字，最终由出版商进行排版。如今，几乎每位作者都会在计算机上自己准备文章，出版商则从作者的文件中进行工作。在许多学术领域，习惯上使用Microsoft Word或开源的等效软件。在数学、计算机科学和物理学中，LATEX 已成为事实上的标准。

TEX is a typesetting system invented by Donald Knuth in the late 1970s that has a particular strength in han- dling mathematics. LATEX is a macro package, written originally by Leslie Lamport, that sits on top of TEX. A TEX or LATEX file is an ASCII (plain text) file that contains commands that specify how the output is to be format- ted, and it must be compiled to produce the final output (nowadays usually a Portable Document Format (PDF) file). This contrasts with a WYSIWYG (“what you see is what you get”) word processor, such as Microsoft Word, that displays on the screen a representation of what the output will look like. TEX allows finer control than word processors (the latter are sometimes described as “what you see is all you get”), and the ability of LATEX to use style files that set various typesetting parameters makes it very easy to adjust the format of an article to match a particular journal. LATEX is also well suited to large projects such as books. Indeed, this volume is typeset in LATEX, and the editors and production editor find it hard to imagine having produced the volume in any other way.

TEX 是由 Donald Knuth 在 1970 年代末发明的一种排版系统，其在处理数学方面具有特殊优势。LATEX 是一个宏包，最初由 Leslie Lamport 编写，它位于 TEX 之上。TEX 或 LATEX 文件是一个ASCII（纯文本）文件，其中包含指定输出格式的命令，必须进行编译以生成最终输出（现在通常是一个便携式文档格式（PDF）文件）。这与所见即所得的文字处理器（如Microsoft Word）形成对比，后者在屏幕上显示输出的表示形式。TEX 允许比文字处理器更精细的控制（后者有时被描述为“所见即所得”），而LATEX能够使用设置各种排版参数的样式文件，使得很容易调整文章的格式以匹配特定的期刊。LATEX 也非常适用于大型项目，如书籍。实际上，本卷就是使用LATEX排版的，编辑和制作编辑难以想象以其他方式制作本卷。

Figure 1 shows some LATEX source code. Although how the code is formatted makes no difference to the out- put, it is good practice to make the source as readable as possible, with liberal use of spaces. I like to start new sentences on new lines, which makes it easier to cut and paste them during editing.

图1显示了一些LATEX源代码。尽管代码的格式对输出没有影响，但将源代码编写得尽可能可读是一个良好的做法，要大量使用空格。我喜欢在新的一行开始新的句子，这样在编辑时更容易进行剪切和粘贴。

TEX and LATEX are open-source software and are avail- able in various distributions. In particular, the TEX Live distribution is available for Windows, Linux, and Mac systems (and as the augmented MacTEX for the latter).

TEX 和 LATEX 是开源软件，可在各种发行版中使用。特别是，TEX Live 发行版适用于Windows、Linux和Mac系统（对于后者，还有增强版的 MacTEX）。

How does one go about using LATEX? There are two approaches. The first is to edit the LATEX source in a general-purpose text editor such as Emacs, Vim, or a system-specific text editor. Ideally, the editor is cus- tomized so that its syntax highlights the LATEX source, can directly compile the document, can pinpoint the location of compilation errors in the source, and can invoke a preview of the compiled document with two-way synchronization between the location of the cur- sor in the source and the page of the preview. I use Emacs together with the AUCTEX and RefTEX packages, which provides an extremely powerful LATEX environ- ment; indeed I use Emacs for all my editing tasks, rang- ing from programming to writing emails. A popular alternative is to use a program designed specifically for editing LATEX documents, which typically comes with an integrated previewer. Such programs tend to be system specific.

如何使用 LATEX 呢？有两种方法。第一种是在通用文本编辑器（如Emacs、Vim或系统特定的文本编辑器）中编辑 LATEX 源代码。理想情况下，编辑器应该定制，以便对 LATEX 源代码进行语法突出显示，能够直接编译文档，能够准确定位源代码中的编译错误位置，并能够在源代码中的光标位置和预览页面之间进行双向同步。我使用Emacs与AUCTEX和RefTEX软件包一起，提供了一个非常强大的 LATEX 环境；事实上，我将Emacs用于所有的编辑任务，从编程到编写电子邮件都涵盖其中。一个流行的替代方案是使用专门设计用于编辑 LATEX 文档的程序，通常带有集成的预览功能。这类程序往往是系统特定的。

TEX compiles to its own DVI (device independent) file format, which can then be translated into PostScript, a file format commonly used for printing. The stan- dard format for distributing documents is now PDF. While PostScript can be converted to PDF, versions of TEX and LATEX that compile directly to PDF are available (typically invoked as pdftex and pdflatex). Whether one is using the DVI-based or PDF-based versions of LATEX affects how one generates graphics files for inclu- sion in figures. For DVI, included figures are typically in encapsulated PostScript format, whereas for PDF graphics files are typically in PDF or JPEG format and PostScript files are not allowed. I use a PDF workflow, though the Companion itself uses DVI and PostScript, because many of the figures in the book needed fine- tuning and this is more easily done in PostScript than in PDF. It is important to note that the Adobe Acrobat program is not suitable for use as a PDF previewer in the edit–compile–preview cycle as it does not refresh the view when a PDF file is updated on disk. Various open-source alternatives are available that do not have this limitation.

TEX 编译成其自己的 DVI（设备无关）文件格式，然后可以将其翻译成 PostScript，这是常用于打印的文件格式。现在分发文档的标准格式是 PDF。虽然可以将 PostScript 转换为 PDF，但直接编译为 PDF 的 TEX 和 LATEX 版本也是可用的（通常被称为 pdftex 和 pdflatex）。使用基于 DVI 或基于 PDF 的 LATEX 版本会影响生成用于包含在图中的图形文件的方式。对于 DVI，包含的图形通常是封装的 PostScript 格式，而对于 PDF，图形文件通常是 PDF 或 JPEG 格式，不允许使用 PostScript 文件。我使用的是 PDF 工作流程，尽管《指南》本身使用的是 DVI 和 PostScript，因为书中的许多图形需要进行微调，而在 PostScript 中比在 PDF 中更容易完成。重要的是要注意，Adobe Acrobat 程序不适合作为编辑-编译-预览周期中的 PDF 预览器，因为它在磁盘上的 PDF 文件更新时不会刷新视图。有各种开源替代方案可用，它们不具有这个限制。

### 2 Preparing a Bibliography

2 准备参考文献

A potentially time-consuming and error-prone part of writing a paper is preparing the bibliography, which
contains the bibliographic details of the articles that are cited. In a LATEX document the bibliography entries are cited with a command of the form \cite{smit65}, where smit65 is a key that uniquely specifies the entry in a bibliography environment that contains the item being cited. LATEX has a companion program called BibTEX that extracts bibliography entries from a database contained in a bib file (an ASCII file of a special structure with a .bib extension) and automati- cally creates the bibliography environment. Figure 2 shows an example of a bib file entry. Using BibTEX is a great time-saver and ensures accurate bibliographies, assuming that the bib file is accurate and kept up to date. Most journal Web sites allow BibTEX entries for papers to be downloaded, so it is easy to build up a personal bib file. There exist open-source BibTEX refer- ence managers (such as JabRef) that facilitate creating and maintaining bib files.

写论文中可能是一项耗时且容易出错的工作的一部分是准备参考文献，其中包含引用文章的文献详细信息。在 LATEX 文档中，使用类似 \cite{smit65} 的命令引用参考文献条目，其中 smit65 是一个键，唯一地指定了包含被引用项的参考文献环境中的条目。LATEX 有一个名为 BibTEX 的伴随程序，它从包含在 bib 文件中的数据库中提取参考文献条目（这是一个特殊结构的带有 .bib 扩展名的 ASCII 文件），并自动创建参考文献环境。图2显示了一个 bib 文件条目的示例。使用 BibTEX 是一个很好的时间节省工具，并确保准确的参考文献，前提是 bib 文件准确且保持更新。大多数期刊网站允许下载用于论文的 BibTEX 条目，因此很容易建立起个人的 bib 文件。存在开源的 BibTEX 参考管理器（例如 JabRef），可以方便地创建和维护 bib 文件。


A digital object identifier (DOI) is a character string that uniquely identifies an electronic document. It can be resolved into a uniform resource locator (URL) by preceding it with the string http://dx.doi.org/. Nowa- days most papers (and many books) have DOIs and many older papers have been assigned DOIs. A DOI remains valid even if the location of the document changes, provided that the publisher updates the meta- data. It is recommended to record DOIs in BibTEX databases, and it is then possible with the use of a suit- able BibTEX style file and the LATEX hyperref package to include clickable links in a paper’s bibliography (for example, from a paper’s title).

数字对象标识符（DOI）是一个字符串，用于唯一标识电子文档。可以通过在其前面加上字符串 http://dx.doi.org/ 来将其解析为统一资源定位符（URL）。如今，大多数论文（以及许多书籍）都有DOI，许多早期的论文也被分配了DOI。即使文档的位置发生变化，只要出版商更新元数据，DOI仍然有效。建议在BibTEX数据库中记录DOI，然后使用适当的BibTEX样式文件和LATEX hyperref包，可以在论文的参考文献中包含可点击的链接（例如，从论文的标题）。

### 3 Graphics

3 图形

Mathematics papers often contain figures that plot functions, depict physical setups, or graph experimen- tal results. These can be produced in many different ways. In a LATEX workflow one can generate a graphic outside LATEX and then include it as an external JPEG, PostScript, or PDF file or generate it from within LATEX.


数学论文通常包含绘制函数、描绘物理设置或绘制实验结果的图形。这些图形可以通过许多不同的方式生成。在 LATEX 工作流程中，可以在 LATEX 外部生成图形，然后将其作为外部 JPEG、PostScript 或 PDF 文件包含，或者在 LATEX 中生成它。

The most popular LATEX packages for graphics are TikZ and PGFPlots, which are built on top of the low-level primitives provided by the PGF (portable graphics for- mat) package. Most of the figures in part I of this vol- ume were generated using these packages. A major benefit of them is that they can incorporate LATEX com- mands and fonts, thus providing consistency with the main text. These powerful packages are not easy to use, but one can usually find an example online that provides a starting point for modification.

用于图形的最流行的 LATEX 包是 TikZ 和 PGFPlots，它们建立在由 PGF（便携图形格式）包提供的低级原语之上。本卷第I部分中的大部分图形都是使用这些包生成的。它们的一个主要优势是可以结合 LATEX 命令和字体，从而与主文本保持一致。这些强大的包并不容易使用，但通常可以在线找到一个示例，为修改提供一个起点。

### 4 Version Control and Backups

4 版本控制和备份

Every good workflow contains procedures for making regular backups of files and recording a history of dif- ferent versions of the files. Backups store one or more copies of the current version of key files on a separate disk or machine, so that a hard disk failure or the loss of a complete machine does not result in loss of files. Version control serves a different purpose, which is to record in a repository intermediate states of files so that authors can revert to an earlier version of a file or reinstate part of one. The use of the plural in “authors” refers to the fact that version control systems allow more than one user to contribute to a repository and allow any user to check out the latest versions of files. Although version control originated in software devel- opment, it is equally useful for documents. As long as the repository is kept on a different disk or machine, version control also provides a form of backup.

每个良好的工作流都包含定期备份文件并记录文件的不同版本历史的程序。备份将关键文件的当前版本的一个或多个副本存储在单独的磁盘或机器上，以便硬盘故障或整个机器丢失不会导致文件丢失。版本控制有不同的目的，即记录文件的中间状态，以便作者可以还原到文件的早期版本或重新启用部分文件。在“作者”中使用复数形式是因为版本控制系统允许多个用户贡献到一个存储库，并允许任何用户检出文件的最新版本。尽管版本控制起源于软件开发，但它对文档同样有用。只要存储库保存在不同的磁盘或机器上，版本控制也提供了一种形式的备份。

Of course a simple version control system is to regu- larly copy a file to another directory, renaming it with a version number (paper1.tex, paper2.tex, . . . ). However, this is tedious and error prone. A proper version con- trol system keeps files in a database and stores only the lines that have changed between one version and the next. Popular version control systems include Git and Subversion (SVN). Although these are command based and can be difficult to learn, graphical user interfaces (GUIs) are available that simplify their usage.

当然，一个简单的版本控制系统是定期将文件复制到另一个目录，并用版本号重命名它（例如，paper1.tex，paper2.tex，...）。然而，这种方法繁琐且容易出错。一个正确的版本控制系统将文件保存在数据库中，仅存储在一个版本和下一个版本之间发生变化的行。流行的版本控制系统包括 Git 和 Subversion（SVN）。尽管它们是基于命令的，可能难以学习，但也提供了简化使用的图形用户界面（GUI）。

Microsoft Word’s “track changes” feature provides annotations of who made what changes to a document (and is a primitive and widely used form of version con- trol). In LATEX a similar effect can be achieved by using the latexdiff command-line program provided with some LATEX distributions, which takes as input two dif- ferent version of a LATEX file and produces a third LATEX file that marks up the differences between them; see figure 3 for an example.

Microsoft Word的“跟踪更改”功能提供了对文档进行何种更改的注释（这是一种原始且广泛使用的版本控制形式）。在LATEX中，可以通过使用一些LATEX发行版提供的latexdiff命令行程序来实现类似的效果。该程序接受两个不同版本的LATEX文件作为输入，并生成一个标记它们之间差异的第三个LATEX文件；请参见图3中的示例。

### 5 Computational Experiments

5 计算实验

In papers that involve computational experiments, one needs to include figures or tables summarizing the results. It is typical that as a paper is developed the experiments are refined and repeated. One therefore needs an efficient way to regenerate tables and figures. Cutting and pasting the output of a program into the paper is not a good approach. It is much better to make the program output the results in a form that can be directly included in the paper (e.g., via an \input com- mand in LATEX). literate programming [VII.11] tech- niques allow program code to be included within the source code for a paper, and they automate the run- ning of the programs and the insertion of the results back into the paper source code.

在涉及计算实验的论文中，需要包含总结结果的图形或表格。随着论文的发展，实验通常会被完善和重复。因此，需要一种有效的方法来重新生成表格和图形。将程序的输出剪切并粘贴到论文中不是一个好的方法。最好的做法是让程序以可以直接包含在论文中的形式输出结果（例如，通过在LATEX中使用 \input 命令）。文学编程技术允许将程序代码包含在论文的源代码中，并自动运行程序并将结果插入回论文源代码中。


### 6 Putting It All Together

6 统稿

Here are the things I do when I start to write a paper. I create a directory (folder) with a name that denotes the project in question. In that directory I copy a file paper.tex from a recent paper that I have written and use it as a template. I delete most of the content of paper.tex but keep the macros and some of the basic structural commands. I set up a repository in my ver- sion control system and commit paper.tex to it. I cre- ate a subdirectory for the computer programs I will write and a subdirectory named figs into which the PDF figures will be placed.

在开始写论文时，我会进行以下几个步骤。我创建一个目录（文件夹），以表示所涉及的项目。在该目录中，我从我最近写过的一篇论文中复制一个文件paper.tex，并将其用作模板。我删除paper.tex的大部分内容，但保留宏和一些基本的结构性命令。我在版本控制系统中设置一个存储库，并将paper.tex提交到其中。我创建一个用于编写计算机程序的子目录，以及一个名为figs的子目录，用于放置PDF图形。

### 7 Presentations

7 演示

As well as writing a paper about a piece of research, one may want to give a presentation about it in a seminar or at a conference. This will normally involve preparing slides or a poster, although it is still sometimes possible to give a blackboard talk. LATEX has excellent tools for preparing slides and posters.

除了写一篇关于某项研究的论文外，人们可能还想在研讨会或会议上进行相关演示。这通常涉及准备幻灯片或海报，尽管有时候还可以进行黑板演讲。LATEX有出色的工具用于准备幻灯片和海报。

The Beamer class is the most widely used way to pre- pare slides in LATEX. It can create overlays, allowing aslide to change dynamically (perhaps as an equation is built up, a piece at a time). Slide color and back- ground, and elements such as a header (which may con- tain a mini-table of contents) and a footer, are all readily customized. Figure 4 shows an example slide.

Beamer类是在LATEX中准备幻灯片最广泛使用的方式。它可以创建覆盖层，允许幻灯片动态变化（例如，逐步构建方程式）。幻灯片的颜色、背景以及诸如页眉（可能包含一个小目录）和页脚等元素都可以轻松定制。图4显示了一个示例幻灯片。

Various LATEX packages are available for producing posters, at up to A0 paper size. A popular one is the beamerposter package built on Beamer.

有各种LATEX包可用于制作海报，可达到A0纸张大小。其中一个流行的包是基于Beamer的beamerposter包。

### 8 Collaboration

8 合作

In the early days of the Internet the most common way for authors to collaborate was to email documents back and forth. A regularly encountered problem was that Unix mailers would insert a greater than sign in front of any word “from” that appeared at the start of a line of a plain text message, so LATEX files would often have stray > characters. For many people, email still serves as a useful mechanism for collaborative writing, but more sophisticated approaches are available. A file-hosting service such as Dropbox enables a group of users to share and synchronize a folder on their disks via the cloud. Version control based on a shared repository hosted on the Internet is the most powerful approach; it is widely used by programmers (e.g., on sites such as GitHub and SourceForge) and is increasingly popular with authors of papers.

在互联网早期，作者进行协作的最常见方式是通过电子邮件来回传递文档。经常遇到的问题是Unix邮件程序会在纯文本消息的行首插入一个大于号，该行以单词“from”开头，因此LATEX文件经常会出现杂乱的 > 字符。对许多人来说，电子邮件仍然是进行协作写作的有用机制，但也有更复杂的方法可用。文件托管服务（如Dropbox）可以使一组用户通过云共享和同步他们磁盘上的文件夹。基于在互联网上托管的共享存储库的版本控制是最强大的方法；它被程序员广泛使用（例如在GitHub和SourceForge等站点上），并且在论文作者中越来越受欢迎。

### 9 Workflow for This Book

9 本书的工作流

I wrote my articles using Emacs and TEX Live, with all files under version control with Git. I edited some of my figures in Adobe Photoshop. The production editor/ typesetter, Sam Clark, used WinEdt and TEX Live with a PostScript-based workflow, editing PostScript figures in Adobe Illustrator.

I produced a draft index for the articles that I authored using LATEX indexing commands and the Make- Index program. A professional indexer then expanded the index to cover the whole book.

The font used for this book is Lucida Bright, which has a full set of mathematical symbols that work well in TEX. It is from the same family as the Lucida Grande sans serif font that was used throughout the Mac OS X user interface up until version 10.9.

我使用Emacs和TEX Live编写我的文章，所有文件都在Git版本控制下。我在Adobe Photoshop中编辑了一些图形。制作编辑/排版者Sam Clark使用WinEdt和TEX Live进行基于PostScript的工作流，使用Adobe Illustrator编辑PostScript图形。

我为我编写的文章制作了初稿索引，使用了LATEX索引命令和MakeIndex程序。然后，一位专业的索引制作人扩展了索引，涵盖整本书。

本书使用的字体是Lucida Bright，它具有在TEX中良好工作的完整数学符号集。它与Lucida Grande无衬线字体同属于同一字体家族，后者曾在Mac OS X用户界面中一直使用到版本10.9。

### Further Reading

Of the many good references on LATEX I recommend Grif- fiths and D. J. Higham (1997) for a brief introduction and Kopka and Daly (2004) for a more comprehensive treatment. Knuth (1986) continues to be worth read- ing, even for those who use only LATEX. Various aspects of workflow are covered in Higham (1998). Version con- trol is best explored with the many freely available Web resources.

A good place to start looking for information about TEX and LATEX is the Web site of the TEX Users Group, http://tug.org. A large collection of LATEX packages is available at the Comprehensive TeX Archive Network (CTAN), http://www.ctan.org.

进一步阅读

在众多关于LATEX的良好参考资料中，我推荐Griffiths和D. J. Higham（1997）进行简要介绍，以及Kopka和Daly（2004）进行更全面的处理。Knuth（1986）仍然值得阅读，即使是那些仅使用LATEX的人。关于工作流的各个方面在Higham（1998）中有所涉及。版本控制最好通过众多免费提供的网络资源进行探索。

关于TEX和LATEX的信息，一个很好的起点是TEX用户组的网站，http://tug.org。大量的LATEX包可以在综合TeX档案网络（CTAN），http://www.ctan.org上找到。

Griffiths, D. F., and D. J. Higham. 1997. Learning LATEX. Philadelphia, PA: SIAM.
Higham, N. J. 1998. Handbook of Writing for the Mathemat- ical Sciences, 2nd edn. Philadelphia, PA: SIAM.
Knuth, D. E. 1986. The TEXbook. Reading, MA: Addison- Wesley.
Kopka, H., and P. W. Daly. 2004. Guide to LATEX, 4th edn. Boston, MA: Addison-Wesley.