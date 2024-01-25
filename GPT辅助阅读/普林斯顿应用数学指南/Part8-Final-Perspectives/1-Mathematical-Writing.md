## VIII.1 Mathematical Writing
Timothy Gowers

### 1 Introduction

The purpose of this article is not to offer advice about how to write mathematics well. Such advice can be found in many places. However, I do have three pieces of very general advice, which inform the rest of the arti- cle. The first is to be clear about your intended read- ership; for example, if you want what you write to be understood by an undergraduate, then do not assume knowledge of any terminology that is not standardly taught in undergraduate mathematics courses. The sec- ond is to aim for this readership to be as wide as pos- sible. If, with a small amount of extra explanation, you can make what you write comprehensible to an expert in another field of mathematics, then put in that extra effort. Whatever you do, do not worry that experts will not need the explanation; if that is true (which it often is not), then they can easily skip it. The third, which is related to the second, is to set the scene before you start. Some people who read what you have written will do so because they want to understand all the techni- cal details and use them in their own work, but the vast majority will not. Most readers, including people who need to make quick judgments that will profoundly affect your career, will want to read the introduction quickly to see what you have done and assess how important it is. However much you might wish every- one to read what you have written in complete detail, you should be realistic and cater for readers who just want to skim it.

For the rest of this article I shall discuss various choices that one must make when writing a mathemat- ical document. I will not advocate choosing one way rather than another, since the choices you should make depend on what you want to achieve; my final piece of general advice is merely that you should make the choices consciously rather than by accident.

### 2 Formality versus Informality

There are (at least) two goals that one might have when writing a mathematical document. One is to establish a mathematical result by whatever means are appropri- ate to the field; in pure mathematics the usual require- ment is unambiguous definitions and rigorous proofs, whereas in applied mathematics other forms of evi- dence, such as heuristic arguments and experimental backing, may be acceptable. The other is to convey mathematical ideas to the reader.

These two goals are often in tension. If a pure math- ematician discovers a complicated proof of a theorem, then that proof will be hard to understand. However, sometimes the apparent complication of a proof is mis- leading; what is really going on is that the author had one or two key ideas, and the complication of the argu- ment is the natural working out of the details of those ideas. For the expert reader, an informal explanation of the ideas that drive the proof may well be more valuable than the proof itself.

Nobody would advocate writing papers with just informal explanations of ideas, since plausible-looking ideas often turn out not to work. However, there is still a choice to make, since it is considered acceptable to display proofs and not explain the underlying ideas. There may sometimes be circumstances where this is appropriate; for example, perhaps the proof is short, and explaining the ideas that generate it will double the length of what you are writing and put off readers. But usually, the advice I gave earlier—to broaden your readership if it not too difficult to do so—would dic- tate that technical arguments should be accompanied by informal explanations.

### 3 Giving Full Detail versus Leaving Details to the Reader

When you are writing you need to decide how much detail to give. If you give too little, then the reader you are aiming at will not be able to understand what you have written. But you also want to avoid making too many points that the reader will find completely obvious.

Of these two potential problems, the first is undoubt- edly more serious. It is much easier for readers to skip details that they find too obvious to be worth saying than it is for them to fill in details that they do not find obvious at all.

The question of how much detail to give is related to the question of how formal to be, but it is not the same question. It is true that there is a tendency in informal mathematical writing to leave out details, but with even the most formal writing a decision has to be made about how much detail to give; it is just that in formal writing one probably wants to signal more care- fully when details have been left out. This can be done in various ways. One can use expressions such as “It is an easy exercise to check that...,” or “The second case is similar,” which basically say to the reader, “I have decided not to spell out this part of the argument.” One can also give small hints, such as “By compact- ness,” or “An obvious inductive argument now shows that...,” or “Interchanging the order of summation and simplifying, we obtain....”

If you do decide to leave out detail, it is a good idea to signal to the reader how difficult it would be to put that detail in. A mistake that some writers make is to give references to other papers for arguments that can eas- ily be worked out by the reader, without saying that the particular result that is needed is easy. This is straight- forwardly misleading; it suggests that the best thing to do is to go and look up the other paper when in fact the best thing to do is to work out the argument for oneself.

### 4 Letters versus Words

The following is problem 10 of book 1 of an English translation of Diophantus’s Arithmetica.
Given two numbers, to add to the lesser and to subtract from the greater the same (required) number so as to make the sum in the first case have to the difference in the second case a given ratio.

A modern writer would express the same problem more like this.

$$
\begin{aligned}&\text{Given two numbers }a\mathrm{~and~}b\text{ and a ratio }\rho\text{, find }x\mathrm{~such}\\&\mathrm{that~}a+x=\rho(b-x).\end{aligned}
$$

The main difference between these two ways of describ- ing the problem is that in the second formulation the numbers under discussion have been given names. These names take the form of letters, which allow us to replace wordy expressions such as “the second number” or “the given ratio” by letters such as $b$ and $\rho$.”

The advantage of modern notation is that it is much more concise. This is not just a matter of saving paper; the extra length of “to make the sum in the first case have to the difference in the second case a given ratio” over “such that $a+x=\rho(b-x)$” makes it significantly harder to understand because it is difficult to take in the entire phrase at once.

However, the concision that comes from naming mathematical objects comes at a cost: one has to learn the names. In the example above, that is very easy and the cost is negligible. However, sometimes it is far from negligible. The following proposition comes from a paper in Banach space theory.

**Proposition.** Let $0\leqslant\alpha\leqslant\frac12$ and $1/p=\frac12-\alpha.$ Then
$$
\mathfrak{P}_2(E,F)\subset\mathfrak{L}_{p,\infty}^{(a)}(E,F)
$$
for all Banach spaces $F$ if and only if $E\subset \Gamma_{\alpha}.$

Just before the proposition, the reader has been told that $\mathfrak{p}_{2}$ is the ideal of 2-summing operators from $E$ to $F$, which is a standard definition in the area. As for $\mathcal{L}_{p,\infty}^{(a)}(E,F)$, this has been defined early in the paper as follows. (It is not necessary to understand these definitions to understand the point I am making.)

Given an operator $T$, the $approximation~ number$  $a_n(T)$ is defined to be $\inf \{ \|T- L\|:$ rank$( L) < n\} .$ Then 
$\mathfrak{L}_{s,w}^{(a)}(E,F)$ is the set of operators $T$ such that the sequence $(a_n(T))_{n=1}^\infty$ belongs to the Marcinkiewicz space $\ell_{s,w}.$

The definition of the Marcinkiewicz space is again standard in the area. Finally, the set $\Gamma_{\alpha}$ is defined to be the set of all Banach spaces of weak Hilbert type $\alpha$. That is not a standard definition, but it is given earlier on in the paper.

Thus, another way of stating the proposition is as follows.

**Proposition**. Let $0\leqslant\alpha\leqslant\frac12$,let $1/p= \frac 12- \alpha, $and let $E$ be a Banach space. Then the following two statements are equivalent.
- (1) For every Banach space $F$ and every 2-summing
operator  $T{:}E~\to~F$ , the sequence $(a_n(T))_{n=1}^{\infty}$  of approximation numbers belongs to the Marcinkiewicz space $\ell_{p,\infty}.$
- (2) $E$ is a space of weak Hilbert type $\alpha.$

This time, it is the wordier definition that places a smaller burden on the reader’s memory. If you know what 2-summing operators, approximation numbers, the Marcinkiewicz space, and weak Hilbert type are, most of which are standard definitions in the area, then you can understand without much effort what the proposition is claiming. With the first formulation, there is an extra step you have to perform to unpack the notation into those standard definitions. Another advantage of the second formulation is that a suffi- ciently expert reader who is skimming the paper will be able to understand it without having to look back in the paper to find out what everything means. The first formulation does not leave that option open.

Thus, in more complicated mathematical writing, there is another source of tension. If you use too lit- tle notation, your sentences will become hopelessly clumsy and repetitive, but if you use too much, you are placing excessive demands on the memory of your readers.

This may be a delicate balance to strike, but there is one principle that applies universally: if you do decide to use some nonstandard notation, then make sure that the reader can easily find where it is defined. This can be done by means of a section devoted to preliminary definitions, though it will often be kinder to give defi- nitions just before they are used. If that is not possible, one can give reminders of definitions, or at the very least pointers to where they can be found.



### 5 Single Long Arguments versus Arguments Broken Up into Modules

If you are trying to justify a mathematical statement and the justification is long and complicated, then what you write may well be hard to understand unless you can somehow break the argument up into smaller “modules” that fit together to give you what you want. In pure mathematics, these modules usually take the form of lemmas. If you are proving a theorem and you do not want the proof to become unwieldy, then you try to identify parts of the argument that can be extracted and proved separately. One can then simply quote these results in the main argument. Lemmas play a role in proofs that is similar to the role of subroutines in computer programs.

For breaking up an argument to be a good idea, it greatly helps if the part of the argument you want to extract is not too context dependent. If the statement of a lemma requires a long piece of scene setting, then it is probably better to leave it in the main body of the argu- ment, where the scene has already been set. However, if it can be stated without reference to the particular con- text, which usually means that it is more general than the particular application needed of it in the main argu- ment, then it is more appropriate to extract it. Again, this is a matter of judgment.

A disadvantage of more modular arguments is that extracting lemmas, or more general modules, forces you to put them somewhere where they do not arise naturally. If you put them before the main argument, so that they will be available when needed, then the reader is presented with statements of no obvious use and is expected to remember them. If they are particu- larly memorable, then that is not a problem, but often they are not; for instance, they may depend on two or three slightly odd conditions that just happen to be satisfied in the later argument. If you put them after the main argument, then the reader keeps being told, “We will prove this claim later” and reaches the end of the argument with the uneasy feeling that the proof is incomplete. A third possibility is to state and prove lemmas within an argument, but nested statements of this kind can be fairly ugly.

With some complicated arguments, there may be no truly satisfactory solution to these problems. In that case, the best thing to do may well be to choose an unsatisfactory solution and mitigate the problems somehow. The default option is probably to state lem- mas before they are used. If you choose that option and the lemmas are somewhat complicated and hard to remember, then you can always add a few words of explanation about the role that the lemma will play. If even that is hard to do, then another option is to advise the reader to read the main argument first and return to the lemma only when the need for it has become clear. (An experienced reader may well do that anyway, but it is still helpful to be told by the author that it is a good approach to understanding the argument.)

6 Logical Order versus Order of Discovery
Suppose you wish to present the fact that a sequence of continuous functions that converges pointwise does not have to converge uniformly. Here is one way that you might do it.

**Theorem**. There exists a sequence of continuous functions $f_n:[0,1]\to[0,1]$ that converges pointwise but not uniformly.

**Proof**. For each positive integer $n$ and each $x\in[0,1]$, let $f_n(x)=nx\mathrm{e}^{-nx}$. Then, for $x>0$ we have e$^{-x}<1$, so $n\mathrm{e} ^{- nx}= n( \mathrm{e} ^{- x}) ^n\to 0$ as $n\to \infty.$ It follows that $f_n( x) \to 0$ as $n\to \infty$.Also, when $x= 0$ we have $f_n( x) =  0$ for every $n$ so again $f_n( x) \to 0$ as $n\to \infty.$ Therefore, $f_n(x)\to0$ pointwise.

However, the convergence is not uniform. To see this, observe that $f_n(n^{-1})=\mathrm{e}^{-1}$ for every $n$. Thus, for every $n$ there exists $x$ such that $|f_n(x)-0|\geqslant\mathrm{e}^{-1}.$   口

This proof has a feature that is common in mathe- matics: it is easier to follow the steps than it is to see where the steps came from. If you are told to try the functions $f_n(x)=nx\mathrm{e}^{-nx}$, then checking that they satisfy the conditions is a straightforward exercise, but what made anybody think of that particular sequence of functions?

Here is what we might write if we wanted to make the answer to that last question clearer.


**Proof**. If $f_n\to f$ pointwise but not uniformly, then $f_n-f\to0$ pointwise but not uniformly, so we may as well look for functions that converge to zero. In order to ensure that they do not converge uniformly to zero, we need a positive number $\theta$ such that for infinitely many $n$ there exists $x\in[0,1]$ with $|f_n(x)|\geqslant\theta.$ Since infinitely many of these $f_n(x)$ will have the same sign, and since we can multiply all functions by $\theta^{-1}$, we may as well look for a sequence of functions $f_n$ that converges pointwise to 0 such that for every $n$ there exists $x_n$ with $f_n(x_n)\geqslant1.$



