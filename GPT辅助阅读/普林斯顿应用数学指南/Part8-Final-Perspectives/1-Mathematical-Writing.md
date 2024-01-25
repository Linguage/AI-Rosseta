## VIII.1 Mathematical Writing
Timothy Gowers

### 1 Introduction

1 导言

The purpose of this article is not to offer advice about how to write mathematics well. Such advice can be found in many places. However, I do have three pieces of very general advice, which inform the rest of the arti- cle. The first is to be clear about your intended read- ership; for example, if you want what you write to be understood by an undergraduate, then do not assume knowledge of any terminology that is not standardly taught in undergraduate mathematics courses. The sec- ond is to aim for this readership to be as wide as pos- sible. If, with a small amount of extra explanation, you can make what you write comprehensible to an expert in another field of mathematics, then put in that extra effort. Whatever you do, do not worry that experts will not need the explanation; if that is true (which it often is not), then they can easily skip it. The third, which is related to the second, is to set the scene before you start. Some people who read what you have written will do so because they want to understand all the techni- cal details and use them in their own work, but the vast majority will not. Most readers, including people who need to make quick judgments that will profoundly affect your career, will want to read the introduction quickly to see what you have done and assess how important it is. However much you might wish every- one to read what you have written in complete detail, you should be realistic and cater for readers who just want to skim it.

本文的目的并不是提供如何写好数学的建议。这样的建议可以在许多地方找到。然而，我有三条非常普遍的建议，这些建议构成了本文的基础。第一条是要明确你的目标读者群体；例如，如果你希望你所写的内容被本科生理解，那么就不要假设他们掌握本科数学课程中未被标准教授的任何术语。第二条是要尽可能拓展你的读者群体。如果通过一点额外的解释，你可以使你所写的内容对另一个数学领域的专家可理解，那么就付出额外的努力。无论你做什么，都不要担心专家不需要解释；如果这是真的（通常并非如此），那么他们可以轻松跳过它。第三条，与第二条相关，是在开始之前设定场景。一些阅读你所写内容的人这样做是因为他们想要理解所有的技术细节并在自己的工作中使用它们，但绝大多数人不会。大多数读者，包括那些需要做出对你的职业生涯产生深远影响的快速判断的人，都希望快速阅读介绍，以了解你所做的工作并评估其重要性。无论你多么希望每个人都仔细阅读你所写的内容，你都应该保持现实，并为那些只想浏览的读者提供便利。

For the rest of this article I shall discuss various choices that one must make when writing a mathemat- ical document. I will not advocate choosing one way rather than another, since the choices you should make depend on what you want to achieve; my final piece of general advice is merely that you should make the choices consciously rather than by accident.

在本文的其余部分，我将讨论在撰写数学文档时必须做出的各种选择。我不会主张选择一种方式而不是另一种，因为你应该做出的选择取决于你想要实现的目标；我最后的一条普遍建议只是你应该有意识地做出选择，而不是偶然间做出选择。

### 2 Formality versus Informality

2 正式性与非正式性

There are (at least) two goals that one might have when writing a mathematical document. One is to establish a mathematical result by whatever means are appropri- ate to the field; in pure mathematics the usual require- ment is unambiguous definitions and rigorous proofs, whereas in applied mathematics other forms of evi- dence, such as heuristic arguments and experimental backing, may be acceptable. The other is to convey mathematical ideas to the reader.

撰写数学文档时可能有（至少）两个目标。一个目标是通过适合领域的手段建立数学结果；在纯数学中，通常要求清晰明确的定义和严格的证明，而在应用数学中，其他形式的证据，如启发式论证和实验支持，可能是可以接受的。另一个目标是向读者传达数学思想。

These two goals are often in tension. If a pure math- ematician discovers a complicated proof of a theorem, then that proof will be hard to understand. However, sometimes the apparent complication of a proof is mis- leading; what is really going on is that the author had one or two key ideas, and the complication of the argu- ment is the natural working out of the details of those ideas. For the expert reader, an informal explanation of the ideas that drive the proof may well be more valuable than the proof itself.

这两个目标经常存在紧张关系。如果一位纯数学家发现了一个复杂的定理证明，那么那个证明将很难理解。然而，有时证明的表面复杂性是误导性的；真正的情况可能是作者有一两个关键的想法，而证明的复杂性是这些想法细节的自然展开。对于专业读者来说，对证明驱动思想的非正式解释很可能比证明本身更有价值。

Nobody would advocate writing papers with just informal explanations of ideas, since plausible-looking ideas often turn out not to work. However, there is still a choice to make, since it is considered acceptable to display proofs and not explain the underlying ideas. There may sometimes be circumstances where this is appropriate; for example, perhaps the proof is short, and explaining the ideas that generate it will double the length of what you are writing and put off readers. But usually, the advice I gave earlier—to broaden your readership if it not too difficult to do so—would dic- tate that technical arguments should be accompanied by informal explanations.

没有人会主张仅仅使用对思想的非正式解释来撰写论文，因为看似合理的想法往往最终不起作用。然而，仍然存在选择，因为显示证明而不解释其潜在思想是被认为是可以接受的。可能有时候存在这样的情况；例如，也许证明很简短，解释产生它的思想将使你所写的内容长度加倍并使读者失去兴趣。但通常，我之前给出的建议——如果不是太困难的话，扩大你的读者群体——会决定技术论证应该附有非正式解释。

### 3 Giving Full Detail versus Leaving Details to the Reader

3 提供充分细节与留给读者的细节

When you are writing you need to decide how much detail to give. If you give too little, then the reader you are aiming at will not be able to understand what you have written. But you also want to avoid making too many points that the reader will find completely obvious.

在写作过程中，你需要决定给出多少细节。如果你给得太少，那么你所针对的读者将无法理解你所写的内容。但你也要避免提出太多读者完全显而易见的观点。

Of these two potential problems, the first is undoubt- edly more serious. It is much easier for readers to skip details that they find too obvious to be worth saying than it is for them to fill in details that they do not find obvious at all.

在这两个潜在的问题中，第一个无疑更为严重。读者要跳过他们认为过于显而易见而不值得说的细节要容易得多，而填补他们根本不觉得显而易见的细节则要困难得多。

The question of how much detail to give is related to the question of how formal to be, but it is not the same question. It is true that there is a tendency in informal mathematical writing to leave out details, but with even the most formal writing a decision has to be made about how much detail to give; it is just that in formal writing one probably wants to signal more care- fully when details have been left out. This can be done in various ways. One can use expressions such as “It is an easy exercise to check that...,” or “The second case is similar,” which basically say to the reader, “I have decided not to spell out this part of the argument.” One can also give small hints, such as “By compact- ness,” or “An obvious inductive argument now shows that...,” or “Interchanging the order of summation and simplifying, we obtain....”

给出多少细节的问题与形式化程度有关，但并非相同的问题。在非正式的数学写作中，通常会有意忽略细节，但即使在最正式的写作中，也必须决定给出多少细节；只是在正式写作中，可能希望更加谨慎地表明细节被省略了。这可以通过各种方式来实现。可以使用诸如“很容易验证...”或“第二种情况类似”这样的表达方式，基本上告诉读者，“我已经决定不详细说明论证的这一部分。”也可以给出一些小提示，比如“通过紧致性”，或“一个明显的归纳论证现在表明...”，或“交换求和顺序并简化，我们得到...”。

If you do decide to leave out detail, it is a good idea to signal to the reader how difficult it would be to put that detail in. A mistake that some writers make is to give references to other papers for arguments that can eas- ily be worked out by the reader, without saying that the particular result that is needed is easy. This is straight- forwardly misleading; it suggests that the best thing to do is to go and look up the other paper when in fact the best thing to do is to work out the argument for oneself.

如果你决定省略细节，向读者表明放入这些细节的难度是一个好主意。一些写作者犯的错误是为那些读者很容易解决的论证给出其他论文的参考文献，而没有说明所需要的特定结果是很容易的。这是直接误导性的；它暗示着最好的做法是去查找其他论文，而事实上最好的做法是自己解决论证。

### 4 Letters versus Words

4 符号vs词语

The following is problem 10 of book 1 of an English translation of Diophantus’s Arithmetica.
Given two numbers, to add to the lesser and to subtract from the greater the same (required) number so as to make the sum in the first case have to the difference in the second case a given ratio.

以下是《Diophantus's Arithmetica》英文译本第一册的第10题问题。
给定两个数，为了使第一个情况的和与第二个情况的差之间有一个给定的比率，加到较小的数上并从较大的数上减去相同（必需）的数。


A modern writer would express the same problem more like this.

> Given two numbers $a$ and $b$ and a ratio $\rho$, find $x$ such that $a+x=\rho(b-x)$.

一个现代的写作者可能会更像这样表达同样的问题。

> 给定两个数$a$和$b$以及一个比率$\rho$，找到$x$使得$a+x=\rho(b-x)$成立。

The main difference between these two ways of describ- ing the problem is that in the second formulation the numbers under discussion have been given names. These names take the form of letters, which allow us to replace wordy expressions such as “the second number” or “the given ratio” by letters such as $b$ and $\rho$.”

在描述问题的这两种方式之间的主要区别在于，在第二种表述中，讨论的数字已经被赋予了名称。这些名称采用字母的形式，使我们能够用字母如$b$和$\rho$代替冗长的表达，比如“第二个数字”或“给定的比率”。

The advantage of modern notation is that it is much more concise. This is not just a matter of saving paper; the extra length of “to make the sum in the first case have to the difference in the second case a given ratio” over “such that $a+x=\rho(b-x)$” makes it significantly harder to understand because it is difficult to take in the entire phrase at once.

现代符号的优势在于它更加简洁。这不仅仅是为了节约纸张；“使第一个情况的和与第二个情况的差之间有一个给定的比率”的长度比“$a+x=\rho(b-x)$”长很多，这使得理解起来更加困难，因为很难一次理解整个短语。

However, the concision that comes from naming mathematical objects comes at a cost: one has to learn the names. In the example above, that is very easy and the cost is negligible. However, sometimes it is far from negligible. The following proposition comes from a paper in Banach space theory.

然而，通过给数学对象命名而产生的简洁性是有代价的：人们必须学会这些名称。在上面的例子中，这非常容易，成本可以忽略不计。然而，有时候这个成本远非可以忽略的。下面的命题来自Banach空间理论的一篇论文。

> **Proposition.** Let $0\leqslant\alpha\leqslant\frac12$ and $1/p=\frac12-\alpha.$ Then
$$
\mathfrak{P}_2(E,F)\subset\mathfrak{L}_{p,\infty}^{(a)}(E,F)
$$
for all Banach spaces $F$ if and only if $E\subset \Gamma_{\alpha}.$

> **命题.** 设$0\leqslant\alpha\leqslant\frac12$且$1/p=\frac12-\alpha.$ 那么对于所有的Banach空间$F$，当且仅当$E\subset \Gamma_{\alpha}$时，
$$\mathfrak{P}_2(E,F)\subset\mathfrak{L}_{p,\infty}^{(a)}(E,F)$$ 
> 成立。

Just before the proposition, the reader has been told that $\mathfrak{p}_{2}$ is the ideal of 2-summing operators from $E$ to $F$, which is a standard definition in the area. As for $\mathcal{L}_{p,\infty}^{(a)}(E,F)$, this has been defined early in the paper as follows. (It is not necessary to understand these definitions to understand the point I am making.)

在命题之前，读者已被告知 $\mathfrak{p}_{2}$ 是从$E$到$F$的2-求和算子的理想，这是该领域的一个标准定义。至于 $\mathcal{L}_{p,\infty}^{(a)}(E,F)$，它在文章的开头被定义如下。（理解这些定义并不是理解我所要表达的观点所必需的。）

Given an operator $T$, the $approximation~ number$  $a_n(T)$ is defined to be $\inf \{ \|T- L\|:$ rank$( L) < n\} .$ Then 
$\mathfrak{L}_{s,w}^{(a)}(E,F)$ is the set of operators $T$ such that the sequence $(a_n(T))_{n=1}^\infty$ belongs to the Marcinkiewicz space $\ell_{s,w}.$


给定一个算子$T$，$逼近数$ $a_n(T)$被定义为$\inf \{ \|T- L\|:$ rank$( L) < n\} .$ 然后，$\mathfrak{L}_{s,w}^{(a)}(E,F)$是那些使序列$(a_n(T))_{n=1}^\infty$ 属于Marcinkiewicz空间 $\ell_{s,w}$ 的算子 $T$ 的集合。

The definition of the Marcinkiewicz space is again standard in the area. Finally, the set $\Gamma_{\alpha}$ is defined to be the set of all Banach spaces of weak Hilbert type $\alpha$. That is not a standard definition, but it is given earlier on in the paper.

Marcinkiewicz空间的定义在该领域中也是标准的。最后，集合 $\Gamma_{\alpha}$ 被定义为所有弱希尔伯特类型 $\alpha$ 的Banach空间的集合。虽然这不是一个标准的定义，但它在论文的前面已经给出。


Thus, another way of stating the proposition is as follows.

> **Proposition**. Let $0\leqslant\alpha\leqslant\frac12$,let $1/p= \frac 12- \alpha, $and let $E$ be a Banach space. Then the following two statements are equivalent.
> - (1) For every Banach space $F$ and every 2-summing
operator  $T{:}E~\to~F$ , the sequence $(a_n(T))_{n=1}^{\infty}$  of approximation numbers belongs to the Marcinkiewicz space $\ell_{p,\infty}.$
> - (2) $E$ is a space of weak Hilbert type $\alpha.$


因此，陈述命题的另一种方式如下所示。

>**命题**. 设 $0\leqslant\alpha\leqslant\frac12$，令 $1/p= \frac 12- \alpha$，$E$ 是一个Banach空间。那么以下两个陈述是等价的。
> - (1) 对于每一个Banach空间 $F$和每一个2-求和算子$T{:}E~\to~F$，逼近数序列 $(a_n(T))_{n=1}^{\infty}$ 属于Marcinkiewicz空间 $\ell_{p,\infty}$。
> - (2) $E$是一个弱希尔伯特类型$\alpha$的空间。

This time, it is the wordier definition that places a smaller burden on the reader’s memory. If you know what 2-summing operators, approximation numbers, the Marcinkiewicz space, and weak Hilbert type are, most of which are standard definitions in the area, then you can understand without much effort what the proposition is claiming. With the first formulation, there is an extra step you have to perform to unpack the notation into those standard definitions. Another advantage of the second formulation is that a suffi- ciently expert reader who is skimming the paper will be able to understand it without having to look back in the paper to find out what everything means. The first formulation does not leave that option open.

这一次，更冗长的定义对读者的记忆负担较小。如果你知道什么是2-求和算子、逼近数、Marcinkiewicz空间和弱希尔伯特类型，其中大部分是该领域的标准定义，那么你就可以轻松理解命题在主张什么。对于第一种表述，你需要进行额外的步骤来将符号解释为这些标准定义。第二种表述的另一个优点是，足够熟练的读者在快速浏览论文时，能够理解其含义，而无需回头查找论文中所有术语的含义。第一种表述没有留下这个选择。

Thus, in more complicated mathematical writing, there is another source of tension. If you use too lit- tle notation, your sentences will become hopelessly clumsy and repetitive, but if you use too much, you are placing excessive demands on the memory of your readers.

因此，在更复杂的数学写作中，还存在另一个紧张关系的来源。如果你使用的符号太少，你的句子将变得笨拙而重复，但如果你使用的符号太多，你会对读者的记忆提出过高的要求。

This may be a delicate balance to strike, but there is one principle that applies universally: if you do decide to use some nonstandard notation, then make sure that the reader can easily find where it is defined. This can be done by means of a section devoted to preliminary definitions, though it will often be kinder to give defi- nitions just before they are used. If that is not possible, one can give reminders of definitions, or at the very least pointers to where they can be found.

这可能是一个微妙的平衡，但有一个普遍适用的原则：如果你决定使用一些非标准符号，那么确保读者能够轻松找到其定义是至关重要的。这可以通过专门的初步定义部分来实现，尽管在使用之前直接给出定义往往更友好。如果这样做不太可能，可以提醒读者定义，或者至少指出它们的位置。


### 5 Single Long Arguments versus Arguments Broken Up into Modules

If you are trying to justify a mathematical statement and the justification is long and complicated, then what you write may well be hard to understand unless you can somehow break the argument up into smaller “modules” that fit together to give you what you want. In pure mathematics, these modules usually take the form of lemmas. If you are proving a theorem and you do not want the proof to become unwieldy, then you try to identify parts of the argument that can be extracted and proved separately. One can then simply quote these results in the main argument. Lemmas play a role in proofs that is similar to the role of subroutines in computer programs.

For breaking up an argument to be a good idea, it greatly helps if the part of the argument you want to extract is not too context dependent. If the statement of a lemma requires a long piece of scene setting, then it is probably better to leave it in the main body of the argu- ment, where the scene has already been set. However, if it can be stated without reference to the particular con- text, which usually means that it is more general than the particular application needed of it in the main argu- ment, then it is more appropriate to extract it. Again, this is a matter of judgment.

A disadvantage of more modular arguments is that extracting lemmas, or more general modules, forces you to put them somewhere where they do not arise naturally. If you put them before the main argument, so that they will be available when needed, then the reader is presented with statements of no obvious use and is expected to remember them. If they are particu- larly memorable, then that is not a problem, but often they are not; for instance, they may depend on two or three slightly odd conditions that just happen to be satisfied in the later argument. If you put them after the main argument, then the reader keeps being told, “We will prove this claim later” and reaches the end of the argument with the uneasy feeling that the proof is incomplete. A third possibility is to state and prove lemmas within an argument, but nested statements of this kind can be fairly ugly.

With some complicated arguments, there may be no truly satisfactory solution to these problems. In that case, the best thing to do may well be to choose an unsatisfactory solution and mitigate the problems somehow. The default option is probably to state lem- mas before they are used. If you choose that option and the lemmas are somewhat complicated and hard to remember, then you can always add a few words of explanation about the role that the lemma will play. If even that is hard to do, then another option is to advise the reader to read the main argument first and return to the lemma only when the need for it has become clear. (An experienced reader may well do that anyway, but it is still helpful to be told by the author that it is a good approach to understanding the argument.)

### 6 Logical Order versus Order of Discovery

Suppose you wish to present the fact that a sequence of continuous functions that converges pointwise does not have to converge uniformly. Here is one way that you might do it.

**Theorem**. There exists a sequence of continuous functions $f_n:[0,1]\to[0,1]$ that converges pointwise but not uniformly.

**Proof**. For each positive integer $n$ and each $x\in[0,1]$, let $f_n(x)=nx\mathrm{e}^{-nx}$. Then, for $x>0$ we have e$^{-x}<1$, so $n\mathrm{e} ^{- nx}= n( \mathrm{e} ^{- x}) ^n\to 0$ as $n\to \infty.$ It follows that $f_n( x) \to 0$ as $n\to \infty$.Also, when $x= 0$ we have $f_n( x) =  0$ for every $n$ so again $f_n( x) \to 0$ as $n\to \infty.$ Therefore, $f_n(x)\to0$ pointwise.

However, the convergence is not uniform. To see this, observe that $f_n(n^{-1})=\mathrm{e}^{-1}$ for every $n$. Thus, for every $n$ there exists $x$ such that $|f_n(x)-0|\geqslant\mathrm{e}^{-1}.$   口

This proof has a feature that is common in mathe- matics: it is easier to follow the steps than it is to see where the steps came from. If you are told to try the functions $f_n(x)=nx\mathrm{e}^{-nx}$, then checking that they satisfy the conditions is a straightforward exercise, but what made anybody think of that particular sequence of functions?

Here is what we might write if we wanted to make the answer to that last question clearer.


**Proof**. If $f_n\to f$ pointwise but not uniformly, then $f_n-f\to0$ pointwise but not uniformly, so we may as well look for functions that converge to zero. In order to ensure that they do not converge uniformly to zero, we need a positive number $\theta$ such that for infinitely many $n$ there exists $x\in[0,1]$ with $|f_n(x)|\geqslant\theta.$ Since infinitely many of these $f_n(x)$ will have the same sign, and since we can multiply all functions by $\theta^{-1}$, we may as well look for a sequence of functions $f_n$ that converges pointwise to 0 such that for every $n$ there exists $x_n$ with $f_n(x_n)\geqslant1.$

**证明**: 如果$f_n\to f$逐点但不一致，那么$f_n-f\to0$逐点但不一致，因此我们不妨寻找收敛到零的函数。为了确保它们不一致地收敛到零，我们需要一个正数$\theta$，使得对于无限多个$n$，存在$x\in[0,1]$，
使得$|f_n(x)\geqslant\theta$。由于这些 $f_n(x)$中有无限多个将具有相同的符号，并且由于我们可以将所有函数乘以$\theta^{-1}$，因此我们不妨寻找一个函数序列$f_n$，它逐点收敛到0，使得对于每个$n$都存在$x_n$，使得$f_n(x_n)\geqslant1$。


Now, if $f_n( x_n) \geqslant 1$ and $f_n$ is continuous, then there exists an open interval $I_n=(x_n-\delta_n,x_n+\delta_n)$ around $x_n$ such that $f_n(y)\geqslant\frac12$ for every $y\in I_n.$ We are going to have to make sure that we do not have infinitely many of these intervals overlapping in some point $u$, since then we would have $f_n(u)\geqslant\frac12$ for infinitely many $n$, which would imply that $f_n(u)$ does not tend to zero.

How can we find infinitely many open intervals without infinitely many of them overlapping? The simplest way of doing it is to take intervals of the form $(a,b_n)$ for a sequence $(b_n)$ that converges to $a$. So, for example, we could take $I_n$ to be the interval $(0,1/n).$

This suggests that we should let $f_n$ be a continuous function that takes the value 1 somewhere inside the interval $(0,1/n)$ and is small outside that interval. One way of defining a function that reaches 1 for a small value of $x$ and then quickly drops back down again is to take a function that grows rapidly to $1,\operatorname{such}\operatorname{as}g_n(x)=$ $\lambda x$, and multiply it by a function that is roughly 1 for a little while and then decays rapidly, such as e $^{-\mu x}$. The rapid decay of e $^{-\mu x}$ starts when $x$ is around $1/\mu$, which suggests that we should take $\mu$ to be around $n.$ Since we want $g_n(x)$ to reach 1 in the interval $(0,1/n)$, we should probably take $\lambda$ to be around $n$ as well.

It is now easy to check that the functions $f_n(x)=$ $nx\mathrm{e}^{-nx}$ converge pointwise to zero but not uniformly.
口

Of course, one might well give a detailed proof that the functions $nx\mathrm{e}^{-nx}$ do the job.

As with the other choices, there are advantages and disadvantages that need to be weighed up when decid- ing how much to explain the origin (or at least a possi- ble origin) of the ideas one presents. If one’s main con- cern is verification of a result—that is, convincing the reader of its truth—then it may not matter too much where the ideas come from as long as they work. But if the aim is to teach the reader how to solve problems of a certain kind, then presenting solutions that appear out of nowhere as if by magic is not helpful. What is more, demonstrating where the ideas come from gives the reader a much clearer idea of which features are essential and which merely incidental. For example, in the argument above it is clear from the second presentation that there is nothing special about the functions $f_n(x)=nx\mathrm{e}^{-nx}$ : for $f_n(x)$ one could take any nonnegative function such that $f_n(0)=0,f_n(1/n)\geqslant c$ (for some fixed constant $c) , $ and $f_n( x)$ is small for every $x\geqslant2/n.$ For instance, one could take a “witch's hat" that equals $nx$ when $0\leqslant x\leqslant1/n,2-nx$ when $1/n\leqslant x\leqslant 2/n$, and $0$ when $2/n\leqslant x\leqslant 1.$

That is not to say that a diligent reader cannot look at a presentation of the first kind and work out for him/herself where the idea might have come from. In this case, if one sketches the graph of $f_n(x)$, one sees that it grows and shrinks rapidly in a small interval near 0 and is small thereafter, and then it becomes clear why these functions are suitable. However, one needs experience to be able to do this with an argument. So the extent to which you should explain where your arguments come from depends largely on the level of experience of your intended reader—both generally and in the specific area you are writing about.

### 7 Definitions First versus Examples First

Suppose that one wanted to write an explanation of what a topological manifold is. An obvious approach would be to start by giving the definition. That could be done as follows.

**Definition**. A d-dimensional topological manifold is a topological space $X$ such that every point $x$ in $X$ has a neighborhood that is homeomorphic to a connected open subset of $\mathbb{R}^{d}$.

Having done that, one would give a few examples of topological manifolds, such as spheres and tori, to illuminate the definition.

An alternative approach is to start with a brief discus- sion of the examples. One could point out, for instance, that it is easy to come up with a satisfactory coordinate system for any small region of the world but that it is not possible to find a good coordinate system for the world in its entirety; there will always be annoying prob- lems such as the poles not having well-defined longi- tudes. A discussion of that kind will give the reader the informal concept of a space that is “locally like Rd” and after that the formal definition is motivated: it is the formal expression of an informal idea that the reader already has.

The advantage of the second approach is that an abstract definition is often much easier to understand if one has a good idea of what it is abstracting. One will read the definition with strong expectations of what it will look like, and all one will have to commit to mem- ory is the ways in which the definition does not quite fit those expectations. If the definition is presented first, then one will be expected to hold the whole thing in one’s head, rather than what one might think of as the difference between the definition and one’s prior expectation of it.

Whether or not this advantage makes it worth pre- senting examples before giving a definition depends on how difficult you expect it to be for your reader to grasp the definition. To give an example where it might not be worth giving examples first, suppose that you want to introduce the notion of a commutative ring for a reader who is already familiar with groups and fields. A natural way of doing it would be to list the axioms for a com- mutative ring and make the remark that what you have listed is very similar to the list of axioms for a field but you no longer assume that elements have multiplica- tive inverses, and sometimes you do not even assume that your rings have multiplicative identities.

Once you have said that, it will still be a very good idea to give some important examples, such as the ring $\mathbb{Z}$ of all integers, the ring $\mathbb{Z}[x]$of all polynomials with
integer coefficients, and the ring $\mathbb{Z}[\sqrt{2}]$ of all numbers of the form $a+b\sqrt{2}$ where $a$ and $b$ are integers. However, the argument for presenting these examples first
is weaker than it was for topological manifolds, for two reasons.

The first reason is that the definition is easy to grasp: rings are like fields but without multiplicative inverses. Therefore, giving the definition straight away does not place a burden on the reader’s memory. Of course, the reader will want reassurance that there are interesting examples, but that can be given immediately after the definition.

The second reason is that the necessity for this par- ticular abstraction is less obvious than it is for man- ifolds. Given examples such as spheres and tori, it is natural to think that they are all examples of the same basic “thing” and then to try to work out what that “thing” is. But the benefits of thinking of the integers and the polynomials with integer coefficients as exam- ples of the same underlying algebraic structure are not clear in advance; they become clear only after one has developed a considerable amount of theory. So it is more natural in this case to think of the abstraction as primary, at least in the first instance.
As ever, the decision about how to present a new mathematical concept involves a judgment that is sometimes quite delicate. Broadly speaking, the harder a definition is to grasp, the more helpful it will be to the reader to have some examples in mind when read- ing it. But that depends both on the reader and on the intrinsic complexity of the definition. However, one general piece of advice is still possible here, which is at least to consider the possibility of starting with exam- ples. It may not always be appropriate to do so, but many mathematical writers like to start with definitions under all circumstances, and the result is that many expositions are harder to understand than they need to be.

Let me close this section by pointing out that the examples-first device is quite a general one. Indeed, I have used it in a number of places in this article; see the openings of sections 4 and 6 and of this very section.

### 8 Traditional Methods of Dissemination versus New Methods

A person who wishes to produce mathematical writing today faces a choice that did not exist twenty years ago. Until recently, almost all mathematical writing took the form of books or journal articles. But now the Internet has given us new methods of dissemination, which have already had an impact and are likely to have a much bigger impact in the future.

In particular, the existence of the Internet affects every single one of the considerations discussed in this article. Let me take them in turn.

#### 8.1 Level of Formality

The main task of each generation of mathematicians is to add to the body of mathematical knowledge. How- ever, there is a second task that is almost as important as the first, and not entirely separate from it, which is to digest this new knowledge and present it in a form that subsequent generations will find as easy as pos- sible to grasp. This process of digestion can of course happen many times to the same piece of mathematics.

Sometimes, digesting a piece of mathematics is itself a significant advance in mathematical knowledge. For example, a theory may be developed that yields quite easily a number of already existing and seemingly dis- parate results. The traditional publication system is well suited to this situation; one can just write an arti- cle about the theory and get it published in the normal way.

Sometimes, however, digesting a piece of mathemat- ics does not constitute a mathematical advance. It can be something more minor, such as thinking of a way of looking at an argument that makes it clearer where the ideas have come from or drawing an informal anal- ogy between one piece of mathematics and another that is simpler or better known. Insights of this kind can be hard earned and extremely valuable to other mathematicians, but they do not lead to publishable papers.

With the Internet, there are many ways that more informal mathematical thoughts can be shared. An obvious one is to write a conventional mathematical text and make it available on one’s home page. Another option, which an increasing number of mathematicians have adopted, is to have a blog. The advantage of this is that one obtains feedback from one’s readers, and experience has shown that the quality of much of this feedback is very high.

There are other forms of mathematical literature that would not be conventionally publishable but that could be extremely valuable. For example, an article about a serious but failed attempt to solve a problem would not be accepted by a journal, and the result is a great deal of duplication of work; if the problem is important and the attempt looks plausible to begin with, then many peo- ple will try it. A database of failed proof attempts would be very useful, and in principle the Internet makes it easy to set up, though so far nobody has done so.

In general, the Internet allows us much greater free- dom in choosing the level of formality at which we wish to write and allows us to publish documents that do not fit the mould of a standard journal article.

#### 8.2 Level of Detail

Suppose that you use a mathematical result or defini- tion that will be familiar to some readers but not to oth- ers. In a print document you have to decide whether to explain it and, if so, how elaborate an explanation to give.
In a hyperlinked document on the web, one is no longer forced to make this choice. One can write a version for experts, but with certain key words and phrases underlined, so that readers who need these words and phrases explained further can click on them and read explanations. This kind of writing has become very common on Wikipedia and other wikis.

It also introduces a new balance that needs to be struck. Sometimes wiki articles are hard to read because the writers use the existence of links to other wiki pages as a license not to explain terms that they might otherwise have explained. The result is that unless one is familiar with most of the definitions in the original article, one can get lost in a complicated graph of linked wiki pages as one finds that the page that explains an unfamiliar concept itself requires one to click through to several other pages. So if you are going to exploit hyperlinks, you need to think carefully about what the experience of following those links will be like for your intended readers.
Another inconvenience of hyperlinks is that they require you to visit an entirely new page, which makes it easy to forget where you were before (especially if you backtrack and then follow some other sequence of links). However, there is plenty of software that gets round this problem. For example, on some sites one can incorporate “sliders,” pieces of text that insert them- selves into what you are reading when you click on an appropriate box and disappear when you click on it again. So if, for example, one wrote, “by the second isomorphism theorem,” one could have a box with the words “What does that say?” on it, so that readers who needed it could click on the box and have a short para- graph about the second isomorphism theorem inserted into the text. One can have sliders within sliders, so perhaps within that slider one could have the option of bringing up a proof of the theorem as well.

The main point is that the Internet has made it pos- sible to write new kinds of documents where one is no longer forced to make choices such as of how much detail to give. One can leave that decision to the reader. Such documents have a huge potential to improve the way mathematics is presented, and this potential will only increase as technology improves.

#### 8.3 Letters versus Words

I will not say much about this, since most of what I have to say is very similar to what I have already said about the level of detail in which a document is written. With the kinds of electronic documents that are now possi- ble, one can save the reader the trouble of searching through a paper to find out what a letter stands for by incorporating a reminder that appears when you click on the letter. Perhaps better still, it could appear in a little box when you hover over the letter. One could also have condensed statements involving lots of let- ters with the option of converting them into equivalent wordier statements. Again, the point is that there are many more options now.

#### 8.4 Modularity

The kinds of electronic documents I have been dis- cussing make possible a form of top-down mathemat- ical writing that would be far less convenient in a print document. One could write a high-level account of some piece of mathematics, giving the reader the option of expanding any part of that high-level account into a lower-level account that justifies it in more detail. And there could be many levels of this, so that if you clicked on everything you would end up with a presentation of the entire argument in full gory detail.

A less ambitious possibility is one that solves the problem discussed earlier about where to place a lemma. The difficulty was that in a print document you will either put it before the proof where it is used, in which case it is not adequately motivated, or during the proof, in which case it looks ugly, or after the proof, in which case the proof itself leaves you with awkward promises to fill in gaps later. But with an electronic doc- ument, putting a lemma exactly where it is needed is no longer ugly. During the proof, one can say, “We are now going to make use of the following statement,” and give the reader a button to click on that will bring up a proof of that statement.

#### 8.5 Order of Presentation

If you do not want to decide whether to give an abstract definition first or start with motivating examples, then you can give the reader the choice. Just start with a page of headings and invite the reader to decide whether to click on “Motivating examples” first or “The formal definition” first.

To some extent, the same goes for the decision about whether to present arguments in their logical order or in a way that brings out how they were discovered. If at some point the logical order requires you to draw a rabbit out of a hat, you could at the very least introduce a slider that explains where that rabbit actually came from.
