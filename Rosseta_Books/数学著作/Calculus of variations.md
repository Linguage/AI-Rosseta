# CALCULUS OF VARIATIONS  

I.M.Gelfand and S.V.Fomin  

Translated and Edited by Richard ASilverman  

# CALCULUS OF VARIATIONS  

I. M. GELFAND S. V. FOMIN Moscow State University  

Revised English Edition Translated and Edited by Richard A. Silverman  

# SELECTED RUSSIAN PUBLICATIONS IN THE MATHEMATICAL SCIENCES Richard A. Silverman, Editor  

$\circledcirc$ 1963 by PRENTICE-HALL, INC. Englewood Cliffs, N. J.  

All rights reserved. No part of this book may be reproduced in any form, by mimeograph or any other means, without permission in writing from the publisher.  

Current printing (last digit ) : 20 19 18 17 16 15  

PRENTICE-HALL INTERNATIONAL, INC., LONDON PRENTICE-HALL OF AUSTRALIA, PTY., LID., SYDNEY PRENTICE-HALL OF CANADA, LID., TORONTO PRENTICE-HALL OF INDIA (PRIVATE) LID., NEW DELHI PRENTICE-HALL OF JAPAN. INC.. TOKYO  

# Library of Congress Catalog Card Number 63-18806  

Printed in the United States of America  

C 11229  

The pres ent course is bas ed on l ectures given by I. M. Gelfand in the Mechanics and Mathematics Department of Moscow State University. However, the book goes considerably beyond the material actually presented in the l ectures. Our aim is to give a treatment of the ele­ ments of the calculus of variations in a form which is both easily understandable and sufficiently modem. Considerable attention is devoted to physical applica­ tions of variational methods, e. g. , canonical equations, variational principles of mechanics and conservation laws.  

The reader who merely wishes to become familiar with the most basic concepts and methods of the calculus of variations n eed only study the first chapter. The first three chapters, taken together, form a more compre­ hensive course on the elements of the calculus of varia­ tions,-but one which is still quite elementary (involving only n ecessary conditions for extrema) . The first six chapters contain, more or l ess, the material given in the usual university course in the calculus of variations (with applications to the mechanics of systems with a finite number of degrees of freedom ) ,  including the theory of fields (presented in a somewhat novel way) and sufficient conditions for weak and strong extrema. Chapter 7 is devoted to the application of variational methods to the study of systems with infinitely many degrees of freedom. Chapter 8 contains a brief treat­ ment of direct methods in the calculus of variations.  

The authors are grateful to M. A. Yevgrafov and A. G. Kostyuchenko, who read the book in manuscript and made many useful comments.  

This book is a modern int1;oduction to the calculus of variations and certain of its ramifications, and I trust that its fresh and lively point of view will serve to make it a welcome atldition to the English-language literature on the subject. The present edition is rather different from the Russian original. With the authors' consent, I have given free rein to the tendency of any mathe­ matically educated translator to assume the functions of annotator and stylist. In so doing, I have had two special assets : 1) A substantial list of revisions and corrections from Professor S . V. Fomin himself, and 2) A variety of helpful suggestions from Professor J. T. Schwartz of New York University, who read the entire translation in typescript.  

The problems appearing at the end of each of the eight chapters and two appendices were made specifically for the English edition, and many of them comment further on the corresponding parts of the text. A variety of Russian sources have played an important role in the synthesis of this material. In particular, I have consulted the textbooks on the calculus of variations by N. I. Akhiezer, by L. E. Elsgolts, and by M. A. Lavrentev and L. A. Lyusternik, as well as Volume 2 of the well­ known problem collection by N. M. Gyunter and R. o. Kuzmin, and Chapter 3 of G. E. Shilov's "Mathematical Analysis, A Special Course."  

At the end of the book I have added a Bibliography containing suggestions for collateral and supplementary reading. This list is not intended as an exhaustive cata­ log of the literature , and is in fact confined to books available in English.  

1 ELEMENTS OF THE THEORY Page 1. 1: Func­ tionals. Some Simple Variational Problems, 1. 2: Func­ tion Spaces, 4. 3: The Variation of a Functional. A Necessary Condition for an Extremum, 8. 4: The Sim­ plest Variational Problem. Euler's Equation, 14. 5: The Case of Several Variables, 22. 6: A Simple Variable End Point Problem, 25. 7: The Variational Derivative, 27. 8 :  Invariance of Euler's Equation, 29. Problems, 31.  

2 FURTHER GENERALIZATIONS Page 34. 9: The Fixed End Point Problem for $\pmb{n}$ Unknown Functions, 34. 10. Variational Problems in Parametric Form, 38. 11: Functionals Depending on Higher-Order Derivatives, 40. 12: Variational Problems with Subsidiary Conditions, 42. Problems, 50.  

3 THE GENERAL VARIATION OF A FUNCTIONAL Page 54. 13: Derivation of the Basic Formula, 54. 14: End Points Lying on Two Given Curves or Surfaces, 59. 15: Broken Extremals. The Weierstrass-Erdmann Condi­ tions, 61. Problems, 63.  

4 THE CANONICAL FORM OF THE EULER EQUA­ TIONS AND RELATED TOPICS Page 67. 16: The Canonical Form of the Euler Equations, 67. 17: First Integrals of the Euler Equations, 70. 18: The Legendre Transformation, 71. 19: Canonical Transformations, 77. 20: Noether's Theorem, 79. 21: The Principle of Least Action, 83. 22: Conservation Laws, 85. 23: The Ham­ ilton-Jacobi Equation. Jacobi's Theorem, 8 8 . Problems, 94.  

vi CONTENTS  

5 THE SECOND VARIATION. SUFFICIENT CONDI­ TIONS FOR A WEAK EXTREMUM Page 97. 24: Quadratic Functionals. The Second Variation of a Func­ tional, 97. 25: The Formula for the Second Variation. Legendre's Condition, 101. 26: Analysis of the Quadratic Functional $\int_{a}^{b}\left(P h^{\prime2}+Q h^{2}\right)d x.$ , 105. 27: Jacobi's Necessary Condition. More on Conjugate Points, 111. 28: Sufficient Conditions for a Weak Extremum, 115. 29: Generalization to $\pmb{n}$ Unknown Functions, 117. 30: Connection Between Jacobi's Condition and the Theory of Quadratic Forms, 125. Problems, 129.  

6 FIELDS. SUFFICIENT CONDITIONS FOR A STRONG EXTREMUM Page 131. 31: Consistent Boundary Con­ ditions. General Definition of a Field, 131. 32: The Field of a Functional, 137. 33: Hilbert's Invariant In­ tegral, 145. 34: The Weierstrass $E$ -Function. Sufficient Conditions for a Strong Extremum, 146. Problems, 150.  

7 VARIATIONAL PROBLEMS INVOLVING MULTIPLE INTEGRALS Page 152. 35: Variation of a Functional Defined on a Fixed Region, 152. 36: Variational Deriva­ tion of the Equations of Motion of Continuous Me­ chanical Systems, 154. 37: Variation of a Functional Defined on a Variable Region, 168. 38: Applications to Field Theory, 180. Problems, 190.  

8 DIRECT METHODS IN THE CALCULUS OF V ARIA­ TIONS Page 192. 39: Minimizing Sequences, 193. 40: The Ritz Method and the Method of Finite Differ­ ences, 195. 41: The Sturm-Liouville Problem, 198. Problems, 206.  

# APPENDIX I PROPAGATION OF DISTURBANCES AND THE CA­ NONICAL EQUATIONS Page 208.  

# APPENDIX II VARIATIONAL METHODS IN PROBLEMS OF OP­ TIMAL CONTROL Page 218.  

BIBLIOGRAPHY Page 227.  

INDEX Page 228.  

#  

# I. Fu nctionals. Some Si m ple Variational Pro b l e m s  

Variable quantities called functionals play an important role i n many problems arising in analysis, mechanics, geometry, etc. By a functional, we mean a correspondence which assigns a definite (real) number to each function (or curve) belonging to some class. Thus, one might say that a functional is a kind of function, where the independent variable is itself a function (or curve). The following are examples of functionals:  

1 .  Consider the set of all rectifiable plane curves. 1 A definite number is associated with each such curve, namely, its length. Thus, the length of a curve is a functional defined on the set of rectifiable curves.   
2. Suppose that each rectifiable plane curve is regarded as being made out of some homogeneous material. Then if we associate with each such curve the ordinate of its center of mass, we again obtain a functional.   
3. Consider all possible paths joining two given points $A$ and $\pmb{B}$ i n the plane. Suppose that a particle can move along any of these paths, and let the particle have a definite velocity $v(x,y)$ at the point $(x,y)$ . Then we obtain a functional by associating with each path the time the particle takes to traverse the path.  

4. Let $y(x)$ be an arbitrary continuously differentiable function, defined on the interval $[a,b]$ .2 Then the formula  

$$
J[y]=\int_{a}^{b}y^{\prime2}(x)d x
$$  

defines a functional on the set of all such functions $y(x)$ .  

5. As a more general example, let $F(x,y,z)$ be a continuous function of three variables. Then the expression  

$$
J[y]=\int_{a}^{b}F[x,y(x),y^{\prime}(x)]d x,
$$  

where $y(x)$ ranges over the set of all continuously differentiable functions defined on the interval $[a,b]$ , defines a functional. By choosing different functions $F(x,y,z)$ , we obtain different functionals. For exam ple, if  

$$
F(x,y,z)={\sqrt{1+z^{2}}},
$$  

$J[y]$ is the length of the curve $y=y(x),$ , as in th e first example, while if  

$$
F(x,y,z)=z^{2},
$$  

$J[y]$ reduces to the case considered in the fourth example. In what follows, we shall be concerned mainly with functionals of the form (1).  

Particular instances of problems involving the concept of a functional were considered more than three hundred years ago, and in fact, the first important results in this area are due to Euler ( 1 707 -1 783). Nevertheless, up to now, the " calculus of functionals" still does not have methods of a generality comparable to the methods of classical analysis (Le. , the ordinary " calculus of functions"). The most developed branch of the " calculus of functionals" s concerned with finding the maxima and minima offunctionals, and is called the " calculus of variations." Actually, it would be more a ppropriate to call this subject th e " calculus of variations in the narrow sense, " since the significance of the concept of th e variation of a functional is by no means confined to its applications to the problem of determining the extrema of functionals.  

We now indicate some typical examples of variational problems, by which we mean problems involving the determination of maxima and minima of functionals.  

1 .  Find the shortest plane curve joining two points $A$ and B, i.e. , find the curve $y=y(x)$ for which the functional  

$$
\int_{a}^{b}{\sqrt{1+y^{\prime}{}^{2}}}d x
$$  

achieves its minimum. The curve in question turns out to be the straight line segment j oining $A$ and $\pmb{B}$ .  

2. Let $A$ and $\pmb{B}$ be two fixed points. Then the time it takes a particle to slide under the influence of gravity along some path j oining $A$ and $\pmb{B}$ depends on the choice of the path (curve), and hence is a functional. The curve such that the particle takes the least time to go from $A$ to $\pmb{B}$ is called the brachistochrone. The brachistochrone problem was posed by John Bernoulli in 1 696, and played an important part in the develop­ ment of the calculus of variations. The problem was solved by J ohn Bernoulli, James Bernoulli, Newton, and L'Hospital. The brachisto­ chrone turns out to be a cycloid, lying in the vertical plane and passing through $A$ and $\pmb{B}$ (cf. p. 26).  

3. The following variational problem, called the isoperimetric problem, was solved by Euler : Among all closed curves of a given length I, find the curve enclosing the greatest area. The required curve turns out to be a circle.  

All of the above problems involve functionals which can be written in the form  

$$
\int_{a}^{b}F(x,y,y^{\prime})d x.
$$  

Such functionals have a " localization property " consisting of the fact that if we divide the curve $y=y(x)$ into parts and calculate the value of the functional for each part, the sum of the values of the functional for the separate parts equals the value of the functional for the whole curve. It is just these functionals which are usually considered in the calculus of variations. As an example of a " nonlocal functional," consider the expression  

$$
{\frac{\displaystyle\int_{a}^{b}x{\sqrt{1+y^{'2}}}d x}{\displaystyle\int_{a}^{b}{\sqrt{1+y^{'2}}}d x}},
$$  

which gives the abscissa of the center of mass of a curve $y=y(x),a\leqslant x\leqslant b.$ , made out of some homogeneous material.  

An important factor in the development of the calculus of variations was the investigation of a number of mechanical and physical problems, e.g., the brachistochrone problem mentioned above. In turn, the methods of the calculus of variations are widely applied in various physical problems. It should be emphasized that the application of the calculus of variations to physics does not consist merely in the solution of individual, albeit very important problems. The so-called " variational principles," to be discussed in Chapters 4 and 7, are essentially a manifestation of very general physical laws, which are valid in diverse branches of physics, ranging from classical mechanics to the theory of elementary particles.  

To understand the basic meaning of the problems and methods of the calculus of variations, it is very important to see how they are related to problems of classical analysis, i.e., to the study of functions of $\pmb{n}$ variables. Thus, consider a functional of the form  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x,y(a)=A,y(b)=B.
$$  

Here, each curve is assigned a certain number. To find a related function of the sort considered in classical analysis, we may proceed as follows. Using the points  

$$
a=x_{0},\quad x_{1},\ldots,\quad x_{n},\quad x_{n+1}=b,
$$  

we divide the interval $[a,b]$ into $n+1$ equal parts. Then we replace the curve $y=y(x)$ by the polygonal line with vertices  

$$
(x_{0},A),\quad(x_{1},y(x_{1})),\ldots,\quad(x_{n},y(x_{n})),\quad(x_{n+1},B),
$$  

and we approximate the functional $J[y]$ by the sum  

$$
J(y_{1},...,y_{n})=\sum_{i=1}^{n+1}F\left(x_{i},y_{i},{\frac{y_{i}-y_{i-1}}{h}}\right)h,
$$  

where  

$$
y_{i}=y(x_{i}),\quad\quad h=x_{i}-x_{i-1}.
$$  

Each polygonal line is uniquely determined by the ordinates $y_{1},...,y_{n}$ of its vertices (recall that $y_{0}=A$ and $y_{n+1}=B$ are fixed), and the sum (2) is therefore a function of the $\pmb{n}$ variables $y_{1},...,y_{n}$ . Thus, as an approxi­ mation, we can regard the variational problem as the problem of finding the extrema of the function $J(y_{1},...,y_{n})$ . In solving variati onal problems, Euler made extensive use of this method offinite difefrences. By replacing smooth curves by polygonal lines, he reduced the problem of finding extrema of a functional to the problem of finding extrema of a function of $\pmb{n}$ variables, and then he obtained exact solutions by passing to the limit as ${\pmb n}\rightarrow\infty$ . I n this sense, functionals can b.e regarded as " functions of infinitely many variables " [i.e., the values of the function $y(x)$ at separate points], and the calculus of variations can be regarded as the corresponding analog of differential calculus.  

# 2. Fu nction S paces  

In the study of functions of $\pmb{n}$ variables, it is convenient to use geometric language, by regarding a set of $\pmb{n}$ numbers $(y_{1},...,y_{n})$ as a point in an $\pmb{n}$ -dimensional space. In just the same way, geometric language is useful when studying functionals. Thus, we shall regard each function $y(x)$ belonging to some class as a point in some space, and spaces whose elements are functi ons will be called function spaces.  

In the study of functions of a finite number $\pmb{n}$ of independent variables, it is sufficient to consider a single space, i . e . , $\pmb{n}$ -dimensional Euclidean space $\smash{\mathcal{E}_{p}^{\prime}}$ ' 3 H owever, in the case of function spaces, there is n o such " universal" space. In fact, the nature of the problem under consideration determines the choice of the function space. For example, if we are dealing with a functional of the form  

$$
\int_{a}^{b}F(x,y,y^{\prime})d x,
$$  

it is natural to regard the functional as defined on the set of all functions with a continuous first derivative, while in the case of a functi onal of the form  

$$
\int_{a}^{b}F(x,y,y^{\prime},y^{\prime\prime})d x,
$$  

the appropriate function space is the set of all functions with two continuous derivatives. Therefore, in studying functi onals of various types, it is reasonable to use various function spaces.  

The concept of continuity plays an important role for functionals, just as it d oes for the ordinary functions considered in classical analysis. In order to formulate this concept for functionals, we must somehow introduce a concept of " closeness" for elements in a functi on space. This is most conveniently done by introducing the concept of the norm of a functi on, analogous to the concept of the distance between a point in Euclidean space and the origin of coordinates. Although in what follows we shall always be concerned with function spaces, it will be most convenient to introduce the concept of a norm in a m ore general and abstract form, by introducing the concept of a normed linear space.  

By a linear space, we mean a set $\mathcal{R}$ of elements $x,y,z,\ldots$ of any kind, for which the operations of ad dition and m ultiplication by (real) numbers $\alpha,\beta,\ldots$ are defined and obey the following axioms:  

1 . $x+y=y+x$ ;   
2. $(x+y)+z=x+(y+z)$ ;   
3. There exists an element 0 (the zero element) such that $x+0=x$ for   
any $\boldsymbol{x}\in\mathcal{R}$ ; 4   
4. For each $\boldsymbol{x}\in\mathcal{R}$ , there exists an element $-x$ such that $x+(-x)=0$ ;   
5. $\mathbf{l}\cdot x=x$ ;   
6. $\alpha(\beta x)=(\alpha\beta)x$ ;   
7. $(\alpha+\beta)x=\alpha x+\beta x;$ ：   
8 . $\alpha(x+y)=\alpha x+\alpha y$ .  

A linear space $\mathscr{R}$ is said to be normed, if each element $\boldsymbol{x}\in\mathcal{R}$ is assigned a nonnegative number $\left\|x\right\|$ , alled the norm of $x_{i}$ , uch that  

1. $\left\|{\boldsymbol{x}}\right\|=0$ if and only if $x=0$ ;   
2 . $\|\alpha x\|=|\alpha|\|x\|$ ;   
3. $\left\|x+y\right\|\leqslant\left\|x\right\|+\left\|y\right\|$ ·  

In a normed linear space, we can talk about distances between elements, by defining the distance between $x$ nd $y$ o be the quantity $\|x-y\|$ .  

The elements of a normed linear space can be objects of any kind, e.g., numbers, vectors (directed line segments), matrices, functions, etc. The following normed linear spaces are important for our subsequent purposes : l. The space $\mathscr{C}$ e, or more precisely $\mathcal{C}(\boldsymbol{a},\boldsymbol{b}).$ , consisting of all continuous functions $y(x)$ defined on a (closed) interval $[a,b]$ . By addition of elements of $\mathscr{C}$ e and multiplication of elements of $\mathscr{C}$ e by numbers, we mean ordinary addition of functions and multiplication of functions by  

![](https://cdn-mineru.openxlab.org.cn/extract/c29daec4-3bde-4c07-a565-58de41e65c3b/67fa528682d979885f8e06d9f7c7b9411446c4c41dc93d2eab1b228a75078206.jpg)  
FIGURE 1  

numbers, while the norm is defined as the maximum of the absolute value, i . e . ,  

$$
\|y\|_{0}=\operatorname*{max}_{a\leqslant z\leqslant b}|y(x)|.
$$  

Thus, in the space $\mathscr{C}$ , the distance between the function $y^{*}(x)$ and the function $y(x)$ does not exceed e: if the graph of the function $y^{*}(x)$ ies inside a strip of width 2e: (in the vertical direction) " bordering" the graph of the function $y(x)$ , s shown in Figure 1.  

2. The space $\mathcal{D}_{1}$ > or more precisely $\mathcal{D}_{1}(a,b)$ , consisting of all functions $y(x)$ defined on an interval $[a,b]$ which are continuous and have continuous first derivatives. The operations of addition and multi­ plication by numbers are the same as in $\mathscr{C}$ , but the norm is defined by the formula  

$$
\|y\|_{1}=\operatorname*{max}_{a\leqslant x\leqslant b}|y(x)|+\operatorname*{max}_{a\leqslant x\leqslant b}|y^{\prime}(x)|.
$$  

Thus, two functions in $\mathcal{D}_{1}$ are regarded as close together if both the functions themselves and their first derivatives are close together, since  

$$
\|y-z\|_{1}<\varepsilon
$$  

implies that  

$$
|y(x)-z(x)|<\varepsilon,\qquad|y^{\prime}(x)-z^{\prime}(x)|<\varepsilon
$$  

for all $a\leqslant x\leqslant b$ .  

3. The space ${\mathcal{D}}_{n}$ , or more precisely ${\mathcal{D}}_{n}(a,b)$ , consisting of all functions $y(x)$ defined on an interval $[a,b]$ which are continuous and have continuous derivatives up to order $\pmb{n}$ inclusive, where $\pmb{n}$ is a fixed integer. Addition of elements of ${\mathcal{D}}_{n}$ and multiplication of elements of ${\mathcal{D}}_{n}$ by numbers are defined just as in the preceding cases, but the norm is now defined by the formula  

$$
\|y\|_{n}=\sum_{i=0}^{n}\operatorname*{max}_{a\leqslant x\leqslant b}|y^{(i)}(x)|,
$$  

where $y^{t}(x)=(d/d x)^{i}y(x)$ and $y^{\scriptscriptstyle(0)}(x)$ denotes the function $y(x)$ itself. Thus, two functions in ${\mathcal{D}}_{n}$ are regarded as close together if the values of the functions themselves and of all their derivatives up to order $\pmb{n}$ inclusive are close together. It is easily verified that all the axioms of a normed linear space are actually satisfied for each of the spaces $\mathcal{C},\mathcal{D}_{1}$ > and $\mathcal{D}_{n}$ .  

Similarly, we can introduce spaces of functions of several variables, e.g., the space of continuous functions of $\pmb{n}$ variables, the space of functions of $\pmb{n}$ variables with continuous first derivatives, etc. After a norm has been introduced in the linear space $\mathcal{R}$ (which may be a function space), it is natural to talk about continuity of functionals defined on $\mathscr{R}$ (JI:  

DEFINITION. The functional $J[y]$ is said to be continuous at the point $\hat{y}\in\mathcal{R}$ iffor any $\mathfrak{s}>0$ , there is a $\delta>0$ such that  

$$
|J[y]-J[\hat{y}]|<\varepsilon,
$$  

provided that $\|y-\hat{y}\|<\delta$ .  

Remark $\boldsymbol{{\mathit{1}}}$ . The inequality (3) is equivalent to t he two inequalities  

$$
J[y]-J[{\hat{y}}]>-\varepsilon
$$  

and  

$$
J[y]-J[{\hat{y}}]<\varepsilon.
$$  

If n the definition of continuity, we replace (3) by (4), $J[y]$ is said to be lower semicontinuous at $\hat{y}$ , while if we replace (3) by (5), $J[y]$ is said to be upper semicontinuous at $\hat{y}$ . These concepts will be needed in Chapter 8.  

Remark 2 . A t first, it might appear that the space $\mathscr{C}$ , which is the largest of those enumerated, would be adequate for the study of variational problems. However, this is not the case. In fact, as already mentioned, one of the basic types of functionals considered in the calculus of variations has the form  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x.
$$  

It is easy to see that such a functional (e.g., arc length) will be continuous if we interpret closeness of functions as closeness in the space $\mathcal{D}_{\mathbf{1}}$ . H owever, in general, the functional will not be continuous if we use the norm intro­ duced in the space $\mathscr{C}$ ,5 even though it is continuous in the norm of the space $\mathcal{D}_{1}$ , Since we want to be able to use ordinary analytic methods, e.g. , passage to the limit, then, given a functional, it is reasonable to choose a function space such that the functional is continuous.  

Remark 3. So far, we have talked about linear spaces and functionals defined on them . However, in many variational problems, we have to deal with functionals defined on sets of functions which do not form linear spaces. In fact, the set of functions (or curves) satisfying the constraints of a given variational problem, called the admissible functions (or admissible curves), is in general not a linear space. For example, the admissible curves for the "simplest " variational problem (see Sec. 4) are the smooth plane curves passing through two fixed points, and the sum of two such curves does not pass through the two points. Nevertheless, the concept of a normed linear space and the related concepts of the distance between functions, continuity of functionals, etc., play an important role in the calculus of variations. A similar situation is encountered in elementary analysis, where, in dealing with functions of $\pmb{n}$ variables, it is convenient to use the concept of an $\pmb{n}$ -dimensional Euclidean space $\smash{\mathcal{E}_{p}^{\prime}}$ , even though the domain of definition of a function may not be a linear subspace of $\smash{\mathcal{E}_{p}^{\prime}}$ '  

# 3. The Variation of a F u n ctional . A Necessary Cond ition fo r an Ext re m u m  

3.1. I n  this section, we introduce the concept of the variation (or difefrential) of a functional, analogous to the concept of the differential of a function of $\pmb{n}$ variables. The concept will then be used to find extrema of functionals. First, we give some preliminary facts and definitions.  

DEFINITION. Given a normed linear space $\mathcal{R}$ , let each element $\pmb{h}\in\mathcal{R}$ be assigned a number $\varphi[h]$ , i. e. , let $\varphi[h]$ be afunctional defined on $\mathcal{R}$ . Then $\varphi[h]$ is said to be $a$ (continuous) linear functional i  

l . $\varphi[\alpha h]=\alpha\varphi[h]$ for any $\pmb{h}\in\mathcal{R}$ and any real number $\alpha$ ;   
2. $\varphi[h_{1}+h_{2}]=\varphi[h_{1}]+\varphi[h_{2}]$ for any $h_{1}$ ${\bf\Phi}_{1},h_{2}\in\mathcal{R}$ Ji ;   
3. $\varphi[h]$ is continuous (for all $\pmb{h}\in\mathcal{R}$ ) .  

Example 1. If we associate with each function $\boldsymbol{h}(\boldsymbol{x})\in\mathcal{C}(\boldsymbol{a},\boldsymbol{b})$ i t s value at a fixed point $x_{0}$ in $[a,b],$ i.e., if we define the functional $\varphi[h]$ by the formula  

$$
\varphi[h]=h(x_{0}),
$$  

then $\varphi[h]$ is a linear functional on $\mathcal{C}(\boldsymbol{a},\boldsymbol{b})$ .  

Example 2. The integral  

$$
\varphi[h]=\int_{a}^{b}h(x)d x
$$  

defines a linear functional on ${\mathcal{C}}(a,b)$ .  

Example 3. The integral  

$$
\varphi[h]=\int_{a}^{b}\alpha(x)h(x)d x,
$$  

where $\alpha(x)$ is a fixed function in $\mathcal{C}(\boldsymbol{a},\boldsymbol{b})$ , defines a linear functional on $\mathcal{C}(\boldsymbol{a},\boldsymbol{b})$ .  

Example 4. More generally, the integral  

$$
\varphi[h]=\int_{a}^{b}\left[\alpha_{0}(x)h(x)+\alpha_{1}(x)h^{\prime}(x)+\cdot\cdot\cdot+\alpha_{n}(x)h^{\scriptscriptstyle(n)}(x)\right]d x,
$$  

where the $\alpha_{i}(x)$ are fixed functions in $\mathcal{C}(\boldsymbol{a},\boldsymbol{b})$ , defines a linear functional on ${\mathcal{D}}_{n}(a,b)$ .  

Suppose the linear functional (6) vanishes for all $h(x)$ belonging to some c.lass. Then what can be said about the functions $\alpha_{i}(x)?$ Some typical results in this direction are given by the following lemmas :  

LEMMA 1 .  I $\alpha(x)$ is continuous in $[a,b]$ , and i  

$$
\int_{a}^{b}\alpha(x)h(x)d x=0
$$  

for every function $\boldsymbol{h}(\boldsymbol{x})\in\mathcal{C}(\boldsymbol{a},\boldsymbol{b})$ such that $h(a)=h(b)=0;$ , then $\alpha(x)=0$ for all $x$ in $[a,b]$ .  

Proof Suppose the function $\alpha(x)$ is nonzero, say positive, at some point in $[a,b]$ . Then $\alpha(x)$ is also positive in some interval $[x_{1},x_{2}]$ contained in $[a,b]$ . If we set  

$$
h(x)=(x-x_{1})(x_{2}-x)
$$  

for $x$ in $[x_{1},x_{2}]$ and $h(x)=0$ otherwise, then $h(x)$ obviously satisfies the conditions of the lemma. However,  

$$
\int_{a}^{b}\alpha(x)h(x)\ d x=\int_{x_{1}}^{x_{2}}\alpha(x)(x-x_{1})(x_{2}-x)d x>0,
$$  

since the integrand is positive (except at $x_{1}$ and $x_{2}$ ). This contradiction proves the lemma.  

Remark. The lemma still holds if we replace $\mathcal{C}(\boldsymbol{a},\boldsymbol{b})$ by ${\mathcal{D}}_{n}(a,b)$ . To see this, we use the same proof with  

$$
h(x)=[(x-x_{1})(x_{2}-x)]^{n+1}
$$  

for $x$ in $[x_{1},x_{2}]$ and $h(x)=0$ otherwise.  

LEMMA 2. I $\pmb{\alpha}(\pmb{x})$ is continuous in $[a,b],$ and i  

$$
\int_{a}^{b}\alpha(x)h^{\prime}(x)d x=0
$$  

for every function $h(x)\in{\mathcal{D}}_{1}(a,b)$ such that $h(a)=h(b)=0;$ , then $\alpha(x)=c$ for all $x$ in $[a,b]$ , where c is a constant.  

Proof. Let $c$ be the constant defined by the condition  

$$
\int_{a}^{b}\left[\alpha(x)-c\right]d x=0,
$$  

and let  

$$
h(x)=\int_{a}^{x}\left[\alpha(\xi)-c\right]d\xi,
$$  

so that $h(x)$ automatically belongs to $\mathcal{D}_{1}(a,b)$ and satisfies the con­ ditions $h(a)=h(b)=0$ . Then on the one hand,  

$$
\int_{a}^{b}{[{\alpha(x)}-c]}h^{\prime}(x)d x=\int_{a}^{b}\alpha(x)h^{\prime}(x)d x-c[h(b)-h(a)]=0,
$$  

while on the other hand,  

$$
\int_{a}^{b}[\alpha(x)-c]h^{\prime}(x)d x=\int_{a}^{b}[\alpha(x)-c]^{2}d x.
$$  

It follows that $\alpha(x)-c=0,$ i . e . , $\alpha(x)=c$ , for all $x$ in $[a,b]$ .  

The next lemma will be needed in Chapter 8 :  

LEMMA 3 . I $\alpha(x)$ is continuous in $[a,b]$ , and i  

$$
\int_{a}^{b}\alpha(x)h^{\prime\prime}(x)d x=0
$$  

for every function $h(x)\in{\mathcal{D}}_{2}(a,b)$ such that $h(a)=h(b)=0$ and $h^{\prime}(a)=h^{\prime}(b)=0$ , then $\alpha(x)=c_{0}+c_{1}x$ for all $x$ in $[a,b]$ , where $c_{0}a n d c_{1}$ are constants.  

Proof. Let $c_{0}$ and $c_{1}$ be defined by the conditions  

$$
\begin{array}{r}{{\displaystyle\int_{a}^{b}}\left[\alpha(x)-c_{0}-c_{1}x\right]d x=0,}\\ {{\displaystyle\int_{a}^{b}}d x\int_{a}^{x}\left[\alpha(\xi)-c_{0}-c_{1}\xi\right]d\xi=0,}\end{array}
$$  

and let  

$$
h(x)=\int_{a}^{\tau}d\xi\int_{a}^{\xi}\left[\alpha(t)-c_{0}-c_{1}t\right]d t,
$$  

so that $h(x)$ automatically belongs to $\mathcal{D}_{2}(a,b)$ and satisfies the conditions $h(a)=h(b)=0,h^{\prime}(a)=h^{\prime}(b)=0.$ . Then on the one hand,  

$$
\begin{array}{r l}{\lefteqn{\int_{a}^{b}[\alpha(x)-c_{0}-c_{1}x]h^{\prime}(x)d x}}\\ &{=\int_{a}^{b}\alpha(x)h^{\prime}(x)d x-c_{0}[h^{\prime}(b)-h^{\prime}(a)]-c_{1}\int_{a}^{b}x h^{\prime\prime}(x)d x}\\ &{=-c_{1}[b h^{\prime}(b)-a h^{\prime}(a)]-c_{1}[h(b)-h(a)]=0,}\end{array}
$$  

while on the other hand,  

$$
\int_{a}^{b}{[{\alpha(x)}-{\mathit{c}}_{0}-{\mathit{c}}_{1}x]}h^{\prime}(x)d x=\int_{a}^{b}{[{\alpha(x)}-{\mathit{c}}_{0}-{\mathit{c}}_{1}x]^{2}}d x=0.
$$  

It follows that $\alpha(x)-c_{0}-c_{1}x=0$ , i . e . , $\begin{array}{r}{\alpha(x)=c_{0}+c_{1}x,}\end{array}$ for all $x$ in $[a,b].$ .  

LEMMA 4. I $\alpha(x)$ and $\beta(x)$ are continuous in $[a,b]$ , and i  

$$
\int_{a}^{b}\left[\alpha(x)h(x)+\beta(x)h^{\prime}(x)\right]d x=0
$$  

for every function $h(x)\in{\mathcal{D}}_{1}(a,b)$ such that $h(a)=h(b)=0$ , then $\beta(x)$ is differentiable, and $\beta^{\prime}(x)=\alpha(x)$ for all $x$ in $[a,b]$ .  

Proof. Setting  

$$
A(x)=\int_{a}^{x}\alpha(\xi)d\xi,
$$  

and integrating by parts, we find that  

$$
\int_{a}^{b}\alpha(x)h(x)d x=-\int_{a}^{b}A(x)h^{\prime}(x)d x,
$$  

i.e., (8) can be rewritten as  

$$
\int_{a}^{b}{\left[{-A(x)+\beta(x)}\right]}h^{\prime}(x)d x=0.
$$  

But, according to Lemma 2, this implies that  

$$
\beta(x)-A(x)=\mathrm{const},
$$  

and hence by the definition of $\boldsymbol{A}(\boldsymbol{x})$ ,  

$$
\beta^{\prime}(x)=\alpha(x),
$$  

for all $x$ in $[a,b]$ , as asserted. We emphasize that the differentiability of the function $\beta(x)$ was not assumed in advance.  

3.2. We now introduce the concept of the variation (or differential) of a functional. Let $J[y]$ be a functional defined on some normed linear space, and let  

$$
\Delta J[h]=J[y+h]-J[y]
$$  

be its increment, corresponding to the increment $h=h(x)$ of the " independent variable " $y=y(x)$ . If $y$ is fi xed, $\Delta J[h]$ is a functional of $\pmb{h}$ , in general a nonlinear functional. Suppose that  

$$
\Delta J[h]=\varphi[h]+\varepsilon\|h\|,
$$  

where $\varphi[h]$ is a linear functional and ${\pmb\varepsilon}\rightarrow{\pmb0}$ as $\left\|h\right\|\to0$ . Then the functional $J[y]$ is said to be differentiable, and the principal l inear part of the increment  

$\Delta J[h]$ , i . e . , the linear functional $\varphi[h]$ which differs from $\Delta J[h]$ by an infinitesi­ mal of order higher than 1 relative to $\left\|h\right\|$ , is called the variation (or difefr ential) of $J[y]$ and is denoted by $\updelta J[h]$ . 6  

THEOREM 1. The difefrential of $a$ difefrentiable functional is unique.  

Proof First, we note that if $\varphi[h]$ is a linear functional and if  

$$
{\frac{\varphi[h]}{\left\|h\right\|}}\to0
$$  

as $\left\|h\right\|\to0$ , then $\varphi[h]\equiv0;$ , i . e . , $\varphi[h]=0$ for all $h$ . In fact, suppose $\varphi[h_{0}]\neq0$ for some $h_{0}\neq0$ . Then, setting  

$$
h_{n}=\frac{h_{0}}{n},\qquad\uplambda=\frac{\varphi[h_{0}]}{\left\|h_{0}\right\|},
$$  

we see that $\left\|h_{n}\right\|\to0$ as $n\rightarrow\infty$ ,  but  

$$
\operatorname*{lim}_{n\to\infty}\ {\frac{\varphi[h_{n}]}{\left\|h_{n}\right\|}}=\ \operatorname*{lim}_{n\to\infty}\ {\frac{n\varphi[h_{0}]}{n\left\|h_{0}\right\|}}=\uplambda\neq0,
$$  

contrary to hypothesis.  

Now, suppose the differential of the functional $J[y]$ is not uniquely defined, so that  

$$
\begin{array}{r}{\Delta J[h]=\varphi_{1}[h]+\varepsilon_{1}\|h\|,}\\ {\Delta J[h]=\varphi_{2}[h]+\varepsilon_{2}\|h\|,}\end{array}
$$  

where $\varphi_{1}[h]$ and $\varphi_{2}[h]$ are linear functionals, and $\mathfrak{s}_{1},\mathfrak{s}_{2}\to0$ as $\left\|h\right\|\to0$ . T his implies  

$$
\mathfrak{p}_{1}[h]-\mathfrak{p}_{2}[h]=\mathfrak{e}_{2}\|h\|
$$  

and hence $\varphi_{1}[h]-\varphi_{2}[h]$ is an infinitesimal of order higher than 1 relative to $\left\|h\right\|$ . But since $\varphi_{1}[h]-\varphi_{2}[h]$ is a linear functional, it follows from the first part of the proof that $\varphi_{1}[h]-\varphi_{2}[h]$ vanishes identically, as asserted.  

Next, we use the concept of the variation (or) differential of a functional to establish a necessary condition for a functional to have an extremum. We begin by recalling the corresponding concepts from analysis. Let $F(x_{1},\ldots,x_{n})$ be a differentiable function of $\pmb{n}$ variables. Then $F(x_{1},\ldots,x_{n})$ is said to have a (relative) extremum at the point $(\hat{x}_{1},...,\hat{x}_{n})$ if  

$$
\Delta F=F(x_{1},\ldots,x_{n})-F({\hat{x}}_{1},\ldots,{\hat{x}}_{n})
$$  

has the same sign for all points $(x_{1},...,x_{n})$ belonging to some neighborhood of $(\hat{x}_{1},...,\hat{x}_{n})$ , where the extremum $F(\hat{x}_{1},....,\hat{x}_{n})$ is a minimum if $\Delta F\geqslant0$ and a maximum if $\Delta F\leqslant0$ .  

Analogously, we say that the functional $J[y]$ has a (relative) extremum for $\boldsymbol{y}=\boldsymbol{\hat{y}}$ f $J[y]-J[\hat{y}]$ does not change its sign in some neighborhood of the curve $y={\hat{y}}(x)$ . Subsequently, we shall be concerned with functionals defined on some set of continuously differentiable functions, and the functions themselves can be regarded either as elements of the space $\mathscr{C}$ or elements of the space $\mathcal{D}_{\mathbf{1}}$ . Corresponding to these two possibilities, we can define two kinds of extrema: We shall say that the functional $J[y]$ has a weak extremum for $y=\hat{y}$ if there exists an $\mathfrak{s}>0$ such that $J[y]-J[{\hat{y}}]$ has the same sign for all $y$ in the domain of definition of the functional which satisfy the condition $\|y-\hat{y}\|_{1}<\varepsilon$ , where $\bigstar\bigstar\bigstar|\bigstar\bigstar\bigstar||_{\mathbf{1}}$ denotes the norm in the space $\mathcal{D}_{1}$ . On the other hand, we shall say that the functional $J[y]$ has a strong extremum for $\boldsymbol{y}=\boldsymbol{\hat{y}}$ if there exists an- E $>0$ such that $J[y]-J[{\hat{y}}]$ has the same sign for all $y$ in the domain of definition of the functional which satisfy the condition $\|y-\hat{y}\|_{0}<\varepsilon,$ , where $\Vert\quad\Vert_{\textbf{0}}$ denotes the norm in the space $\mathscr{C}$ . It is clear that every strong extremum is simultaneously a weak extremum, since if $\|y-\hat{y}\|_{1}<\varepsilon,$ , then $\|y-\hat{y}\|_{0}<\varepsilon$ , a fortiori, and hence, if $J[\hat{y}]$ is an extremum with respect to all $y$ such that $\|y-\hat{y}\|_{0}<\varepsilon$ , then $J[\hat{y}]$ is certainly an extremum with respect to all $y$ such that $\|y-\hat{y}\|_{1}<\varepsilon$ . How­ ever, the converse is not true in general, i.e. , a weak extremum may not be a strong extremum. As a rule, finding a weak extremum is simpler than finding a strong extremum. The reason for this is that. the functionals usually considered in the calculus of variations are continuous in the norm of the space $\mathcal{D}_{1}$ (as noted at the end of the previous section), and this con­ tinuity can be exploited in the'theory of weak extrema. In general, however, our functionals will not be continuous in the norm of the space $\mathscr{C}$ .  

THEOREM 2. $A$ necessary condition for the differentiable functional $J[y]$ to have an extremum for $\boldsymbol{y}=\boldsymbol{\hat{y}}$ is that its v,ariation vanish for $y=\hat{y}$ , i.e. , that  

$$
\begin{array}{r}{\delta J[h]=0}\end{array}
$$  

for $\boldsymbol{y}=\boldsymbol{\hat{y}}$ and all admissible $\pmb{h}$ .  

Proof To be explicit, suppose $J[y]$ has a mIDlmum for $\boldsymbol{y}=\boldsymbol{\hat{y}}$ . According to the definition of the variation $\updelta J[h]$ , we have  

$$
\Delta J[h]=\updelta J[h]+\upvarepsilon\lVert h\rVert,
$$  

where $\varepsilon\rightarrow0$ as $\left\|h\right\|\to0$ . Thus, for sufficiently small $\left\|h\right\|$ , the sign of $\Delta J[h]$ will be the same as the sign of $\updelta J[h]$ . Now, suppose that $\updelta J[h_{0}]\neq0$ for some admissible $h_{0}$ • Then for any $\alpha>0$ , no matter how small, we have  

$$
\updelta J[-\alpha h_{0}]=-\updelta J[\alpha h_{0}].
$$  

Hence, (9) can be made to have either sign for arbitrarily small $\left\|h\right\|$ . But this is impossible, since by hypothesis $J[y]$ has a minimum for $\boldsymbol{y}=\boldsymbol{\hat{y}}$ , i . e . ,  

$$
\Delta J[h]=J[\hat{y}+h]-J[\hat{y}]\geqslant0
$$  

for all sufficiently small $\left\|h\right\|$ . This contradiction proves the theorem.  

Remark. In elementary analysis, it is proved that for a function to have a minimum, it is necessary not only that its first differential vanish $(d f=0)$ , but also that its second differential be nonnegative. Consideration of the analogous problem for functionals will be postponed until Chapter 5.  

# 4. The S i m p l est Variat i o n al Pro b l e m . E u l e r's Eq uation  

4.1. We begin our study of concrete variational problems by considering what might be called the "simplest " variational problem, which can be formulated as follows: Let $F(x,y,z)$ be a function with continuous first and second (partial ) derivatives with respect to all its arguments. Then, among all functions $y(x)$ which are continuously differentiable for $a\leqslant x\leqslant b$ and satisfy the boundary conditions  

$$
y(a)=A,\qquady(b)=B,
$$  

find the function for which the functional  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x
$$  

has a weak extremum. In other words, the simplest variational problem consists of finding a weak extremum of a functional of the form ( I I), where the class of admissible curves (see p. 8) consists of all smooth curves joining two points. The first two examples on pp. 2, 3, involving the brachistochrone and the shortest distance between two points, are variational problems of j ust this type. To apply the necessary condition for an extremum (found in Sec. 3.2) to the problem just formulated, we have to be able to calculate the variation of a functional of the type ( I I). We now derive the appropriate formula for this variation.  

Suppose we give $y(x)$ an increment $h(x)$ , where, in order for the function  

$$
y(x)+h(x)
$$  

to continue to satisfy the boundary conditions, we must have  

$$
h(a)=h(b)=0.
$$  

Then, since the corresponding increment of the functional ( I I ) equals  

$$
\begin{array}{l}{\displaystyle\Delta J=J[y+h]-J[y]=\int_{a}^{b}F(x,y+h,y^{\prime}+h^{\prime})d x-\int_{a}^{b}F(x,y,y^{\prime})d x}\\ {=\int_{a}^{b}\left[F(x,y+h,y^{\prime}+h^{\prime})-F(x,y,y^{\prime})\right]d x,}\end{array}
$$  

it follows by using Taylor's theorem that  

$$
\Delta J=\int_{a}^{b}\left[F_{y}(x,y,y^{\prime})h+F_{y}(x,y,y^{\prime})h^{\prime}\right]d x+\cdot\cdot\cdot,
$$  

where the subscripts denote partial derivatives with respect to the corres­ ponding arguments, and the dots denote terms of order higher than 1 relative to $h$ and $h^{\prime}$ . The integral in the right-hand side of ( 1 2) represents the principal linear part of the increment $\Delta J$ , and hence the variation of $J[y]$ is  

$$
\displaystyle\mathfrak{J}J=\int_{a}^{b}\left[F_{y}(x,y,y^{\prime})h+F_{y^{\prime}}(x,y,y^{\prime})h^{\prime}\right]d x.
$$  

According to Theorem 2 of Sec. 3.2, a necessary condition for $J[y]$ to have an extremum for $y=y(x)$ is that  

$$
\updelta J=\int_{a}^{b}\left(F_{y}h+F_{y},h^{\prime}\right)d x=0
$$  

for all admissible $\pmb{h}$ . But according to Lemma 4 of Sec. 3 . 1 ,  ( 1 3) implies that  

$$
F_{y}-\frac{d}{d x}F_{y^{\prime}}=0,
$$  

a result known as Euler s equation.7 Thus, we have proved  

THEOREM 1 .  Let $J[y]$ be a functional of the form  

$$
\int_{a}^{b}F(x,y,y^{\prime})d x,
$$  

defined on the set offunctions $y(x)$ which have continuous first derivatives in $[a,b]$ and satisfy the boundary conditions $y(a)=A,$ , $y(b)=B$ . Then a necessary condition for $J[y]$ to have an extremum for $a$ given function $y(x)$ is that $y(x)$ satisfy Euler s equationB  

$$
F_{y}-{\frac{d}{d x}}F_{y^{\prime}}=0.
$$  

The integral curves of Euler's equation are called extremals. Since Euler's equation is a second-order differential equation, its solution will in general depend on two arbitrary constants, which are determined from the boundary conditions $y(a)=A,y(b)=B.$ . The problem usually considered in the theory of differential equations is that of finding a solution which is defined in the neighborhood of some point and satisfies given initial con­ ditions (Cauchy s problem). However, in solving Euler's equation, we are looking for a solution which is defined over all of some fixed region and satisfies given boundary conditions. Therefore, the question of whether or not a certain variational problem has a solution does not just reduce to the usual existence theorems for differential equations. In this regard, we now state a theorem due to Bernstein,9 concerning the existence and uniqueness of solutions "in the large " of an equation of the form  

$$
y^{\prime\prime}=F(x,y,y^{\prime}).
$$  

THEOREM 2 (Bernstein). If the functions $F$ , $F_{y}$ and $F_{y},$ are continuous at every finite point $(x,y)$ for any finite $y^{\prime}$ , and if a constant $k>0$ and functions  

$$
\alpha=\alpha(x,y)\geqslant0,\qquad\beta=\beta(x,y)\geqslant0
$$  

(which are bounded in every finite region of the plane) can be found such that  

$$
F_{y}(x,y,y^{\prime})>k,\qquad|F(x,y,y^{\prime})|\leqslant\alpha y^{\prime2}+\beta,
$$  

then one and only one integral curve of equation ( 1 5) passes through any two points $(a,A)$ and $(b,B)$ with different abscissas $(a\neq b)$ .  

Equation ( 1 3) gives a necessary condition for an extremum, but in general, one which is not sufficient. The question of sufficient conditions for an extremum will be considered in Chapter 5. In many cases, however, Euler's equation by itself is enough to give a complete solution of the prob­ lem. In fact, the existence of an extremum is often clear from the physical or geometric meaning of the problem, e.g. , in the brachistochrone problem, the problem concerning the shortest distance between two points, etc. If in such a case there exists only one extremal satisfying the boundary conditions of the problem, this extremal must perforce be the curve for which the extremum is achieved.  

For a functional of the form  

$$
\int_{a}^{b}F(x,y,y^{\prime})d x
$$  

Euler's equation is in general a second-order differential equation, but it may turn out that the curve for which the functional has its extremum is not twice differentiable. For example, consider the functional  

$$
J[y]=\int_{-1}^{1}y^{2}(2x-y^{\prime})^{2}d x,
$$  

where  

$$
y(-1)=0,\qquady(1)=1.
$$  

The minimum of $J[y]$ equals zero and is achieved for the function  

$$
y=y(x)={\left\{\begin{array}{l l}{0}&{{\mathrm{for}}\quad-1\leqslant x\leqslant0,}\\ {x^{2}}&{{\mathrm{for}}\quad\quad0<x\leqslant1,}\end{array}\right.}
$$  

which has no second derivative for $x=0$ . Nevertheless, $y(x)$ satisfies the appropriate Euler equation. In fact, since in this case  

$$
F(x,y,y^{\prime})=y^{2}(2x-y^{\prime})^{2},
$$  

it follows that all the functions  

$$
F_{y}=2y(2x-y^{\prime})^{2},~F_{y^{\prime}}=-2y^{2}(2x-y^{\prime}),~\frac{d}{d x}F_{y^{\prime}}
$$  

vanish identically for $-1\leqslant x\leqslant1$ .  Thus, despite the fact that Euler's equation is of the second order and $y^{\prime\prime}(x)$ does not exist everywhere in $[-1,1]$ , substitution of $y(x)$ into Euler's equation converts it into an identity.  

We now give conditions guaranteeing that a solution of Euler's equation has a second derivative :  

THEOREM 3. Suppose $y=y(x)$ has a continuous first derivative and satisfies Euler's equation  

$$
F_{y}-{\frac{d}{d x}}F_{y^{\prime}}=0.
$$  

Then, if the function $F(x,y,y^{\prime})$ has continuousfirst and second derivatives with respect to all its arguments, $y(x)$ has a continuous second derivative at al l points $(x,y)$ where  

$$
F_{y^{\prime}y^{\prime}}[x,y(x),y^{\prime}(x)]\neq0.
$$  

Proof. Consider the difference  

$$
\begin{array}{r l}&{\Delta F_{y^{\prime}}=F_{y^{\prime}}(x+\Delta x,y+\Delta y,y^{\prime}+\Delta y^{\prime})-F_{y^{\prime}}(x,y,y^{\prime})}\\ &{\qquad=\Delta x\bar{F}_{y^{\prime}x}+\Delta y\bar{F}_{y^{\prime}y}+\Delta y^{\prime}\bar{F}_{y^{\prime}y},}\end{array}
$$  

where the overbar indicates that the corresponding derivatives are evalu­ ated along certain intermediate curves. We divide this difference by $\Delta x$ , and consider the limit of the resulting expression  

$$
\overline{{F}}_{y^{\prime}x}+\frac{\Delta y}{\Delta x}\:\overline{{F}}_{y^{\prime}y}+\frac{\Delta y^{\prime}}{\Delta x}\:\overline{{F}}_{y^{\prime}y},
$$  

as $\Delta x\rightarrow0$ . (This limit exists, since $F_{y},$ has a derivative with respect to $x$ , which, according to Euler's equation, equals $F_{y}$ .) Since, by hypoth­ esis, the second derivatives of $F(x,y,z)$ are continuous, then, as $\Delta x\rightarrow0$ , $\overline{{F}}_{y^{\prime}x}$ converges to $F_{y^{\prime}x},$ i.e., to the value of $\partial^{2}F/\partial y^{\prime}\partial x$ at the point $x$ . It follows from the existence of $y^{\prime}$ and the continuity of the second derivative $F_{y^{\prime}y}$ that the second term $(\Delta y/\Delta x)\overline{{F}}_{y^{\prime}y}$ also has a limit as $\Delta x\to0$ . But then the third term also has a limit (since the limit of the sum of the three terms exists), i.e., the limit  

$$
\operatorname*{lim}_{\Delta x\to0}\frac{\Delta y^{\prime}}{\Delta x}\bar{F}_{y^{\prime}y^{\prime}}
$$  

exists. As $\Delta x\to0$ , $\overline{{F}}_{y^{\prime}y^{\prime}}$ converges to $F_{y^{\prime}y^{\prime}}\neq0$ , and hence  

$$
\operatorname*{lim}_{\Delta x\to0}{\frac{\Delta y^{\prime}}{\Delta x}}=y^{\prime}(x)
$$  

exists. Finally, from the equation  

$$
\frac{d}{d x}F_{y^{\prime}}-F_{y}=0,
$$  

we can find an expression for $y^{\prime\prime}$ , from which it is clear that $y^{\prime\prime}$ is continuous wherever $F_{y^{\prime}y^{\prime}}\neq0$ . This proves the theorem.  

Remark. Here it is assumed that the extremaIs are smooth. lO In Sec. 1 5 we shall consider the case where the solution of a variational problem may only be piecewise smooth, i.e., may have "corners " at certain points.  

4.2. Euler's equation ( 1 4) plays a fundamental role in the calculus of variations, and is in general a second-order differential equation. We now indicate some special cases where Euler's equation can be reduced to a first­ order differential equation, or where its solution can be obtained entirely in terms of quadratures (i.e., by evaluating integrals).  

Case 1. Suppose the integrand does not depend on y, i.e., let the functional under consideration have the form  

$$
\int_{a}^{b}F(x,y^{\prime})d x,
$$  

where $F$ does not contain $y$ explicitly. In this case, Euler's equation becomes  

$$
\frac{d}{d x}F_{y^{\prime}}=0,
$$  

which obviously has the first integral  

$$
F_{y^{\prime}}=C,
$$  

where $c$ is a constant. This is a first-order differential equation which does not contain $y$ . Solving ( 1 6) for $y^{\prime}$ , we obtain an equation of the form  

$$
y^{\prime}=f(x,C),
$$  

from which $y$ can be found by a quadrature.  

Case 2. If the integrand does not depend on $x$ , i . e . , if  

then  

$$
\begin{array}{c}{{J[y]=\displaystyle\int_{a}^{b}F(y,y^{\prime})d x,}}\\ {{{}}}\\ {{F_{y}-\displaystyle\frac{d}{d x}F_{y^{\prime}}=F_{y}-F_{y^{\prime}y}y^{\prime}-F_{y^{\prime}y^{\prime}}y^{\prime\prime}.}}\end{array}
$$  

Multiplying ( 1 7) by $y^{\prime}$ , we obtain  

$$
F_{y}y^{\prime}-F_{y^{\prime}y}y^{\prime2}-F_{y^{\prime}y^{\prime}}y^{\prime}y^{\prime\prime}={\frac{d}{d x}}(F-y^{\prime}F_{y^{\prime}}).
$$  

Thus, in this case, Euler's equation has the first integral  

$$
F-y^{\prime}F_{y^{\prime}}=C,
$$  

where $c$ is a constant.  

Case 3. i $\pmb{F}$ does not depend on $y^{\prime}$ , Euler's equation takes the form  

$$
F_{y}(x,y)=0,
$$  

and hence is not a differential equation, but a "finite " equation, whose solution consists of one or more curves $y=y(x)$ .  

Case 4. In a variety of problems, one encounters functionals of the form  

$$
\int_{a}^{b}f(x,y){\sqrt{1+y^{\prime}{}^{2}}}d x,
$$  

representing the integral of a function $f(x,y)$ with respect to the arc length $s(d s=\sqrt{1+y^{\prime2}}d x)$ . In this case, Euler's equation can be transformed into  

$$
\begin{array}{l}{{\displaystyle\frac{\partial F}{\partial y}-\frac{d}{d x}\left(\frac{\partial F}{\partial y^{\prime}}\right)=f_{y}(x,y)\sqrt{1+y^{\prime2}}-\frac{d}{d x}\left[f(x,y)\frac{y^{\prime}}{\sqrt{1+y^{\prime2}}}\right]}}\\ {{\mathrm{}=f_{y}\sqrt{1+y^{\prime2}}-f_{z}\frac{y^{\prime}}{\sqrt{1+y^{\prime2}}}-f_{y}\frac{y^{\prime2}}{\sqrt{1+y^{\prime2}}}-f\frac{y^{\prime\prime}}{\left(1+y^{\prime2}\right)^{3}}}}\\ {{\mathrm{}=\frac{1}{\sqrt{1+y^{\prime2}}}\left[f_{y}-f_{x}y^{\prime}-f\frac{y^{\prime\prime}}{1+y^{\prime2}}\right]=0,}}\end{array}
$$  

i . e . ,  

$$
f_{y}-f_{x}y^{\prime}-f{\frac{y^{\prime\prime}}{1+y^{\prime2}}}=0.
$$  

Example 1. Suppose that  

$$
J[y]=\int_{1}^{2}\frac{\sqrt{1+y^{'2}}}{x}d x,y(1)=0,y(2)=1.
$$  

The integrand does not contain $y$ , and hence Euler's equation has the form $F_{y^{\prime}}=C$ (cf. Case 1 ) . Thus,  

$$
{\frac{y^{\prime}}{x{\sqrt{1+y^{\prime2}}}}}=C,
$$  

so that  

$$
y^{\prime2}(1-C^{2}x^{2})=C^{2}x^{2}
$$  

or  

$$
y^{\prime}=\frac{C x}{\sqrt{1-C^{2}x^{2}}},
$$  

from which it follows that  

$$
y=\int{\frac{C x d x}{{\sqrt{1-C^{2}x^{2}}}}}={\frac{1}{C}}{\sqrt{1-C^{2}x^{2}}}+C_{1}
$$  

or  

$$
(y-C_{1})^{2}+x^{2}={\frac{1}{C^{2}}}.
$$  

Thus, the solution is a circle with its center on the $y$ -axis. From the conditions $y(1)=0,y(2)=1$ , we find that  

$$
C={\frac{1}{\sqrt{\less5}}},\qquadC_{1}=2,
$$  

so that the final solution is  

$$
(y-2)^{2}+x^{2}=5.
$$  

Example 2. Among all the curves joining two given points $(x_{0},y_{0})$ and $(x_{1},y_{1})$ ,jind the one which generates the surface ofminimum area when rotated about the $x$ -axis. As we know, the area of the surface of revolution generated by rotating the curve $y=y(x)$ about the $x$ -axis is  

$$
2\pi\int_{x_{0}}^{x_{1}}y\sqrt{1+y^{\prime}{}^{2}}d x.
$$  

Since the integrand does not depend explicitly on $x$ , Euler's equation has the first integral  

$$
F-y^{\prime}F_{y^{\prime}}=C
$$  

(cf. Case 2), i . e . ,  

$$
y{\sqrt{1+y^{\prime2}}}-y{\frac{y^{\prime2}}{\sqrt{1+y^{\prime2}}}}=C
$$  

or  

$$
y=C\sqrt{1+y^{\prime2}},
$$  

so that  

$$
y^{\prime}={\sqrt{\frac{y^{2}-C^{2}}{C^{2}}}}.
$$  

Separating variables, we obtain  

$$
d x={\frac{C d y}{\sqrt{y^{2}-C^{2}}}},
$$  

i . e . ,  

$$
x+C_{1}=C\ln\frac{y+\sqrt{y^{2}-C^{2}}}{C},
$$  

so that  

$$
y=C\cosh{\frac{x+C_{1}}{C}}.
$$  

Thus, the required curve is a catenary passing through the two given points. The surface generated by rotation of the catenary is called a catenoid. The values of the arbitrary constants $c$ and $C_{1}$ are determined by the conditions  

$$
y(x_{0})=y_{0},\qquady(x_{1})=y_{1}.
$$  

It can be shown that the following three cases are possible, depending on the positions o f the points $(x_{0},y_{0})$ and $(x_{1},y_{1})$ :  

1 .  If a single curve of the form (1 8) can be drawn through the points $(x_{0},y_{0})$ and $(x_{1},y_{1})$ , this curve is the solution of the problem [see Figure 2(a)].   
2. If two extremals can be drawn through the points $(x_{0},y_{0})$ and $(x_{1},y_{1})$ , one of the curves actually corresponds to the surface of revolution of minimum area, and the other does not.   
3 . If there is no curve of the form ( 1 8) passing through the points $(x_{0},y_{0})$ and $(x_{1},y_{1})$ , there is no surface in the class of smooth surfaces of revo­ lution which achieves the minimum area. In fact, if the location of the  

![](https://cdn-mineru.openxlab.org.cn/extract/c29daec4-3bde-4c07-a565-58de41e65c3b/c5ebc0b9dc8adcf3d79d080f456ffc2b68745ffe5bc17ccd8d51b38c6ee45216.jpg)  
FIGURE 2  

two points is such that the distance between them is sufficiently large compared to their distances from the $x$ -axis, then the area of the surface consisting of two circles of radius $y_{0}$ and $y_{1}$ , plus the segment of the $x$ -axis j oining them [see Figure 2(b)] will be less than the area of any surface of revolution generated by a smooth curve passing through the points. Thus, in this case the surface of revolution generated by the polygonal line $A x_{0}x_{1}B$ has the minimum area, and there is no surface of minimum area in the class of surfaces generated by rotation about the $x$ -axis of smooth curves passing through the given points. (This case, corresponding to a " broken extremal," will be discussed further in Sec. 1 5 .)  

Example 3. For the functional  

$$
J[y]=\int_{a}^{b}(x-y)^{2}d x,
$$  

Euler's equation reduces to a finite equation (see Case 3), whose solution is the straight line $y=x$ . In fact, the integral ( 1 9) vanishes along this line.  

# 5. The Case of Several Variables  

So far, we have considered functionals depending on functions of one variable, i.e., on curves. In many problems, however, one encounters functionals depending on functions of several independent variables, i.e., on surfaces. Such multidimensional problems will be considered in detail in Chapter 7. For the time being, we merely give an idea of how the formula­ tion and solution of the simplest variational problem discussed above carries over to the case of functionals depending on surfaces.  

To keep the notation simple, we confine ourselves to the case of two independent variables, but all our considerations remain the same when there are $\pmb{n}$ independent variables. Thus, let $F(x,y,z,p,q)$ be a function with continuous first and second (partial) derivatives with respect to all its argu­ ments, and consider a functional of the form  

$$
J[z]=\int\int_{R}F(x,y,z,z_{x},z_{y})d x d y,
$$  

where $R$ is some closed region and $z_{x},z_{y}$ are the partial derivatives of $z=z(x,y)$ . Suppose we are looking for a function $z(x,y)$ such that  

1. $z(x,y)$ and its first and second derivatives are continuous in $R$ ;   
2 . $z(x,y)$ takes given values on the boundary $\Gamma$ of $R$ ;   
3 .  The functional (20) has an extremum for $z=z(x,y)$ .  

Since the proof of Theorem 2 of Sec. 3.2 does not depend on the form of the functional $J$ , then, just as in the case of one variable, a necessary condition for the functional (20) to have an extremum is that its variation (i.e., the principal linear part of its increment) vanish. However, to find Euler's equation for the functional (20), we need the following lemma, which is analogous to Lemma 1 of Sec. 3. 1 (see also the remark on p. 9):  

LEMMA. If $\alpha(x,y)$ is a fixed function which is continuous in a closed region $R,$ and if the integral  

$$
\int\int_{R}\alpha(x,y)h(x,y)d x d y
$$  

vanishes for every function $h(x,y)$ which has continuous first and second derivatives in $R$ and equals zero on the boundary $\Gamma$ of $R_{:}$ , then $\alpha(x,y)=0$ everywhere in $R$ .  

Proof. Suppose the function $\alpha(x,y)$ is nonzero, say positive, at some point in $R$ . Then $\alpha(x,y)$ is also positive in some circle  

$$
(x-x_{0})^{2}+(y-y_{0})^{2}\leqslant\varepsilon^{2}
$$  

contained in $R$ , with center $(x_{0},y_{0})$ and radius e. If we set $h(x,y)=0$ outside the circle (22) and  

$$
h(x,y)=[(x-x_{0})^{2}+(y-y_{0})^{2}-\varepsilon^{2}]^{3}
$$  

inside the circle, then $h(x)$ satisfies the conditions of the lemma. How­ ever, in this case, (2 1 ) reduces to an integral over the circle (22) and is obviously positive. This contradiction proves the lemma.  

In order to apply the necessary condition for an extremum of the functional (20), i . e . , $\ \delta J=0$ , we must first calculate the variation $\otimes J$ . Let $h(x,y)$ be an arbitrary function which has continuous first and second derivatives in the region $R$ and vanishes on the boundary $\Gamma$ of $R$ . Then if $z(x,y)$ belongs to the domain of definition of the functional (20), so does $z(x,y)+h(x,y)$ . Since  

$$
\Delta J=J[z+h]-J[z]=\int\int_{R}\left[F(x,y,z+h,z_{x}+h_{x},z_{y}+h_{y})\right.}\\ {\left.-\ F(x,y,z,z_{x},z_{y})\right]d x d y,
$$  

it follows by using Taylor's theorem that  

$$
\Delta J=\int\int_{R}\left(F_{z}h+F_{z_{z}}h_{x}+F_{z_{y}}h_{y}\right)d x d y+\cdot\cdot\cdot,
$$  

where the dots denote terms of order higher than 1 relative to $h,h_{x}$ and $\begin{array}{r}{h_{y}}\end{array}$ • The integral on the right represents the principal linear part of the increment $\Delta J$ , and hence the variation of $\boldsymbol{J}[\boldsymbol{z}]$ is  

$$
\updelta J=\int\int_{R}\left(F_{z}h+F_{z_{z}}h_{x}+F_{z_{y}}h_{y}\right)d x d y.
$$  

Next, we observe that  

$$
\begin{array}{r l r}{\lefteqn{\int_{R}\int_{\mathbb{R}}\left(F_{z_{u}}h_{x}+F_{z_{y}}h_{y}\right)d x d y}}\\ &{}&{=\int_{R}\left[\frac{\hat{\partial}}{\partial x}\left(F_{z_{x}}h\right)+\frac{\hat{\partial}}{\partial y}\left(F_{z_{y}}h\right)\right]d x d y-\int_{R}\left(\frac{\hat{\partial}}{\partial x}F_{z_{x}}+\frac{\hat{\partial}}{\partial y}F_{z_{y}}\right)h d x d y}\\ &{}&{=\int_{\mathbb{r}}\left(F_{z_{z}}h d y-F_{z_{y}}h d x\right)-\int\int_{R}\left(\frac{\hat{\partial}}{\partial x}F_{z_{z}}+\frac{\hat{\partial}}{\partial y}F_{z_{y}}\right)h d x d y,}\end{array}
$$  

where in the last step we have used Green's theoreml l  

$$
\int\int_{R}\left({\frac{\partial Q}{\partial x}}-{\frac{\partial P}{\partial y}}\right)d x d y=\int_{\Gamma}(P d x+Q d y).
$$  

The integral along $\Gamma$ is zero, since $h(x,y)$ vanishes on $\Gamma_{\/{\/}}$ , and hence, comparing the last two formulas, we find that  

$$
\S J=\int\int_{R}\left(F_{z}-\frac{\partial}{\partial x}F_{z_{z}}-\frac{\partial}{\partial y}F_{z_{y}}\right)h(x,y)d x d y.
$$  

Thus, the condition $\ \delta J=0$ implies that the double integral (23) vanishes for any $h(x,y)$ satisfying the stipulated conditions. According to the lemma, this leads to the following second-order partial differential equation, again known as Euler's equation :  

$$
F_{z}-\frac{\partial}{\partial x}F_{z_{z}}-\overset{\partial}{\partial y}F_{z_{y}}=0.
$$  

We are looking for a solution of (24) which takes given values on the boundary $\Gamma$ .  

Example. Find the surface of least area spanned by $a$ given contour. This problem reduces to finding the minimum of the functional  

$$
J[z]=\int\int_{R}\sqrt{1+z_{x}^{2}+z_{y}^{2}}d x d y,
$$  

so that Euler's equation has the form  

$$
r(1+q^{2})-2s p q+t(1+p^{2})=0,
$$  

where  

$$
p=z_{x},q=z_{y},r=z_{x x},s=z_{x y},t=z_{y y}.
$$  

Equation (25) has a simple geometric meaning, which we explain by using the formula  

$$
M={\frac{1}{2}}\left({\frac{1}{\varkappa_{1}}}+{\frac{1}{\varkappa_{2}}}\right)={\frac{E g-2F f+G e}{2(E G-F^{2})}}
$$  

for the mean curvature of the surface, where $E,F,G$ and $e,f,g$ are the coefficients of the first and second fundamental quadratic forms of the surface. 12 If the surface is given by an explicit equation of the form $z=z(x,y)$ , then  

$$
E=1+p^{2},~F=p q,~G=1+q^{2},
$$  

$$
e={\frac{r}{\displaystyle{\sqrt{1+p^{2}+q^{2}}}}},f={\frac{s}{\displaystyle{\sqrt{1+p^{2}+q^{2}}}}},g={\frac{t}{\displaystyle{\sqrt{1+p^{2}+q^{2}}}}},
$$  

and hence  

$$
{\cal M}={\frac{(1+p^{2})t-2s p q+(1+q^{2})r}{{\sqrt{1+p^{2}+q^{2}}}}}.
$$  

Here, the numerator coincides with the left-hand side of Euler's equation (25). Thus, (25) implies that the mean curvature of the required surface equals zero. Surfaces with zero mean curvature are called minimal surfaces.  

# 6. A S i m pl e Variable End Poi nt Pro b l e m  

There are, o f course, many other kinds o f variational problems besides the " simplest " variational problem considered so far, and such problems will be studied in Chapters 2 and 3 . However, this is a suitable place for acquainting the reader with one of these problems, i.e., the variable end point problem, a particular case of which can be stated as follows : Among all curves whose end points lie on two given vertical lines $x=a$ and $x=b$ , find the curve for which the functional  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x
$$  

has an extremum. 3  

We begin by calculating the variation $\otimes J$ of the functional (26). As before, $\otimes J$ means the principal linear part of the increment  

$$
\Delta J=J[y+h]-J[y]=\int_{a}^{b}{[F(x,y+h,y^{\prime}+h^{\prime})-F(x,y,y^{\prime})]d x}.
$$  

Using Taylor's theorem to expand the integrand, we obtain  

$$
\Delta J=\int_{a}^{b}\left(F_{y}h+F_{y}.h^{\prime}\right)d x+\cdot\cdot\cdot,
$$  

where the dots denote terms of order higher than 1 relative to $\boldsymbol{h}$ and $h^{\prime}$ , and hence  

$$
\displaystyle\mathfrak{d}J=\int_{a}^{b}\left(F_{y}h+F_{y},h^{\prime}\right)d x.
$$  

Here, unlike the fixed end point problem, $h(x)$ need no longer vanish at the points $a$ and $\pmb{b}$ , so that integration by parts now gives 14  

$$
\begin{array}{l}{\displaystyle\vartheta J=\int_{a}^{b}\left(F_{y}-\frac{d}{d x}F_{y}.\right)h(x)d x+F_{y}.h(x)|_{x=a}^{x=b}}\\ {\displaystyle\quad=\int_{a}^{b}\left(F_{y}-\frac{d}{d x}F_{y}.\right)h(x)d x+F_{y}.|_{x=b}h(b)-F_{y}.|_{x=a}h(a).}\end{array}
$$  

We first consider functions $h(x)$ such that $h(a)=h(b)=0$ . Then, as in the simplest variational problem, the condition $\delta J=0$ implies that  

$$
F_{y}-{\frac{d}{d x}}F_{y^{\prime}}=0.
$$  

Therefore, in order for the curve $y=y(x)$ to be a solution of the variable end point problem, $y$ must be an extremal, i.e., a solution of Euler's equation.  

But if $y$ is an extremal, the integral in the expression (27) for $\otimes J$ vanishes, and then the condition $\ \delta J=0$ takes the form  

$$
F_{y^{\prime}}|_{x=b}h(b)-F_{y^{\prime}}|_{x=a}h(a)=0,
$$  

from which it follows that  

$$
F_{y^{\prime}}|_{x=a}=0,\qquadF_{y^{\prime}}|_{x=b}=0,
$$  

since $h(x)$ is arbitrary. Thus, to solve the variable end point problem, we must first find a general integral of Euler's equation (28), and then use the conditions (29), sometimes called the natural boundary conditions, to determine the values of the arbitrary constants.  

Besides the case of fixed end points and the case of variable end points, we can also consider the mixed case, where one end is fixed and the other is variable. For example, suppose we are looking for an extremum of the functional (26) with respect to the class of curves joining a given point $A$ (with abscissa $a$ ) and an arbitrary point of the line $x=b$ . In this case, the conditions (29) reduce to the single condition  

$$
\left.F_{y^{\prime}}\right|_{x=b}=0,
$$  

and $y(a)=A$ serves as the second boundary condition.  

Example. Starting from the point $P=(a,A)$ , $a$ heavy particle slides down a curve in the vertical plane. Find the curve such that the particle reaches the vertical line $x=b(\neq a)$ in the shortest time. (This is a variant of the brachistochrone problem, p. 3.)  

For simplicity, we assume that the original point coincides with the origin of coordinates. Since the velocity of motion along the curve equals  

$$
v={\frac{d s}{d t}}={\sqrt{1+y^{\prime2}}}{\frac{d x}{d t}},
$$  

we have  

$$
d t=\frac{\sqrt{1+y^{\prime2}}}{v}d x=\frac{\sqrt{1+y^{\prime2}}}{\sqrt{2g y}}d x,
$$  

so that the transit time $T$ is given by the equation  

$$
T=\int\frac{\sqrt{1+y^{\prime2}}}{\sqrt{2g y}}d x.
$$  

The general solution of the corresponding Euler equation consists of a family of cycloids  

$$
x=r({\boldsymbol{\theta}}-\sin{\boldsymbol{\theta}})+c,\qquady=r(1-\cos{\boldsymbol{\theta}}).
$$  

Since the curve must pass through the origin, we must have $\boldsymbol{c}=0$ . To determine $r$ , we use the second condition  

$$
F_{y^{\prime}}=\frac{y^{\prime}}{\sqrt{2g y}\sqrt{1+y^{'2}}}=0\qquad\mathrm{for}\quad x=b,
$$  

i.e. , $y^{\prime}=0$ for $x=b$ , which means that the tangent to the curve at its right end point must be horizontal. It follows that $r=b/\pi$ , and hence the required curve is given by the equations  

$$
x=\frac{b}{\pi}(\theta-\sin\theta),~y=\frac{b}{\pi}(1-\cos\theta).
$$  

# 7. The Variational Derivative  

In Sec. 3.2 we introduced the concept of the differential of a functional. We now introduce the concept of the variational (or functional) derivative, which plays the same role for functionals as the concept of the partial derivative plays for functions of $\pmb{n}$ variables. We begin by considering functionals of the type  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x,\qquady(a)=A,\quad y(b)=B,
$$  

corresponding to the simplest variational problem. Our approach is to first go from the variational problem to an $\pmb{n}$ -dimensional problem, and then pass to the limit $n\rightarrow\infty$ .  

Thus, we divide the interval $[a,b]$ into $n+1$ equal subintervals by introducing the points  

$$
x_{0}=a,\ x_{1},\ldots,x_{n},\ x_{n+1}=b,\qquad(x_{i+1}-x_{i}=\Delta x),
$$  

and we replace the smooth function $y(x)$ by the polygonal line with vertices  

$$
(x_{0},y_{0}),(x_{1},y_{1}),\dotsc,(x_{n},y_{n}),(x_{n+1},y_{n+1}),
$$  

where $y_{i}=y(x_{i}).$ 15 Then (30) can be approximated by the sum  

$$
J(y_{1},\dots,y_{n})\equiv\sum_{i=0}^{n}F\left(x_{i},y_{i},{\frac{y_{i+1}-y_{i}}{\Delta x}}\right)\Delta x,
$$  

which is a function of $\pmb{n}$ variables. (Recall that $y_{0}=A$ and $y_{n+1}=B$ are fixed.)  

Next, we calculate the partial derivatives  

$$
\frac{\partial J(y_{1},\ldots,y_{n})}{\partial y_{k}},
$$  

and we consider what happens to these derivatives as the number of points of subdivision increases without limit. Observing that each variable $y_{k}$  

in (3 1 ) appears in just two terms, corresponding to $i=k$ and $i=k-1$ , we find that  

$$
\begin{array}{r l r}{\lefteqn{\frac{\partial J}{\partial y_{k}}=F_{y}\left(x_{k},y_{k},\frac{y_{k+1}-y_{k}}{\Delta x}\right)\Delta x}}\\ &{}&{+\ F_{y}\cdot\left(x_{k-1},y_{k-1},\frac{y_{k}-y_{k-1}}{\Delta x}\right)-\ F_{y}\cdot\left(x_{k},y_{k},\frac{y_{k+1}-y_{k}}{\Delta x}\right).}\end{array}
$$  

As $\Delta x\to0.$ i.e., as the number of points of subdivision increases without limit, the right-hand side of (32) obviously goes to zero, since it is a quantity of order $\Delta x$ . In order to obtain a limit which is in general nonzero as $\Delta x\rightarrow0$ , we divide (32) by $\Delta x,$ , obtaining  

$$
\begin{array}{l}{\displaystyle\frac{\partial J}{\partial y_{k}\Delta x}=F_{y}\left(x_{k},y_{k},\frac{y_{k+1}-y_{k}}{\Delta x}\right)}\\ {\displaystyle-\frac{1}{\Delta x}\left[F_{y^{\prime}}\left(x_{k},y_{k},\frac{y_{k+1}-y_{k}}{\Delta x}\right)-F_{y^{\prime}}\left(x_{k-1},y_{k-1},\frac{y_{k}-y_{k-1}}{\Delta x}\right)\right].}\end{array}
$$  

We note that the expression $\partial y_{k}\Delta x$ appearing in the denominator on the left has a direct geometric meaning, and is in fact just the area of the region lying between the solid and the dashed curves in Figure 3.  

![](https://cdn-mineru.openxlab.org.cn/extract/c29daec4-3bde-4c07-a565-58de41e65c3b/3547b3fbc60f4ca7d4005a6e7c665012e3e94e4996a9f8bac2a155794fd1f46d.jpg)  
FIGURE 3  

As $\Delta x{\rightarrow}0$ , the expression (33) converges to the limit  

$$
\frac{\delta J}{\delta y}\equiv F_{y}(x,y,y^{\prime})-\frac{d}{d x}F_{y^{\prime}}(x,y,y^{\prime}),
$$  

called the variational derivative of the functional (30). We see that the variational derivative $8J/\updelta y$ is just the left-hand side of Euler's equation (28), and hence the meaning of Euler's equation is just that the variational derivative of the functional under consideration should vanish at every point. This is the analog of the situation encountered in elementary analysis, where a necessary condition for a function of $\pmb{n}$ variables to have an extremum is that all its partial derivatives vanish.  

In the general case, the variational derivative is defined as follows : Let $J[y]$ be a functional depending on the function $y(x)$ , and suppose we give $y(x)$ an increment $h(x)$ which is different from zero only in the neighborhood of a point $\scriptstyle x_{0}$ . Dividing the corresponding increment $J[y+h]-J[y]$ of the functional by the area $\Delta\sigma$ lying between the curve $y=h(x)$ and the $x$ -axis, 16 we obtain the ratio  

$$
\frac{J[y+h]-J[y]}{\Delta\sigma}.
$$  

Next, we let the area $\Delta\sigma$ go to zero in such a way that both max $|h(x)|$ and the length of the interval in which $h(x)$ is nonvanishing go to zero. Then, if the ratio (34) converges to a limit as $\Delta\sigma\to0$ , this limit is called the variational derivative of the functional $J[y]$ at the point $\scriptstyle x_{0}$ [for the curve $y=y(x)],$ , and is denoted by  

$$
\left.\frac{\delta J}{\delta y}\right|_{x=x_{0}}
$$  

It can be shown that the analogs of all the familiar rules obeyed by ordinary derivatives (e.g. , the formulas for differentiating sums and products of func­ tions, composite functions, etc.) are valid for variational derivatives.  

Remark. It is clear from the definition of the variational derivative that if $h(x)$ is different from zero in a neighborhood of the point $\scriptstyle x_{0}$ and if $\Delta\sigma$ is the area between the curve $y=h(x)$ and the $x$ -axis, then  

$$
\Delta J\equiv J[y+h]-J[y]=\left\{\frac{\delta J}{\delta y}\right|_{x=x_{0}}+\varepsilon\right\}\Delta\sigma,
$$  

where $\varepsilon\to0$ as both max $|h(x)|$ and the length of the interval in which $h(x)$ is nonvanishing go to zero. It follows that in terms of the variational derivative, the differential or variation of the functional $J[y]$ at the point $\scriptstyle x_{0}$ [for the curve $y=y(x)]$ is given by the formula  

$$
\updelta J=\frac{\updelta J}{\updelta y}\bigg|_{z=z_{0}}\Delta\upsigma.
$$  

# 8. I nvariance of E u l e r's Eq uation  

Suppose that instead of the rectangular plane coordinates $x$ and $y$ , we introduce curvilinear coordinates $\pmb{u}$ and $\boldsymbol{v}$ , where  

$$
\begin{array}{c c}{{x=x(u,v),}}&{{\quad\left|x_{u}\quad x_{v}\right|\mathrm{~\neq~}0.}}\\ {{y=y(u,v),}}&{{\quad\left|y_{u}\quad y_{v}\right|\mathrm{~\neq~}0.}}\end{array}
$$  

Then the curve given by the equation $y=y(x)$ in the $x y.$ -plane corresponds to the curve given by some equation  

$$
\boldsymbol{v}=\boldsymbol{v}(\boldsymbol{u})
$$  

in the uv-plane. When we make the change of variables (35), the functional  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x
$$  

goes into the functional  

$$
\begin{array}{l}{{J_{1}[v]=\int_{a_{1}}^{b_{1}}F\left[x(u,v),y(u,v),{\frac{y_{u}+y_{v}v^{\prime}}{x_{u}+x_{v}v^{\prime}}}\right](x_{u}+x_{v}v^{\prime})d u}}\\ {{\ =\int_{a_{1}}^{b_{1}}F_{1}(u,v,v^{\prime})d u,}}\end{array}
$$  

where  

$$
F_{1}(u,v,v^{\prime})=F\left[x(u,v),y(u,v),{\frac{y_{u}+y_{v}v^{\prime}}{x_{u}+x_{v}v^{\prime}}}\right](x_{u}+x_{v}v^{\prime}).
$$  

We now show that if $y=y(x)$ satisfies the Euler equation  

$$
\frac{\partial F}{\partial y}-\frac{d}{d x}\frac{\partial F}{\partial y^{\prime}}=0
$$  

corresponding to the original functional $J[y],$ then $\boldsymbol{v}=\boldsymbol{v}(\boldsymbol{u})$ satisfies the Euler equation  

$$
\frac{\partial F_{1}}{\partial v}-\frac{d}{d u}\frac{\partial F_{1}}{\partial v^{\prime}}=0
$$  

corresponding to the new functional $J_{\boldsymbol{\imath}}[\boldsymbol{v}]$ . To prove this, we use the concept of the variational derivative, introduced in the preceding section. Let $\Delta\sigma$ denote the area bounded by the curves $y=y(x)$ and $y=y(x)+h(x).$ and let $\Delta\pmb{\sigma_{1}}$ denote the area bounded by the corresponding curves $v=v(u)$ and $v=v(u)+\eta(u)$ i n the $\boldsymbol{u v}$ -plane. By the standard formula for the trans­ formation of areas, the limit as $\Delta\upsigma,\Delta\upsigma_{1}\rightarrow0$ of the ratio $\Delta\sigma/\Delta\sigma_{1}$ approaches the Jacobian  

$$
{\left|\begin{array}{l l}{x_{u}}&{x_{v}}\\ {y_{u}}&{y_{v}}\end{array}\right|},
$$  

which by hypothesis is nonzero. Thus, if  

$$
\operatorname*{lim}_{\Delta\sigma\to0}\frac{J[y+h]-J[y]}{\Delta\sigma}=0,
$$  

then  

$$
\operatorname*{lim}_{\Delta\sigma_{1}\to0}\frac{J_{1}[v+\eta]-J_{1}[v]}{\Delta\sigma_{1}}=0
$$  

as well. It follows that $v(u)$ satisfies (37) if $y(x)$ satisfies (36). In other words, whether or not a curve is an extremal is a property which is independent of the choice of the coordinate system.  

In solving Euler's equation, changes of variables can often be used to advantage. Because of the invariance property just proved, the change of variables can be made directly in the integral representing the functional rather than in Euler's equation, and we can then write Euler's equation for the new integral.  

Example. Suppose we are looking for the extremals of the functional  

$$
J[r]=\int_{\varphi_{0}}^{\varphi_{1}}\sqrt{r^{2}+r^{\prime2}}d\varphi,
$$  

where $r=r(\varphi)$ . The corresponding Euler equation has the form  

$$
{\frac{r}{{\sqrt{r^{2}+r^{\prime2}}}}}-{\frac{d}{d\varphi}}{\frac{r^{\prime}}{\sqrt{r^{2}+r^{\prime2}}}}=0.
$$  

The change of variables  

$$
x=r\cos\varphi,\qquady=r\sin\varphi
$$  

transforms (38) into an integral of the form  

$$
\int_{z_{0}}^{z_{1}}{\sqrt{1+y^{\prime}{}^{2}}}d x,
$$  

which has the Euler equation  

$$
y^{\prime\prime}=0,
$$  

with general solution  

$$
y=\alpha x+\beta.
$$  

Therefore, the solution of (38) is  

$$
r\sin\varphi=\alpha r\cos\varphi+\beta.
$$  

# PROBLEMS  

1. Use the method of finite differences (Sec. 1) to find the shortest plane curve joining two points $\pmb{A}$ and $\pmb{B}$ .  

2. A set $\mathcal{M}$ i in a normed linear space $\mathscr{R}$ is said to be convex if $\mathcal{M}$ i contains all elements of the form $\alpha x+\beta y$ , where $\alpha,\beta\geqslant0,\alpha+\beta=1;$ , provided that $\mathcal{M}$ contains $\pmb{x}$ and $_y$ . Prove that the set of all elements ${\pmb x}\in\mathcal{R}$ satisfying the inequality $\|\pmb{x}-\pmb{x_{0}}\|\leqslant c$ , where $\scriptstyle\mathbf{\pmb{x_{0}}}$ is a fixed element of $\mathcal{R}$ and $c>0$ , is convex.  

3. Show that the set $\overline{{\mathscr{C}}}(a,b)$ of all continuous functions defined on the interval $[a,b]$ , equipped with the norm  

$$
\|y\|=\bigg\{\int_{a}^{b}|y(x)|^{2}d x\bigg\}^{1/2},
$$  

forms a normed linear space.  

4. An infinite sequence of elements $y_{1},y_{2},\ldots$ of elements of a normed linear space $\mathcal{R}$ is called a Cauchy sequence (or fundamental sequence) if, given any e: $>0$ , there exists an integer $N=N(\mathfrak{c})$ such that $\|y_{m}-y_{n}\|<\varepsilon$ , provided that $m>N,n>N.$ . A normed linear space $\mathcal{R}$ is said to be complete if every Cauchy sequence in $\mathcal{R}$ converges to some element in $\mathcal{R}$ . Prove that the space $\overline{{\mathscr{C}}}(a,b)$ introduced in the preceding problem is not complete, but that the space $\mathcal{C}(\boldsymbol{a},\boldsymbol{b})$ introduced in Sec. 2 is complete.  

Comment. See e.g., G. E. Shilov, OPe cit. , p . 249.  

5. Prove that any norm defined on a linear space $\mathscr{R}$ is a continuous functional on $\mathscr{R}$ .  

6. Suppose the norm of the space ${\mathcal{D}}_{n}(a,b)$ is defined as  

$$
\|y\|=\operatorname*{max}_{a\leqslant x\leqslant b}\{|y(x)|,|y^{\prime}(x)|,...,|y^{(n)}(x)|\},
$$  

instead of  

$$
\|y\|=\sum_{i=0}^{n}\operatorname*{max}_{a\leqslant x\leqslant b}|y^{(i)}(x)|,
$$  

as o n p . 7 .  Prove that any functional o n ${\mathcal{D}}_{n}(a,b)$ which is continuous with respect to one of these norms is continuous with respect to the other.  

7. Let $J[y]$ be the arc-length functional, defined for all $y\in\mathcal{D}_{1}(a,b)$ . Show that $J[y]$ is lower semicontinuous with respect to the norm of the space $\mathcal{C}(\boldsymbol{a},\boldsymbol{b})$ .  

Comment. As remarked in footnote 5, p. 8, J [y] is not continuous with respect to the norm of $\mathcal{C}(\boldsymbol{a},\boldsymbol{b})$ .  

8. Let $\varphi[h]$ be a linear functional defined on a normed linear space $\mathscr{R}$ . Prove that if $\boldsymbol{\varphi}[h]$ is continuous for $\pmb{h}=\pmb{0}$ , it is continuous for all $\pmb{h}\in\mathcal{R}$ lt .  

9. Prove that a linear functional $\varphi[h]$ cannot have an extremum unless $\varphi[h]\equiv0$ .  

10. Prove that if two linear functionals $\boldsymbol{\varphi}[h]$ and $\boldsymbol{\Psi}[h]$ defined on the same space vanish on the same set of elements, then $\varphi[h]=\lambda\Psi[h],$ , where $\lambda$ . is a constant.  

11. Show that constants $\scriptstyle{c_{0}}$ and $\pmb{c}_{1}$ can always be chosen satisfying the conditions (7) used to prove Lemma 3, p. 10.  

U. Prove that the square of a differentiable functional is differentiable, and write a formula for its differential (variation).  

13. Prove that if two differentiable functionals defined on the same normed linear space have the same differential at every point of the space, then they differ by a constant.  

14. Analyze the variational problems corresponding to the following func tionals, where in each case $y(0)=0,y(1)=1$ :  

$$
\int_{0}^{1}y^{\prime}d x;\qquad{\mathrm{\boldmath~b)~}}\int_{0}^{1}y y^{\prime}d x;\qquad{\mathrm{\boldmath~c)~}}\int_{0}^{1}x y y^{\prime}d x.
$$  

15. Find the extremals of the following functionals :  

$$
{\begin{array}{r l r l}&{\displaystyle\int_{a}^{b}\left(y^{2}+y^{\prime2}-2y\sin x\right)d x;}&&{\mathrm{~b)~}\displaystyle\int_{a}^{b}{\frac{y^{\prime2}}{x^{3}}}d x;}\\ &{\displaystyle\int_{a}^{b}\left(y^{2}-y^{\prime2}-2y\cosh x\right)d x;}&&{\mathrm{~d)~}\displaystyle\int_{a}^{b}\left(y^{2}+y^{\prime2}+2y e^{x}\right)d x;}\\ &{\displaystyle\int_{a}^{b}\left(y^{2}-y^{\prime2}-2y\sin x\right)d x.}\end{array}}
$$  

Ans. b) $y=C_{1}x^{4}+C_{2};\qquad\mathrm{d}){\mathrm{~}}y=\pm x e^{x}+C_{1}e^{x}+C_{2}e^{-x}.$  

16. Prove the uniqueness part o f Bernstein's theorem (p. 1 6).  

Hint. Let $\Delta(x)=\varphi_{2}(x)-\varphi_{1}(x)$ , where $\varphi_{1}(x)$ and $\varphi_{2}(x)$ are two solutions of ( 1 5), write an expression for $\Delta^{\prime}(x)$ and use the condition $F_{y}(x,y,y^{\prime})>k$ .  

17. Prove that one and only one extremal of each of the functionals  

$$
\int e^{-2y^{2}}(y^{\prime2}-1)d x,\qquad\int(y^{2}+y^{\prime}\tan^{-1}y^{\prime}-\ln\sqrt{1+y^{\prime2}})d x
$$  

passes through any two points of the plane with different abscissas.  

Hint. Apply Bernstein's theorem.  

18. Find the general solution of the Euler equation corresponding to the functional  

$$
J[y]=\int_{a}^{b}f(x){\sqrt{1+y^{\prime2}}}d x,
$$  

and investigate the special cases $f(x)={\sqrt{x}}$ and $f(x)=x$ .  

Comment. The case $f(x)=1/x$ is treated in Example 1 ,  p. 1 9 .  

19. Find all minimal surfaces whose equations have the form $z=\varphi(x)+\psi(y)$ . Ans. $z=A x+B y+C,\qquade^{a(z-z_{0})}=\frac{\cos a(y-y_{0})}{\cos a(x-x_{0})}\cdot$  

20. Which curve minimizes the integral  

$$
\int_{0}^{1}{(\pm y^{\prime}{}^{2}+y y^{\prime}+y^{\prime}+y)d x},
$$  

when the values of $_y$ are not specified at the end points ?  

Ans. $y=\frac{1}{2}(x^{2}-3x+1)$ .  

21. Calculate the variational derivative at the point $\scriptstyle{\pmb{x_{0}}}$ of the quadratic functional  

$$
J[y]=\int_{a}^{b}\int_{a}^{b}K(s,t)y(s)y(t)d s d t.
$$  

22. Find the extremals of the functional  

$$
\int{\sqrt{x^{2}+y^{2}}}{\sqrt{1+y^{\prime2}}}d x.
$$  

Hint. Use polar coordinates.   
Ans. $x^{2}$ cos $\alpha+2x y$ sin $a-y^{2}$ cos $\alpha=\beta,$ where $\alpha$ and $\beta$ are constants.  

# 2  

# FURTHER GENERALIZATIONS  

In this chapter, we consider some further generalizations of the simplest variational problem. These include variational problems in spaces of dimen­ sion greater than two (Sec. 9), problems in parametric form (Sec. 10), problems involving higher derivatives (Sec. 1 1 ), and problems with subsidiary conditions (Sec. 1 2) .  

# 9. The Fixed End Poi nt Problem for $\pmb{n}$ U n known F u n ctions  

Let $F(x,y_{1},...,y_{n},z_{1},...,z_{n})$ be a function with continuous first and second (partial) derivatives with respect to all its arguments. Consider the problem of finding necessary conditions for an extremum of a functional of the form  

$$
J[y_{1},...,y_{n}]=\int_{a}^{b}F(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})d x,
$$  

which depends on $\pmb{n}$ continuously differentiable functions $y_{1}(x),...,y_{n}(x)$ satisfying the boundary conditions  

$$
y_{i}(a)=A_{i},\quad y_{i}(b)=B_{i}\qquad(i=1,...,n).
$$  

In other words, we are looking for an extremum of the functional ( 1 ) defined on the set of the set of smooth curves joining two fixed points in $(n+1)\cdot$ ­ dimensional Euclidean space $\mathcal{E}_{n+1}$ . The problem of finding geodesics, i.e., shortest curves joining two points of some manifold, is of this type. The same kind of problem arises in geometric optics, in finding the paths along which light rays propagate in an inhomogeneous medium. In fact, according to Fermat 's principle, light goes from a point $P_{0}$ to a point $P_{1}$ along the path for which the transit time is the smallest.  

T o find necessary conditions for the functional ( I ) t o have an extremum, we first calculate its variation. Suppose we replace each $y_{i}(x)$ by a " varied " function $y_{i}(x)+h_{i}(x)$ . By the variation $\otimes J$ of the functional $J[y_{1},...,y_{n}]_{:}$ we mean the expression which is linear in $h_{i},h_{i}^{\prime}(i=1,...,n)$ a n d differs from the increment  

$$
\Delta J=J[y_{1}+h_{1},...,y_{n}+h_{n}]-J[y_{1},...,y_{n}]
$$  

by a quantity of order higher than I relative to $h_{i},h_{i}^{\prime}(i=1,...,n)$ . Since both $y_{i}(x)$ and $y_{i}(x)+h_{i}(x)$ satisfy the boundary conditions (2), for each $i$ , it is clear that  

$$
h_{i}(a)=h_{i}(b)=0\qquad(i=1,...,n).
$$  

We now use Taylor's theorem, obtaining  

$$
\begin{array}{l}{{\Delta J=\displaystyle\int_{a}^{b}\left[F(x,...,y_{i}+h_{\mathrm{i}},y_{\mathrm{i}}^{\prime}+h_{\mathrm{i}}^{\prime},...)d x-F(x,...,y_{\mathrm{i}},y_{\mathrm{i}}^{\prime},...)\right]d x}}\\ {{\displaystyle\quad=\displaystyle\int_{a}^{b}\sum_{\mathrm{i}=1}^{n}\left(F_{y_{\mathrm{i}}}h_{\mathrm{i}}+F_{y_{\mathrm{i}}}h_{\mathrm{i}}^{\prime}\right)d x+\cdot\cdot\cdot,}}\end{array}
$$  

where the dots denote terms of order higher than I relative to $h_{i},\ h_{i}^{\prime}$ $(i=1,...,n)$ . The last integral on the right represents the principal linear part of the increment $\Delta J$ , and hence the variation of $J[y_{1},...,y_{n}]$ is  

$$
\displaystyle\mathfrak{d}J=\int_{a}^{b}\sum_{i=1}^{n}\left(F_{y_{i}}h_{i}+F_{y_{i}^{\prime}}h_{i}^{\prime}\right)d x.
$$  

Since all the increments $h_{i}(x)$ are independent, we can choose one of them quite arbitrarily (as long as the boundary conditions are satisfied), setting all the others equal to zero. Therefore, the necessary condition $\ \delta J=0$ for an extremum implies  

$$
\int_{a}^{b}\left(F_{y_{i}}h_{i}+F_{y_{i}}h_{i}^{\prime}\right)d x=0\qquad(i=1,...,n).
$$  

Using Lemma 4 of Sec. 3. 1 ,  we obtain the following system of Euler equations :  

$$
F_{y_{i}}-{\frac{d}{d x}}F_{y_{i}^{'}}=0\qquad(i=1,...,n).
$$  

Since (3) is a system of $\pmb{n}$ second-order differential equations, its general solution contains $2n$ arbitrary constants, which are determined from the boundary conditions (2). Thus, we have proved the following  

THEOREM. $A$ necessary condition for the curve  

$$
y_{i}=y_{i}(x)\qquad(i=1,\ldots,n)
$$  

to be an extremal of the functional  

$$
\int_{a}^{b}F(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})d x
$$  

is that the functions $y_{i}(x)$ satisfy the Euler equations (3).  

Remark 1. We have just shown how to find a well-defined system of Euler equations (3) for every functional of the form ( 1 ). However, two different integrands $F$ can lead to the same set of Euler equations. In fact, let  

$$
\Phi=\Phi(x,y_{1},...,y_{n})
$$  

be any twice differentiable function, and let  

$$
\Psi(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})={\frac{\partial\Phi}{\partial x}}+\sum_{i=1}^{n}{\frac{\partial\Phi}{\partial y_{i}}}y_{i}^{\prime}.
$$  

Then we find at once by direct calculation that  

$$
\frac{\partial}{\partial y_{i}}-\frac{d}{d x}\left(\frac{\partial\Psi}{\partial y_{i}^{\prime}}\right)\equiv0,
$$  

and hence the functionals  

$$
\int_{a}^{b}F(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})d x
$$  

and  

$$
\int_{a}^{b}\left[F(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})+\Psi(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})\right]d x
$$  

lead to the same system of Euler equations.  

Given any curve $y_{i}=y_{i}(x)$ , the function (4) is just the derivative  

$$
{\frac{d}{d x}}\Phi[x,y_{1}(x),...,y_{n}(x)].
$$  

Therefore, the integral  

$$
\int_{a}^{b}\Psi(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})d x=\int_{a}^{b}{\frac{d\Phi}{d x}}d x
$$  

takes the same value along all curves satisfying the boundary conditions (2). In other words, the functionals (5) and (6), defined on the class of functions satisfying (2), differ only by a constant. In particular, we can choose $\Phi$ in such a way that this constant vanishes (but $\Psi\not\equiv0$ ) .  

Remark 2. Two functionals are said to be equivalent if they have the same extremals. According to Remark 1 ,  two functionals of the form ( 1 ) are equivalent i f their integrands differ b y a function o f the form (4). I t is also clear that two functionals of this form are equivalent if their integrands differ by a constant factor $c\neq0$ . More generally, the functional (5) is equivalent to the functional (6) with $F$ replaced by $c F$ .  

Example 1. Propagation of light in an inhomogeneous medium. Suppose that three-dimensional space is filled with an optically inhomogeneous medium , such that the velocity of propagation of light at each point is some function $v(x,y,z)$ of the coordinates of the point. According to Fermat's principle (see p. 34), light goes from one point to another along the curve for which the transit time of the light is the smallest. If the curve j oining two points $A$ and $B$ is specified by the equations  

$$
y=y(x),\qquadz=z(x),
$$  

the time it takes light to traverse the curve equals  

$$
\int_{a}^{b}{\frac{\sqrt{1+y^{\prime2}+z^{\prime2}}}{v(x,y,z)}}d x.
$$  

Writing the system of Euler equations for this functional, i.e.,  

$$
\begin{array}{r}{\frac{\partial v}{\partial y}\frac{\sqrt{1+y^{\prime2}+z^{\prime2}}}{v^{2}}+\frac{d}{d x}\frac{y^{\prime}}{v\sqrt{1+y^{\prime2}+z^{\prime2}}}=0,}\\ {\frac{\partial v}{\partial z}\frac{\sqrt{1+y^{\prime2}+z^{\prime2}}}{v^{2}}+\frac{d}{d x}\frac{z^{\prime}}{v\sqrt{1+y^{\prime2}+z^{\prime2}}}=0,}\end{array}
$$  

we obtain the differential equations for the curves along which the light propagates.  

Example 2. Geodesics. Suppose we have a surface $\pmb{\sigma}$ specifier! by a vector equation  

$$
{\bf r}={\bf r}(u,v).
$$  

The shortest curve lying on $\pmb{\sigma}$ and connecting two points of $\pmb{\sigma}$ is called the geodesic connecting the two points. Clearly, the equations for the geodesics of $\pmb{\sigma}$ are the Euler equations of the corresponding variational problem, i.e., the problem of finding the minimum distance (measured along $\pmb{\sigma}$ ) between two points of $\pmb{\sigma}$ .  

A curve lying on the surface (7) can be specified by the equations  

$$
u=u(t),\qquadv=v(t).
$$  

The arc length between the points corresponding to the values $t_{1}$ and $t_{2}$ of the parameter $t$ equals  

$$
J[u,v]=\int_{t_{0}}^{t_{1}}\sqrt{E u^{\prime2}+2F u^{\prime}v^{\prime}+G v^{\prime2}}d t,
$$  

where $E,~{\boldsymbol{F}}$ and $G$ are the coefficients of the first fundamental (quadratic) form of the surface (7), i.e. ,2  

$$
E={\bf r}_{u}.{\bf r}_{u},\qquadF={\bf r}_{u}.{\bf r}_{v},\qquadG={\bf r}_{v}.{\bf r}_{v}.
$$  

Writing the Euler equations for the functional (8), we obtain  

$$
\begin{array}{r}{\frac{E_{u}u^{\prime2}+2F_{u}u^{\prime}v^{\prime}+G_{u}v^{\prime2}}{\sqrt{E u^{\prime2}+2F u^{\prime}v^{\prime}+G v^{\prime2}}}-\frac{d}{d t}\frac{2(E u^{\prime}+F v^{\prime})}{\sqrt{E u^{\prime2}+2F u^{\prime}v^{\prime}+G v^{\prime2}}}=0,}\\ {\frac{E_{v}u^{\prime2}+2F_{v}u^{\prime}v^{\prime}+G_{v}v^{\prime2}}{\sqrt{E u^{\prime2}+2F u^{\prime}v^{\prime}+G v^{\prime2}}}-\frac{d}{d t}\frac{2(F u^{\prime}+G v^{\prime})}{\sqrt{E u^{\prime2}+2F u^{\prime}v^{\prime}+G v^{\prime2}}}=0.}\end{array}
$$  

As a very simple illustration of these considerations, we now find the geodesics of the circular cylinder  

$$
\boldsymbol{\mathsf{r}}=(a\cos\varphi,a\sin\varphi,z),
$$  

where the variables $\varphi$ and $z$ play the role of the parameters $\pmb{u}$ and $\pmb{v}$ . Since the coefficients of the first fundamental form of the cylinder (9) are  

$$
{\cal E}=a^{2},\qquad{\cal F}=0,\qquad{\cal G}=1,
$$  

the geodesics of the cylinder have the equations  

i.e. ,  

$$
\begin{array}{c}{{\displaystyle{\frac{d}{d t}\frac{a^{2}\varphi^{\prime}}{\sqrt{a^{2}\varphi^{\prime2}+z^{\prime2}}}=0,\frac{d}{d t}\frac{z^{\prime}}{\sqrt{a^{2}\varphi^{\prime2}+z^{\prime2}}}=0,}}}\\ {{\frac{a^{2}\varphi^{\prime}}{\sqrt{a^{2}\varphi^{\prime2}+z^{\prime2}}}=C_{1},\frac{z^{\prime}}{\sqrt{a^{2}\varphi^{\prime2}+z^{\prime2}}}=C_{2}.}}\end{array}
$$  

Dividing the second of these equations by the first, we obtain  

$$
\frac{d z}{d\varphi}=c_{1},
$$  

which has the solution  

$$
z=c_{1}\varphi+c_{2},
$$  

representing a two-parameter family of helical lines lying on the cylinder (9).  

The concept of a geodesic can be defined not only for surfaces, but also for higher-dimensional manifolds. Clearly, finding the geodesics of an $\pmb{n}$ -dimensional manifold reduces to solving a variational problem for a functional depending on $\pmb{n}$ functions.  

# 1 0. Variational P ro b l e m s in Para m et r i c Fo rm  

So far, we have considered functionals ofcurves given by explicit equations, e.g., by equations of the form  

$$
y=y(x)
$$  

in the two-dimensional case. However, it is often more convenient to consider functionals of curves given in parametric form, and in fact we have already encountered this case in Example 2 of the preceding section (involving geodesics on a surface). Moreover, in problems involving closed curves (like the isoperimetric problem mentioned on p. 3), it is usually impossible to get along without representing the curves in parametric form. Thus, in this section, we extend our previous results to the case where the curves are given parametrically, confining ourselves to the simplest variational problem.  

Suppose that in the functional  

$$
\int_{x_{0}}^{x_{1}}F(x,y,y^{\prime})d x,
$$  

we wish t o regard the argument $y$ a s a curve which i s given i n parametric form, rather than in the form ( t o). Then ( 1 1 ) can be written as  

$$
\int_{t_{0}}^{t_{1}}F\left[x(t),y(t),{\frac{{\dot{y}}(t)}{{\dot{x}}(t)}}\right]{\dot{x}}(t)d t=\int_{t_{0}}^{t_{1}}\Phi(x,y,{\dot{x}},{\dot{y}})d t
$$  

(where the overdot denotes differentiation with respect to $t$ ) , i . e . , as a functional depending on two unknown functions $x(t)$ and $y(t)$ . The function $\Phi$ appearing in the right-hand side of ( 1 2) does not involve $t$ explicitly, and is positive-homogeneous of degree $\boldsymbol{{\mathit{1}}}$ in $\dot{x}(t)$ and $\dot{y}(t)$ , which means that  

$$
\Phi(x,y,\lambda\dot{x},\lambda\dot{y})\equiv\lambda\Phi(x,y,\dot{x},\dot{y})
$$  

for every $\lambda>0$ 3  

Conversely, let  

$$
\int_{t_{0}}^{t_{1}}\Phi(x,y,\dot{x},\dot{y})d t
$$  

be a functional whose integrand $\Phi$ does not involve $t$ explicitly and is positive­ homogeneous of degree 1 in $\dot{x}$ and $\dot{y}$ . We now show that the value of such a functional depends only on the curve in the $x y$ -plane defined by the para­ metric equations $x=x(t),\ y=y(t)$ , and not on the functions $x(t),y(t)$ themselves, i.e., that if we go from $t$ to some new parameter $\bar{\boldsymbol{\uptau}}$ by setting  

$$
t=t(\tau),
$$  

where $d t/d\tau>0$ and the interval $[t_{0},t_{1}]$ goes into $[\tau_{0},\tau_{1}],$ , then  

$$
\int_{\tau_{0}}^{\tau_{1}}\Phi\left(x,y,\frac{d x}{d\tau},\frac{d y}{d\tau}\right)d\tau=\int_{t_{0}}^{t_{1}}\Phi(x,y,\dot{x},\dot{y})d t.
$$  

$$
\int_{t_{0}}^{t_{1}}\sqrt{\dot{x}^{2}+\dot{y}^{2}}d t,
$$  

whose value does not depend on the direction in which the curve $x=x(t),y=y(t)$ is traversed, shows why ( 1 3) does not hold for $\lambda<0$ .  

In fact, since $\Phi$ is positive-homogeneous of degree 1 in $\dot{x}$ and $\dot{y}$ , it follows that  

$$
\begin{array}{r l}&{\int_{\tau_{0}}^{\tau_{1}}\Phi\left(x,y,\frac{d x}{d\tau},\frac{d y}{d\tau}\right)d\tau=\int_{\tau_{0}}^{\tau_{1}}\Phi\left(x,y,\dot{x}\frac{d t}{d\tau},\dot{y}\frac{d t}{d\tau}\right)d\tau}\\ &{\qquad=\int_{\tau_{0}}^{\tau_{1}}\Phi(x,y,\dot{x},\dot{y})\frac{d t}{d\tau}d\tau=\int_{t_{0}}^{t_{1}}\Phi(x,y,\dot{x},\dot{y})d t,}\end{array}
$$  

as asserted. Thus, we have proved the following  

THEOREM. $A$ necessary and sufficient condition for the functional  

$$
\int_{t_{0}}^{t_{1}}\Phi(t,x,y,\dot{x},\dot{y})d t
$$  

to depend only on the curve in the xy-plane defined by the parametric equations $x=x(t)$ , $y=y(t)$ and not on the choice of the parametric representation of the curve, is that the integrand $\Phi$ should not involve t explicitly and should be a positive-homogeneous function of degree 1 in $\dot{x}$ and $\dot{y}.$ .  

Now, suppose some parameterization of the curve $y=y(x)$ reduces the functional ( 1 1 ) to the form  

$$
\int_{t_{0}}^{t_{1}}F\left(x,y,{\frac{\dot{y}}{{\dot{x}}}}\right){\dot{x}}d t=\int_{t_{0}}^{t_{1}}\Phi(x,y,{\dot{x}},{\dot{y}})d t.
$$  

The variational problem for the right-hand side of ( 1 4) leads to the pair of Euler equations  

$$
\Phi_{x}-\frac{d}{d t}\Phi_{\dot{x}}=0,\Phi_{y}-\frac{d}{d t}\Phi_{\dot{y}}=0,
$$  

which must be equivalent to the single Euler equation  

$$
F_{y}-\frac{d}{d x}F_{y^{\prime}}=0,
$$  

corresponding to the variational problem for the original functional ( 1 1). Hence, the equations ( 1 5) cannot be independent, and in fact it is easily verified that they are connected by the identity  

$$
\dot{x}\left(\Phi_{x}-\frac{d}{d t}\Phi_{z}\right)+\dot{y}\left(\Phi_{y}-\frac{d}{d t}\Phi_{\dot{y}}\right)=0.
$$  

We shall discuss this point further in Sec. 37.5.  

# I I . F u n ct i o n als Depe n d i ng o n H ig h e r-O rd e r Derivat ives  

So far, we have considered functionals of the form  

$$
\int_{a}^{b}F(x,y,y^{\prime})d x,
$$  

depending on the function $y(x)$ and its first derivative $y^{\prime}(x)$ , or of the more general form  

$$
\int_{a}^{b}F(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})d x,
$$  

depending on several functions $y_{i}(x)$ and their first derivatives $y_{i}^{\prime}(x)$ . How­ ever, many problems (e.g. , in the theory of elasticity) involve functionals whose integrands contain not only $y_{i}(x)$ and $y_{i}^{\prime}(x),$ but also higher-order derivatives $y_{i}^{\prime\prime}(x),y_{i}^{\prime\prime}(x),\ldots$ The method given above for finding extrema of functionals (in the context of necessary conditions for weak extrema) can be carried over to this more general case without essential changes. For sim­ plicity, we confine ourselves to the case of a single unknown function $y(x)$ .  

Thus, let $F(x,y,z_{1},\ldots,z_{n})$ be a function with continuous first and second (partial) derivatives with respect to all its arguments, and consider a functional of the form  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime},...,y^{(n)})d x.
$$  

Then we pose the following problem : Among all functions $y(x)$ belonging to the space ${\mathcal{D}}_{n}(a,b)$ and satisfying the conditions  

$$
\begin{array}{r}{y(a)=A_{0},\ y^{\prime}(a)=A_{1},\ ...,\ y^{(n-1)}(a)=A_{n-1},}\\ {y(b)=B_{0},\ y^{\prime}(b)=B_{1},\ ...,\ y^{(n-1)}(b)=B_{n-1},}\end{array}
$$  

find the function for which ( 1 7) has an extremum. To solve this problem, we start from the general result which states that a necessary condition for a functional $J[y]$ to have an extremum is that its variation vanish (Theorem 2, p. 1 3). Thus, suppose we replace $y(x)$ by the " varied " function $y(x)+h(x)$ , where $h(x),$ like $y(x),$ belongs to ${\mathcal{D}}_{n}(a,b)$ . 4 By the variation $\otimes J$ of the functional $J[y]_{:}$ we mean the expression which is linear in $h,h^{\prime},\ldots,h^{(n)}$ , and which differs from the increment  

$$
\Delta J=J[y+h]-J[y]
$$  

by a quantity of order higher than 1 relative to $h,h^{\prime},....,h^{(n)}$ . Since both $y(x)$ and $y(x)+h(x)$ satisfy the boundary conditions ( 1 8), it is clear that  

$$
\begin{array}{c}{{h(a)=h^{\prime}(a)=\cdot\cdot\cdot=h^{(n-1)}(a)=0,}}\\ {{h(b)=h^{\prime}(b)=\cdot\cdot\cdot=h^{(n-1)}(b)=0.}}\end{array}
$$  

Next, we use Taylor's theorem, obtaining  

$$
\begin{array}{l}{{\Delta J=\displaystyle\int_{a}^{b}\left[F(x,y+h,y^{\prime}+h^{\prime},\ldots,y^{(n)}+h^{(n)})-F(x,y,y^{\prime},\ldots,y^{(n)})\right]d x}}\\ {{\mathrm{}=\displaystyle\int_{a}^{b}\left(F_{y}h+F_{y}{h^{\prime}}+\cdots{F_{y}}^{(n)}h^{(n)}\right)d x+\cdots,}}\end{array}
$$  

where the dots denote terms of order higher than 1 relative to $h,h^{\prime},...,h^{(n)}$ . The last integral on the right represents the principal linear part of the increment $\Delta J$ , and hence the variation of $J[y]$ is  

$$
\delta J=\int_{a}^{b}\left(F_{y}h+F_{y},h^{\prime}+\cdot\cdot\cdot+F_{y^{(n)}}h^{(n)}\right)d x.
$$  

Therefore, the necessary condition $\ \delta J=0$ for an extremum implies that  

$$
\int_{a}^{b}\left(F_{y}h+F_{y},h^{\prime}+\cdot\cdot\cdot+F_{y^{(n)}}h^{(n)}\right)d x=0.
$$  

Repeatedly integrating (20) by parts and using the boundary conditions ( 1 9), we find that  

$$
\int_{a}^{b}\left[F_{y}-{\frac{d}{d x}}F_{y^{\prime}}+{\frac{d^{2}}{d x^{2}}}F_{y^{\prime}}-\cdot\cdot\cdot+(-1)^{n}{\frac{d^{n}}{d x^{n}}}F_{y^{(n)}}\right]h(x)d x=0
$$  

for any function $\pmb{h}$ which has $\pmb{n}$ continuous derivatives and satisfies ( 1 9). It follows from an obvious generalization of Lemma 1 of Sec. 3. 1 that  

$$
F_{y}-{\frac{d}{d x}}F_{y^{\prime}}+{\frac{d^{2}}{d x^{2}}}F_{y^{\prime\prime}}-\cdot\cdot\cdot+(-1)^{n}{\frac{d^{n}}{d x^{n}}}F_{y^{(n)}}=0,
$$  

a result again called Euler's equation. Since (22) is a differential equation of order $2n,$ its general solution contains $2n$ arbitrary constants, which can be determined from the boundary conditions ( 1 8).  

Remark. This derivation of the Euler equation (22) is not completely rigorous, since the transition from (20) to (2 1 ) presupposes the existence of the derivatives  

$$
{\frac{d}{d x}}F_{y^{\prime}},{\frac{d^{2}}{d x^{2}}}F_{y^{\prime}},...,{\frac{d^{n}}{d x^{n}}}F_{y^{(n)}.}
$$  

However, by a somewhat more elaborate argument, it can be shown that (20) implies (22) without this additional hypothesis. In fact, the argument in question proves the existence of the derivatives (23), as in Lemma 4 of Sec. 3 . 1 . 5  

# 1 2. Variat i o n a l P ro ble m s with S u bs i d iary Con d itions  

12.1. The isoperimetric problem. In the simplest variational problem considered in Chapter I ,  the class of admissible curves was specified (apart from certain smoothness requirements) by conditions imposed on the end points of the curves. However, many applications of the calculus of varia­ tions lead to problems in which not only boundary conditions, but also conditions of quite a different type known as subsidiary conditions (synony­ mously, side conditions or constraints) are imposed on the admissible curves. As an example, we first consider the isoperimetric problem,6 which can be stated as follows : Find the curve $y=y(x)$ for which the functional  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x
$$  

has an extremum, where the admissible curves satisfy the boundary conditions  

$$
y(a)=A,\qquady(b)=B,
$$  

and are such that another functional  

$$
K[y]=\int_{a}^{b}G(x,y,y^{\prime})d x
$$  

takes a fixed value I.  

To solve this problem, we assume that the functions $F$ and $G$ defining the functionals (24) and (25) have continuous first and second derivatives in $[a,b]$ for arbitrary values of $y$ and $y^{\prime}$ . Then we have  

THEOREM 1 .7 Given the functional  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x,
$$  

let the admissible curves satisfy the conditions  

$$
y(a)=A,\qquady(b)=B,\qquadK[y]=\int_{a}^{b}G(x,y,y^{\prime})d x=l,
$$  

where $\boldsymbol{K}[\boldsymbol{y}]$ is another functional, and let $J[y]$ have an extremum for $y=y(x)$ . Then, $f y=y(x)$ is not an extremal of $K[y]$ , there exists $\pmb{a}$ constant $\lambda$ such that $y=y(x)$ is an extremal of the functional  

$$
\int_{a}^{b}\left(F+\lambda G\right)d x,
$$  

i.e. , $y=y(x)$ satisfies the difefrential equation  

$$
F_{y}-\frac{d}{d x}F_{y^{\prime}}+\uplambda\left(G_{y}-\frac{d}{d x}G_{y^{\prime}}\right)=0.
$$  

Proof Let $J[y]$ have an extremum for the curve $y=y(x)$ , subject to the conditions (26). We choose two points $x_{1}$ and $x_{2}$ in the interval $[a,b].$ , where $x_{1}$ is arbitrary and $x_{2}$ satisfies a condition to be stated below, but is otherwise arbitrary. Then we give $y(x)$ an increment $\updelta_{1}y(x)$ $+\ \S_{2}y(x)$ , where $\updelta_{1}y(x)$ is nonzero only in a neighborhood of $x_{1},$ 0 and $\updelta_{2}y(x)$ is nonzero only in a neighborhood of $x_{2}$ . (Concerning this notation, see footnote 4, p. 4 1 .) Using variational derivatives, we can write the corresponding increment $\Delta J$ of the functional $J$ in the form  

$$
\Delta J=\left\langle\frac{\8F}{\ \delta y}\right|_{x=z_{1}}+\left.\varepsilon_{1}\right\rangle\Delta\sigma_{1}+\left.\left\langle\frac{\delta F}{\ \delta y}\right|_{x=z_{2}}+\left.\varepsilon_{2}\right\rangle\Delta\sigma_{2},
$$  

where  

$$
\Delta\sigma_{1}=\int_{a}^{b}\updelta_{1}y(x)d x,\quad\quad\Delta\sigma_{2}=\int_{a}^{b}\updelta_{2}y(x)d x
$$  

and e $_1,\varepsilon_{2}\to0$ as $\Delta\upsigma_{1},\Delta\upsigma_{2}\rightarrow0$ (see the Remark on p. 29).  

We now require that the " varied " curve  

$$
y=y^{*}(x)=y(x)+\S_{1}y(x)+\S_{2}y(x)
$$  

satisfy the condition  

$$
K[y^{*}]=K[y].
$$  

Writing $\Delta K$ in a form similar to (28), we obtain  

$$
\begin{array}{r l r}{\lefteqn{\Delta K=K[y^{*}]-K[y]=\left.\left\{\frac{\partial G}{\partial y}\right|_{z=z_{1}}}}\\ &{}&{+\left.\varepsilon_{1}^{\prime}\right\}\Delta\sigma_{1}+\left\{\frac{\partial G}{\partial y}\right|_{z=z_{2}}+\left.\varepsilon_{2}^{\prime}\right\}\Delta\sigma_{2}=0,}\end{array}
$$  

where $\mathfrak{E}_{1}^{'},\mathfrak{E}_{2}^{'}\to0$ as $\Delta\upsigma_{1},\Delta\upsigma_{2}\rightarrow0.$ Next, we choose $\scriptstyle x_{2}$ to be a point for which  

$$
\left.{\frac{\delta G}{\delta y}}\right|_{z=z_{2}}\neq0.
$$  

Such a point exists, since by hypothesis $y=y(x)$ is not an extremal of the functional $K$ . With this choice of $x_{2}$ , we can write the condition (29) in the form  

$$
\Delta\sigma_{2}=-\left\{\frac{\frac{\delta G}{\delta y}\bigg|_{x=x_{1}}}{\frac{\delta G}{\delta y}\bigg|_{x=x_{2}}}+\varepsilon^{\prime}\right\}\Delta\sigma_{1},
$$  

where $\varepsilon^{\prime}\to0$ as $\Delta\sigma_{1}\rightarrow0.$ . Setting  

$$
\lambda=-\frac{\left.\frac{\delta F}{\delta y}\right|_{x=x_{2}}}{\left.\frac{\delta G}{\delta y}\right|_{x=x_{2}}},
$$  

and substituting (30) into the formula (28) for $\Delta J_{;}$ , we obtain  

$$
\Delta J=\left\{\frac{\delta F}{\delta y}\bigg\vert_{z=z_{1}}+\left.\lambda\frac{\delta G}{\delta y}\right\vert_{z=z_{1}}\right\}\Delta\sigma_{1}+\varepsilon\Delta\sigma_{1},
$$  

where $\varepsilon\to0$ as $\Delta\upsigma_{1}\rightarrow0$ . This expression for $\Delta J$ explicitly involves variational derivatives only at $x=x_{1},$ and the increment $h(x)$ is now j ust $\updelta_{1}y(x)$ , since the " compensating increment " $\updelta_{2}y(x)$ has been taken into account automatically by using the condition $\Delta K=0$ . Thus, the first term in the right-hand side of (3 1 ) is the principal linear part of $\Delta J$ , i.e., the variation of the functional $J$ at the point $x_{1}$ is  

$$
\delta J=\left\{\frac{\delta F}{\delta y}\atop{x=x_{1}}}+\lambda\frac{\delta G}{\delta y}\right|_{x=x_{1}}\}\Delta\sigma_{1}.
$$  

Since a necessary condition for an extremum is that $\ \delta J=0$ , and since $\Delta\upsigma_{1}$ is nonzero while $x_{1}$ is arbitrary, we finally have  

$$
\frac{\mathfrak{F}}{\mathfrak{F}y}+\uplambda\frac{\mathfrak{F}}{\mathfrak{F}y}=F_{y}-\frac{d}{d x}F_{y^{\prime}}+\uplambda\left(G_{y}-\frac{d}{d x}G_{y^{\prime}}\right)=0,
$$  

which is precisely equation (27). This completes the proof of the theorem.  

To use Theorem 1 to solve a given isoperimetric problem, we first write the general solution of (27), which will contain two arbitrary constants in addition to the parameter $\lambda$ . We then determine these three quantities from the boundary conditions $y(a)=A$ , $y(b)=B$ and the subsidiary condition $\begin{array}{r}{K[y]=l.}\end{array}$  

Everything j ust said generalizes immediately to the case of functionals depending on several functions $y_{1},...,y_{n}$ and subject to several subsidiary conditions of the form (25). In fact, suppose we are looking for an extremum of the functional  

$$
J[y_{1},...,y_{n}]=\int_{a}^{b}F(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})d x,
$$  

subject to the conditions  

$$
y_{i}(a)=A_{i},y_{i}(b)=B_{i}(i=1,...,n)
$$  

and  

$$
\int_{a}^{b}G_{j}(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})d x=l_{j}\qquad(j=1,...,k).
$$  

In this case a necessary condition for an extremum is that  

$$
\frac{\partial}{\partial y_{i}}\left(F+\sum_{j=1}^{k}\lambda_{j}G_{j}\right)-\frac{d}{d x}\left\{\frac{\partial}{\partial y_{i}^{\prime}}\left(F+\sum_{j=1}^{k}\lambda_{j}G_{j}\right)\right\}=0\quad(i=1,...,n).
$$  

The $2n$ arbitrary constants appearing in the solution of the system (35), and the values of the $k$ parameters $\lambda_{1},...,\lambda_{k},$ sometimes called Lagrange multipliers, are determined from the boundary conditions (33) and the subsidiary conditions (34). The proof of (35) is not essentially different from the proof of Theorem I , and will not be given here.  

12.2. Finite subsidiary conditions. In the isoperimetric problem, the subsidiary conditions which must be satisfied by the functions $y_{1},...,y_{n}$ are of the form (34), i.e., they are specified by functionals. We now consider a problem of a different type, which can be stated as follows : Find the functions $y_{i}(x)$ for which the functional (32) has an extremum, where the admissible functions satisfy the boundary conditions  

$$
y_{i}(a)=A_{i},\quad y_{i}(b)=B_{i}\qquad(i=1,...,n)
$$  

and $k$ "finite " subsidiary conditions $(k<n)$  

$$
g_{j}(x,y_{1},...,y_{n})=0\qquad(j=1,...,k).
$$  

In other words, the functional (32) is not considered for all curves satisfying the boundary conditions (33), but only for those which lie in the $(n-k)$ ­ dimensional manifold defined by the system (36).  

For simplicity, we confine ourselves to the case $n=2,k=1$ .  Then we have  

THEOREM 2. Given the functional  

$$
J[y,z]=\int_{a}^{b}F(x,y,z,y^{\prime},z^{\prime})d x,
$$  

let the admissible curves lie on the surface  

$$
g(x,y,z)=0
$$  

and satisfy the boundary conditions  

$$
\begin{array}{r l}{y(a)=A_{1},}&{{}\quad y(b)=B_{1},}\\ {z(a)=A_{2},}&{{}\quad z(b)=B_{2},}\end{array}
$$  

and moreover, let $J[y]$ have an extremum for the curve  

$$
y=y(x),\qquadz=z(x).
$$  

Then, i ${\pmb g}_{\pmb y}$ and $\scriptstyle{g_{z}}$ do not vanish simultaneously at any point of the surface (38), there exists a function $\uplambda(x)$ such that (40) is an extremal of the functional  

$$
\int_{a}^{b}\left[F+\lambda(x)g\right]d x,
$$  

i.e. , satisfies the difefrential equations  

$$
\begin{array}{l}{{\displaystyle F_{y}+\O\mathrm{\lambda}\mathrm{\lambda}\mathrm{g}_{y}-\frac{d}{d x}\ F_{y^{\prime}}=0\mathrm{,}}}\\ {{\displaystyle F_{z}+\O\mathrm{\lambda}\mathrm{g}_{z}-\frac{d}{d x}\ F_{z^{\prime}}=0.}}\end{array}
$$  

Proof As might be expected, the proof of this theorem closely resembles that of Theorem 1 .  Let $J[y,z]$ have an extremum for the curve (40), subject to the conditions (38) and (39), and let $x_{1}$ be an arbi­ trary point of the interval $[a,b]$ . Then we give $y(x)$ an increment $\updelta y(x)$ and $z(x)$ an increment $\delta z(x)$ where both $\updelta y(x)$ and $\delta z(x)$ are nonzero only in a neighborhood $[\alpha,\beta]$ of $x_{1}$ ' Using variational derivatives, we can write the corresponding increment $\Delta J$ of the functional $J[y,z]$ in the form  

$$
\Delta J=\left\{\frac{\8F}{\delta y}\bigg|_{x=x_{1}}+\varepsilon_{1}\right\}\Delta\sigma_{1}+\left\{\frac{\delta F}{\delta z}\bigg|_{x=x_{1}}+\varepsilon_{2}\right\}\Delta\sigma_{2},
$$  

where  

$$
\Delta\sigma_{1}=\int_{a}^{b}\updelta y(x)d x,\quad\quad\Delta\sigma_{2}=\int_{a}^{b}\updelta z(x)d x,
$$  

and $\mathfrak{s}_{1},\mathfrak{s}_{2}\to0$ as $\Delta\pmb{\sigma}_{1}$ , $\Delta\sigma_{2}\to0$ .  

We now require that the " varied " curve  

$$
y=y^{*}(x)=y(x)+\mathfrak{J}{\mathfrak{J}}(x),\qquadz=z^{*}(x)=z(x)+\mathfrak{J}z(x)
$$  

satisfy the condition 8  

$$
g(x,y^{\ast},z^{\ast})=0.
$$  

In view of (38), this means that  

$$
\begin{array}{l}{0=\displaystyle\int_{a}^{b}\left[g(x,y^{\ast},z^{\ast})-g(x,y,z)\right]d x=\displaystyle\int_{a}^{b}\left(\bar{g}_{y}\S\ y+\bar{g}_{z}\S z\right)d x}\\ {=\displaystyle\left\{g_{y}\big\vert_{x=x_{1}}+\mathfrak{e}_{1}^{\prime}\right\}\Delta\sigma_{1}+\{g_{z}\big\vert_{x=x_{1}}+\mathfrak{e}_{2}^{\prime}\}\Delta\sigma_{2},}\end{array}
$$  

where $\mathfrak{E}_{1}^{\prime},\mathfrak{E}_{2}^{\prime}\to0$ as $\Delta\upsigma_{1}$ h $\Delta\sigma_{2}\to0$ , and the overbar indicates that the corresponding derivatives are evaluated along certain intermediate curves. By hypothesis, either $\left|g_{y}\right|_{x=x_{1}}$ or $\left|g_{z}\right|_{z=x_{1}}$ is nonzero. If $\left.g_{z}\right|_{z=x_{1}}\neq0$ , we can write the condition (43) in the form  

$$
\Delta\sigma_{2}=-\left\lbrace\frac{g_{y}|_{x=x_{1}}}{g_{z}|_{x=x_{1}}}+\mathfrak{e}^{\prime}\right\rbrace\Delta\sigma_{1},
$$  

where $\pmb{\varepsilon}^{\prime}\rightarrow0$ as $\Delta\upsigma_{1}\rightarrow0$ . Substituting (44) into the formula (42) for $\Delta J_{:}$ lJ, we obtain  

$$
\Delta J=\left\{\frac{\updelta F}{\updelta y}\bigg|_{x=x_{1}}-\left(\frac{g_{y}}{g_{z}}\frac{\updelta F}{\updelta z}\right)\bigg|_{x=x_{1}}\right\}\Delta\sigma_{1}+\varepsilon\Delta\sigma_{1},
$$  

where $\mathfrak{s}\to0$ as $\Delta\sigma_{1}\cdots0$ . The first term in the right-hand side is the principal linear part of $\Delta J$ , i.e., the variation of the functional $J$ at the point $x_{1}$ is  

$$
\delta J=\left\langle\frac{\delta F}{\delta y}\right|_{x=x_{1}}-\left.\left(\frac{g_{y}}{g_{z}}\frac{\delta F}{\delta z}\right)\right|_{x=x_{1}}\right\rangle\Delta\sigma_{1}.
$$  

Since a necessary condition for an extremum is that $\ \delta J=0$ , and since $\Delta\sigma_{1}$ is nonzero while $x_{1}$ is arbitrary, we finally have  

$$
\frac{\updelta F}{\updelta y}-\frac{g_{y}}{g_{z}}\frac{\updelta F}{\updelta z}=F_{y}-\frac{d}{d x}F_{y^{\prime}}-\frac{g_{y}}{g_{z}}\left(F_{z}-\frac{d}{d x}F_{z^{\prime}}\right)=0
$$  

or  

$$
{\frac{F_{y}-{\frac{d}{d x}}F_{y^{\prime}}}{g_{y}}}={\frac{F_{z}-{\frac{d}{d x}}F_{z^{\prime}}}{g_{z}}}.
$$  

Along the curve $y=y(x)$ , $z=z(x)$ , the common value of the ratios (45) is some function of $x$ . If we denote this function by $-\lambda(x)$ , then (45) reduces to precisely the system (4 1 ) . This completes the proof of the theorem.  

Remark $\boldsymbol{{\mathit{1}}}$ . We note without proof that Theorem 2 remains valid when the class of admissible curves consists of smooth space curves satisfying the differential equation 9  

$$
g(x,y,z,y^{\prime},z^{\prime})=0.
$$  

More precisely, if the functional $J$ has an extremum for a curve $\upgamma$ , subject to the condition (46), and if the derivatives $g_{y^{\prime}},\ g_{z^{\prime}}$ do not vanish simul­ taneously along $\upgamma$ , then there exists a function $\uplambda(x)$ such that $\upgamma$ is an integral curve of the system  

$$
\Phi_{y}-\frac{d}{d x}\Phi_{y^{\prime}}=0,\Phi_{z}-\frac{d}{d x}\Phi_{z^{\prime}}=0,
$$  

where  

$$
\Phi=F+\lambda G.
$$  

Remark 2. In a certain sense, we can consider a variational problem with a finite subsidiary condition to be a limiting case of an isoperimetric problem. In fact, if we assume that the condition (38) does not hold everywhere, but only at some fixed point  

$$
g(x_{1},y,z)=0,
$$  

we obtain a condition whose left-hand side can be regarded as a functional of $y$ and $z$ , i.e., a condition of the type appearing in the isoperimetric problem.  

Thus, the condition (38) can be regarded as an infinite set of conditions, each of which is a functional. As we have seen, in the isoperimetric problem the number of Lagrange multipliers $\lambda_{1},...,\lambda_{k}$ equals the number of con­ ditions of constraint., In the same way, the function $\uplambda(x)$ appearing in the problem with a finite subsidiary condition can be interpreted as a " Lagrange multiplier for each point $x$ . "  

Example 1. Among all curves of length $\iota$ in the upper hal-fplane passing through the points $(-a,0)$ and $(a,0).$ , find the one which together with the interval $[-a,a]$ encloses the largest area. We are looking for the function $y=y(x)$ for which the integral  

$$
J[y]=\int_{-a}^{a}y d x
$$  

takes the largest value subject to the conditions  

$$
y(-a)=y(a)=0,\qquadK[y]=\int_{-a}^{a}{\sqrt{1+y^{\prime}^{2}}}d x=l.
$$  

Thus, we are dealing with an isoperimetric problem. Using Theorem 1 , we form the functional  

$$
J[y]+\lambda K[y]=\int_{-a}^{a}\left(y+\lambda\sqrt{1+y^{\prime2}}\right)d x,
$$  

and write the corresponding Euler equation  

$$
1+\lambda\frac{d}{d x}\frac{y^{\prime}}{\sqrt{1+y^{\prime2}}}=0,
$$  

which implies  

$$
x+\lambda\frac{y^{\prime}}{\sqrt{1+y^{\prime2}}}=C_{1}.
$$  

Integrating (47), we obtain the equation  

$$
(x-C_{1})^{2}+(y-C_{2})^{2}=\lambda^{2}
$$  

of a family of circles. The values of $C_{1},C_{2}$ and $\lambda$ are then determined from the conditions  

$$
y(-a)=y(a)=0,\qquadK[y]=l.
$$  

Example 2. Among all curves lying on the sphere $x^{2}+y^{2}+z^{2}=a^{2}$ and passing through two given points $(x_{0},y_{0},z_{0})$ and $(x_{1},y_{1},z_{1})$ , find the one which has the least length. The length of the curve $y=y(x)$ , $z=z(x)$ is given by the integral  

$$
\int_{x_{0}}^{z_{1}}{\sqrt{1+y^{\prime}^{2}+z^{\prime2}}}d x.
$$  

Using Theorem 2, we form the auxiliary functional  

$$
\int_{x_{0}}^{z_{1}}{[\sqrt{1+y^{\prime}{}^{2}+z^{\prime}{}^{2}}+\lambda(x)(x^{2}+y^{2}+z^{2})]d x},
$$  

and write the corresponding Euler equations  

$$
\begin{array}{l}{\displaystyle2y\lambda(\boldsymbol{x})-\frac{d}{d x}\frac{y^{\prime}}{\sqrt{1+y^{\prime}{}^{2}+z^{\prime}{}^{2}}}=0,}\\ {\displaystyle2z\lambda(\boldsymbol{x})-\frac{d}{d x}\frac{z^{\prime}}{\sqrt{1+y^{\prime}{}^{2}+z^{\prime}{}^{2}}}=0.}\end{array}
$$  

Solving these equations, we obtain a family of curves depending on four constants, whose values are determined from the boundary conditions  

$$
\begin{array}{r l}{y(x_{0})=y_{0},\quad}&{{}y(x_{1})=y_{1},}\\ {z(x_{0})=z_{0},\quad}&{{}z(x_{1})=z_{1}.}\end{array}
$$  

Remark. As is familiar from elementary analysis, in finding an extremum of a function of $\pmb{n}$ variables subject to $k$ constraints $(k<n)$ , we can use the constraints to express $k$ variables in terms of the other $n-k$ variables. In this way, the problem is reduced to that of finding an unconstrained extremum of a function of $n-k$ variables, i.e., an extremum subject to no subsidiary conditions. The situation is the same in the calculus of variations. For example, the problem of finding geodesics on a given surface can be regarded as a problem subject to a constraint, as in Example 2 of this section. On the other hand, if we express the coordinates $x,y$ and $z$ as functions of two parameters, we can reduce the problem to that of finding an unconstrained extremum, as in Example 2 of Sec. 9.  

# PROBLEMS  

1. Find the extremals of the functional  

$$
J[y,z]=\int_{0}^{\pi/2}\left(y^{\prime2}+z^{\prime2}+2y z\right)d x,
$$  

subject to the boundary conditions  

$$
y(0)=0,\qquady(\pi/2)=1,\qquadz(0)=0,\qquadz(\pi/2)=1.
$$  

2. Find the extremals of the fixed end point problems corresponding to the following functionals :  

$$
\begin{array}{l}{\displaystyle\int_{x_{0}}^{z_{1}}\left(y^{\prime2}+z^{\prime2}+y^{\prime}z^{\prime}\right)d x;}\\ {\displaystyle\int_{x_{0}}^{z_{1}}\left(2y z-2y^{2}+y^{\prime2}-z^{\prime2}\right)d x.}\end{array}
$$  

3. Find the extremals of a functional of the form  

$$
\int_{x_{0}}^{x_{1}}F(y^{\prime},z^{\prime})d x,
$$  

given that $F_{y^{\prime}y^{\prime}}F_{z^{\prime}z^{\prime}}-(F_{y^{\prime}z^{\prime}})^{2}\ne0$ for $x_{0}\leqslant x\leqslant x_{1}$ '  

Ans. A family of straight lines in three dimensions.  

4. State and prove the generalization of Theorem 3 of Sec. 4. 1 for functionals of the form  

$$
\int_{a}^{b}F(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})d x.
$$  

Hint. The condition $F_{y^{\prime}y^{\prime}}\neq0$ is replaced by the condition det $\|\pmb{F_{y}}_{i y_{k}^{\prime}}\|\neq0$ .  

5. What is the condition for a functional of the form  

$$
\int_{t_{0}}^{t_{1}}F(t,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})d t,
$$  

depending on an $\pmb{n}$ -dimensional curve $y_{\ell}=y_{\ell}(x),i=1,...,n,$ to be independent of the parameterization ?  

6. Generalizing the definition of Sec. 10, we say that the function $f(x_{1},\ldots,x_{n})$ is positive-homogeneous of degree $\pmb{k}$ in $x_{1},...,x_{n}$ if  

$$
f(\lambda x_{1}....,\lambda x_{n})\equiv\lambda^{k}f(x_{1},...,x_{n})
$$  

for every $\lambda>0$ . Prove the following result, known as Euler's theorem : If $f(x_{1},...,x_{n})$ is continuously differentiable and positive-homogeneous of degree $k,$ then  

$$
\sum_{i=1}^{n}{\frac{\partial f}{\partial x_{i}}}x_{i}=k f.
$$  

7. State and prove the converse of Euler's theorem.  

8. Verify formula ( 1 6) of Sec. ( 1 0). Hint. Use Euler's theorem.  

9. Prove that the Euler equations (15) of the variational problem in para­ metric form can be written as  

$$
\Phi_{z\dot{y}}-\Phi_{\dot{z}y}+(\dot{x}\ddot{y}-\ddot{x}\dot{y})\Phi_{1}=0,
$$  

where ${\Phi}_{1}$ is a positive-homogeneous function of degree $-3$ satisfying the relations  

$$
\Phi_{t t}=\dot{y}^{2}\Phi_{1},\qquad\Phi_{t\dot{y}}=-\dot{x}\dot{y}\Phi_{1},\qquad\Phi_{\dot{y}\dot{y}}=\dot{x}^{2}\Phi_{1}.
$$  

Comment. Equation (a) is known as Weierstrass' form of the Euler equations. It can also be written as  

$$
\frac{1}{\rho}=\frac{\Phi\mathrm{~~-~}\Phi_{z\dot{y}}}{\Phi_{1}(\dot{x}^{2}+\dot{y}^{2})^{3/2}},
$$  

where $p$ is the radius of curvature of the extremal.  

10. Prove that Weierstrass' form of the Euler equations is invariant under parameter changes $t=t(\tau),d t/d\tau>0$ .  

11. Find the extremals of the functional  

$$
J[y]=\int_{0}^{1}\left(1+y^{\prime\prime2}\right)d x,
$$  

subject to the boundary conditions  

$$
y(0)=0,\qquady^{\prime}(0)=1,\qquady(1)=1,\qquady^{\prime}(1)=1.
$$  

12. Find the extremals of the functional  

$$
J[y]=\int_{0}^{\pi/2}\left(y^{\prime\prime2}-y^{2}+x^{2}\right)d x,
$$  

subject to the boundary conditions  

$$
y(0)=1,\qquady^{\prime}(0)=0,\qquady(\pi/2)=0,\qquady^{\prime}(\pi/2)=1.
$$  

13. Show that the Euler equation of the functional  

$$
\int_{x_{0}}^{x_{1}}F(x,y,y^{\prime},y^{\prime\prime})d x
$$  

has the first integral  

$$
F_{y^{\prime}}-\frac{d}{d x}F_{y^{\prime\prime}}=\mathrm{const}
$$  

if the integrand does not depend o n $_y$ , and the first integral  

$$
F-y^{\prime}\Big(F_{y^{\prime}}-\frac{d}{d x}F_{y^{\prime\prime}}\Big)-y^{\prime\prime}F_{y^{\prime\prime}}=\mathrm{const}
$$  

if the integrand does not depend on $\pmb{x}$ .  

14. Find the curve j oining the points (0, 0) and ( 1 , 0) for which the integral  

$$
\int_{0}^{1}y^{\prime\prime}{}^{2}d x
$$  

is a minimum if  

a) $y^{\prime}(0)=a,y^{\prime}(1)=b $ ;   
b) N o  other conditions are prescribed.  

15. Supply the details of the argument mentioned in the remark on p. 42.  

16. By direct calculation, without recourse to variational methods, prove that the isosceles triangle has the greatest area among all triangles with a given bllse line and a given perimeter.  

Hint. All the triangles in question have the given base line and a vertex lying on a certain ellipse.  

17. Find the equilibrium position of a heavy flexible inextensible cord of length I, fastened at its ends.  

Hint. Minimize the ordinate of the center of gravity of the cord. By making a suitable change of variables, reduce the problem to Example 2 of Sec. 4.2.  

18. Find the extremals of the functional  

$$
J[y]=\int_{0}^{1}\left(y^{\prime2}+x^{2}\right)d x,
$$  

subject to the conditions  

$$
y(0)=0,\qquady(1)=0,\qquad\int_{0}^{1}y^{2}d x=2.
$$  

19. Suppose an airplane with fixed air speed $\scriptstyle v_{0}$ makes a flight lasting $T$ seconds. Along what closed curve should it fly if this curve is to enclose the greatest area ? It is assumed that the wind velocity has constant direction and magnitude $\textbf{\em a}<\ v_{0}$ .  

Ans. An ellipse whose major axis is perpendicular to the wind velocity and whose eccentricity is ${\pmb a}/v_{0}$ . The velocity of the airplane is perpendicular to the radius vector of the ellipse.  

20. Given two points $\pmb{A}$ and $\pmb{B}$ in the $x y$ -plane, let $\upgamma$ be a fixed curve joining them. Among all curves of length $\iota$ j oining $\pmb{A}$ and $\pmb{B}$ , find the curve which together with $\upgamma$ encloses the greatest area.  

21. Generalizing the preceding problem, suppose the $x y$ -plane is covered by a mass distribution with continuous density $\upmu(x,y)$ . As before, let $\pmb{A}$ and $\pmb{B}$ be two points in the plane, and let $\upgamma$ be a fixed curve joining them. Among all curves of length $\iota$ j oining $\pmb{A}$ and $\pmb{B}$ , find the curve which together with $\upgamma$ bounds the region of greatest mass.  

Hint. Introduce the auxiliary function $V(x,y)=\textstyle\int\mu(x,y)d x$ . Then use Green's theorem and Weierstrass' form of the Euler equations.  

22. Among all curves joining a given point $(0,b)$ on the $_y$ -axis to a point on the $x$ -axis and enclosing a given area $s$ together with the $x$ -axis, find the curve which generates the least area when rotated about the $x$ -axis.  

Ans. The line  

$$
\frac{x}{a}+\frac{y}{b}=1,
$$  

where $a b=2S$ .  

3  

# THE GENERAL V ARIA TION OF A FUN CTIONAL  

# 1 3. De rivat i o n o f t h e Bas i c Fo rm u l a  

In this section, we derive the general formula for the variation of a functional of the form  

$$
J[y_{1},...,y_{n}]=\int_{x_{0}}^{x_{1}}F(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})d x,
$$  

beginning with the case where ( 1 ) depends on a single function $y$ and hence reduces to  

$$
J[y]=\int_{x_{0}}^{x_{1}}F(x,y,y^{\prime})d x.
$$  

We assume that all admissible curves are smooth, but, departing from our previous hypothesis, we assume that the end points of the curves for which (2) is defined can move in an arbitrary way. By the distance between two curves $y=y(x)$ and $y=y^{*}(x)$ is meant the quantity  

$$
\wp(y,y^{*})=\operatorname*{max}|y-y^{*}|+\operatorname*{max}|y^{\prime}-y^{*\prime}|+\wp(P_{0},P_{0}^{*})+\wp(P_{1},P_{1}^{*}),
$$  

where $P_{0},\ P_{0}^{*}$ denote the left-hand end points of the curves $y=y(x),$ . $y=y^{*}(x)$ , respectively, and $P_{1},\ P_{1}^{*}$ denote their right-hand end points. In general, the functions $y$ and $y^{\star}$ are defined on different intervals $\boldsymbol{\mathit{I}}$ and $I^{*}$ . Thus, in order for (3) to make sense, we have to extend $y$ and $y^{*}$ onto some interval containing both $I$ and $I^{*}$ . For example, this can be done by drawing tangents to the curves at their end points, as shown in Figure 4.  

Now let $y=y(x)$ and $y=y^{*}(x)$ be two neighboring curves, in the sense of the dis tance (3), and let 2  

$$
h(x)=y^{*}(x)-y(x).
$$  

Moreover, let  

$$
P_{0}=(x_{0},y_{0}),\qquadP_{1}=(x_{1},y_{1})
$$  

denote the end points of the curve $y=y(x)$ , while the end points of the curve $y=y^{*}(x)=y(x)+h(x)$ are denoted by  

$$
P_{0}^{*}=(x_{0}+\8x_{0},y_{0}+\ \S y_{0}),\qquadP_{1}^{*}=(x_{1}+\8x_{1},y_{1}+\delta y_{1}).
$$  

![](https://cdn-mineru.openxlab.org.cn/extract/c29daec4-3bde-4c07-a565-58de41e65c3b/3a525d19996cb4ff6800b49fb5015dc0cc4b13480484472fb0d1458a806a2054.jpg)  
FIGURE 4  

The corresponding variation $\otimes J$ of the functional $J[y]$ is defined as the expression which is linear in $h,h^{\prime},\updelta x_{0},\updelta y_{0},\updelta x_{1},\updelta y_{1}$ > and which differs from the increment  

$$
\Delta J=J[y+h]-J[y]
$$  

by a quantity of order higher than 1 relative to $\uprho(y,y+h)$ . Since 3  

$$
\begin{array}{l}{\displaystyle\Delta J=\int_{z_{0}+\delta z_{1}}^{z_{1}+\delta z_{1}}F(x,y+h,y^{\prime}+h^{\prime})d x-\int_{z_{0}}^{z_{1}}F(x,y,y^{\prime})d x}\\ {=\displaystyle\int_{z_{0}}^{z_{1}}\left[F(x,y+h,y^{\prime}+h^{\prime})-F(x,y,y^{\prime})\right]d x}\\ {+\displaystyle\int_{x_{1}}^{z_{1}+\delta z_{1}}F(x,y+h,y^{\prime}+h^{\prime})d x-\displaystyle\int_{z_{0}}^{z_{0}+\delta z_{0}}F(x,y+h,y^{\prime}+h^{\prime})d x}\end{array}
$$  

it follows by using Taylor's theorem and letting the symbol $\sim$ denote equality except for terms of order higher than 1 relative to $\mathsf{\rho}\mathsf{\left(y,\boldsymbol{y}+\boldsymbol{h}\right)}$ that  

$$
\begin{array}{l}{\displaystyle\Delta J\sim\int_{x_{0}}^{x_{1}}\left[F_{y}(x,y,y^{\prime})h+F_{y},(x,y,y^{\prime})h^{\prime}\right]d x}\\ {\displaystyle+\left.F(x,y,y^{\prime})\right|_{x=x_{1}}\delta x_{1}-\left.F(x,y,y^{\prime})\right|_{x=x_{0}}\delta x_{0}}\\ {\displaystyle=\int_{x_{0}}^{x_{1}}\left[F_{y}-\frac{d}{d x}F_{y^{\prime}}\right]\left.h(x)d x+\left.F\right|_{x=x_{1}}\delta x_{1}+\left.F_{y}{\cdot}h\right|_{x=x_{1}}}\\ {\displaystyle-\left.F\right|_{x=x_{0}}\delta x_{0}-\left.F_{y}{\cdot}h\right|_{x=x_{0}},}\end{array}
$$  

where the term containing $\pmb{h}^{\prime}$ has been integrated by parts. However, it is clear from Figure 4 that  

$$
\begin{array}{r}{h(x_{0})\sim\updelta y_{0}-y^{\prime}(x_{0})\updelta x_{0},}\\ {h(x_{1})\sim\updelta y_{1}-y^{\prime}(x_{1})\updelta x_{1},}\end{array}
$$  

where $\sim$ , has the same meaning as before, and hence  

$$
\begin{array}{c}{{\displaystyle\left\{\begin{array}{l}{{\delta J=\int_{x_{0}}^{x_{1}}\left[F_{y}-\frac{d}{d x}F_{y^{\prime}}\right]h(x)d x+F_{y^{\prime}}|_{x=x_{1}}\mathrm{~}\delta y_{1}+(F-F_{y^{\prime}}y^{\prime})|_{x=x_{1}}\mathrm{~}\delta x_{1}}}\\ {{-F_{y^{\prime}}|_{x=x_{0}}\mathrm{~}\delta y_{0}-(F-F_{y^{\prime}}y^{\prime})|_{x=x_{0}}\mathrm{~}\delta x_{0},}}\end{array}\right.}}\end{array}
$$  

or more concisely,  

$$
\left.\left.\left\{J=\int_{z_{0}}^{z_{1}}\left[F_{y}-\frac{d}{d x}F_{y}\right]h(x)d x+F_{y^{\prime}}\delta y\right|_{x=x_{0}}^{x=z_{1}}+(F-F_{y^{\prime}}y^{\prime})\delta x\right|_{x=x_{0}}^{z=z_{1}},
$$  

where we define  

$$
\left.\S x\right|_{x=x_{i}}=\left.\S x_{i},\quad\S y\right|_{x=x_{i}}=\left.\S y_{i}\right(\quad i=0,1).
$$  

This is the basic formula for the general variation of the functional $J[y]$ . If the end points of the admissible curves are constrained to lie on the straight lines $x=x_{0},x=x_{1},$ > as in the simple variable end point problem considered in Sec. 6, then $\updelta x_{0}=\updelta x_{1}=0$ , while, in the case of the fixed end point problem, $\updelta x_{0}=\updelta x_{1}=0$ and $\updelta y_{0}=\updelta y_{1}=0$ .  

Next, we return to the more general functional (1), which depends on $\pmb{n}$ functions $y_{1},...,y_{n}$ . Since any system of $\pmb{n}$ functions can be interpreted as a curve in $(n+1)$ -dimensional Euclidean space $\boldsymbol{\mathcal{E}}_{n+1}$ > we can regard (1) as defined on some set of curves in $\boldsymbol{\mathcal{E}}_{n+1}$ . Paralleling the treatment just given for $n=1$ ,  we now calculate the variation of the functional ( 1 ) when there are no restrictions on the end points of the admissible curves. As before, we write  

$$
h_{i}(x)=y_{i}^{*}(x)-y_{i}(x)\qquad(i=1,...,n),
$$  

where for each $i,$ , the function $y_{i}^{*}(x)$ is close to $y_{i}(x)$ in the sense of the distance (3). Moreover, we let  

$$
P_{0}=(x_{0},y_{1}^{0},...,y_{n}^{0}),\qquadP_{1}=(x_{1},y_{1}^{1},...,y_{n}^{1})
$$  

denote the end points of the curve $y_{i}=y_{i}(x),i=1,...,n,$ while the end points of the curve $y_{i}=y_{i}^{*}(x)=y_{i}(x)+h_{i}(x),i=1,...,n,$ are denoted by  

$$
\begin{array}{r}{P_{0}^{*}=(x_{0}+8x_{0},y_{1}^{0}+8y_{1}^{0},...,y_{n}^{0}+8y_{n}^{0}),}\\ {P_{1}^{*}=(x_{1}+8x_{1},y_{1}^{1}+8y_{1}^{1},...,y_{n}^{1}+8y_{n}^{1}),}\end{array}
$$  

and once more, we extend the functions $y_{i}(x)$ and $y_{i}^{*}(x)$ linearly onto the interval $[x_{0},x_{1}+\updelta x_{1}]$ . The corresponding variation $\delta J$ of the functional $J[y_{1},\ldots,y_{n}]$ is defined as the expression which is linear in $\updelta x_{0},\updelta x_{1}$ and all  

the quantities $h_{i},h_{i}^{\prime},\updelta y_{i}^{0},\updelta y_{i}^{1}(i=1,...,n)$ , and which differs from the increment  

$$
\Delta J=J[y_{1}+h_{1},...,y_{n}+h_{n}]-J[y_{1},...,y_{n}]
$$  

by a quantity of order higher than 1 relative to  

Since  

$$
\uprho(y_{1},y_{1}^{*})+{\bf\nabla}\cdot{\bf\nabla}\cdot{\bf\nabla}+\uprho(y_{n},y_{n}^{*}).
$$  

$$
\begin{array}{l}{\Delta J=\displaystyle\int_{z_{0}+\delta z_{0}}^{z_{1}+\delta z_{1}}F(x,...,y_{i}+h_{i},y_{i}^{\prime}+h_{i}^{\prime},...)d x-\displaystyle\int_{z_{0}}^{z_{1}}F(x,...,y_{i},y_{i}^{\prime},...)d}\\ {=\displaystyle\int_{z_{0}}^{z_{1}}\left[F(x,...,y_{i}+h_{i},y_{i}^{\prime}+h_{i}^{\prime},...)-F(x,...,y_{i},y_{i}^{\prime},...)\right]d x}\\ {+\displaystyle\int_{z_{1}}^{z_{1}+\delta z_{1}}F(x,...,y_{i}+h_{i},y_{i}^{\prime}+h_{i}^{\prime},...)}\\ {-\displaystyle\int_{z_{0}}^{z_{0}+\delta z_{0}}F(x,...,y_{i}+h_{i},y_{i}^{\prime}+h_{i}^{\prime},...)d x,}\end{array}
$$  

it follows by using Taylor's theorem and letting the symbol $\sim$ denote equality except for terms of order higher than 1 relative to the quantity (6) that  

$$
\begin{array}{l}{{\displaystyle\Delta J\sim\int_{z_{0}}^{z_{1}}\sum_{i=1}^{n}\left(F_{y_{i}}h_{i}+F_{y_{i}}h_{i}^{\prime}\right)d x+F|_{x=x_{1}}\left.\delta x_{1}-F\right|_{x=x_{0}}\left.\delta x_{0}\right.}}\\ {{\displaystyle\qquad=\int_{z_{0}}^{z_{1}}\sum_{i=1}^{n}\left.\left(F_{y_{i}}-\frac{d}{d x}F_{y_{i}}\right)h_{i}(x)d x+F|_{x=x_{1}}\left.\delta x_{1}+\sum_{i=1}^{n}F_{y_{i}}h_{i}\right|_{x=x_{1}}}}\\ {{\displaystyle\qquad-\left.F|_{x=x_{0}}\left.\delta x_{0}-\sum_{i=1}^{n}F_{y_{i}}h_{i}\right|_{x=x_{0}}},}\end{array}
$$  

where the terms containing $\pmb{h}_{i}^{\prime}$ have been integrated b y parts. Just as in the case $n=1$ ,  we have  

$$
\begin{array}{r}{h_{i}(x_{0})\sim\delta y_{i}^{0}-y_{i}^{\prime}(x_{0})\updelta x_{0},}\\ {h_{i}(x_{1})\sim\updelta y_{i}^{1}-y_{i}^{\prime}(x_{1})\updelta x_{1},}\end{array}
$$  

and hence  

$$
\begin{array}{l}{\displaystyle\vartheta J=\int_{z_{0}}^{z_{1}}\sum_{i=1}^{n}\left(F_{y_{i}}-\frac{d}{d x}F_{y_{i}}\right)h_{i}(x)d x}\\ {\displaystyle\quad+\sum_{i=1}^{n}\left.F_{y_{i}}\right|_{z=z_{1}}\left.\vartheta y_{i}^{1}+\left(F-\sum_{i=1}^{n}y_{i}^{\prime}F_{y_{i}}\right)\right|_{z=z_{1}}\left.\vartheta x_{1}\right.}\\ {\displaystyle\quad-\left.\sum_{i=1}^{n}F_{y_{i}}\right|_{z=z_{0}}\left.\vartheta y_{i}^{0}-\left(F-\sum_{i=1}^{n}y_{i}^{\prime}F_{y_{i}}\right)\right|_{z=z_{0}}\left.\vartheta x_{0},}\end{array}
$$  

or more concisely,  

$$
\begin{array}{r l}{\displaystyle}&{\displaystyle\mathfrak{J}J=\int_{x_{0}}^{x_{1}}\sum_{i=1}^{n}\left(F_{y_{i}}-\frac{d}{d x}F_{y_{i}}\right)h_{i}(x)d x}\\ {\displaystyle}&{\phantom{\displaystyle}+\left.\sum_{i=1}^{n}F_{y_{i}^{'}}\mathfrak{J}y_{i}\right|_{x=x_{0}}^{x=x_{1}}+\left(F-\sum_{i=1}^{n}y_{i}^{'}F_{y_{i}^{'}}\right)\mathfrak{J}x\left|_{x=x_{0}}^{x=x_{1}},}\end{array}
$$  

where, as before, we define  

$$
\left.{\hat{\delta}}x\right|_{x=x_{j}}=\left.{\hat{\delta}}x_{j},\quad{\hat{\delta}}y_{i}\right|_{x=x_{j}}=\left.{\hat{\delta}}y_{i}^{j}\right.\qquad(j=0,1).
$$  

This is the basic formula for the general variation of the functional $J[y_{1},\ldots,y_{n}]$ .  

We now write an even more concise formula for the variation (7), at the same time introducing some important new ideas, to be discussed in more detail in the next chapter. Let  

$$
p_{\mathfrak{i}}=F_{y_{\mathfrak{i}}^{\prime}}\qquad(i=1,\ldots,n),
$$  

and suppose that the Jacobian  

$$
\frac{\partial(p_{1},...,p_{n})}{\partial(y_{1}^{\prime},...,y_{n}^{\prime})}=\operatorname*{det}\|F_{y_{1}^{\prime}y_{k}^{\prime}}\|
$$  

is nonzero.4 Then we can solve the equations (8) for $y_{1}^{\prime},...,y_{n}^{\prime}$ as functions of the variables  

$$
x,y_{1},...,y_{n},p_{1},...,p_{n}.
$$  

Next, we express the function $F(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})$ appearing in ( I ) in terms o f a new function $H(x,y_{1},...,y_{n},p_{1},...,p_{n})$ related t o $F$ b y the formula  

$$
H=-F+\sum_{i=1}^{n}y_{i}^{\prime}F_{y_{i}^{'}}\equiv-F+\sum_{i=1}^{n}y_{i}^{\prime}p_{i},
$$  

where the $y_{i}^{\prime}$ are regarded as functions of the variables (9). The function $H$ is called the Hamiltonian (function) corresponding to the functional $J[y_{1},...,y_{n}]$ . In this way, we can make a local transformation (see footnote 2, p. 68) from the " variables " $x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime},F$ appearing in ( I ) t o the new quantities $x$ , $y_{1},...,y_{n},p_{1},...,p_{n},H,$ , called the canonical variables (corresponding to the functional $J[y_{1},...,y_{n}])$ . In terms of the can­ onical variables, we can write (7) in the form  

$$
\mathfrak{F}J=\int_{x_{0}}^{x_{1}}\sum_{i=1}^{n}\left(F_{y_{i}}-\frac{d p_{i}}{d x}\right)h_{\mathrm{i}}(x)d x+\left(\sum_{i=1}^{n}p_{\mathrm{i}}\vartheta y_{\mathrm{i}}-H\vartheta x\right)\bigg|_{x=x_{0}}^{x=x_{1}}.
$$  

Remark. Suppose the functional $J[y_{1},\ldots,y_{n}]$ has an extremum (in a certain class of admissible curves) for some curve  

$$
y_{i}=y_{i}(x)\qquad(i=1,...,n)
$$  

joining the points  

$$
P_{0}=(x_{0},y_{1}^{0},...,y_{n}^{0}),\qquadP_{1}=(x_{1},y_{1}^{1},...,y_{n}^{1}).
$$  

Then, since $J[y_{1},\ldots,y_{n}]$ has an extremum for ( 1 0) compared to all admissible curves, it certainly has an extremum for ( 1 0) compared to all curves with fixed end points $P_{0}$ and $P_{1}$ . Therefore, ( 1 0) is an extremal, i.e. , a solution of the Euler equations  

$$
F_{y_{i}}-{\frac{d}{d x}}F_{y_{i}^{'}}=0\qquad(i=1,...,n),
$$  

so that the integral in (7) vanishes, and we are left with the formula  

$$
\delta J=\bigg[\sum_{i=1}^{n}F_{y_{i}^{\prime}}\delta y_{i}+\bigg(F-\sum_{i=1}^{n}y_{i}^{\prime}F_{y_{i}^{\prime}}\bigg)\delta x\bigg]\bigg|_{x=x_{0}}^{x=x_{1}},
$$  

or in canonical variables  

$$
\updelta J=\bigg(\sum_{i=1}^{n}p_{i}\updelta y_{i}-H\updelta x\bigg)\bigg|_{x=x_{0}}^{x=x_{1}}.
$$  

Thus, regardless of the boundary conditions defining our variable end point problem, the curve for which $J[y_{1},....,y_{n}]$ has an extremum must first be an extremal and then satisfy the condition that ( 1 1 ) or ( 1 2) vanish (see Problem 1 ,  p. 63).  

# 1 4. E n d Poi nts Lyi ng on Two G iven C u rves or S u rfaces  

The first two chapters of this book have been devoted mainly to fixed end point problems, where the boundary conditions require that all admissible curves have two given end points. The only exception is the simple variable end point problem considered in Sec. 6, where the end points of the admissible curves are free to move along two fixed straight lines parallel to the $y$ -axis. We now consider a more general variable end point problem. To keep matters simple, we start with the case where there is only one unknown function. Our problem can be stated as follows : Among all smooth curves whose end points $\scriptstyle P_{0}$ and ${\pmb P}_{1}$ lie on two given curves $y=\varphi(x)$ and $y=\Psi(x)$ , find the curve for which the functional  

$$
J[y]=\int_{x_{0}}^{x_{1}}F(x,y,y^{\prime})d x
$$  

has an extremum. For example, the problem of finding the distance between two plane curves is of this type, with  

$$
F(x,y,y^{\prime})=\sqrt{1+y^{\prime2}}.
$$  

As showr, in the preceding section, the general variation of the functional $J[y]$ is gi\ en by formula (5). I f $J[y]$ has an extremum for the curve $y=y(x)$ , then, as noted at the end of Sec. 1 3 , this curve must first of all be an extremal, i.e., a solution of Euler's equation. Hence, the i ntegral in (5) vanishes and we have  

$$
\begin{array}{r}{\begin{array}{r}{\mathfrak{I J}=F_{\pmb{y}^{\prime}}|_{x=x_{1}}\updelta y_{1}+(F-F_{\pmb{y}^{\prime}}{\pmb{y}^{\prime}})|_{x=x_{1}}\updelta x_{1}\qquad}\\ {-F_{\pmb{y}^{\prime}}|_{x=x_{0}}\updelta y_{0}-(F-F_{\pmb{y}^{\prime}}{\pmb{y}^{\prime}})|_{x=x_{0}}\updelta x_{0},}\end{array}}\end{array}
$$  

which must vanish if $J[y]$ is to have an extremum for $y=y(x)$ .  

Next, we observe that according to Figure 5,  

$$
\begin{array}{r l r}{\ensuremath{\delta}\ensuremath{\boldsymbol{y}}_{0}=[\varphi^{\prime}(\ensuremath{\boldsymbol{{x}}})+\varepsilon_{0}]\ensuremath{\delta}\ensuremath{\boldsymbol{{x}}}_{0},}&{}&{\ensuremath{\delta}\ensuremath{\boldsymbol{y}}_{1}=[\psi^{\prime}(\ensuremath{\boldsymbol{{x}}}_{1})+\varepsilon_{1}]\ensuremath{\delta}\ensuremath{\boldsymbol{{x}}}_{1},}\end{array}
$$  

where $\mathfrak{s}_{0}\to0$ as $\updelta x_{0}\rightarrow0$ , and $\mathfrak{E}_{1}\to0$ as $\updelta x_{1}\rightarrow0$ . Thus, in the present case, the condition $\ \delta J=0$ becomes  

$$
\delta J=(F_{y},\psi^{\prime}+F-y^{\prime}F_{y^{\prime}})|_{\tau=x_{1}}\delta x_{1}-(F_{y^{\prime}}\varphi^{\prime}+F-y^{\prime}F_{y^{\prime}})|_{x=x_{0}}\delta x_{0}=0,
$$  

since $\mathfrak{d}J$ contains only terms of the first order in $\mathfrak{8}x_{0}$ and $\updelta x_{1}$ ' Since the increments $\updelta x_{0}$ and $\mathfrak{F}x_{1}$ are independent, ( 1 3) implies the boundary conditions  

or  

$$
\begin{array}{r}{(F_{y}{\cdot}\varphi^{\prime}+F-y^{\prime}F_{y},)|_{x=x_{0}}=0,}\\ {(F_{y}{\cdot}\psi^{\prime}+F-y^{\prime}F_{y},)|_{x=x_{1}}=0,}\\ {[F+(\varphi^{\prime}-y^{\prime})F_{y},]|_{x=x_{0}}=0,}\\ {[F+(\Psi^{\prime}-y^{\prime})F_{y}]|_{x=x_{1}}=0,}\end{array}
$$  

called the transversality conditions. The curve $y=y(x)$ satisfying these conditions is said to be a transversal of the curves $y=\varphi(x)$ and $y=\Psi(x)$ .  

Thus, to solve this kind of variable end point problem, we must first solve Euler's equation  

![](https://cdn-mineru.openxlab.org.cn/extract/c29daec4-3bde-4c07-a565-58de41e65c3b/2340c359b75acbb8ea56c82577f75019cd389d75948383cd4c68a44d8cb72cd8.jpg)  
FIGURE 5  

$$
F_{y}-{\frac{d}{d x}}F_{y^{\prime}}=0,
$$  

and then use the transversality conditions to determine the values of the two arbitrary constants appearing in the general solution of ( 1 4).  

In solving variational problems, we often encounter functionals of the form  

$$
\int_{x_{0}}^{x_{1}}f(x,y){\sqrt{1+y^{\prime}{}^{2}}}d x.
$$  

For such functionals, the transversality conditions have a particularly simple appearance. In fact, in this case,  

$$
F_{y^{\prime}}=f(x,y){\frac{y^{\prime}}{{\sqrt{1+y^{'2}}}}}={\frac{y^{\prime}F}{1+y^{'2}}},
$$  

so that the transversality conditions become  

$$
\begin{array}{c}{{F+(\varphi^{\prime}-y^{\prime})F_{y^{\prime}}=\displaystyle\frac{(1+y^{\prime}\varphi^{\prime})F}{1+y^{\prime}{}^{2}}=0,}}\\ {{F+(\Psi^{\prime}-y^{\prime})F_{y^{\prime}}=\displaystyle\frac{(1+y^{\prime}\Psi^{\prime})F}{1+y^{\prime}{}^{2}}=0.}}\end{array}
$$  

It follows that  

$$
y^{\prime}=-\ \frac{1}{\varphi^{\prime}}
$$  

at the left-hand end point, while  

$$
y^{\prime}=-\mathrm{\small~\frac{1}{\ddagger}},
$$  

at the right-hand end point, i.e., for functionals of the form ( 1 5), trans­ versality reduces to orthogonality.  

The same kind of variable end point problem can be posed for functionals depending on several functions. For example, consider the following problem : Among all smooth curves whose end points lie on two given surfaces $x=\varphi(y,z)$ and $x=\downarrow(y,z)$ find the curve for which the functional  

$$
J[y,z]=\int_{x_{0}}^{x_{1}}F(x,y,z,y^{\prime},z^{\prime})d x
$$  

has an extremum. Setting $n=2$ in formula (7) of the preceding section, we obtain the general variation of the functionaI $J[y,z].$ By the same argument as in the case of one independent function, we find that the required curve $y=y(x),z=z(x)$ m ust again be an extremal , i.e., satisfy the Euler equations  

$$
F_{y}-\frac{d}{d x}F_{y^{\prime}}=0,F_{z}-\frac{d}{d x}F_{z^{\prime}}=0.
$$  

The boundary conditions are now  

$$
\begin{array}{r l r}{\lefteqn{[F_{y^{\prime}}+\frac{\partial\varphi}{\partial y}(F-y^{\prime}F_{y^{\prime}}-z^{\prime}F_{z^{\prime}})]|_{z=z_{0}}=0,}}\\ &{}&\\ &{}&{[F_{z^{\prime}}+\frac{\partial\varphi}{\partial z}(F-y^{\prime}F_{y^{\prime}}-z^{\prime}F_{z})]|_{z=z_{0}}=0,}\\ &{}&\\ &{}&{[F_{y^{\prime}}+\frac{\partial\Psi}{\partial y}(F-y^{\prime}F_{y^{\prime}}-z^{\prime}F_{z^{\prime}})]|_{z=x_{1}}=0,}\\ &{}&\\ &{}&{[F_{z^{\prime}}+\frac{\partial\Psi}{\partial z}(F-y^{\prime}F_{y^{\prime}}-z^{\prime}F_{z})]|_{z=x_{1}}=0,}\end{array}
$$  

and are again called the transversality conditions.  

# 1 5. Broken Extre mals. The We i e rst rass- E rd m an n Co n d i t i o n s  

S o far, w e have only considered functions defined for smooth curves, and hence we have only permitted smooth solutions of variational problems. However, it is easy to give examples of variational problems which have no solutions in the class of smooth curves, but which have solutions if we extend the class of admissible curves to include piecewise smooth curves. Thus, consider the functional  

$$
J[y]=\int_{-1}^{1}y^{2}(1-y^{\prime})^{2}d x,\qquady(-1)=0,\qquady(1)=1.
$$  

The greatest lower bound of the values of $J[y]$ for smooth $y=y(x)$ satisfying the boundary conditions is obviously zero, but it does not achieve this value for any smooth curve. In fact, the minimum is achieved for the curve  

$$
y=y(x)={\left\{\begin{array}{l l}{0}&{{\mathrm{for}}\quad-1\leqslant x\leqslant0,}\\ {x}&{{\mathrm{for}}\quad0<x\leqslant1,}\end{array}\right.}
$$  

which has a corner (i. e . , a discontinuous first derivative) at the point $x=0$ .   
Such a piecewise smooth extremal with corners is called a broken extremal.  

Another problem involving broken extremals has already been encountered in Example 2, p. 20. There it is required to find the curve joining two points $(x_{0},y_{0})$ and $(x_{1},y_{1})$ which generates the surface of least area when rotated about the $x$ -axis. As already noted, if $y_{0}$ and $y_{1}$ are sufficiently small compared to $x_{1}-x_{0},$ the solution of the problem is given by the broken extremal $A x_{0}x_{1}B$ shown in Fig. 2(b), p. 2 1 .  This extremal consists of three line segments (two vertical and one horizontal) and can be included in the class of piecewise smooth curves if we set up the problem in parametric form.  

Guided by the above considerations, we enlarge the class of admissible functions, relaxing the requirement that they be smooth everywhere. Thus, we pose the following problem : Among allfunctions $y(x)$ which are continuously difefrentiable for $a\leqslant x\leqslant b$ except possibly at some point $\boldsymbol{c}$ $(a<c<b)$ , and which satisfy the boundary conditions  

$$
y(a)=A,\qquady(b)=B,
$$  

find the function for which the functional  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x
$$  

has a weak extremum. It is clear that on each of the intervals $[a,c]$ and $[c,b]$ the function for which $J[y]$ has an extremum must satisfy the Euler equation  

$$
F_{y}-{\frac{d}{d x}}F_{y^{\prime}}=0.
$$  

Writing $J[y]$ as a sum of two functionals, i.e. ,  

$$
{\begin{array}{r l}&{J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x}\\ &{\qquad=\int_{a}^{c}F(x,y,y^{\prime})d x+\int_{c}^{b}F(x,y,y^{\prime})d x\equiv J_{1}[y]+J_{2}[y],}\end{array}}
$$  

we calculate the variations $\updelta J_{1}$ and $\mathbf{\delta}\otimes\mathbf{\vec{\mathbf{z}}}$ of the two terms separately. The end points $x=a$ , $x=b$ are fixed, and we require that the two " pieces " of the function $y(x)$ join continuously at $x=c$ , but otherwise the point $x=c$ can move freely. Using formula (5) to write $\delta J_{1}$ and $\mathbf{\delta}\mathfrak{d}_{2}$ , and recalling that $y(x)$ is an extremal , we find that  

$$
\begin{array}{r l}&{\8J_{1}=F_{y^{\prime}}|_{x=c-0}\ \&y_{1}+\ (F-y^{\prime}F_{y^{\prime}})|_{x=c-0}\ \&x_{1},}\\ &{\8J_{2}=\ -\ F_{y^{\prime}}|_{x=c+0}\ \&y_{1}-\ (F-y^{\prime}F_{y^{\prime}})|_{x=c+0}\ \&x_{1}.}\end{array}
$$  

[The condition that $y(x)$ be continuous at $x=c$ implies that $\delta J_{1}$ and $\updelta J_{2}$ involve the same increments $\updelta x_{1}$ and $\updelta{y}_{1}$ .] At an extremum we must have  

$$
\updelta J=\updelta J_{1}+\updelta J_{2}=0,
$$  

and hence  

$$
\begin{array}{r l}{\lefteqn{(F_{y^{\prime}}|_{z=c-0}-F_{y^{\prime}}|_{z=c+0})\ \mathfrak{J}_{1}}\quad}&{}\\ &{\phantom{=}+\ [(F-y^{\prime}F_{y^{\prime}})|_{x=c-0}-(F-y^{\prime}F_{y^{\prime}})|_{z=c+0}]\ \mathfrak{J}_{1}=}\end{array}
$$  

Since $\8x_{1}$ and $\updelta y_{1}$ are arbitrary, the conditions  

$$
\begin{array}{c}{F_{y^{\prime}}|_{x=c-0}=F_{y^{\prime}}|_{x=c+0},}\\ {(F-y^{\prime}F_{y^{\prime}})|_{x=c-0}=(F-y^{\prime}F_{y^{\prime}})|_{x=c+0},}\end{array}
$$  

called the Weierstrass-Erdmann (corner) conditions, hold at the point $\boldsymbol{c}$ where the extremal has a corner.  

In each of the intervals $[a,c]$ and $[c,b].$ the extremal $y=y(x)$ must satisfy Euler's equation ( 1 7), i.e. , a second-order differential equation. Solving these two equations, we obtain four arbitrary constants, which can then be found from the boundary conditions ( 1 6) and the Weierstrass­ Erdmann conditions ( 1 8).  

The Weierstrass-Erdmann conditions take a particularly simple form if we use the canonical variables  

$$
p=F_{y^{\prime}},\qquadH=-F+y^{\prime}F_{y^{\prime}}
$$  

introduced in Sec. 1 3. In fact, then the conditions ( 1 8) just mean that the canonical variables are continuous at a point where the extremal has $\pmb{a}$ corner.  

The Weierstrass-Erdmann conditions have the following simple geometric interpretation : Let $x$ and $y$ take fixed values, plot the value of $y^{\prime}$ along one coordinate axis, and plot the values of $F(x,y,y^{\prime})$ along the other. The result is a curve, called the indicatrix, representing $F(x,y,y^{\prime})$ as a function of $y^{\prime}$ . Then the first of the conditions ( 1 8) means that the tangents to the indicatrix at the points $y^{\prime}(c-0)$ and $y^{\prime}(c+0)$ are parallel, while the second condition, which can be written in the form  

$$
F|_{x=c+0}-F|_{x=c-0}=F_{y},y^{\prime}|_{x=c+0}-F_{y},y^{\prime}|_{x=c-0},
$$  

means that the two tangents are not only parallel, but in fact coincide.  

# PROBLEMS  

1 . Justify the application o f Theorem 2 , p . 1 3  t o the case o f variable end point problems.  

2. Derive the formula for the general variation of a functional of the form  

$$
J[y]=\int_{z_{0}}^{z_{1}}F(x,y,y^{\prime})d x+G(x_{0},y_{0},x_{1},y_{1}).
$$  

3. Derive the formula for the general variation of a functional of the form  

$$
J[y]=\int_{z_{0}}^{z_{1}}F(x,y,y^{\prime},y^{\prime})d x.
$$  

4. Find the curves for which the functional  

$$
J[y]=\int_{0}^{\pi/4}\left(y^{2}-y^{\prime2}\right)d x,
$$  

can have extrema, given that $y(0)=0$ , while the right-hand end point can vary along the line $x=\pi/4$ .  

5. Find the curves for which the functional  

$$
J[y]=\int_{0}^{z_{1}}\frac{\sqrt{1+y^{'2}}}{y}d x,\qquady(0)=0
$$  

can have extrema if  

a) The point $(x_{1},y_{1})$ an vary along the line $y=x-5$ ;   
b) The point $(x_{1},y_{1})$ an vary along the circle $(x-9)^{2}+y^{2}=9$ .  

$$
\mid y=\pm{\sqrt{10x-x^{2}}};\qquad{\mathsf{b}})~y=\pm{\sqrt{8x-x^{2}}}
$$  

6. Find the curve connecting two given circles in the (vertical) plane along which a particle falls in the shortest time under the influence of gravity.  

7. Find the shortest distance between the surfaces $z=\varphi(x,y)$ and $z=\Psi(x,y)$ .  

8. Write the transversality conditions for the functional in Prob. 2 if the end points of the admissible curves $y=y(x)$ lie on two given curves $y=\varphi({\boldsymbol{x}})$ and $y=\psi({\boldsymbol{x}})$ .  

9. Write the transversality conditions for a functional of the form  

$$
J[y,z]=\int_{x_{0}}^{z_{1}}f(x,y,z)\sqrt{1+y^{\prime2}+z^{\prime2}}d x
$$  

defined for curves whose end points lie on two given surfaces $z=\varphi(x,y)$ and $z=\Psi(x,y)$ . Interpret the conditions geometrically.  

10. Find the curves for which the functional  

$$
J[y,z]=\int_{0}^{z_{1}}\left(y^{\prime2}+z^{\prime2}+2y z\right)d x
$$  

can have extrema, given that $y(0)=z(0)=0$ , while the point $(x_{1},y_{1},z_{1})$ can vary in the plane $\pmb{x}=\pmb{x_{1}}$ .  

11. Show that for functionals of the form  

$$
J[y]=\int_{x_{0}}^{x_{1}}f(x,y){\sqrt{1+y^{\prime}{}^{2}}}e^{\pm\tan^{-1}y^{\prime}}d x,
$$  

the transversality conditions reduce to the requirement that the curve $y=y({\boldsymbol{x}})$ intersect the curves $y=\varphi({\boldsymbol{x}})$ and $y=\psi({\boldsymbol{x}})$ [along which its end points vary] at an angle of $45^{\circ}$ .  

11. Find the curves for which the functional  

$$
J[y]=\int_{0}^{1}\left(1~+~y^{\prime2}\right)d x
$$  

can have extrema, given that $y(0)=0,y^{\prime}(0)=1,y(1)=1$ ,  while $y^{\prime}(1)$ can vary arbitrarily.  

13. Minimize the functional  

$$
J[y]=\int_{-1}^{1}x^{2/3}y^{\prime2}d x,\qquady(-1)=-1,~y(1)=1.
$$  

Hint. Although the extremal $y=x^{1/3}$ has n o  derivative at ${\pmb x}={\pmb0}$ , it is easily verified by direct calculation that $y=x^{1/3}$ minimizes $J[y]$ .  

14. Given an extremal $y=y(x)$ , possibly only piecewise smooth, of the functional  

$$
J[y]=\int_{x_{0}}^{x_{1}}F(x,y,y^{\prime})d x,\qquady(x_{0})=y_{0},\quad y(x_{1})=x_{1},
$$  

suppose that  

$$
F_{y^{\prime}y^{\prime}}[x,y(x),z]\neq0
$$  

for all finite $\pmb{z}$ . Prove that $y(x)$ is then actually smooth, with a smooth derivative, in $[x_{0},x_{1}]$ .  

Hint. Use Theorem 3 of Sec. 4 and the geometric interpretation of the Weierstrass-Erdmann conditions given at the end of Sec. 1 5.  

15. Prove that the functional  

$$
J[y]=\int_{x_{0}}^{x_{1}}(a y^{\prime2}+b y y^{\prime}+c y^{2})d x,\qquady(x_{0})=y_{0},\quad y(x_{1})=y_{1},
$$  

where $\alpha\neq0$ , can have no broken extremals.  

16. Does the functional  

$$
J[y]=\int_{0}^{z_{1}}y^{\prime3}d x,\qquady(0)=0,\quad y(x_{1})=y_{1}
$$  

have broken extremals ?  

17. Find the extremals of the functional  

$$
J[y]=\int_{0}^{4}(y^{\prime}-1)^{2}(y^{\prime}+1)^{2}d x,\qquady(0)=0,~y(4)=2
$$  

which have just one corner.  

18. Find the curve for which the functional  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x,\qquady(a)=A,\quad y(b)=B
$$  

has an extremum if the curve can arrive at $(b,B)$ only after touching a given curve $y=\varphi(x)$ .  

19. Given a curve $y=\varphi(x)$ and two points $(a,A),(b,B)$ lying on opposite sides of the curve, consider the functional  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x,\qquady(a)=A,\quad y(b)=B,
$$  

where $F(x,y,y^{\prime})=F_{1}(x,y,y^{\prime})$ on the side of the curve corresponding to $(a,A)$ , and $F(x,y,y^{\prime})=F_{2}(x,y,y^{\prime})$ on the side of the curve corresponding to $(b,B)$ . Find the curve $y=y({\boldsymbol{x}})$ for which $J[y]$ has an extremum.  

20. Using Fermat's pri nciple (pp. 34, 36), specialize the results of Probs . 1 8 and 1 9  t o functionals of the form  

$$
\int_{a}^{b}f(x,y){\sqrt{1+y^{\prime2}}}d x,
$$  

thereby deriving the familiar laws of reflection and refraction for light rays.  

21 . Find the curves for which the functional  

$$
J[y]=\int_{0}^{10}y^{\prime3}\ d x,\qquady(0)=0,\quad y(10)=0
$$  

can have extrema, given that the admissible curves cannot penetrate the interior of the circle with equation  

$$
(x-5)^{2}+y^{2}=9.
$$  

$$
A n s.\quad y=\left\{\begin{array}{l l}{\pm\frac{3}{4}x}&{\quad\mathrm{for}\quad0\leqslant x\leqslant\frac{16}{5},}\\ {\pm\sqrt{9-(x-5)^{2}}}&{\quad\mathrm{for}\quad\frac{16}{5}\leqslant x\leqslant\frac{34}{5},}\\ {\mp\frac{3}{4}(x-10)}&{\quad\mathrm{for}\quad\frac{34}{5}\leqslant x\leqslant10.}\end{array}\right.
$$  

# 4  

# THE CAN ONI CAL FORM OF THE EULER EQUATIONS AND RELATED TOPI CS  

As already remarked in Sec. 1 ,  many physical laws can be expressed as variational principles, i.e., in terms of extremal properties of certain func­ tionals. In this chapter, we s hall illustrate this situation by using variational methods to study the classical mechanics of a system consisting of a finite number of particles. For example, we shall show how the trajectories in phase space of a mechanical system (which describe how the system evolves in time) can be found as the extremals of a certain functional. By using the calculus of variations, we can also find quantities connected with a given physical system which do not change as the system evolves in time. These and related ideas will be our chief concern here. First, we return to the subject of canonical variables (introd uced in Sec. 1 3), and discuss the reduc­ tion of the Euler equations to canonical form . Appendix I (p. 208) is closely related to the subject matter of this chapter, and contains another, independent derivation of the canonical equations and the Hamilton-Jacobi equation.  

# 1 6. The Can o n i cal Fo r m of the E u l e r  Eq u at i o n s  

The Euler equations corresponding t o the functional  

$$
J[y_{1},...,y_{n}]=\int_{a}^{b}F(x,y_{1},...,y_{n},y_{1},...,y_{n}^{\prime})d x
$$  

(which depends on $\pmb{n}$ functions) form a system of $\pmb{n}$ second-order differential equations  

$$
F_{y_{i}}-{\frac{d}{d x}}F_{y_{i}^{\prime}}=0\qquad(i=1,...,n).
$$  

This system can be reduced (in various ways) to a system of $2n$ first-order differential equations. For example, regarding $y_{1}^{\prime},\ldots,y_{n}^{\prime}$ as $\pmb{n}$ new functions, independent of $y_{1},...,y_{n}$ , we can write (2) in the form  

$$
\frac{d y_{i}}{d x}=y_{i}^{\prime},F_{y_{i}}-\frac{d}{d x}F_{y_{i}^{\prime}}=0(i=1,...,n),
$$  

where $y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime}$ are $2n$ unknown functions, and $x$ is the independ­ ent variable. l However, we obtain a much more convenient and symmetric form of the Euler equations if we replace $x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime}$ by another set of variables, i.e., the canonical variables introduced in the preceding chapter. The reader will recall that in Sec. 1 3, we used the equations  

$$
p_{i}=F_{y_{i}^{\prime}}\qquad(i=1,...,n)
$$  

to write $y_{1}^{\prime},\ldots,y_{n}^{\prime}$ as functions of the variables2  

$$
x,y_{1},...,y_{n},p_{1},...,p_{n}.
$$  

Then we expressed the function $F(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})$ appearing in ( I ) in terms of a new function $H(x,y_{1},...,y_{n},p_{1},...,p_{n})$ related to $F$ by the formula  

$$
H=-\ F+\ \sum_{i=1}^{n}\ y_{i}^{\prime}p_{i},
$$  

where the $y_{i}^{\prime}$ are regarded as functions of the variables (5). The function $H$ is called the Hamiltonian (corresponding to the functional $J[y_{1},...,y_{n}])$ . Finally, we introduced the new variables  

$$
x,y_{1},...,y_{n},p_{1},...,p_{n},H,
$$  

called the canonical variables (corresponding to the functional $J[y_{1},...,y_{n}])$ , which were used on p. 58 to write a concise expression for the general variation of the functional $J[y_{1},...,y_{n}],$ , and on p. 63 to give a simple interpretation of the Weierstrass-Erdmann conditions.  

We now show how the Euler equations (3) transform when we go over to canonical variables. In order to make this change in the Euler equations, we have to express the partial derivatives $F_{y_{i}}$ (i.e., the partial derivatives of $F$ with respect to $y_{i}$ " evaluated for constant $x,y_{1}^{\prime},\ldots,y_{n}^{\prime})$ in terms of the partial derivatives $H_{y_{i}}$ (evaluated for constant $x,p_{1},....,p_{n})$ .3 The direct evaluation of these derivatives would be rather formidable. Therefore, to avoid lengthy calculations, we write the expression for the differential of the function $H$ . Then, using the fact that the first differential of a function does not depend on the choice of independent variables (i.e., is invariant under changes of the independent variables), we shall obtain the required formulas quite easily.  

By the definition of $H_{;}$ , we have  

$$
d H=-~d F+~\sum_{i=1}^{n}p_{i}~d y_{i}^{\prime}+~\sum_{i=1}^{n}y_{i}^{\prime}~d p_{i},
$$  

s o that  

$$
\begin{array}{r}{d H={\displaystyle-\frac{\partial F}{\partial x}d x}-\displaystyle\sum_{i=1}^{n}\frac{\partial F}{\partial y_{i}}d y_{i}-\displaystyle\sum_{i=1}^{n}\frac{\partial F}{\partial y_{i}^{\prime}}d y_{i}^{\prime}}\\ {+\displaystyle\sum_{i=1}^{n}p_{i}d y_{i}^{\prime}+\sum_{i=1}^{n}y_{i}^{\prime}d p_{i}.}\end{array}
$$  

Ordinarily, before using (8) to obtain expressions for the partial derivatives of $H$ , we would have to express the $d y_{i}^{\prime}$ in terms of $x,y_{i}$ " and $\pmb{p_{i}}$ . However (and this is the important feature of the canonical variables), because of the relations  

$$
\frac{\partial F}{\partial y_{i}^{\prime}}=p_{i}\qquad(i=1,...,n),
$$  

the terms containing $d y_{i}^{\prime}$ in (8) cancel each other out, and we obtain  

$$
d H=-\ {\frac{\partial F}{\partial x}}d x-{\textstyle\sum_{i=1}^{n}{\frac{\partial F}{\partial y_{i}}}d y_{i}}+{\textstyle\sum_{i=1}^{n}{{y_{i}^{\prime}}d p_{i}}}.
$$  

Thus, to obtain the partial derivatives of $H$ , we need only write down the appropriate coefficients of the differentials in the right-hand side of (9), i.e.,  

$$
\frac{\partial H}{\partial x}=-\frac{\partial F}{\partial x},\frac{\partial H}{\partial y_{i}}=-\frac{\partial F}{\partial y_{i}},\frac{\partial H}{\partial p_{i}}=y_{i}^{\prime}.
$$  

In other words, the quantities $\partial F/\partial y_{i}$ and $y_{i}^{\prime}$ are connected with the partial derivatives of the function $H$ by the formulas  

$$
y_{i}^{\prime}={\frac{\partial H}{\partial p_{i}}},\qquad{\frac{\partial F}{\partial y_{i}}}=-\ {\frac{\partial H}{\partial y_{i}}}.
$$  

Finally, using ( 1 0), we can write the Euler equations (3) in the form  

$$
{\frac{d y_{i}}{d x}}={\frac{\partial H}{\partial p_{i}}},{\frac{d p_{i}}{d x}}=-{\frac{\partial H}{\partial y_{i}}}\qquad(i=1,...,n).
$$  

These $2n$ first-order differential equations form a system which i s equivalent to the system (3) and is called the canonical system of Euler equations (or simply the canonical Euler equations) for the functional ( 1 ).  

# 1 7. Fi rst I nteg rals of t h e E u l e r Eq u at i o n s  

It will b e recalled that a first integral o f a system o f differential equations i s a function which has a constant value along each integral curve o f the system. We now look for first integrals of the canonical system (1 I ), and hence of the original system (3) which is equivalent to ( 1   ). First, we consider the case where the function $F$ defining the functional ( I )  does not depend on $x$ explicitly, i . e . , is of the form $F(y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})$ . Then the function  

$$
H=-\ F+\ \sum_{i=1}^{n}\ y_{i}^{\prime}p_{i}
$$  

also does not depend on $x$ explicitly, and hence  

$$
{\frac{d H}{d x}}=\ \sum_{i=1}^{n}\left({\frac{\partial H}{\partial y_{i}}}{\frac{d y_{i}}{d x}}+{\frac{\partial H}{\partial p_{i}}}{\frac{d p_{i}}{d x}}\right).
$$  

Using the Euler equations in the canonical form ( I I ), we find that ( 1 2) becomes  

$$
\frac{d H}{d x}=\sum_{i=1}^{n}\bigg(\frac{\partial H}{\partial y_{i}}\frac{\partial H}{\partial p_{i}}-\frac{\partial H}{\partial p_{i}}\frac{\partial H}{\partial y_{i}}\bigg)=0,
$$  

along each extremal.4 Thus, i $F$ does not depend on $x$ explicitly, the function $H(y_{1},...,y_{n},p_{1},...,p_{n})$ is $a$ first integral of the Euler equations. 5  

$$
{\frac{d H}{d x}}={\frac{\partial H}{\partial x}}
$$  

${\mathsf{s}}_{\mathbf{C}\mathbf{f}}$ . the discussion in Case 2, p. 18 of the integration of Euler's equation for functionals which are independent of $x$ .  

Next, we consider an arbitrary function of the form  

$$
\Phi=\Phi(y_{1},...,y_{n},p_{1},...,p_{n}),
$$  

and we examine the conditions under which $\Phi$ will be a fi rst integral of the system ( I I ). We drop the assumption that $F$ does not depend on $x$ explicitly, and instead we consider the general case. Along each integral curve of the system ( 1 1 ), we have  

$$
\begin{array}{r l r}{\lefteqn{\frac{d\Phi}{d x}=\sum_{i=1}^{n}\frac{\partial\Phi}{\partial y_{i}}\frac{d y_{i}}{d x}+\frac{\partial\Phi}{\partial p_{i}}\frac{d p_{i}}{d x}}}\\ &{}&{=\sum_{i=1}^{n}\frac{\partial\Phi}{\partial y_{i}}\frac{\partial H}{\partial p_{i}}-\frac{\partial\Phi}{\partial p_{i}}\frac{\partial H}{\partial y_{i}}=[\Phi,H],}\end{array}
$$  

where the expression  

$$
[\Phi,H]=\ \sum_{i=1}^{n}\frac{\partial\Phi}{\partial y_{i}}\frac{\partial H}{\partial p_{i}}-\frac{\partial\Phi}{\partial p_{i}}\frac{\partial H}{\partial y_{i}}
$$  

is called the Poisson bracket of the functions $\Phi$ and $H_{\sun}$ . Thus, we have proved the formula  

$$
\frac{d\Phi}{d x}=[\Phi,H].
$$  

It follows from ( 1 3) that $\pmb{a}$ necessary and sufficient condition for a function $\Phi=\Phi(y_{1},...,y_{n},p_{1},...,p_{n})$ to be a first integral of the system of Euler equations ( I I ) is that the Poisson bracket $[\Phi,H]$ vanish identically.s  

# 1 8. The Lege n d re Transformation  

W e now consider another method o f reducing the Euler equations to canonical form, a method which differs from that presented in Sec. 1 6. The idea of this new method is to replace the variational problem under consideration by another, equivalent problem, such that the Euler equations for the new problem are the same as the canonical Euler equations for the original problem.  

18. 1 . We begin by discussing some related topics from the theory of extrema of functions of $n$ variables . First, we consider the case $n=1$ .  

Suppose we are looking for an extremum, say a minimum, of the function $f(\xi)_{}$ , and suppose $f(\xi)$ is (strictly) convex, which means that  

$$
f^{\prime\prime}(\xi)>0
$$  

wherever $f(\xi)$ is defined. We introduce a new independent variable  

$$
p=f^{\prime}(\xi),
$$  

called the tangential coordinate, which is just the slope of the tangent passing through a given point of the curve $\eta=f(\xi)$ . Since by hypothesis  

$$
\frac{d p}{d\xi}=f^{\prime}(\xi)>0,
$$  

we can use ( 1 4) to express $\xi$ in terms of $p$ . In fact, since the function $f(\xi)$ is convex, any point of the curve $\eta=f(\xi)$ is uniquely determined by the slope  

![](https://cdn-mineru.openxlab.org.cn/extract/c29daec4-3bde-4c07-a565-58de41e65c3b/94a861794e5ed278cf1f78eb57c695838e4d0ea218e01bb34682c25073eaceec.jpg)  
FIGURE 6  

of its tangent (see Figure 6). Of course, the same is true for a (strictly) concave function, i.e., a function such that $f^{\prime\prime}(\xi)<0$ everywhere.  

We now introduce the new function  

$$
H(p)=-f(\xi)+p\xi,
$$  

where $\xi$ is regarded as the function of $p$ obtained by solving ( 1 4). The transformation from the variable and function pair $\xi,f(\xi)$ to the variable and function pair $p,H(p)$ , defined by formulas ( 1 4) and ( 1 5), is called the Legendre transform­ ation. It is easy to see that since $f(\xi)$ is convex, so is $H(p)$ . [The convex functions $H(p)$ and $f(\xi)$ are sometimes said to be conjugate.] In fact,  

$$
d H=-f^{\prime}(\xi)d\xi+p d\xi+\xi d p
$$  

implies that  

$$
\frac{d H}{d p}=\xi,
$$  

and hence  

$$
\frac{d^{2}H}{d p^{2}}=\frac{d\xi}{d p}=\frac{1}{\frac{d p}{d\xi}}=\frac{1}{f^{\prime\prime}(\xi)}>0,
$$  

since $f^{\prime\prime}(\xi)>0$ . Moreover, if the Legendre transformation is applied to the pair $p,H(p)$ , we get back the pair $\xi,f(\xi)$ . This fol lows from ( 1 6) and the relation  

$$
-H(p)+p H^{\prime}(p)=f(\xi)-p H^{\prime}(p)+p H^{\prime}(p)=f(\xi).
$$  

Thus, the Legendre transformation is an involution, i . e . , a transformation which is its own inverse.  

Example. If  

$$
f(\xi)=\frac{\xi^{a}}{a}\qquad(a>1),
$$  

then  

$$
f^{\prime}(\xi)=p=\xi^{a-1},
$$  

i . e . ,  

$$
\xi=p^{1/(a-1)}.
$$  

It follows that  

$$
H=-\frac{\xi^{a}}{a}+p\xi=-\frac{p^{a/(a-1)}}{a}+p p^{a/(a-1)}=p^{a/(a-1)}\left(-\frac{1}{a}+1\right),
$$  

and therefore  

$$
H(p)={\frac{p^{\flat}}{b}},
$$  

where $b$ i s related to $\pmb{a}$ b y the formula  

$$
\frac{1}{a}+\frac{1}{b}=1.
$$  

Next, we show that if  

$$
-H(p)+\xi p
$$  

is regarded as a function of two variables, then  

$$
f(\xi)=\operatorname*{max}_{p}[-H(p)+\xi p].
$$  

[In fact, we can use (20) instead of ( 1 5) to define the function $H(p)$ . ] To prove this result, we note that according to ( 1 8), the function ( 1 9) reduces to $f(\xi)$ when the condition  

$$
\frac{\partial}{\partial p}\left[-H(p)+\xi p\right]=-H^{\prime}(p)+\xi=0,
$$  

or  

$$
\xi=H^{\prime}(p),
$$  

is satisfied . Thus, $f(\xi)$ is an extremum of the function $-H(p)+\xi p,$ regarded as a function of $p.$ . Moreover, the extremum is a maximum since  

$$
\frac{\partial^{2}}{\partial p^{2}}\left[-H(p)+\xi p\right]=-H^{\prime\prime}(p)<0
$$  

[cf. ( 1 7)]. It follows that  

$$
\operatorname*{min}_{\mathfrak{s}}f(\xi)=\operatorname*{min}_{\mathfrak{s}}\operatorname*{max}_{\mathfrak{p}}[-H({p})+\xi p],
$$  

i.e., the extremum of $f(\xi)$ is also an extremum of ( 1 9), regarded as a function of two variables.  

Similar considerations apply to functions of several independent variables. Let  

$$
f(\xi_{1},...,\xi_{n})
$$  

be a function of $\pmb{n}$ variables such that  

$$
\begin{array}{r}{\operatorname*{det}\|f_{\xi_{i}\xi_{k}}\|\neq0,}\end{array}
$$  

and let  

$$
p_{i}=f_{\xi_{i}}\qquad(i=1,...,n).
$$  

Then, using (22) to write $\xi_{1},...,\xi_{n}$ in terms of $p_{1},...,p_{n}$ , we form the function  

$$
H(p_{1},...,p_{n})=-f+\sum_{i=1}^{n}\xi_{i}p_{i}.
$$  

A s i n the case o f one variable, i t can b e shown that  

$$
f(\xi_{1},...,\xi_{n})=\operatorname*{ext}_{p_{1},...,p_{n}}[-H(p_{1},...,p_{n})+\sum_{i=1}^{n}p_{i}\xi_{i}]
$$  

and  

$$
\underset{\underset{5_{1},\ldots,5_{n}}{\uparrow}}{\mathrm{ext}}f(\xi_{1},...,\xi_{n})=\underset{\underset{5_{1},\ldots,5_{n},p_{1},\ldots,p_{n}}{\uparrow}}{\mathrm{ext}}\left[-H(p_{1},...,p_{n})+\sum_{i=1}^{n}p_{i}\xi_{i}\right],
$$  

where ext denotes the operation of taking an extremum with respect to the indicated variables. In other words, the extremum of $f(\xi_{1},...,\xi_{n})$ is also an extremum of  

$$
-H(p_{1},...,p_{n})+\sum_{i=1}^{n}p_{i}\xi_{i},
$$  

regarded as a function of $2n$ variables.  

Remark. If instead of (2 1), we impose the stronger condition that the matrix  

$$
\|f_{\xi_{i}\xi_{k}}\|
$$  

be positive definite, i.e., that the quadratic form  

$$
\sum\limits_{i,k=1}^{n}f_{i,k,k}\alpha_{i}\alpha_{k}
$$  

b e positive for arbitrary real numbers $\alpha_{1},...,{\alpha_{n}},^{7}$ then  

$$
f(\xi_{1},...,\xi_{n})=\operatorname*{max}_{p_{1},....p_{n}}~\biggl[-H(p_{1},...,p_{n})+\sum_{i=1}^{n}\xi_{i}p_{i}\biggr].
$$  

7 This is the condition for the function $f(\xi_{1},...,\xi_{n})$ to be (strictly) convex.  

It follows from (23) that  

$$
-H(p_{1},...,p_{n})+\sum_{i=1}^{n}p_{i}\xi_{i}\leqslant f(\xi_{1},...,\xi_{n})
$$  

for arbitrary $p_{1},...,p_{n};$ , i . e . ,  

$$
\sum_{i=1}^{n}p_{i}\xi_{i}\leqslant H(p_{1},...,p_{n})+f(\xi_{1},...,\xi_{n}),
$$  

a result known a s Young's inequality.  

18.2. We now apply the considerations of Sec. 1 8. 1  to functionals. Given a functional  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x,
$$  

we set  

$$
p=F_{y^{\prime}}(x,y,y^{\prime})
$$  

and  

$$
H(x,y,p)=-~F+p y^{\prime}.
$$  

Here we assume that $F_{y^{\prime}y^{\prime}}\neq0$ , so that (25) defines $y^{\prime}$ as a function of $x$ , $y$ and $p$ . Then we introduce the new functional  

$$
J[y,p]=\int_{a}^{b}{\left[{-H(x,y,p)+p y^{\prime}}\right]d x},
$$  

where $y$ and $p$ are regarded as two independent functions, and $y^{\prime}$ is the deriva­ tive of $y$ . This functional is obviously the same as the original functional (24), if we choose $p$ to be given by the expression (25). The Euler equations for the functional (27) are  

$$
-\:\frac{\partial H}{\partial y}-\frac{d p}{d x}=0,-\frac{\partial H}{\partial p}+\frac{d y}{d x}=0,
$$  

i.e. , j ust the canonical equations for the functional (24). If we can show that the functionals (24) and (27) have their extrema for the same curves, this will prove that the equation  

$$
\frac{\partial F}{\partial y}-\frac{d}{d x}\frac{\partial F}{\partial y^{\prime}}=0
$$  

and the equations (28) are equivalent, thereby providing a new derivation of the canonical equations, i ndependent of the derivation given in Sec. 1 6.  

First, we observe that the transformation from the variables $x,y,y^{\prime}$ and the function $F$ to the variables $x,y,p$ and the function $H$ , defined by formulas  

(25) and (26), is an involution, i . e . , if we subject $H(x,y,p)$ to a Legendre transformation, we get back the function $F(x,y,y^{\prime})$ . In fact, since  

$$
d H=-~{\frac{\partial F}{\partial x}}d x-{\frac{\partial F}{\partial y}}d y+y^{\prime}d p,
$$  

it follows that  

$$
\frac{\partial H}{\partial p}=y^{\prime},
$$  

and hence  

$$
-H+p\frac{\partial H}{\partial p}=F-p y^{\prime}+p y^{\prime}=F.
$$  

[Cf. formula (9) of Sec. 1 6. ]  

Next, we note that to prove the equivalence of the variational problems (24) and (27), it is sufficient to show that $J[y]$ is an extremum of $\boldsymbol{J}[\boldsymbol{y},\boldsymbol{p}]$ when $p$ is varied and $y$ is held fixed, symbolically  

$$
J[y]=\mathsf{e x t}J[y,p],
$$  

since then an extremum of $\boldsymbol{J}[\boldsymbol{y},\boldsymbol{p}]$ when both $p$ and $y$ are varied will be an extremum of $J[y]$ . Since $\boldsymbol{J}[\boldsymbol{y},\boldsymbol{p}]$ does not contain $p^{\prime}$ , to find an extremum of $J[y,p]$ it is sufficient to find an extremum of the integrand in (27) at every point (cf. Case 3, p. 1 9). Thus we have  

$$
\frac{\partial}{\partial p}\left[-H+p y^{\prime}\right]=0,
$$  

from which it follows that  

$$
y^{\prime}=\frac{\partial H}{\partial p}\cdot
$$  

But this implies (3 1 ) , since  

$$
-H+p\frac{\partial H}{\partial p}=F,
$$  

according to (30). Thus, we have proved the equivalence of the variational problems (24) and (27), and of the corresponding Euler equations (28) and (29). Although we have only considered functionals depending on a single function, completely analogous considerations apply to the case of functionals depending on several functions.  

Example. Consider the functional  

$$
\int_{a}^{b}\left(P y^{\prime2}+Q y^{2}\right)d x,
$$  

where $P$ and $\boldsymbol{Q}$ are functions of $x$ . In this case,  

$$
p=2P y^{\prime},\qquadH=P y^{\prime2}-Q y^{2}.
$$  

and hence  

$$
H=\frac{p^{2}}{4P}-\ Q y^{2}.
$$  

The corresponding canonical equations are  

$$
\frac{d p}{d x}=2Q y,\frac{d y}{d x}=\frac{p}{2P},
$$  

while the usual form of the Euler equation for the functional (32) is  

$$
2y Q-\frac{d}{d x}\left(2P y^{\prime}\right)=0.
$$  

# 1 9. Can o n i cal Transformations  

Next, w e look for transformations under which the canonical Euler equations preserve their canonical form. The reader will recall that in Sec. 8 we proved the invariance of the Euler equation  

$$
F_{y}-{\frac{d}{d x}}F_{y^{\prime}}=0
$$  

under coordinate transformations of the form  

$$
\begin{array}{r l}{u=u(x,y),\quad}&{{}\left|u_{x}\quad u_{y}\right|}\\ {v=v(x,y),\quad}&{{}\left|v_{x}\quad v_{y}\right|\ne0.}\end{array}
$$  

(Such transformations change $y^{\prime}$ to $d v/d u$ in the original functional.) The canonical Euler equations also have this invariance property. Furthermore, because of the symmetry between the variables $y_{i}$ and $p_{i}$ in the canonical equations, they permit even more general changes of variables, i.e. , we can transform the variables $x,y_{i},p_{i}$ into new variables $x$ ,  

$$
\begin{array}{r}{Y_{i}=Y_{i}(x,y_{1},...,y_{n},p_{1},...,p_{n}),}\\ {P_{i}=P_{i}(x,y_{1},...,y_{n},p_{1},...,p_{n}).}\end{array}
$$  

In other words, we can think of letting the $p_{i}$ transform according to their own formulas, independently of how the variables $y_{i}$ transform. However, the canonical equations do not preserve their form under all transformations (33). We now study the conditions which have to be imposed on the transformations (33) if the Euler equations are to continue to be in canonical form when written in the new variables, i.e., if the canonical equations are to transform into new equations  

$$
\frac{d Y_{i}}{d x}=\frac{\partial H^{*}}{\partial P_{i}},\qquad\frac{d P_{i}}{d x}=-\frac{\partial H^{*}}{\partial Y_{i}},
$$  

where $H^{*}=H^{*}(x,Y_{1},...,Y_{n},P_{1},...,P_{n})$ is some new function. Trans­ formations of the form (33) which preserve the canonical form of the Euler equations are called canonical transformations.  

To find such canonical transformations, we use the fact that the canonical equations  

$$
\frac{d y_{i}}{d x}=\frac{\partial H}{\partial p_{i}},\frac{d p_{i}}{d x}=-\frac{\partial H}{\partial y_{i}}
$$  

are the Euler equations of the functional  

$$
J[y_{1},...,y_{n},p_{1},...,p_{n}]=\int_{a}^{b}\Big(\sum_{i=1}^{n}p_{i}y_{i}^{\prime}-H\Big)d x,
$$  

in which the $y_{i}$ and $p_{i}$ are regarded as $2n$ independent functions. We want the new variables $Y_{i}$ and $P_{i}$ to satisfy the equations (34) for some function $H^{*}$ . This suggests that we write the functional which has (34) as its Euler equations. This functional is  

$$
J^{*}[Y_{1},...,Y_{n},P_{1},...,P_{n}]=\int_{a}^{b}\left(\sum_{i=1}^{n}P_{i}Y_{i}^{\prime}-H^{*}\right)d x,
$$  

where $\textstyle\Y_{i}$ and $P_{i}$ are the functions of $x,y_{i}$ and $p_{i}$ defined by (33), and $\smash{\frac{\gamma_{\perp}^{\prime}}{2}}$ is the derivative of $Y_{i}$ • Thus, the functionals (36) and (37) represent two different variational problems involving the same variables $y_{i}$ and $p_{i}$ and the requirement that the new system of canonical equations (34) be equivalent to the old system (3 5), i . e . , that it be possible to obtain (34) from (35) by making a change of variables (33), is the same as the requirement that the variational problems corresponding to the functionals (36) and (37) be equivalent.  

In the remarks made on p. 36, it was shown that two variational problems are equivalent (i.e., have the same extremals) if the integrands of the corre­ sponding functionals differ from each other by a total differential, which in this case means that  

$$
\sum_{i=1}^{n}p_{i}d y_{\mathfrak{i}}-H d x=\sum_{i=1}^{n}P_{i}d Y_{\mathfrak{i}}-H^{*}d x+d\Phi(x,y_{1},...,y_{n},p_{1},...,p_{n})
$$  

for some function $\Phi$ <1.>. Thus, if a given transformation (33) from the variables $x,y_{i},p_{i}$ to the variables $x,Y_{i},P_{i}$ is such that there exists a function $\Phi$ satis­ fying the condition (38), then the transformation (33) is canonical. In this case, the function $\Phi$ defined by (38) is called the generating function of the canonical transformation. The function $\Phi$ is only specified to within an additive constant, since, as is well known, a function is only specified by its total differential to within an additive constant.  

To justify the term " generating function," we must show how to actually find the canonical transformation correspondi ng to a given generating function $\Phi$ <1.>. This is easily done. Writing (38) in the form  

we find that 8  

$$
d\Phi=\ \sum_{i=1}^{n}p_{i}d y_{i}-\ \sum_{i=1}^{n}P_{i}d Y_{i}+(H^{*}-H)d x,
$$  

$$
p_{i}=\frac{\partial\Phi}{\partial y_{i}},\qquadP_{\mathrm{\ell}}=\frac{\partial\Phi}{\partial Y_{\mathrm{\ell}}},\qquadH^{*}=H+\frac{\partial\Phi}{\partial x}.
$$  

Then (39) is precisely the desired canonical transformation. In fact, the $2n+1$ equations (39) establish the connection between the old variables $y_{i},p_{i}$ and the new variables $Y_{i},P_{i},$ and they also give an expression for the new Hamiltonian $H^{*}$ . Moreover, it is obvious that (39) satisfies the condition (38), so that the transformation (3 8) is indeed canonical. If the generating function $\Phi$ does not depend on $x$ explicitly, then $H^{*}=H$ . In this case, to obtain the new Hamiltonian $H^{*}$ , we need only replace $y_{i}$ and $\pmb{p_{i}}$ i n $H$ by their expressions in terms of $\smash{\ensuremath{Y_{i}}}$ and $\pmb{P_{i}}$ . 9  

In writing (39), we assumed that the generating function is specified as a function of $x$ , the old variables $y_{i}$ and the new variables $Y_{i}$ :  

$$
\Phi=\Phi(x,y_{1},...,y_{n},Y_{1},...,Y_{n}).
$$  

It may be more convenient to express the generating function in terms of $y_{i}$ and $P_{i}$ instead of $y_{i}$ and $Y_{i}$ . To this end, we rewrite (38) in the form  

$$
d\left(\Phi+\sum_{i=1}^{n}P_{i}Y_{i}\right)=\sum_{i=1}^{n}p_{i}d y_{i}+\sum_{i=1}^{n}Y_{i}d P_{i}+(H^{*}-H)d x,
$$  

thereby obtaining a new generating function  

$$
\Phi+\sum_{i=1}^{n}P_{i}Y_{i},
$$  

which is to be regarded as a function of the variables $x,y_{i}$ and $\pmb{P}_{i}$ . Denoting (40) by $\Psi(x,y_{1},...,y_{n},P_{1},...,P_{n})$ , we can write the corresponding canon­ ical transformation in the form  

$$
p_{i}={\frac{\partial\Psi}{\partial y_{i}}},\qquadY_{i}={\frac{\partial\Psi}{\partial P_{i}}},\qquadH^{*}=H+{\frac{\partial\Psi}{\partial x}}.
$$  

# 20. Noether's Theorem  

In Sec. 17 we proved that the system of Euler equations corresponding to the functional  

$$
\int_{a}^{b}F(y_{1},\ .\ ..,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})d x,
$$  

where $F$ does not depend on $x$ explicitly, has the first integral  

$$
H=-F+\sum_{i=1}^{n}y_{i}^{\prime}{\cal F}_{y_{i}^{\prime}}.
$$  

I t s clear that the statement " $F$ does not depend on $x$ explicitly " i s equivalent to the statement ${}^{*}F_{:}$ , and hence the integral (42), remains the same if we replace $x$ by the new variable  

$$
x^{*}=x+\mathfrak{e},
$$  

where e: is an arbitrary constant. " It follows that $H$ i s a first integral of the system of Euler equations corresponding to the functional (42) if and only if (42) is invariant under the transformation (43). 10  

We now show that even in the general case, there is a connection between the existence of certain first integrals of a system of Euler equations and the invariance of the corresponding functional under certain transformations of the variables x, Yl, . . $x,y_{1},\ldots,y_{n}$ ' We begin by defining more precisely what is meant by the invariance of a functional under some set of transformations. Suppose we are given a functional  

$$
J[y_{1},...,y_{n}]=\int_{z_{0}}^{z_{1}}F(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})d x,
$$  

which we write in the concise form  

$$
J[y]=\int_{z_{0}}^{z_{1}}F(x,y,y^{\prime})d x,
$$  

where now $y$ indicates the $\pmb{n}$ -dimensional vector $(y_{1},...,y_{n})$ and $y^{\prime}$ the $\pmb{n}$ -dimensional vector $(y_{1}^{\prime},...,y_{n}^{\prime})$ . Consider the transformation  

$$
\begin{array}{r l}&{x^{*}=\Phi(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})\ =\Phi(x,y,y^{\prime}),}\\ &{y_{i}^{*}=\Psi_{i}(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})=\Psi_{i}(x,y,y^{\prime}),}\end{array}
$$  

where $i=1,...,n.$ The transformation (45) carries the curve $\upgamma$ , with the vector equation  

$$
y=y(x)\qquad(x_{0}\leqslant x\leqslant x_{1}),
$$  

into another curve $\upgamma^{\ast}$ . In fact, replacing $y,y^{\prime}$ in (45) by $y(x),y^{\prime}(x)$ , and eliminating $x$ from the resulting $\boldsymbol{n}+\boldsymbol{1}$ equations, we obtain the vector equation  

$$
y^{*}=y^{*}(x^{*})\qquad(x_{0}^{*}\leqslant x^{*}\leqslant x_{1}^{*})
$$  

for $\upgamma^{\ast}$ , where $y^{*}=(y_{1}^{*},...,y_{n}^{*})$ .  

DEFINITION. The functional (44) is said to be invariant under the transformation (45) i $J[\gamma^{*}]=J[\gamma]$ , i . e . , if  

$$
\int_{x_{0}^{*}}^{x_{1}^{*}}F\left(x^{*},y^{*},{\frac{d y^{*}}{d x^{*}}}\right)d x^{*}=\int_{x_{0}}^{x_{1}}F\left(x,y,{\frac{d y}{d x}}\right)d x.
$$  

10 The fact that $\pmb{H}$ is a first integral only if (42) is invariant under the transformation (43) follows from the formula  

$$
{\frac{d H}{d x}}={\frac{\partial H}{\partial x}}
$$  

(see footnote 4, p. 70), since $\partial H/\partial x=0$ only if $\partial F/\partial x=0.$ .  

1 1 To avoid confusion in what follows, the reader should note that the subscripts can play two different roles ; when indexing $_x$ , they refer to different values, while when indexing $y_{;}$ , they refer to different functions. For example, the $y_{i}^{*}$ are new functions, while $x_{0}^{*}$ and $x_{1}^{*}$ are the new positions of the end points of the interval $[x_{0},x_{1}]$ .  

Example 1. The functional  

$$
J[y]=\int_{x_{0}}^{x_{1}}y^{\prime2}d x
$$  

is invariant under the transformation  

$$
x^{*}=x+\mathfrak{e},\qquady^{*}=y,
$$  

where E s an arbitrary constant. In fact, given a curve $\upgamma$ with equation  

$$
y=y(x)\qquad(x_{0}\leqslant x\leqslant x_{1}),
$$  

the " transformed " curve $\upgamma^{\ast}$ , i.e., the curve obtained from $\upgamma$ by shifting it a distance E long the $x$ -axis, has the equation  

$$
y^{*}=y(x^{*}-\mathfrak{c})=y^{*}(x^{*})\qquad(x_{0}+\mathfrak{c}\leqslant x^{*}\leqslant x_{1}+\mathfrak{c}),
$$  

and then  

$$
\begin{array}{l}{{J[\gamma^{*}]=\displaystyle\int_{x_{0}^{*}}^{x_{1}^{*}}\left[\frac{d y^{*}(x^{*})}{d x^{*}}\right]^{2}d x^{*}=\displaystyle\int_{x_{0}+\varepsilon}^{x_{1}+\varepsilon}\left[\frac{d y(x^{*}-\varepsilon)}{d x^{*}}\right]^{2}d x^{*}}}\\ {{\displaystyle=\int_{x_{0}}^{x_{1}}\left[\frac{d y(x)}{d x}\right]^{2}d x=J[\gamma].}}\end{array}
$$  

Example 2. The integral  

$$
J[y]=\int_{x_{0}}^{x_{1}}x y^{\prime2}d x
$$  

is an example of a functional which is not invariant under the transformation (46). In fact, carrying out the same calculations as in Example 1 ,  we obtain  

$$
\begin{array}{l}{{J[\gamma^{*}]=\displaystyle\int_{x_{0}^{*}}^{z_{1}^{*}}x^{*}\left[\frac{d y^{*}(x^{*})}{d x^{*}}\right]^{2}d x^{*}=\displaystyle\int_{x_{0}+\varepsilon}^{x_{1}+\varepsilon}x^{*}\left[\frac{d y(x^{*}-\varepsilon)}{d x^{*}}\right]^{2}d x^{*}}}\\ {{=\displaystyle\int_{x_{0}}^{z_{1}}\left(x+\varepsilon\right)\left[\frac{d y(x)}{d x}\right]^{2}d x=J[\gamma]+\varepsilon\displaystyle\int_{x_{0}}^{z_{1}}\left[\frac{d y(x)}{d x}\right]^{2}d x\neq J[\gamma].}}\end{array}
$$  

Suppose now that we have a family of transformations  

$$
\begin{array}{r}{x^{*}=\Phi(x,y,y^{\prime};\mathfrak{s}),}\\ {y_{i}^{*}=\Psi_{i}(x,y,y^{\prime};\mathfrak{s}),}\end{array}
$$  

depending on a parameter E, where the functions $\Phi$ and $\Psi_{i}(i=1,...,n)$ are differentiable with respect to E, and the value $\mathfrak{s}=0$ corresponds to the identity transformation :  

$$
\begin{array}{c}{{\Phi(x,y,y^{\prime};0)=x,}}\\ {{\Psi_{i}(x,y,y^{\prime};0)=y_{i}.}}\end{array}
$$  

Then we have the following result :  

THEOREM (Noether). If the functional  

$$
J[y]=\int_{x_{0}}^{x_{1}}F(x,y,y^{\prime})d x
$$  

is invariant under the family of transformations (47) for arbitrary $\scriptstyle x_{0}$ and $x_{1},$ then  

$$
\sum_{i=1}^{n}F_{y_{i}^{\prime}}\Psi_{i}+\left(F-\sum_{i=1}^{n}y_{i}^{\prime}F_{y_{i}^{\prime}}\right)\varphi=\mathrm{const}
$$  

along each extremal of $J[y]$ , where  

$$
\begin{array}{l}{\displaystyle\varphi(x,y,y^{\prime})=\frac{\partial\Phi(x,y,y^{\prime};\varepsilon)}{\partial\varepsilon}\biggm\vert_{\varepsilon=0},}\\ {\displaystyle\psi_{i}(x,y,y^{\prime})=\frac{\partial\Psi_{i}(x,y,y^{\prime};\varepsilon)}{\partial\varepsilon}\biggm\vert_{\varepsilon=0}.}\end{array}
$$  

In other words, every one-parameter family of transformations leaving $J[y]$ invariant leads to a first integral of its system of Euler equations.  

Proof Suppose e is a small quantity. Then, by Taylor's theorem, we have 12  

$$
\begin{array}{r l}&{x^{*}=\Phi(x,y,y^{\prime};\mathfrak{e})\ =\Phi(x,y,y^{\prime};0)+\mathfrak{e}\ \frac{\partial\Phi(x,y,y^{\prime};\mathfrak{e})}{\partial\mathfrak{e}}\ \Big|_{\mathfrak{e}=0}+o(\mathfrak{e}),}\\ &{y_{i}^{*}=\Psi_{\mathfrak{i}}(x,y,y^{\prime};\mathfrak{e})=\Psi_{\mathfrak{i}}(x,y,y^{\prime};0)+\mathfrak{e}\frac{\partial\Psi_{\mathfrak{i}}(x,y,y^{\prime};\mathfrak{e})}{\partial\mathfrak{e}}\Big|_{\mathfrak{e}=0}+o(\mathfrak{e}),}\end{array}
$$  

or using (48) and (5 1 ),  

$$
\begin{array}{r}{x^{*}=x+\mathfrak{e}\varphi(x,y,y^{\prime})\ +\ o(\mathfrak{e}),}\\ {y_{i}^{*}=y_{i}+\mathfrak{e}\Psi_{i}(x,y,y^{\prime})+o(\mathfrak{e}).}\end{array}
$$  

Assuming that the curve  

$$
y_{\mathfrak{i}}=y_{\mathfrak{i}}(x)\qquad(1\leqslant i\leqslant n)
$$  

is an extremal of $J[y]$ , we can use formula ( I I ) of Sec. 1 3 to write an expression for the variation of $J[y]$ corresponding to the transformation (52). Since in the present case 1 3  

$$
\updelta x=\upvarepsilon\uprho,\updelta y_{\mathsf{i}}=\upvarepsilon\updownarrow_{i},
$$  

the result is  

$$
\delta J=\varepsilon\bigg[\sum_{i=1}^{n}F_{y_{i}^{\prime}}\psi_{i}+\bigg(F-\sum_{i=1}^{n}y_{i}^{\prime}F_{y_{i}^{\prime}}\bigg)\varphi\bigg]_{x=x_{0}}^{x=x_{1}}.
$$  

Since by hypothesis, $J[y]$ is invariant under (52), $\updelta J$ vanishes, i . e . ,  

$$
\begin{array}{r l}{\lefteqn{\bigg[\sum_{i=1}^{n}F_{y_{i}^{*}}\big\forall_{i}+\bigg(F-\sum_{i=1}^{n}y_{i}^{\prime}F_{y_{i}^{*}}\bigg)\big\forall\bigg]_{z=z_{0}}}\quad}&{}\\ &{=\bigg[\sum_{i=1}^{n}F_{y_{i}^{*}}\big\forall_{i}+\bigg(F-\sum_{i=1}^{n}y_{i}^{\prime}F_{y_{i}^{*}}\bigg)\big\triangledown\bigg]_{z=z_{1}}}\end{array}
$$  

The fact that (50) holds along each extremal now follows from the arbitrariness of $x_{0}$ and $x_{1}$ '  

Remark. In terms of the canonical variables $p_{i}$ and $H$ , equation (50 becomes simply  

$$
\sum_{i=1}^{n}p_{i}\psi_{i}-H\varphi=\mathrm{const.}
$$  

Example 3. Consider the functional  

$$
J[y]=\int_{x_{0}}^{x_{1}}F(y,y^{\prime})d x,
$$  

whose integrand does not depend on $x$ explicitly. Then, by exactly the same argument as given in Example $1,J[y]$ is invariant u nder the one­ parameter family of transformations  

$$
x^{*}=x+\mathfrak{e},\qquady_{i}^{*}=y_{i}.
$$  

In this case,  

$$
\varphi=1,\qquad\psi_{i}=0,
$$  

and (53) reduces to just  

$$
H=\mathrm{const},
$$  

i.e., the Hamiltonian $H$ is constant along each extremal of $J[y]$ . Thus, we again obtain a result already proved in Sec. 1 7 :  For a functional of the form (54), which does not depend on $x$ explicitly, the Hamiltonian is a first integral of the system of Euler equations.  

# 2 1 .  The Pri nci p l e of Least Act i o n  

We now apply the general results obtained in the preceding sections to some mechanical problems. Suppose we are given a system of $\pmb{n}$ particles (mass points), where no constraints whatsoever are imposed on the system. Let the ith particle have m ass $m_{i}$ and coordinates $x_{i},y_{i},z_{i}$ $(i=1,...,n)$ . Then the kinetic energy of the system is 14  

$$
T={\frac{1}{2}}\sum_{i=1}^{n}m_{i}(\dot{x}_{i}^{2}+\dot{y}_{i}^{2}+\dot{z}_{i}^{2}).
$$  

We assume that the system has potential energy $U$ , i.e., that there exists a function  

$$
U=U(t,x_{1},y_{1},z_{1},...,x_{n},y_{n},z_{n})
$$  

such that the force acting on the ith particle has components  

$$
X_{\mathfrak{i}}=-{\frac{\partial U}{\partial x_{\mathfrak{i}}}},\quad Y_{\mathfrak{i}}=-{\frac{\partial U}{\partial y_{\mathfrak{i}}}},\quad Z_{\mathfrak{i}}=-{\frac{\partial U}{\partial z_{\mathfrak{i}}}}.
$$  

Next, we introduce the expression  

$$
L=T-U, 
$$  

called the Lagrangian (function) of the system of particles. Obviously, $L$ is a function of the time $t$ ana of the positions $(x_{i},y_{i},z_{i})$ and velocities $({\dot{x}}_{i},{\dot{y}}_{i},{\dot{z}}_{i})$ of the $\pmb{n}$ particles in the system.  

Suppose that at time $t_{0}$ the system is in some fixed position. Then the subsequent evolution of the system in time is described by a curve  

$$
x_{i}=x_{i}(t),y_{i}=y_{i}(t),z_{i}=z_{i}(t)(i=1,...,n)
$$  

in a space of $3n$ dimensions. It can be shown that among all curves passing through the point corresponding to the initial position of the system, the curve which actually describes the motion of the given system, under the influence of the forces acting upon it, satisfies the following condition, known as the principle of least action :  

THEOREM. The motion of a system of $\pmb{n}$ particles during the time interval $[t_{0},t_{1}]$ is described by those functions $x_{i}(t),y_{i}(t),z_{i}(t),1\leqslant i\leqslant n,$ for which the integral  

$$
\int_{t_{0}}^{t_{1}}L d t,
$$  

called the action, is a minimum.  

Proof We show that the principle of least action implies the usual equations of motion for a system of $\pmb{n}$ particles. If the functional (59) has a minimum, then the Euler equations  

$$
\begin{array}{r l r}{\displaystyle\frac{\partial L}{\partial x_{i}}-\frac{d}{d t}\frac{\partial L}{\partial\dot{x}_{i}}=0\mathrm{,}}&\\ {\displaystyle\frac{\partial L}{\partial y_{i}}-\frac{d}{d t}\frac{\partial L}{\partial\dot{y}_{i}}=0\mathrm{,}}&\\ {\displaystyle\frac{\partial L}{\partial z_{i}}-\frac{d}{d t}\frac{\partial L}{\partial\dot{z}_{i}}=0}&\end{array}
$$  

must be satisfied for $i=1,\ldots,n.$ Bearing in mind that the potential energy $U$ depends only on t, $x_{i},y_{i},z_{i},$ and not on $\dot{x}_{i},\dot{y}_{i},\dot{z}_{i},$ while $T$ is a  

sum of squares of the velocity components $\dot{x}_{i},\dot{y}_{i},\dot{z}_{i}$ (with coefficients $\scriptstyle{\frac{1}{2}}m_{i})$ , we can write the equations (60) in the form  

$$
\begin{array}{c}{{\displaystyle-\frac{\partial U}{\partial x_{i}}-\frac{d}{d t}m_{i}\dot{x}_{i}=0,}}\\ {{\displaystyle-\frac{\partial U}{\partial y_{i}}-\frac{d}{d t}m_{i}\dot{y}_{i}=0,}}\\ {{\displaystyle-\frac{\partial U}{\partial z_{i}}-\frac{d}{d t}m_{i}\dot{z}_{i}=0.}}\end{array}
$$  

Finally, since the derivatives  

$$
-{\frac{\partial U}{\partial x_{i}}},\quad-{\frac{\partial U}{\partial y_{i}}},\quad-{\frac{\partial U}{\partial z_{i}}}
$$  

are the components of the force acting on the ith particle, the system (6 1 ) reduces to  

$$
\begin{array}{c}{{m_{i}\ddot{x}_{i}=X_{i},}}\\ {{m_{i}\ddot{y}_{i}=Y_{i},}}\\ {{m_{i}\ddot{z}_{i}=Z_{i},}}\end{array}
$$  

which are just Newton's equations of motion for a system of $\pmb{n}$ particles, subject to no constraints.  

Remark 1 .  The principle of least action remains valid in the case where the system of particles is subject to constraints, except that then the admissible curves, for which the functional (59) is considered, have to satisfy the con­ straints. In other words, in this case, application of the principle of least action leads to a variational problem with subsidiary conditions.  

Remark 2. Actually, as we shall see later (Sec. 36.2), the principle of least action only holds for sufficiently small time intervals $[t_{0},t_{1}]$ , and has to be modified for continuous mechanical systems.  

# 22. Conservation Laws  

We have just seen that the equations of motion of a mechanical system consisting of $\pmb{n}$ particles, with kinetic energy (56), potential energy (57) and Lagrangian (58), can be obtained from the principle of least action, i.e., by minimizing the integral  

$$
\int_{t_{0}}^{t_{1}}L d t=\int_{t_{0}}^{t_{1}}\left(T-U\right)d t.
$$  

The canonical variables corresponding to the functional (62) turn out to be  

$$
\begin{array}{c c c}{{p_{i z}=\displaystyle\frac{\partial{\cal L}}{\partial\dot{x}_{i}}=m_{i}\dot{x}_{i},}}\\ {{{}}}&{{}}\\ {{p_{i y}=\displaystyle\frac{\partial{\cal L}}{\partial\dot{y}_{i}}=m_{i}\dot{y}_{i},}}\\ {{{}}}&{{}}\\ {{p_{i z}=\displaystyle\frac{\partial{\cal L}}{\partial\dot{z}_{i}}=m_{i}\dot{z}_{i},}}\end{array}
$$  

which are just the components of the momentum of the ith particle. 15 In terms of $p_{i z},p_{i y}$ and $p_{i z}$ we have  

$$
H=\sum_{i=1}^{n}\left(\dot{x}_{i}p_{1x}+\dot{y}_{i}p_{i y}+\dot{z}_{i}p_{i z}\right)-L=2T-\left(T-U\right)=T+U,
$$  

S O  that $H$ i s the total energy o f the system.  

Using the form of the ntegrand in (62), we can find various functions which maintain constant values along each trajectory of the system, thereby obtaining so-called conservation laws.  

1 . Conservation of energy. Suppose the given system is conservative, which means that the Lagrangian $L$ (or more precisely, the potential energy $U$ ) does not depend on time explicitly. Then, as shown in Sec. 1 7 (see also Sec. 20, Example 3), $H=$ const along each extremal, i.e., the total energy of a conservative system does not change during the motion of the system.  

2. Conservation ofmomentum. First, we recall that according to Noether's theorem (Sec. 20), invariance of the functional (49) under the family of transformations  

$$
\begin{array}{l}{{x^{*}=\Phi(x,y,y^{\prime};\varepsilon)=x,}}\\ {{y_{i}^{*}=\Psi_{i}(x,y,y^{\prime};\varepsilon)}}\end{array}
$$  

implies that the corresponding system of Euler equations has the first integral  

$$
\sum_{i=1}^{n}F_{y_{i}^{\prime}}\Psi_{i}=\mathrm{const},
$$  

where  

$$
\Psi_{i}(x,y,y^{\prime})=\frac{\partial\Psi_{i}(x,y,y^{\prime};\boldsymbol{\mathfrak{e}})}{\partial\boldsymbol{\mathfrak{e}}}\Bigg\rvert_{\varepsilon=0},
$$  

since in this case,  

$$
\begin{array}{l}{\displaystyle\varphi(x,y,y^{\prime})=\frac{\partial\Phi(x,y,y^{\prime};\boldsymbol{\mathfrak{e}})}{\partial\boldsymbol{\mathfrak{e}}}\bigg\vert_{\boldsymbol{\varepsilon}=0}=0.}\end{array}
$$  

Therefore, the invariance of the functional (62) under the transformation  

$$
x_{i}^{*}=x_{i}+\varepsilon,\qquady_{i}^{*}=y_{i},\qquadz_{i}^{*}=z_{i}
$$  

implies that  

i . e . ,  

$$
\begin{array}{c}{{\displaystyle\sum_{i=1}^{n}\frac{\partial{\cal L}}{\partial\dot{x}_{i}}=\mathrm{const},}}\\ {{\displaystyle\sum_{i=1}^{n}p_{i x}=\mathrm{const}.}}\end{array}
$$  

Similarly, it follows from the invariance of (62) under displacements along the $y.$ -axis that  

$$
\sum_{i=1}^{n}p_{i y}=\mathrm{const},
$$  

and from the invariance o f (62) under displacements along the $z$ -axis that  

$$
\sum_{i=1}^{n}p_{i z}=\mathrm{const.}
$$  

The vector $\mathbf{P}$ with components  

$$
P_{x}=\sum_{i=1}^{n}p_{i x},\qquadP_{y}=\sum_{i=1}^{n}p_{i y},\qquadP_{z}=\sum_{i=1}^{n}p_{i z}
$$  

i s called the total momentum of the system. Thus, w e have just proved that the total momentum is conserved dt;ring the motion of the system if the integral (62) is invariant under parallel displacements. [It is clear from these considerations that the invariance of (62) under displace­ ments along any coordinate axis, e.g. , along the $x$ -axis, i mplies that the corresponding component of the total momentum is conserved.]  

3. Conservation of angular momentum. Suppose the integral (62) is invariant under rotations about the $z$ -axis, i.e., under coordinate transformations of the form  

$$
\begin{array}{l}{x_{i}^{*}=x_{i}\cos\tt{\tt{\tt{t}}}+y_{i}\sin\tt{\tt{\tt t}},}\\ {y_{i}^{*}=-x_{i}\sin\tt{\tt{\tt{t}}}+y_{i}\cos\tt{\tt{\tt{t}}},}\\ {z_{i}^{*}=z_{i}.}\end{array}
$$  

In this case,  

$$
\begin{array}{l}{\displaystyle{\Psi_{i x}=\frac{\partial x_{i}^{*}}{\partial\varepsilon}\bigg\vert_{\varepsilon=0}=y_{i},}}\\ {\displaystyle{\Psi_{i y}=\frac{\partial y_{i}^{*}}{\partial\varepsilon}\bigg\vert_{\varepsilon=0}=-x_{i},}}\\ {\displaystyle{\Psi_{i z}=\frac{\partial z_{i}^{*}}{\partial\varepsilon}\bigg\vert_{\varepsilon=0}=0,}}\end{array}
$$  

and hence Noether's theorem implies that  

$$
\sum_{i=1}^{n}\left(\frac{\partial L}{\partial\dot{x}_{i}}y_{i}-\frac{\partial L}{\partial\dot{y}_{i}}x_{i}\right)=\mathrm{const},
$$  

i . e . ,  

$$
\sum_{i=1}^{n}{\bigl(}p_{\imath\tau}y_{i}-p_{i y}x_{i}{\bigr)}={\mathrm{const.}}
$$  

Each term in this sum represents the $z$ -component of the vector product $\pmb{\mathrm{p}}_{\mathrm{:}}\times\pmb{\mathrm{r}}_{\mathrm{:}}$ , where $\mathbf{r}_{i}=(x_{i},y_{i},z_{i})$ is the position vector and $\mathbf{p}_{i}=(p_{i x},p_{i y},p_{i z})$ the momentum of the ith particle. The vector $\mathbf{p}_{i}\times\mathbf{r}_{i}$ is called the angular momentum of the ith particle, about the origin of coordinates, and (63) means that the sum of the z-components of the angular momenta of the separate particles, i.e., the $z.$ -component of the total angular momentum (of the whole system) is a constant. Similar asser­ tions hold for the $x$ and $y.$ -components of the total angular momentum, provided that the integral (62) is invariant under rotations about the $x$ and $y$ -axes. Thus, we have proved that the total angular momentum does not change during the motion of the system if (62) is invariant under all rotations.  

Example 1. Consider the motion of a particle which is attracted to a fixed point, according to some law. In this case, energy is conserved, since $L$ is time-invariant, and angular momentum is also conserved, since $L$ is invariant under rotations. However, momentum is not conserved during the motion of the particle.  

Example 2. A particle is attracted to a homogeneous linear mass distri bution lying along the $z$ -axis. In this case, the following quantities are conserved :  

l .  The energy (since $L$ is independent of time) ;   
2. The $z$ -component of the momentum ;   
3. The z-component of the angular momentum.  

# 23. The Ham i l ton-J acobi Eq u at i o n . J aco b i ' s Theore m 1 6  

Consider the functional  

$$
J[y]=\int_{x_{0}}^{x_{1}}F(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})d x
$$  

defined on the curves lying in some region $R$ , and suppose that one and only one extremal of (64) goes through two arbitrary points $A$ and $B$ . The integral  

$$
S=\int_{x_{0}}^{x_{1}}F(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})d x
$$  

evaluated along the extremal joining the points  

$$
A=(x_{0},y_{1}^{0},...,y_{n}^{0}),\qquadB=(x_{1},y_{1}^{1},...,y_{n}^{1})
$$  

is called the geodetic distance between $A$ and $B$ . The quantity $s$ is obviously a single-valued function of the coordinates of the points $A$ and $B$ .  

Example 1. If the functional $J$ is arc length, $s$ is the distance (in the usual sense) between the points $A$ and $B$ .  

Example 2. Consider the propagation of light in an inhomogeneous and anisotropic medium, where it is assumed that the velocity of light at any point depends both on the coordinates of the point and on the direction of propagation, i.e.,  

$$
v=v(x,y,z,\dot{x},\dot{y},\dot{z}).
$$  

The time it takes light to go from one point to another along some curve  

$$
x=x(t),\qquady=y(t),\qquadz=z(t)
$$  

i s given b y the integral  

$$
T=\int_{t_{0}}^{t_{1}}{\frac{\sqrt{{\dot{x}}^{2}+{\dot{y}}^{2}+{\dot{z}}^{2}}}{v}}d t.
$$  

According to Fermat's principle, light propagates in any medium along the curve for which the transit time $T$ is smallest, i.e. , along the extremal of the functional (67). Thus, for the functional (67), $s$ is the time it takes light to go from the point $A$ to the point $B$ .  

Example 3. Consider a mechanical system with Lagrangian $L$ . According to Sec. 2 1 ,  the integral  

$$
\int_{t_{0}}^{t_{1}}L(t,x_{1},y_{1},z_{1},...,x_{n},y_{n},z_{n})d t
$$  

evaluated along the extremal passing through two given points, i.e. , two configurations of the system, is the " least action " corresponding to the motion of the system from the first configuration to the second.  

I ft h e nitial point $A$ is regarded as fixed and the final point $B=(x,y_{1},...,y_{n})$ is regarded as variable, 1 7 then in the region $R$ ,  

$$
S=S(x,y_{1},...,y_{n})
$$  

is a single-valued function of the coordinates of the point $B$ . We now derive a differential eq uation satisfied by the function (68). We first calculate the partial derivatives  

$$
{\frac{\partial S}{\partial x}},\quad{\frac{\partial S}{\partial y_{\mathrm{i}}}}\qquad(i=1,\ldots,n),
$$  

by writing down the total differential of the function $s$ , i . e . , the principal linear part of the increment  

$$
\Delta S=S(x+d x,y_{1}+d y_{1},...,y_{n}+d y_{n})-S(x,y_{1},...,y_{n}).
$$  

Since, by definition, $\Delta s$ is the difference  

$$
J[\gamma^{*}]-J[\gamma],
$$  

where $\upgamma$ is the extremal going from $A$ to the point $(x,y_{1},....,y_{n})$ and $\upgamma^{\ast}$ is the extremal going from $A$ to the point $(x+d x,y_{1}+d y_{1},...,y_{n}+d y_{n})$ , we have  

$$
d S=\ \delta J,
$$  

where the " unvaried " curve is the extremal $\upgamma$ and the initial point $\pmb{A}$ is held fixed. (The fact that the " varied " curve $\upgamma^{\ast}$ is also an extremal is not important here.)  

Thus, using formula ( 1 2) of Sec. 13 for the general variation of a functional, we obtain  

$$
d S(x,y_{1},...,y_{n})=\vartheta J=\sum_{i=1}^{n}p_{i}d y_{i}-H d x,
$$  

where (69) is evaluated at the point $B.$ . It follows that  

$$
{\frac{\partial S}{\partial x}}=-H,{\frac{\partial S}{\partial y_{i}}}=p_{i},
$$  

where  

$$
p_{i}=p_{i}(x,y_{1},...,y_{n})=F_{y_{1}}[x,y_{1},...,y_{n},y_{1}^{\prime}(x),...,y_{n}^{\prime}(x)]
$$  

and  

$$
H=H[x,y_{1},...,y_{n},p_{1}(x,y_{1},...,y_{n}),...,p_{n}(x,y_{1},...,y_{n})]
$$  

are functions of $x,y_{1},\ldots,y_{n}$ . Then from (70) we find that $s,$ , as a function of the coordinates of the point $B$ , satisfies the equation  

$$
{\frac{\partial S}{\partial x}}+H\left(x,y_{1},...,y_{n},{\frac{\partial S}{\partial y_{1}}},...,{\frac{\partial S}{\partial y_{n}}}\right)=0.
$$  

The partial differential equation (72), which is in general nonlinear, is called the Hamilton-Jacobi equation. There is an intimate connection between the Hamilton-Jacobi equation and the canonical Euler equations. In fact, the canonical equations represent the so-called characteristic system associated with equation (72). 19 We shall approach this matter from a somewhat different point of view, by establishing a connection between solutions of the Hamilton-Jacobi equation and first integrals of the system of Euler equations :  

THEOREM 1 . Let  

$$
S=S(x,y_{1},...,y_{n},\alpha_{1},...,\alpha_{m})
$$  

be a solution, depending on m $(\leqslant n)$ parameters $\alpha_{1},...,\alpha_{m}$ of the Hamilton-Jacobi equation (72). Then each derivative  

$$
\frac{\partial S}{\partial\alpha_{i}}\qquad(i=1,...,m)
$$  

is a first integral of the system of canonical Euler equations  

$$
\frac{d y_{i}}{d x}=\frac{\partial H}{\partial p_{i}},\frac{d p_{i}}{d x}=-\frac{\partial H}{\partial y_{i}},
$$  

i. e . ,  

$$
{\frac{\partial S}{\partial\alpha_{\mathrm{i}}}}=\mathrm{const}\qquad(i=1,\ldots,m)
$$  

along each extremal.  

Proof We have to show that  

$$
\frac{d}{d x}\left(\frac{\partial S}{\partial\alpha_{i}}\right)=0\qquad(i=1,...,m)
$$  

along each extremal. Calculating the left-hand side of (74), we find that  

$$
\frac{d}{d x}\left(\frac{\partial S}{\partial\alpha_{i}}\right)=\frac{\partial^{2}S}{\partial x\partial\alpha_{i}}+\ \sum_{k=1}^{n}\frac{\partial^{2}S}{\partial y_{k}\partial\alpha_{i}}\frac{d y_{k}}{d x}.
$$  

Substituting (73) into the Hamilton-Jacobi equation (72), and differentiating the result with respect to $\alpha_{i}$ , we obtain  

$$
\frac{\partial^{2}S}{\partial x\partial\pmb{\alpha}_{i}}=-\sum_{k=1}^{n}\frac{\partial H}{\partial p_{k}}\frac{\partial^{2}S}{\partial y_{k}\partial\pmb{\alpha}_{i}}.
$$  

Then substitution of (76) into (75) gives  

$$
\begin{array}{l}{\displaystyle\frac{d}{d x}\left(\frac{\partial S}{\partial\alpha_{i}}\right)=-\sum_{k=1}^{n}\frac{\partial H}{\partial p_{k}}\frac{\partial^{2}S}{\partial y_{k}\partial\alpha_{i}}+\sum_{k=1}^{n}\frac{\partial^{2}S}{\partial y_{k}\partial\alpha_{i}}\frac{d y_{k}}{d x}}\\ {=\sum_{k=1}^{n}\frac{\partial^{2}S}{\partial y_{k}\partial\alpha_{i}}\left(\frac{d y_{k}}{d x}-\frac{\partial H}{\partial p_{k}}\right).}\end{array}
$$  

Since  

$$
{\frac{d y_{k}}{d x}}-{\frac{\partial H}{\partial p_{k}}}=0\qquad(k=1,...,n)
$$  

along each extremal, it follows that (74) holds along each extremal, which proves the theorem.  

THEOREM 2 (Jacobi). Let  

$$
S=S(x,y_{1},...,y_{n},\alpha_{1},...,\alpha_{n})
$$  

be a complete integral of the Hamilton-Jacobi equation (72), i.e. , a general  

solution of (72) depending on n parameters $\alpha_{i},...,\alpha_{n}$ • Moreover, let the determinant of the $\textit{\textbf{n}}\times\textit{\textbf{n}}$ matrix  

$$
\left\|\frac{\partial^{2}S}{\partial\alpha_{i}\partial y_{k}}\right\|
$$  

be nonzero, and let $\beta_{1},...,\beta_{n}$ be $\pmb{n}$ arbitrary constants. Then the functions  

$$
y_{i}=y_{i}(x,\alpha_{1},...,\alpha_{n},\beta_{1},...,\beta_{n})(i=1,...,n)
$$  

defined by the relations  

$$
\frac{\partial}{\partial\alpha_{i}}S(x,y_{1},...,y_{n},\alpha_{1},...,\alpha_{n})=\beta_{i}(i=1,...,n),
$$  

together with the functions  

$$
p_{i}=\frac{\partial}{\partial y_{i}}S(x,y_{1},...,y_{n},\alpha_{1},...,\alpha_{n})(i=1,...,n),
$$  

where the $y_{\mathfrak{i}}$ are given by (79), constitute a general solution of the canonical system  

$$
{\frac{d y_{i}}{d x}}={\frac{\partial H}{\partial p_{i}}},{\frac{d p_{i}}{d x}}=-{\frac{\partial H}{\partial y_{i}}}\qquad(i=1,...,n).
$$  

Proof 1 .  According to Theorem I ,  the $\scriptstyle n$ relations (80) correspond to first integrals of the canonical system (82) . To obtain the general solution of (82), we first use (80) to define the $n$ functions (79) [this is possible since (78) has a nonvanishing determinant], and then use (8 1) to define the $\pmb{n}$ functions $p_{i}$ . To show that the functions $y_{i}$ and $p_{i}$ so defined actually satisfy the canonical equations (82), we argue as follows : Differentiating (80) with respect to $x.$ , where the $y_{i}$ are regarded as functions of $x$ [cf. (79) ] , we obtain  

$$
\frac{d}{d x}\left(\frac{\partial S}{\partial\alpha_{i}}\right)=\frac{\partial^{2}S}{\partial x\partial\alpha_{i}}+\sum_{k=1}^{n}\frac{\partial^{2}S}{\partial y_{k}\partial\alpha_{i}}\frac{d y_{k}}{d x}=\sum_{k=1}^{n}\frac{\partial^{2}S}{\partial y_{k}\partial\alpha_{i}}\Big(\frac{d y_{k}}{d x}-\frac{\partial H}{\partial p_{k}}\Big),
$$  

where in the last step we have used (76). Since the determinant of the matrix (78) is nonzero, it follows that  

$$
{\frac{d y_{i}}{d x}}={\frac{\partial H}{\partial p_{i}}}\qquad(i=1,...,n),
$$  

which is j ust the first set of equations (82) .  

Next, we differentiate (8 1 ) with respect to $x$ , obtaining  

$$
\frac{d p_{i}}{d x}=\frac{d}{d x}\left(\frac{\partial S}{\partial y_{i}}\right)=\frac{\partial^{2}S}{\partial x\partial y_{i}}+\sum_{k=1}^{n}\frac{\partial^{2}S}{\partial y_{k}\partial y_{i}}\frac{d y_{k}}{d x}=\frac{\partial^{2}S}{\partial x\partial y_{i}}+\sum_{k=1}^{n}\frac{\partial^{2}S}{\partial y_{k}\partial y_{i}}\frac{\partial H}{\partial p_{k}},
$$  

where we have used (83). Then, taking account of (8 1 )  and differ­ entiating the Hamilton-Jacobi equation (72) with respect to $y_{i}$ h we find that  

$$
\frac{\partial^{2}S}{\partial x\partial y_{i}}=-\frac{\partial H}{\partial y_{i}}-\mathrm{~\sum_{\boldsymbol{k}=1}^{\boldsymbol{n}}~}\frac{\partial H}{\partial p_{\boldsymbol{k}}}\frac{\partial^{2}S}{\partial y_{\boldsymbol{k}}\partial y_{i}}.
$$  

A comparison of the last two equations shows that  

$$
{\frac{d p_{\mathrm{i}}}{d x}}=-{\frac{\partial H}{\partial y_{\mathrm{i}}}}\qquad(i=1,\ldots,n),
$$  

which is j ust the second set of equations (82).  

Proof 2. Our second proof of Jacobi's theorem is based on the use of a canonical transformation. Let (77) be a complete integral of the Hamilton-Jacobi equation. We make a canonical transformation of the system (82), choosing the function (77) as the generating function, $\alpha_{1},\ldots,\alpha_{n}$ as the new momenta (cf. footnote 1 5, p. 86), and $\beta_{1},...,\beta_{n}$ as the new coordinates. Then, according to formula (4 1 )  of Sec. 1 9,  

$$
p_{i}=\frac{\partial S}{\partial y_{i}},\qquad\beta_{i}=\frac{\partial S}{\partial\alpha_{i}},\qquadH^{*}=H+\frac{\partial S}{\partial x}.
$$  

But since the function $s$ satisfies the Hamilton-Jacobi equation, we have  

$$
H^{*}=H+{\frac{\partial S}{\partial x}}=0.
$$  

Therefore, in the new variables, the canonical equations become  

$$
\frac{d\alpha_{i}}{d x}=0,\frac{d\beta_{i}}{d x}=0,
$$  

from which it follows that $\alpha_{i}=$ const, $\beta_{i}=$ const along ea{;h extremal. Thus, we again obtain the same $\pmb{n}$ first integrals  

$$
\frac{\partial S}{\partial\alpha_{i}}=\beta_{i}
$$  

of the system of Euler equations. If we now use these equations to de­ termine the functions (79) of the $2n$ parameters $\alpha_{1},\ldots,\alpha_{n},\beta_{1},\ldots,\beta_{n},$ ' and if, as before, we set  

$$
p_{i}={\frac{\partial}{\partial y_{i}}}S(x,y_{1},...,y_{n},\alpha_{1},...,\alpha_{n}),
$$  

where the $y_{i}$ are given by (79), we obtain $2n$ functions  

$$
\begin{array}{r}{y_{i}(x,\alpha_{1},...,\alpha_{n},\beta_{1},...,\beta_{n}),}\\ {p_{i}(x,\alpha_{1},...,\alpha_{n},\beta_{1},...,\beta_{n}),}\end{array}
$$  

which constitute a general solution of the canonical system (82).  

# PROBLEMS  

1. Use the canonical Euler equations to find the extremals of the functional  

$$
\int{\sqrt{x^{2}+y^{2}}}\ {\sqrt{1+y^{\prime2}}}\ d x,
$$  

and verify that they agree with those found in Chap. I ,  Prob. 22.  

Hint. The Hamiltonian is  

$$
H(x,y,p)=-\sqrt{x^{2}+y^{2}-p^{2}},
$$  

and the corresponding canonical system  

$$
{\frac{d p}{d x}}={\frac{y}{\sqrt{x^{2}+y^{2}-p^{2}}}},\frac{d y}{d x}={\frac{p}{\sqrt{x^{2}+y^{2}-p^{2}}}}
$$  

has the first integral  

$$
p^{2}-y^{2}=C^{2},
$$  

where $c$ is a constant.  

2. Consider the action functional  

$$
J[x]={\frac{1}{2}}\int_{t_{0}}^{t_{1}}\left(m{\dot{x}}^{2}-\varkappa x^{2}\right)d t
$$  

corresponding to a simple harmonic oscillator, i.e., a particle of mass m acted upon by a restoring force $-x x$ (cf. Sec. 36.2). Write the canonical system of Euler equations corresponding to $J[x],$ , and interpret them. Calcu­ late the Poisson brackets $[x,p],\ [x,H]$ and $[p,H]$ . Is $\pmb{p}$ a first integral of the canonical Euler equations ?  

3. Use the principle of least action to give a variational formulation of the problem of the plane motion of a particle of mass $\mathbf{\nabla}m$ attracted to the origin of coordinates by a force inversely proportional to the square of its distance from the origin. Write the corresponding equations of motion, the Hamil­ tonian and the canonical system of Euler equations. Calculate the Poisson brackets $[r,p_{r}],\ [\Theta,p_{\Theta}],\ [p_{r},H]$ and $[p_{\Theta},H],$ where  

$$
p_{r}=\frac{\partial L}{\partial\dot{r}},\qquadp_{\Theta}=\frac{\partial L}{\partial\dot{\Theta}}.
$$  

Is ${\pmb p}_{\pmb{\uptheta}}$ a first integral of the canonical Euler equations ?  

Hint. The action functional is  

$$
J[r,\theta]=\int_{t_{0}}^{t_{1}}\left[{\frac{m}{2}}(\dot{r}^{2}+r^{2}\dot{\theta}^{2})+\frac{k}{r}\right]d t,
$$  

where $\pmb{k}$ is a constant, and $r,\theta$ are the polar coordinates of the particle.  

4. Verify that the change of variables  

$$
Y_{\imath}=p_{\imath},~P_{\imath}=y_{\imath}
$$  

is a canonical transformation, and find the corresponding generating function.  

5. Verify that the fu nctional $J[r,0]$ of Prob. 3 is invariant u nder rotations, and use Noether's theorem (in polar coordinates) to find the corresponding conservation law. What geometric fact does this law express ?  

Ans. The line segment joining the particle to the origin sweeps out equal areas in equal times.  

6. Write and solve the Hamilton-Jacobi equation corresponding to the functional  

$$
J[y]=\int_{x_{0}}^{z_{1}}y^{\prime2}d x,
$$  

and use the result to determine the extremals of $J[y]$ .  

Ans. The Hamilton-Jacobi equation is  

$$
4\:\frac{\partial S}{\partial x}\:+\:\left(\frac{\partial S}{\partial y}\right)^{2}=0.
$$  

7. Write and solve the H amilton-Jacobi equation corresponding to the functional  

$$
J[y]=\int_{x_{0}}^{x_{1}}f(y){\sqrt{1+y^{'2}}}d x,
$$  

and use the result to find the extremals of $J[y]$ .  

Ans. The H amilton-Jacobi equation is  

$$
\left(\frac{\partial S}{\partial x}\right)^{2}+\left(\frac{\hat{c}S}{\hat{c}y}\right)^{2}=f^{2}(y),
$$  

with solution  

$$
S=\alpha x+\int_{y_{0}}^{y}\sqrt{f^{2}(\eta_{i})-\alpha^{2}}d\eta+\beta.
$$  

The extremals are  

$$
x\ -\ \alpha\int_{y_{0}}^{y}{\frac{d\eta}{\sqrt{f^{2}(\eta_{i})\ -\ \alpha^{2}}}}=\mathrm{const.}
$$  

8. Use the H amilton-Jacobi equation to find the extremals of the functional of Prob.  

Hint. Try a solution of the form $S={\scriptstyle{\frac{1}{2}}}(A x^{2}+2B x y+C y^{2})$ .  

9. What fu nct ional leads to the H amilton-Jacobi equation  

$$
\left({\frac{\partial S}{\hat{c}x}}\right)^{2}+\left({\frac{\partial S}{\partial y}}\right)^{2}=1?
$$  

10. Prove that the Hamilton-Jacobi equation can be solved by quadratures if it can be written in the form  

$$
\Phi\bigg(x,\frac{\partial S}{\partial x}\bigg)+\Psi^{\prime}\bigg(y,\frac{\partial S}{\partial y}\bigg)=0.
$$  

1 1 .  By a Liouville sur/ace is meant a surface on which the arc-length functional has the form  

$$
J[y]=\int_{x_{0}}^{x_{1}}\sqrt{\varphi_{1}(x)+\varphi_{2}(y)}\sqrt{1+y^{\prime2}}d x.
$$  

Prove that the equations of the geodesics on such a surface are  

$$
\int\frac{d x}{\sqrt{\varphi_{1}(x)\mathrm{~-~}\alpha}}-\int\frac{d y}{\sqrt{\varphi_{2}(y)\mathrm{~+~}\alpha}}=\beta,
$$  

where $\alpha$ and $\beta$ are constants. Show that surfaces of revolution are Liouville surfaces.  

5  

# THE SE COND VARIATION. SUFFI CIENT CONDITIONS FOR A WEAK EXTREMUM  

Until now, i n studying extrema o f functionals, w e have only considered a particular necessary condition for a functional to have a weak (relative) extremum for a given curve $\upgamma$ , i.e. , the condition that the variation of the functional vanish for the curve $\upgamma$ . In this chapter, we shall derive sufficient conditions for a functional to have a weak extremum. To find these sufficient conditions, we must first introduce a new concept, namely, the second variation of a functional. We then study the properties of the second varia­ tion, and at the same time, we derive some new necessary conditions for an extremum.  

As will soon be apparent, there exist sufficient conditions for an extremum which resemble the necessary conditions and are easy to apply. These sufficient conditions differ from the necessary conditions (also derived in this chapter) in much the same way as the sufficient conditions $y^{\prime}=0$ , $y^{\prime\prime}>0$ for a function of one variable to have a minimum differ from the corresponding necessary conditions $y^{\prime}=0$ , $y^{\prime\prime}\geqslant0$ .  

# 24. Quad ratic F u n ctionals. The Seco n d Variation of a F u n ctional  

W e begin b y introducing some general concepts that will b e needed later. A functional $B[x,y]$ depending on two elements $x$ and $y$ , belonging to some  

normed linear space $\mathcal{R}$ , is said to be bilinear if it is a linear functional of $y$ for any fixed $x$ and a linear functional of $x$ for any fixed $y$ (cf. p. 8). Thus,  

and  

$$
\begin{array}{c}{{B[x+y,z]=B[x,z]+B[y,z],}}\\ {{B[\alpha x,y]=\alpha B[x,y],}}\\ {{{}}}\\ {{B[x,y+z]=B[x,y]+B[x,z],}}\\ {{B[x,\alpha y]=\alpha B[x,y]}}\end{array}
$$  

for any $x,y,z\in{\mathcal{R}}$ and any real number $\alpha$ .  

If we set $y=x$ in a bilinear functional, we obtain an expression called a quadratic functional. A quadratic functional $A[x]=B[x,x]$ is said to be positive definitel if $A[x]>0$ for every nonzero element $x$ .  

A bilinear functional defined on a finite-dimensional space is called a bilinear form. Every bilinear form $B[x,y]$ can be represented as  

$$
B[x,y]=\sum_{i,k=1}^{n}b_{i k}\xi_{i}\eta_{k},
$$  

where $\xi_{1},...,\xi_{n}$ and $\eta_{1},\ldots,\eta_{n}$ are the components of the "vectors" $x$ and $y$ relative to some basis. 2 If we set $y=x$ i n this expression, we obtain a quadratic form  

$$
A[x]=B[x,y]=\sum_{i,k=1}^{n}b_{i k}\xi_{i}\xi_{k}.
$$  

Example 1. The expression  

$$
B[x,y]=\int_{a}^{b}x(t)y(t)d t
$$  

is a bilinear functional defined on the space $\mathcal{C}$ of all functions which are continuous in the interval $a\leqslant t\leqslant b$ . The corresponding quadratic func­ tional is  

$$
A[x]=\int_{a}^{b}x^{2}(t)d t.
$$  

Example 2. A more general bilinear functional defined on $\mathcal{C}$ is  

$$
B[x,y]=\int_{a}^{b}\alpha(t)x(t)y(t)d t,
$$  

where $\alpha(t)$ is a fixed function. I f $\alpha(t)>0$ for all $t$ in $[a,b]$ , then the corre­ sponding quadratic functional  

$$
A[x]=\int_{a}^{b}\alpha(t)x^{2}(t)d t
$$  

is positive definite.  

Example 3. The expression  

$$
A[x]=\int_{a}^{b}{[\alpha(t)x^{2}(t)+\beta(t)x(t)x^{\prime}(t)+\gamma(t)x^{\prime2}(t)]d t}
$$  

is a quadratic functional defined on the space $\mathcal{D}_{1}$ of all functions which are continuously differentiable in the interval $[a,b]$ .  

Example 4. The integral  

$$
B[x,y]=\int_{a}^{b}\int_{a}^{b}K(s,t)x(s)y(t)d s d t,
$$  

where $K(s,t)$ is a fixed function of two variables, is a bilinear functional defined on $\mathcal{C}$ (f. Replacing $y(t)$ by $x(t)$ , we obtain a quadratic functional.  

We now introduce the concept of the second variation (or second difefrential) of a functional. Let $J[y]$ be a functional defined on some normed linear space $\mathcal{R}$ . In Chapter 1 , we called the functional $J[y]$ difefren tiable if its increment  

$$
\Delta J[h]=J[y+h]-J[y]
$$  

can be written in the form  

$$
\Delta J[h]=\varphi[h]+\varepsilon\|h\|,
$$  

where $\varphi[h]$ is a linear functional and $\varepsilon\to0$ as $\left\|h\right\|\to0$ . The quantity $\varphi[h]$ is the principal li near part of the increment $\Delta J[h]$ , and is called the (first) variation $[\mathsf{o r}(\hbar r s t)$ difefrential] of $J[y]$ , denoted by $\updelta J[h]$ .  

Similarly, w e say that the functional $\boldsymbol{J}[\boldsymbol{y}]$ i s twice difefrentiable i f ts incre­ ment can be written in the form  

$$
\Delta J[h]=\varphi_{1}[h]+\varphi_{2}[h]+\varepsilon\|h\|^{2},
$$  

where $\varphi_{1}[h]$ is a linear functional (in fact, the first variation), $\varphi_{2}[h]$ is a q uad­ ratic functional, and $\varepsilon\to0$ as $\left\|\boldsymbol h\right\|\to0$ . The quadratic functional $\varphi_{2}[h]$ is called the second variation (or second difefrential) of the functional $\boldsymbol{J}[\boldsymbol{y}]$ , and is denoted by $\mathbb{8}^{2}J[h]$ , 3 From now on, it wiII be tacitly assumed that we are dealing with functionals which are twice differentiable. The second variation of such a functional is uniquely defined . This is proved in just the same way as the uniqueness of the first variation of a differentiable function (see Theorem I of Sec. 3.2).  

THEOREM I .  A necessary condition for the functional $J[y]$ to have $a$ minimum for $\boldsymbol{y}=\boldsymbol{\hat{y}}$ is that  

$$
\S^{2}J[y]\geqslant0
$$  

for $\boldsymbol{y}=\boldsymbol{\hat{y}}$ and all admissible $\pmb{h}$ . For $\textbf{\em a}$ maximum, the sign $\geqslant$ in ( 1 ) is replaced $b y\leqslant$ .  

Proof By definition, we have  

$$
\Delta J[h]=\updelta J[h]+\updelta^{2}J[h]+\upvarepsilon\lVert h\rVert^{2},
$$  

where $\mathfrak{s}\to0$ as $\left\|\boldsymbol h\right\|\rightarrow0.$ . According to Theorem 2 of Sec. 3.2, $\begin{array}{r}{\mathbb{\delta}J[h]=0}\end{array}$ for $\boldsymbol{y}=\boldsymbol{\hat{y}}$ and all admissible $h,$ and hence (2) becomes  

$$
\Delta J[h]=\mathbb{\delta}^{2}J[h]+\varepsilon\|h\|^{2}.
$$  

Thus, for sufficiently small $\left\|h\right\|$ , the sign of $\Delta J[h]$ will be the same as the sign of $\mathbb{8}^{2}J[h]$ . Now suppose that $\delta^{2}J[h_{\mathrm{o}}]<0$ for some admissible $h_{0}$ . Then for any $\alpha\neq0$ , no matter how small , we have  

$$
\tilde{\delta}^{2}J[\alpha h_{0}]=\alpha^{2}\tilde{\delta}^{2}J[h_{0}]<0.
$$  

Hence, (3) can be made negative for arbitrarily small $\left\|\boldsymbol{h}\right\|$ . But this is impossible, since by hypothesis $J[y]$ has a minimum for $\boldsymbol{y}=\boldsymbol{\hat{y}}$ , i . e . ,  

$$
\Delta J[h]=J[\hat{y}+h]-J[\hat{y}]\geqslant0
$$  

for all sufficiently small $\left\|h\right\|$ . This contradiction proves the theorem.  

The condition $\begin{array}{r}{\delta^{2}J[h]\geqslant0}\end{array}$ is necessary but of course not sufficient for the functional $J[y]$ to have a minimum for a given function. To obtain a sufficient condition, we introduce the following concept : We say that a quadratic functional $\varphi_{2}[h]$ defined on some normed linear space $\mathcal{R}$ is strongly positil'e if there exists a constant $k>0$ such that  

$$
\varphi_{2}[h]\geqslant k\|h\|^{2}
$$  

for all h . 4  

THEOREM 2. A sufficient condition for a functional $J[y]$ t o hOl'e a mini­ mum for $\boldsymbol{y}=\boldsymbol{\hat{y}}$ , given that the first rariation $\updelta J[h]$ mnishes for $\boldsymbol{y}=\boldsymbol{\hat{y}}$ , is that its second mriation $\delta^{2}J[h]$ be strongly positive for $\boldsymbol{y}=\boldsymbol{\hat{y}}$ .  

Proof For $\boldsymbol{y}=\boldsymbol{\hat{y}}$ , we have $\updelta J[h]=0$ for a l l ad missible $h$ , and hence  

$$
\Delta J[h]=\updelta^{2}J[h]+\upvarepsilon\Vert h\Vert^{2},
$$  

where $\varepsilon\rightarrow0$ as $\left\|\boldsymbol h\right\|\to0$ . Moreover, for $\boldsymbol{y}=\boldsymbol{\hat{y}}$ ,  

$$
\begin{array}{r}{\updelta^{2}J[h]\geqslant k\|h\|^{2},}\end{array}
$$  

where $k=\mathrm{const}>0$ . Thus, for sufficiently small ${\mathfrak{s}}_{1},\ \left|\mathfrak{s}\right|<{\frac{1}{2}}k$ if $\left\|\boldsymbol{h}\right\|<\mathfrak{s}_{1}$ ' I t fol l ows that  

$$
\Delta J[h]=\mathbb{\delta}^{2}J[h]+\varepsilon\|h\|^{2}>\frac{1}{2}k\|h\|^{2}>0
$$  

if $\left\|\boldsymbol{h}\right\|<\mathfrak{s}_{1}$ , i . e . , $\boldsymbol{J}[\boldsymbol{y}]$ has a minim um for $y=\hat{y};$ , as asserted .  

# 25. The Form u l a  for t h e Seco n d Var i at i o n . Lege n d re's Co n d ition  

Let $F(x,y,z)$ b e a function with continuous partial derivatives u p to order three with respect to all its arguments. ( H enceforth, similar sm ooth­ ness requirements will be assumed to hold whenever needed .) We now find an expression for the second variation in the case of the simplest varia­ tional problem, i.e. , for functionals of the form  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x,
$$  

defined for curves $y=y(x)$ with fixed end points  

$$
y(a)=A,\qquady(b)=B.
$$  

First, we give the function $y(x)$ an increment $h(x)$ satisfying the boundary conditions  

$$
h(a)=0,\quad\quad h(b)=0.
$$  

Then, using Taylor's theorem with remainder, we write the increment of the functional $J[y]$ as  

$$
\begin{array}{l}{{\Delta J[h]=J[y+h]-J[y]}}\\ {{\ }}\\ {{\displaystyle\ =\int_{a}^{b}\left(F_{y}h+F_{y}{\cdot}h^{\prime}\right)d x+\frac{1}{2}\int_{a}^{b}\left(\bar{F}_{y y}h^{2}+2\bar{F}_{y y}{\cdot}h h^{\prime}+\bar{F}_{y^{\prime}y}{\cdot}h^{\prime2}\right)d x,}}\end{array}
$$  

where, as usual, the overbar indicates that the corresponding derivatives are evaluated along certain intermediate curves, i.e.,  

$$
\begin{array}{r}{\overline{{F}}_{y y}=F_{y y}(x,y+\theta h,y^{\prime}+\theta h^{\prime})\qquad(0<6<1),}\end{array}
$$  

and similarly for $\overline{{F}}_{y y^{\prime}}$ and $\overline{{F}}_{y^{\prime}y^{\prime}}$  

If we replace ${\overline{{F}}}_{y y},{\overline{{F}}}_{y y},$ and $\overline{{F}}_{y^{\prime}y^{\prime}}$ by the derivatives $F_{y y},F_{y y^{\prime}}$ and $F_{y^{\prime}y^{\prime}}$ eval­ uated at the point $(x,y(x),y^{\prime}(x))$ , then (6) becomes  

$$
\Delta J[h]=\int_{a}^{b}\left(F_{y}h+F_{y}{\cdot}h^{\prime}\right)d x+\frac{1}{2}\int_{a}^{b}\left(F_{y y}h^{2}+2F_{y y}{\cdot}h h^{\prime}+F_{y^{\prime}y}{\cdot}h^{\prime2}\right)d x+\mathfrak{e},
$$  

where E can be written as  

$$
\int_{a}^{b}{(\varepsilon_{1}h^{2}+\varepsilon_{2}h h^{\prime}+\varepsilon_{3}h^{\prime2})d x}.
$$  

Because of the continuity of the derivatives $F_{y y},\ F_{y y}.$ ' and $F_{y^{\prime}y^{\prime}}$ it foll ows that $\mathfrak{e}_{1},\mathfrak{e}_{2},\mathfrak{e}_{3}\to0$ as $\|h\|_{1}\to0$ , from which it is apparent that $\tt{\varepsilon}$ is a n i n fi n ites­ imal of order higher than 2 relative to $\|h\|_{1}^{2}$ . The fi rst term in the right­ hand side of (7) is $\updelta J[h]$ , and the second term , which is quad ratic in $\pmb{h}$ , is the second variation $\delta^{2}J[h]$ . Thus, for the fu nctional (4) we have  

$$
\S^{2}J[h]={\frac{1}{2}}\int_{a}^{b}\left(F_{y y}h^{2}+2F_{y y}.h h^{\prime}+F_{y^{\prime}y}.h^{\prime2}\right)d x.
$$  

We now transform (9) into a more convenient form. Integrating by parts and taking account of (5), we obtain  

$$
\int_{a}^{b}2F_{y y^{\prime}}h h^{\prime}d x=-\int_{a}^{b}\bigg(\frac{d}{d x}F_{y y^{\prime}}\bigg)h^{2}d x.
$$  

Therefore, (9) can be written as  

$$
\tilde{\delta}^{2}J[h]=\int_{a}^{b}\left(P h^{\prime2}+Q h^{2}\right)d x,
$$  

where  

$$
P=P(x)={\frac{1}{2}}F_{y^{\prime}y^{\prime}},\qquadQ=Q(x)={\frac{1}{2}}\Bigl(F_{y y^{\prime}}-{\frac{d}{d x}}F_{y y^{\prime}}\Bigr).
$$  

This is the expression for the second variation which will be used below.  

The following consequence of formulas (7) and (8) should be noted. If $J[y]$ has an extremum for the curve $y=y(x)$ , and if $y=y(x)+h(x)$ is an admissible curve, then  

$$
\Delta J[h]=\int_{a}^{b}\left(P h^{\prime2}+Q h^{2}\right)d x+\int_{a}^{b}\left(\xi h^{2}+\eta h^{\prime2}\right)d x,
$$  

where $\xi,\eta\to0$ as $\|h\|_{1}\to0$ . In fact, since $J[y]$ has an extremum for $y=y({\boldsymbol{x}}),$ the linear terms in the right-hand side of (7) vanish, while the quantity (8) can be written in the form  

$$
\int_{a}^{b}{(\xi h^{2}+\eta h^{\prime}{}^{2})d x}
$$  

by integrating the term ${\tt\varepsilon}_{2}h h^{\prime}$ by parts and using the boundary conditions (5). Formula ( 1 2) will be used later, when we derive sufficient conditions for a weak extremum (see Sec. 27).  

It was proved in Sec. 24 that a necessary condition for a functional $J[y]$ to have a minimum is that its second variation $\mathbb{8}^{2}J[h]$ be nonnegative. In the case of a functional of the form (4), we can use formula ( 1 0) to establish a necessary condition for the second variation to be nonnegative. The argu­ ment goes as follows : Consider the quadratic functional ( 1 0) for functions $h(x)$ satisfying the condition $h(a)=0$ . With this condition, the function $h(x)$ will be small in the interval $[a,b]$ if its derivative $h^{\prime}(x)$ is small in $[a,b]$ . However, the converse is not true, i.e. , we can construct a function $h(x)$ which is itself small but has a large derivative $h^{\prime}(x)$ in $[a,b]$ . This implies that the term $P h^{\prime}{}^{2}$ plays the dominant role in the quadratic functional ( 1 0), in the sense that $P h^{\prime}{}^{2}$ can be much larger than the second term $Q h^{2}$ but it cannot be much smaller than $Q h^{2}$ (it is assumed that $P\neq0.$ ). Therefore, it might be expected that the coefficient $P(x)$ determines whether the func­ tional ( 1 0) takes values with j ust one sign or values with both signs. We now make this qualitative argument precise :  

LEMMA. $A$ necessary condition for the quadratic functional  

$$
\tilde{\delta}^{2}J[h]=\int_{a}^{b}\left(P h^{\prime2}+Q h^{2}\right)d x,
$$  

defined for all functions $h(x)\in{\mathcal{D}}_{1}(a,b)$ such that $h(a)=h(b)=0;$ , to be nonnegative is that  

$$
P(x)\geqslant0\qquad(a\leqslant x\leqslant b).
$$  

Proof Suppose ( 1 4) does not hold, i.e., suppose (without loss of generality) that $P(x_{0})=-2\beta(\beta>0)$ at some point $\scriptstyle x_{0}$ in $[a,b]$ . Then, since $P(x)$ is continuous, there exists an $\alpha>0$ such that $a\leqslant x_{0}-\alpha,$ , $x_{0}+\alpha\leqslant b$ , and  

$$
P(x_{0})<-\ \beta\qquad(x_{0}-\alpha\leqslant x\leqslant x_{0}+\alpha).
$$  

We now construct a function $h(x)\in{\mathcal{D}}_{1}(a,b)$ such that the functional ( 1 3) is negative. In fact, let  

$$
h(x)=\left\{{\begin{array}{l l}{\sin^{2}\displaystyle\frac{\pi\left(x-x_{0}\right)}{\alpha}}&{\mathrm{for}\quad x_{0}-\alpha\leqslant x\leqslant x_{0}+\alpha,}\\ {0}&{\mathrm{otherwise}.}\end{array}}\right.
$$  

Then we have  

$$
\begin{array}{r l r}{\lefteqn{\int_{a}^{b}\left(P h^{\prime2}+Q h^{2}\right)d x=\int_{x_{0}-\infty}^{x_{0}+\infty}P\frac{\pi^{2}}{\alpha^{2}}\sin^{2}\frac{2\pi\left(x-x_{0}\right)}{\alpha}d x}}&{}&{{\left(16,\pi\right)}}\\ &{}&{+\int_{x_{0}-\infty}^{x_{0}+\infty}Q\sin^{4}\frac{\pi\left(x-x_{0}\right)}{\alpha}d x<-\frac{2\beta\pi^{2}}{\alpha}+2M\alpha,}\end{array}
$$  

where  

$$
M=\operatorname*{max}_{a\leqslant x\leqslant b}\ |Q(x)|.
$$  

For s u fficiently small $\alpha$ , the right-hand side of ( 1 6) becomes negative. and hence ( 1 3) is negative for the corresponding function $h(x)$ defined by ( 1 5). This proves the lemma.  

Using the lemma and the necessary condition for a minimum proved in Sec. 24, we immediately obtain  

THEOREM (Legendre). $A$ necessary condition for the functional  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x,\qquady(a)=A,\qquady(b)=B
$$  

to hare $a$ minimum for the curve $y=y(x)$ is that the inequality  

$$
F_{y^{\prime}y^{\prime}}\geqslant0
$$  

(Legendre's condition) be satisfied at el'ery point of the curve.  

Legendre attempted (unsuccessfully) to show that a sufficient condition for $J[y]$ to have a (weak) minimum for the curve $y=y(x)$ i s that the strict inequality  

$$
F_{y^{\prime}y^{\prime}}>0
$$  

(the strengthened Legendre condition) be satisfied at every point of the curve. His approach was to first write the seco nd variatio n ( 1 0) in the form  

$$
\delta^{2}J[h]=\int_{a}^{b}\left[P h^{\prime2}+2w h h^{\prime}+(Q+w^{\prime})h^{2}\right]d x,
$$  

where $w(x)$ is an arbitrary differentiable function, using the fact that  

$$
0=\int_{a}^{b}{\frac{d}{d x}}\left(\nu h^{2}\right)d x=\int_{a}^{b}\left(\nu^{\prime}h^{2}+2\nu h h^{\prime}\right)d x,
$$  

since $h(a)=h(b)=0$ . Next, he observed that the condition ( 1 7) would indeed be sufficient if it were possible to find a function $w(x)$ for which the integrand in ( I 8) i s a perfect square. H owever, this is not always possible, as was fi rst shown by Legend re himself, since then $w(x)$ would have to satisfy the equation  

$$
P(Q+w^{\prime})=w^{2},
$$  

and although this equation is " locally solvable," it may not have a solution in a sufficiently large interval. 5  

Actually, the following argument shows that the requirement that  

$$
F_{y^{\prime}y^{\prime}}[x,y(x),y^{\prime}(x)]>0
$$  

b e satisfied a t every point o f a n extremal $y=y(x)$ cannot b e a sufficient condition for the extremal to be a minimum of the functional $\boldsymbol{J}[\boldsymbol{y}]$ . The condition (2 1 ) , like the condition  

$$
F_{y}-{\frac{d}{d x}}F_{y^{\prime}}=0
$$  

characterizing the extremal is of a " l ocal " character, i . e . , it d oes not pertain to the curve as a whole, but only to i ndividual points of the curve. Therefore, if the co ndition (2 1 )  holds for any two cu rves $A B$ and $B C$ , it also holds for the curve $_{A C}$ formed by joining $_{A B}$ and $B C$ . On the other hand, the fact that a functional has an extre m u m for each part $_{A B}$ and $B C$ of some curve $_{A C}$ does not i mply that it has an extremum for the whole curve $_{A C}$ . For example, a great circle arc on a given sphere is the shortest curve joining its end points if the arc consists of less than half a circle, but it is not the shortest curve (even i n the class of neighboring curves) if the arc consists of more than half a circle. H owever, every great circle arc on a given sphere is a n extremal of the fu nctional which represents arc length on the sphere, and i n fact it is easi ly verified that for t h i s fu nctional, (2 1 )  holds at every poi nt of the great circle arc. Therefore, (2 1 )  cannot be a sufficient condition for an extremum, nor, for that matter, can any set of p u rely local conditions be sufficient.  

Although the condition (20) does not guarantee a minimum, the idea of completing the square of the integrand in formula (I 8) for the second varia­ tion, with the aim of fi nding sufficient conditions for an extremum, turns out to be very fruitful. In fact, the differential equation (20), which comes to the fore when trying to implement this idea, leads to new necessary conditions for an extremum (which are no longer local !). We shall d iscuss these matters further i n the next two sections.  

# 26. A n a l ys i s of the Q u ad rat i c  F u n ct i o n al $\int_{a}^{b}\left(P h^{\prime2}+Q h^{2}\right)d x$  

As shown in the preceding section, to pursue our study of the " simplest " variational problem , i.e., that of finding the extrema of the functional  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x,
$$  

where  

$$
y(a)=A,\qquady(b)=B,
$$  

we have to analyze the quadratic functional6  

$$
\int_{a}^{b}\left(P h^{\prime2}+Q h^{2}\right)d x,
$$  

defined on the set of functions $h(x)$ satisfying the conditions  

$$
h(a)=0,\quad\quad h(b)=0.
$$  

Here, the functions $P$ and $\boldsymbol{Q}$ are related to the function $F$ appearing in the integrand of (22) by the formulas  

$$
P={\frac{1}{2}}F_{y^{\prime}y^{\prime}},Q={\frac{1}{2}}\left(F_{y y}-{\frac{d}{d x}}F_{y y^{\prime}}\right).
$$  

For the time being, we ignore the fact that (23) is a second variation , satisfying the relations (25), and instead , we treat the analysis of (23) as a n independent problem, i n its own right.  

In the last sectio n , we saw that the condition  

$$
P(x)\geqslant0\qquad(a\leqslant x\leqslant b)
$$  

is necessary but not sufficient for the q uadratic functional (23) to be $\geqslant0$ for a l l admissible $h(x)$ . I n this sectio n , it will be assumed that the strength­ ened ineq uality  

$$
P(x)>0\qquad(a\leqslant x\leqslant b)
$$  

holds. We then proceed to find conditions which are both necessary and sufficient for the functional (23) to be $>0$ for all admissible $h(x)\not\equiv0$ , i . e . , to be positive definite. We begin by writing the Euler equation  

$$
-\frac{d}{d x}(P h^{\prime})+Q h=0
$$  

corresponding to the functional (23).7 This is a linear differential equation of the second order, which is satisfied, together with the boundary conditions (24), or more generally, the boundary conditions  

$$
h(a)=0,\qquadh(c)=0,\qquad(a<c\leqslant b),
$$  

by the function $h(x)\equiv0$ . However, in general, (26) can have other, non­ trivial solutions satisfying the same boundary conditions. In this connection, we introduce the following important concept :  

DEFINITION. The point $\Tilde{a}\ (\neq a)$ is said to be conjugate to the point a i the equation (26) has a solution which wnishes for $x=a$ and $x=\tilde{a}$ but is not identically zero.  

Remark. If $h(x)$ is a solution of (26) which is not identically zero and satisfies the conditions $h(a)=h(c)=0$ , then $C h(x)$ is also such a solution, where $C=\mathsf{c o n s t}\neq0$ . Therefore, for definiteness, we can impose some kind of normalization on $h(x)$ , and in fact we shall usually assume that the con­ stant $c$ has been chosen to make $h^{\prime}(a)=1$ . 8  

The following theorem effectively realizes Legendre's idea, mentioned on p . 1 04 .  

THEOREM I .  If  

$$
P(x)>0\qquad(a\leqslant x\leqslant b),
$$  

and if the interval $[a,b]$ contains no points conjugate to $a$ , then the quad­ ratic functional  

$$
\int_{a}^{b}{(P h^{\prime}}^{2}\mathrm{~+~}Q h^{2})\mathrm{~}d x
$$  

is positive definite for all $h(x)$ such that $h(a)=h(b)=0$ .  

Proof The fact that the functional (27) is positive definite will be proved if we can reduce it to the form  

$$
\int_{a}^{b}P(x)\varphi^{2}(\cdot\cdot\cdot)d x,
$$  

where $\varphi^{2}(\cdots)$ s some expression which cannot be identically zero unless $h(x)\equiv0$ . To achieve this, we add a quantity of the form $d(w h^{2})$ to the integrand of (27), where $w(x)$ is a differentiable function. This will not change the value of the functional (27), since $h(a)=h(b)=0$ implies that  

$$
\int_{a}^{b}d(w h^{2})d x=0
$$  

[cf. equation ( 1 9)] .  

We now select a function $w(x)$ such that the expression  

$$
P h^{\prime2}\:+\:Q h^{2}\:+\:\frac{d}{d x}\left(w h^{2}\right)=P h^{\prime2}\:+\:2w h h^{\prime}\:+\:(Q\:+\:w^{\prime})h^{2}
$$  

is a perfect square. This will be the case if $w(x)$ is chosen to be a solution of the equation  

$$
P(Q+w^{\prime})=w^{2}
$$  

[cf. equation (20) ] . I n fact, i f (29) holds, w e can write (28) in the form  

$$
P\Big(h^{\prime}+\frac{w}{P}h\Big)^{2}.
$$  

Thus, if (29) has a solution defined on the whole interval $[a,b]$ , the quad­ ratic functional (27) can be transformed into  

$$
\int_{a}^{b}P\Big(h^{\prime}+\frac{w}{P}h\Big)^{2}d x,
$$  

and is therefore nonnegative.  

Moreover, if ( 30 ) vanishes for some function $h(x)$ , then obviously  

$$
h^{\prime}(x)+\frac{w}{P}h(x)\equiv0,
$$  

since $P(x)>0$ for $a\leq x\leq b$ . Therefore the boundary condition $h(a)=0$ implies $h(x)\equiv0$ , because of the uniqueness theorem for the first-order differential equation ( 3 1 ) . It follows that the functional ( 3 0 ) is actually positive definite .  

Thus, the proof of the theorem reduces to showing that the absence of points in $[a,b]$ which are conjugate to $\pmb{a}$ guarantees that (29) has a solution defined on the whole interval $[a,\ b]$ . Equation (29) is a Riccati equation, which can be reduced to a linear differential equation of the second order by making a change of variables. In fact, setting  

$$
w=-\frac{u^{\prime}}{u}P,
$$  

where $\pmb{u}$ is a new unknown function, we obtain the equation  

$$
-\frac{d}{d x}(P u^{\prime})+Q u=0
$$  

which is j ust the Euler equation (26) of the functional (27). If there are no points conjugate to $a$ in $[a,b]$ , then (33) has a solution which does not vanish anywhere in $[a,b],^{\mathfrak{g}}$ and then there exists a solution of (29), given by (32), which is defined on the whole interval $[a,b]$ . This com­ pletes the proof of the theorem.  

Remark. The reduction of the quadratic functional (27) to the form (30) is the continuous analog of the reduction of a quadratic form to a sum of squares. The absence of points conjugate to $a$ in the interval $[a,b]$ is the "analog of the familiar criterion for a quadratic form to be positive definite. This connection will be discussed further in Sec. 30.  

Next, we show that the absence of points conjugate to $a$ i n the interval $[a,b]$ is not only sufficient but also necessary for the functional (27) to be positive definite.  

LEMMA. If the function $h=h(x)$ satisfies the equation  

$$
-\ {\frac{d}{d x}}(P h^{\prime})\ +\ Q h=0
$$  

and the boundary conditions  

$$
h(a)=h(b)=0,
$$  

then  

$$
\int_{a}^{b}\left(P h^{\prime2}+Q h^{2}\right)d x=0.
$$  

Proof. The lemma is an immediate consequence of the formula  

$$
0=\int_{a}^{b}\Big[-{\frac{d}{d x}}(P h^{\prime})+Q h\Big]h d x=\int_{a}^{b}\big(P h^{\prime2}+Q h^{2}\big)d x,
$$  

which is obtained by integrating by parts and using (34).  

THEOREM 2. If the quadratic functional  

$$
\int_{a}^{b}\left(P h^{\prime2}+\frac{}{}Q h^{2}\right)d x,
$$  

where  

$$
P(x)>0\qquad(a\leqslant x\leqslant b),
$$  

is positive definite for all $h(x)$ such that $h(a)=h(b)=0$ , then the interval $[a,b]$ contains no points conjugate to $\pmb{a}$ .  

Proof The idea of the proof is the following : We construct a family of positive definite functio nals, depending on a parameter $t$ , which for $t=1$ gives the functional (35) and for $t=0$ gives the very simple quadratic functional  

$$
\int_{a}^{b}h^{\prime}{}^{2}d x,
$$  

for which there can certainly be no points i n $[a,b]$ conj ugate to $a$ . Then we prove that as the parameter $t$ is varied continuously from 0 to I ,  no conj ugate points can appear in the interval $[a,b]$ .  

Thus, consider the functional  

$$
\int_{a}^{b}{[t(P h^{\prime2}+Q h^{2})+(1-t)h^{\prime2}]d x},
$$  

which is obviously positive definite fo r all I, $0\leqslant t\leqslant1$ ,  since ( 3 5) is positive definite by hypothesis. The Euler eq uation corresponding to (36) is  

$$
-\frac{d}{d x}\{[t{\cal P}+(1-t)]h^{\prime}\}+t{\cal Q}h=0.
$$  

Let $h(x,t)$ be the solution of (37) such that $h(a,t)=0$ , $h_{z}(a,t)=1$ for a l l I, $0\leqslant t\leqslant1$ . This solution is a continuous function of the parameter $t$ , which for $t=1$ red uces to the solution $h(x)$ of equation (26) satisfying the boundary conditions $h(a)=0,h^{\prime}(a)=1$ ,  and for $t=0$ reduces to the solution of the equation $h^{\prime\prime}=0$ satisfying the same boundary conditions, i . e . , the fu nction $h=x-a$ . We n ote that i f $h(x_{0},t_{0})=0$ at some point $(x_{0},t_{0})$ , then $h_{x}(x_{0},t_{0})\neq0$ . I n fact, for any fixed t, $h(x,t)$ satisfies (37), and if the equations $h(x_{0},t_{0})=0,h_{x}(x_{0},t_{0})=0$ were satisfied s i m u l­ taneously, we would have $h(x,t_{0})=0$ for a l l $x,a\leqslant x\leqslant b.$ , because of the uniq ueness theorem for li near differential equatio ns. But this is impossible, si nce $h_{x}(a,t)=1$ for a l l t, $0\leqslant t\leqslant1$ .  

Suppose now that the interval $[a,b]$ contai ns a point $\tilde{a}$ conj ugate to $a$ , i . e . , s u ppose that $h(x,\ 1)$ vanishes at some point $x={\tilde{a}}$ in $[a,b]$ . Then ${\tilde{a}}\neq b$ , since otherwise, according to the lemma,  

$$
\int_{a}^{b}\left(P h^{\prime2}+Q h^{2}\right)d x=0
$$  

for a function $h(x)\not\equiv0$ satisfying the conditions $h(a)=h(b)=0$ , which would contradict the assumption that the functional (35) is positive definite. Therefore, the proof of the theorem reduces to showing that $[a,b]$ contains no inlerior point $\tilde{a}$ conjugate to $a$ .  

![](https://cdn-mineru.openxlab.org.cn/extract/c29daec4-3bde-4c07-a565-58de41e65c3b/9505961b67b32d7fecd1b7403993f30353f0613a52556abfbbb440580e60441a.jpg)  
FIGURE 7  

To prove this, we consider the set of all points $(x,t)$ , $a\leqslant x\leqslant b$ , satisfying the condition $h(x,t)=0$ . 1 0 This set, if it is nonempty, represents a curve in the $x t$ -plane, since at each point where $h(x,t)=0$ , the derivative $h_{x}(x,t)$ is different from zero, and hence, according to the implicit function theorem, the equation $h(x,t)=0$ defines a continuous function $x=x(t)$ in the neighborhood of each such pointY By hypothesis, the point $(\tilde{a},1)$ lies on this curve. Thus, starting from the point $(\tilde{a},1)$ , the curve (see Figure 7)  

A. Cannot terminate inside the rectangle $a\leqslant x\leqslant b$ , $0\leqslant t\leqslant1$ , since this would contradict the continuous dependence of the solution $h(x,t)$ on the parameter $t$ ;   
B .  Cannot intersect the segment $x=b,0\leqslant t\leqslant1$ ,  since then, by exactly the same argument as in the lemma [but applied to equation (37), the boundary conditions $h(a,t)=h(b,t)=0$ and the func­ tional (36)] , this would contradict the assumption that the functional is positive definite for all $t_{\cdot}^{\cdot}$   
C. Cannot intersect the segment $a\leqslant x\leqslant b,t=1$ ,  since then for some $t$ we would have $h(x,t)=0$ , $h_{x}(x,t)=0$ simultaneously ;   
D. Cannot intersect the segment $a\leqslant x\leqslant b,\ t=0.$ , since for $t=0$ , equation (37) reduces to $\begin{array}{r}{\begin{array}{r}{h^{\prime\prime}=0}\end{array}}\end{array}$ , whose solution $h=x-a$ would only vanish for $x=a$ ;   
E .  Cannot approach the segment $x=a$ , $0\leqslant t\leqslant1$ ,  since then for some $t$ we would have $h_{\tau}(a,t)=0$ [why ?], contrary to hypothesis.  

It follows that no such curve can exist, and hence the proof is complete.  

If we replace the condition that the functional (35) be positive definite by the condition that it be nonnegative for all admissible $h(x)$ , we obtain the following result :  

THEOREM $2^{\prime}$ . If the quadratic functional  

$$
\int_{a}^{b}\left(P h^{\prime2}+Q h^{2}\right)d x
$$  

where  

$$
P(x)>0\qquad(a\leqslant x\leqslant b)
$$  

is nonnegative for all $h(x)$ such that $h(a)=h(b)\doteq0$ , then the interval $[a,b]$ contains no interior points conjugate to $a$ P  

Proof If the functional (38) is nonnegative, the functional (36) is positive definite for all $t$ except possibly $t=1$ .  Thus, the proof of Theorem 2 remains valid, except for the use of the lemma to prove that ${\tilde{a}}=b$ is impossible. Therefore, with the hypotheses of Theorem $2^{\prime}$ , the possibility that ${\tilde{a}}=b$ is not excluded.  

Combining Theorems I and 2, we finally obtain  

THEOREM 3. The quadratic functional  

$$
\int_{a}^{b}\left(P h^{\prime2}+Q h^{2}\right)d x,
$$  

where  

$$
P(x)>0\qquad(a\leqslant x\leqslant b),
$$  

is positive definite for all $h(x)$ such that $h(a)=h(b)=0$ if and only i the interval $[a,b]$ contains no points conjugate to $\pmb{a}$ .  

# 27. J aco b i 's Necessary Cond ition . More on Conj ugate Poi nts  

We now apply the results obtained in the preceding section to the simplest variational problem , i.e., to the functional  

$$
\int_{a}^{b}F(x,y,y^{\prime})d x
$$  

with the boundary conditions  

$$
y(a)=A,\qquady(b)=B.
$$  

12 In other words, the solution of the equation  

$$
-{\frac{d}{d x}}\left(P h^{\prime}\right)+Q h=0
$$  

satisfying the initial conditi ons $h(a)=0,h^{\prime}(a)=1$ does not van ish at any interior point of the interval $[a,b]$ .  

I t will be recalled from Sec. 25 that the second variation of the functional (39) [in the neighborhood of some extremal $y=y(x)]$ is given by  

$$
\int_{a}^{b}\left(P h^{\prime2}+Q h^{2}\right)d x
$$  

where  

$$
P={\frac{1}{2}}F_{y^{\prime}y^{\prime}},Q={\frac{1}{2}}\left(F_{y y}-{\frac{d}{d x}}F_{y y^{\prime}}\right).
$$  

DEFINITION 1 .  The Euler equation  

$$
-\ {\frac{d}{d x}}(P h^{\prime})+Q h=0
$$  

of the quadratic functional (40) is called the Jacobi equation of the original functional (39).  

DEFINITION 2. The point ii is said to be conjugate to the point a with respect to the functional (39) (f it is conjugate to a with respect to the quadratic functional (40) which is the second rariation of (39), i. e., if it is conjugate to a in the sense of the definition on $p$ .  1 0 6 .  

THEOREM (Jacobi's necessary condition). If the extremal $y=y(.\mathfrak{x})$ corresponds to a minimum of the junctional  

$$
\int_{a}^{b}F(x,y,y^{\prime})d x,
$$  

and if  

$$
F_{y^{\prime}y^{\prime}}>0
$$  

along this extremal, then the open interral $(a,b)$ contains no points con­ jugate to $a$ . 1 3  

Proof I n Sec. 24 it was proved that nonnegativity of the second variation is a necessary condition for a minim u m . Moreover, according to Theorem $2^{\prime}$ of Sec. 26, if the q uadratic fu nctional (40) is nonnegative, the i n terval $(a,b)$ can contai n no points conj ugate to $a$ . The theorem follows at once from these two facts taken together.  

We have j ust defined the Jacobi eq uation of the functional (39) as the Euler equation of the q uadratic fu nctional (40), which represents the second variation of (39). We can also derive Jacobi's eq uation by the following argument : G iven that $y=y({\boldsymbol{x}})$ is an extremal , let us examine the conditions which have to be im posed on $h(\boldsymbol{x})$ if the varied c u rve $y=y^{*}(x)=y(x)+h(x)$ is to be an extremal also. Substituting $y(x)+h(x)$ into Euler's equation  

$$
F_{y}(x,y+h,y^{\prime}+h^{\prime})-\frac{d}{d x}F_{y^{\prime}}(x,y+h,y^{\prime}+h^{\prime})=0,
$$  

using Taylor's formula, and bearing i n mind that $y(x)$ i s already a solution of Euler's equation , we find that  

$$
F_{y y}h+F_{y y},h^{\prime}-\frac{d}{d x}(F_{y y},h+F_{y^{\prime}y},h^{\prime})=o(h),
$$  

where $o(h)$ denotes an infinitesimal of order higher than I relative to $\boldsymbol{h}$ and its derivative. Neglecti ng $o(h)$ and combining terms, we obtain the linear differential equation  

$$
(F_{y y}-\frac{d}{d x}F_{y y^{\prime}})h-\frac{d}{d x}(F_{y^{\prime}y^{\prime}}h^{\prime})=0;
$$  

this is just Jacobi's equation, which w e previously wrote i n the form (42), using the notation (4 1). In other words, Jacobi's equation, except for infini­ tesimals of order higher than I , is the difefrential equation satisfied by the difefrence between two neighboring (i.e. , " infinitely close ") extremals. An equation which is satisfied to within terms of the first order by the difference between two neighboring solutions of a given differential equation is called the variational equation (of the original differential equation). Thus, we have just proved that Jacobi's equation is the variational equation of Euler's equation.  

Remark. These considerations are easily extended to the case of an arbitrary differential equation  

$$
F(x,y,y^{\prime},...,y^{(n)})=0
$$  

of order $n$ . Let $y(x)$ and $y(x)+\updelta y(x)$ be two neighboring solutions of (43). Replacing $y(x)$ by $y(x)+\updelta y(x)$ in (43), using Taylor's formula, and bearing in mind that $y(x)$ satisfies (43), we obtain  

$$
F_{y}\delta y+F_{y^{\prime}}(\delta y)^{\prime}+\cdot\cdot\cdot+F_{y^{(n)}}(\delta y)^{(n)}+\mathfrak{s}=0,
$$  

where E denotes a remainder term, which is an infinitesimal of order higher than I relative to $\updelta\boldsymbol{y}$ and its derivatives. Retaining only terms of the first order, we obtain the linear differential equation  

$$
F_{y}\S y+F_{y^{\prime}}(\delta y)^{\prime}+\cdot\cdot\cdot+F_{y^{(n)}}(\S y)^{(n)}=0,
$$  

satisfied by the variation $\updelta y$ ; as before, this equation is called the variational equation of the original equation (43). For initial conditions which are sufficiently close to zero, this equation defines a function which is the principal linear part of the difference between two neighboring solutions of (43) with neighboring initial conditions.  

We now return to the concept of a conjugate point. It will be recalled that in Sec. 26 the point $\tilde{a}$ was said to be conjugate to the point $a$ if $h(\tilde{a})=0$ , where $h(x)$ is a solution of Jacobi's equation satisfying the initial conditions $h(a)=0;$ , $h^{\prime}(a)=1$ .  As just shown, the difference $z(x)=y^{*}(x)-y(x)$  

corresponding to two neighboring extremals $y=y(x)$ and $y=y^{*}(x)$ drawn from the same initial point m ust satisfy the condition  

$$
-\ \frac{d}{d x}\left(P z^{\prime}\right)+\ Q z=o(z),
$$  

where $o(z)$ is an infinitesimal of order higher than 1 relative to $z$ and its derivative. Hence, to within such an infinitesimal, $y^{*}(x)-y(x)$ is a nonzero solution of Jacobi's equation . This leads to another definition of a con­ j ugate point : 1 4  

DEFINITION 3. Given an extremal $y=y(x)$ , the poin t $\tilde{M}=(\tilde{a},y(\tilde{a}))$ is said to be conjugate to the point $\boldsymbol{M}=(a,y(a))$ if at $\tilde{M}$ the difefrence $y^{*}(x)-y(x)$ , where $y=y^{*}(x)$ is any neighboring extremal drawn from the same initial point $M$ , is an infinitesimal of order higher than I relative to $\|y^{*}(x)-y(x)\|_{1}$  

Still another definition of a conjugate point is possible :  

DEFINITION 4. Given an extremal $y=y(x)$ , the poin t $\tilde{M}=(\tilde{a},y(\tilde{a}))$ is said to be conjugate to the point $M=(a,y(a))$ if $\tilde{M}$ is the limit as $\|y^{*}(x)-y(x)\|_{1}\to0$ of the points of intersection of $y=y(x)$ and the neighboring extremals $y=y^{*}(x)$ drawn from the same initial point $M$ .  

It is clear that if the point $\tilde{M}$ is conjugate to the point $M$ in the sense of Definition 4 (i. e . , if the extremals intersect in the way described), then $\tilde{M}$ is also conjugate to $M$ in the sense of Definition 3. We now verify that the converse is true, thereby establishing the equivalence of Definitions 3 and 4. Thus, let $y=y(x)$ be the extremal under consideration, satisfying the initial condition  

$$
y(a)=A,
$$  

a n d let $y_{\alpha}^{*}(x)$ b e the extremal drawn from the same initial point $M=(a,A)$ , satisfying the condition  

$$
y_{\alpha}^{*\prime}(a)-y^{\prime}(a)=\alpha.
$$  

Then $y_{\alpha}^{*}(x)$ can be represented in the form  

$$
y_{\alpha}^{*}(x)=y(x)+\alpha h(x)+\mathfrak{e},
$$  

where $h(x)$ is a solution of the appropriate Jacobi equation, satisfying the conditions  

$$
h(a)=0,\quad\quad h^{\prime}(a)=1,
$$  

and e is a quantity of order higher than I relative to $\pmb{\alpha}$ . Now let  

$$
h(\tilde{a})=0,\beta=\sqrt{\frac{\varepsilon}{\alpha}}.
$$  

It is clear that $h^{\prime}(\tilde{a})\neq0$ , since $h(x)\neq0$ . Using Taylor's formula, we can easily verify that for sufficiently small $\alpha$ X, the expression  

$$
y_{\alpha}^{*}(x)-y(x)=\alpha h(x)+\varepsilon
$$  

takes values with different signs at the points $\tilde{a}-\beta$ and $\tilde{a}+\beta$ . Since $\beta\rightarrow0$ as $\alpha\rightarrow0$ , this means that $\tilde{M}=(\tilde{a},y(\tilde{a}))$ is the limit as $\alpha\rightarrow0$ of the points of intersection of the extremals $y=y_{\alpha}^{*}(x)$ and the extremal $y=y(x)$ .  

Example. Consider the geodesics on a sphere, i.e. , the great circle arcs. Each such arc is an extremal of the functional which gives arc length on the sphere. The conjugate of any point $M$ on the sphere is the diametrically opposite point $\tilde{M}$ . In fact, given an extremal, all extremals with the same i nitial point $M$ (and not just the neighboring extremals) intersect the given extremal at $\tilde{M}.$ . This property stems from the fact that a sphere has con­ stant curvature, and is no longer true if the sphere is replaced by a " neigh­ boring " ellipsoid (for example).  

We conclude this section by summarizing the necessary conditions for an extremum found so far :  If the functional  

$$
\int_{a}^{b}F(x,y,y^{\prime})d x,\qquady(a)=A,\quad y(b)=B
$$  

has a weak extremum for the curve $y=y(x)$ , then  

1 .  The curve $y=y(x)$ is an extremal, i.e . , satisfies Euler's equation  

$$
F_{y}-{\frac{d}{d x}}F_{y^{\prime}}
$$  

(see Sec. 4) ;  

2. Along the curve $y=y(x),F_{y^{\prime}y^{\prime}}\geqslant0$ for a minimum and $F_{y^{\prime}y^{\prime}}\leqslant0$ for a maximum (see Sec. 25) ;  

3. The interval $(a,b)$ contains no points conjugate to $\pmb{a}$ (see Sec. 27).  

# 28. Sufficient Con d itions fo r a Weak Ext re m u m  

In this section, we formulate a set of conditions which i s  sufficient for a functional of the form  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x,\qquady(a)=A,\quad y(b)=B
$$  

to have a weak extremum for the curve $y=y(x)$ . It should be noted that the sufficient conditions to be given below closely resemble the necessary conditions given at the end of the preceding section. The necessary con­ ditions were considered separately, since each of them is necessary by itself.  

However, the sufficient conditions have to be considered as a set, since the presence of an extremum is assured only if all the conditions are satisfied simultaneously.  

THEOREM. Suppose that for some admissible curve $y=y(x)$ , the functional (44) satisfies the following conditions:  

I .  The curve $y=y(x)$ is an extremal, i. e. , satisfies Euler's equation  

$$
F_{y}-\frac{d}{d x}F_{y^{\prime}}=0;
$$  

2 .  Along the curve $y=y(x)$ ,  

$$
P(x)\equiv{\textstyle\frac{1}{2}}F_{y^{\prime}y^{\prime}}[x,y(x),y^{\prime}(x)]>0
$$  

(the strengthened Legendre condition) ;  

3 . The interval $[a,b]$ contains no points conjugate to the point $a$ (the strengthened Jacobi condition). 15  

Then the functional (44) has $\pmb{a}$ weak minimum for $y=y(x)$ .  

Proof If the interval $[a,b]$ contains no points conjugate to $a$ , and if $P(x)>0$ in $[a,b]$ , then because of the continuity of the solution of Jacobi's eq uation and of the function $P(x)$ , we can find a larger interval $[a,b+\varepsilon]$ which also contains no points conjugate to $a$ , and such that $P(x)>0$ in $[a,b+\varepsilon]$ . Consider the quadratic functional  

$$
\int_{a}^{b}(P h^{\prime2}+Q h^{2})d x-\alpha^{2}\int_{a}^{b}h^{\prime2}d x,
$$  

with the Euler equation  

$$
-\frac{d}{d x}\left[(P-\alpha^{2})h^{\prime}\right]+Q h=0.
$$  

Since $P(x)$ is positive in $[a,b+\varepsilon]$ and hence has a positive (greatest) lower bound on this interval, and since the solution of (46) satisfying the initial cond itions $h(a)=0$ , $h^{\prime}(0)=1$ depends continuously on the parameter $\alpha$ for all sufficiently small $\alpha$ , we have  

I . $P(x)-\alpha^{2}>0$ , a :::; x :::; b ;   
2. The solution of (46) satisfying the boundary conditions $h(a)=0$ , $h^{\prime}(a)=1$ does not vanish for $a<x\leqslant b$ .  

As shown in Theorem I of Sec. 26, these two conditions imply that the quadratic fu nctional (45) is positive defi n i te for all sufficiently small $\alpha$ x . I n other words, there exists a positive number $c>0$ such that  

$$
\int_{a}^{b}\left(P h^{\prime2}+Q h^{2}\right)d x>c\int_{a}^{b}h^{\prime2}d x.
$$  

It is now an easy consequence of (47) that a minimum is actually achieved for the given extremal. In fact, if $y=y(x)$ is the extremal and $y=y(x)+h(x)$ is a sufficiently close neighboring curve, then, according to formula ( 1 2) of Sec. 25,  

$$
J[y+h]-J[y]=\int_{a}^{b}\left(P h^{\prime2}+Q h^{2}\right)d x+\int_{a}^{b}\left(\xi h^{2}+\gamma h^{\prime2}\right)d x,
$$  

where $\xi(x),\eta(x)\rightarrow0$ uniformly for $a\leqslant x\leqslant b$ as $\left\|h\right\|_{1}\to0$ . Moreover, using the Schwarz inequality, we have  

$$
h^{2}(x)=\left(\int_{a}^{x}h^{\prime}d x\right)^{2}\leqslant\left(x-a\right)\int_{a}^{x}h^{\prime2}d x\leqslant\left(x-a\right)\int_{a}^{b}h^{\prime2}d x,
$$  

i . e . ,  

$$
\int_{a}^{b}h^{2}d x\leqslant{\frac{(b-a)^{2}}{2}}\int_{a}^{b}h^{\prime2}d x,
$$  

which implies that  

$$
\left|\int_{a}^{b}\left(\zeta h^{2}+\eta h^{\prime2}\right)d x\right|\leqslant\mathfrak{E}\left(1+\frac{(b-a)^{2}}{2}\right)\int_{a}^{b}h^{\prime2}d x
$$  

if $|\xi(x)|\leqslant\varepsilon,|\eta(x)|\leqslant\varepsilon.$ Since $\mathfrak{s}>0$ can be chosep to be arbitrarily small, it follows from (47) and (49) that  

$$
J[y+h]-J[y]=\int_{a}^{b}\left(P h^{\prime2}+Q h^{2}\right)d x+\int_{a}^{b}\left(\xi h^{2}+\gamma h^{\prime2}\right)d x>0
$$  

for all sufficiently small $\|\boldsymbol{h}\|_{1}$ Therefore, the extremal $y=y(x)$ actually corresponds to a weak minimum of the fu nctional (44), in some sufficiently small neighborhood of $y=y(x)$ . This proves the theorem , thereby establishing sufficient conditions for a weak extremum in the case of the " simplest " variational problem .  

# 29. G e n e ral ization to n U n known F u n ctions  

The concept o f a conjugate point a n d t h e related Jacobi conditions can be generalized to the case where the functional under consideration depends on $n$ functions $y_{1}(x),...,y_{n}(x)$ . I n  this section we carry over to such functionals the definitions and results given earlier for functionals depend­ ing on a single function. To keep the notation simple, we write  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x
$$  

as before, where now $y$ denotes the $n$ -dimensional vector $(y_{1},...,y_{n})$ and $y^{\prime}$  

the $\pmb{n}$ -dimensional vector $(y_{1}^{\prime},\ldots,y_{n}^{\prime})$ [cf. Sec. 20]. By the scalar product $(y,z)$ of two vectors  

$$
y=(y_{1},...,y_{n}),\qquadz=(z_{1},...,z_{n})
$$  

we mean, as usual, the quantity  

$$
(y,z)=y_{1}z_{1}+\cdot\cdot\cdot+y_{n}z_{n}.
$$  

Whenever the transition from the case of a single function to the case of $\pmb{n}$ functions is straightforward, we shall omit details.  

29. 1. The second variation. The Legendre condition. If the increment $\Delta J[h]$ of the functional (50), corresponding to the change from $y$ to $y+h,^{16}$ can be written in the form  

$$
\Delta J[h]=\varphi_{1}[h]+\varphi_{2}[h]+\varepsilon\|h\|^{2},
$$  

where $\varphi_{1}[h]$ is a linear functional, $\varphi_{2}[h]$ is a quadratic functional, and $\varepsilon\rightarrow0$ as $\left\|h\right\|\to0$ , then $\varphi_{2}[h]$ is called the second variation of the original functional (50) and is denoted by $\mathfrak{J}^{2}J[h]$ P In the case of fixed end points, where  

$$
h_{i}(a)=h_{i}(b)=0\qquad(i=1,...,n),
$$  

or more concisely,  

$$
h(a)=h(b)=0,
$$  

we easily find, applying Taylor's formula, that the second variation of (50) is given by  

$$
\delta^{2}J[h]=\frac{1}{2}\int_{a}^{b}\bigg[\sum_{i,k=1}^{n}F_{y_{i}y_{k}}h_{i}h_{k}+2\sum_{i,k=1}^{n}F_{y_{i}y_{k}^{*}}h_{i}h_{k}^{\prime}+\sum_{i,k=1}^{n}F_{y_{i}^{*}y_{k}^{*}}h_{i}^{\prime}h_{k}^{\prime}\bigg]d x.
$$  

Introducing the matrices  

$$
F_{y y}=\|F_{y_{1}y_{k}}\|,\qquadF_{y y^{\prime}}=\|F_{y_{i}y_{k}^{\prime}}\|,\qquadF_{y^{\prime}y^{\prime}}=\|F_{y_{i}y_{k}^{\prime}}\|,
$$  

we can write (5 1 ) in the compact form  

$$
\S^{2}J[h]=\frac{1}{2}\int_{a}^{b}\left[(F_{y y}h,h)+2(F_{y y}.h,h^{\prime})+(F_{y^{\prime}y^{\prime}}h^{\prime},h^{\prime})\right]d x,
$$  

where each term in the integrand is the scalar product of the vector $\pmb{h}$ or $h^{\prime}$ and the vector obtained by applying one of the matrices (52) to $\pmb{h}$ or $h^{\prime}$ . Then, integrating by parts, we can reduce (53) to the form  

$$
\int_{a}^{b}\left[\left(P h^{\prime},h^{\prime}\right)+\left(Q h,h\right)\right]d x,
$$  

1 6 The letter $\pmb{h}$ denotes the vector $(h_{1},....,h_{n})$ , and $\|\pmb{h}\|$ means  

$$
\sum_{\mathfrak{i}=1}^{n}\operatorname*{max}_{a\leqslant x\leqslant b}\left\{\left|h_{\mathfrak{i}}(x)\right|+\left|h_{\mathfrak{i}}^{\prime}(x)\right|\right\}=\sum_{\mathfrak{i}=1}^{n}\|h_{\mathfrak{i}}\|_{1}.
$$  

17 Obviously. $\varphi_{1}[h]$ is the $(\hbar r s t)$ variation of the functional (50).  

where $P=P(x)$ and $Q=Q(x)$ are the matrices  

$$
P=\|P_{i k}\|={\frac{1}{2}}F_{y^{\prime}y^{\prime}},\qquadQ=\|Q_{i k}\|={\frac{1}{2}}\Big(F_{y y}-{\frac{d}{d x}}F_{y y^{\prime}}\Big).
$$  

In deriving ( 54 ) , we assume that $F_{y y^{\prime}}$ is a symmetric matrix,18 i . e . , that $F_{y_{k}y_{i.}^{\prime}}=F_{y_{i}y_{k}^{\prime}}$ for all i, $k=1$ , . . . , $\pmb{n}$ ( $\cdot F_{y\eta}$ and $F_{y^{\prime}y^{\prime}}$ are automati• cally symmetnc, because of the tacItly assumed smoothness of $F$ ) . Just as In the case of one unknown function, it is easily verified that the term $(P h^{\prime},h^{\prime})$ makes the " main contribution " to the quadratic functional (54). More precisely, we have the following result :  

THEOREM 1 .  A necessary condition for the quadratic functional (54) to be nonnegative for all $h(x)$ such that $h(a)=h(b)=0$ is that the matrix $P$ be nonnegative definite. 19  

29.2. Investigation of the quadratic functional (54). As in Sec. 26, we can investigate the functional (54) without reference to the original functional ( 5 0 ) , assuming, however, that $P$ and $\boldsymbol{Q}$ are symmetric matrices. As before ( see Sec. 26 ) ,  we begin by writing the system of Euler equations  

$$
-\frac{d}{d x}\sum_{i=1}^{n}P_{i k}h_{i}^{\prime}+\sum_{i=1}^{n}Q_{i k}h_{i}=0(k=1,...,n),
$$  

corresponding to the functional (54). The equations (55) can be written more concisely as $-\frac{d}{d x}(P h^{\prime})+Q h=0,$ (56)  

in terms of the matrices $P$ and $\ensuremath{\boldsymbol{Q}}$ .  

DEFINITION 1. Let  

$$
\begin{array}{c}{{h^{(1)}=(h_{11},h_{12},...,h_{1n}),}}\\ {{h^{(2)}=(h_{21},h_{22},...,h_{2n}),}}\\ {{.\qquad\cdot\quad\cdot\cdot\cdot\cdot\cdot}}\\ {{h^{(n)}=(h_{n1},h_{n2},...\ ,h_{n n})}}\end{array}
$$  

be a set of n solutions of the system (55), where the i th solution satisfies the initial conditions2o  

$$
h_{i k}(a)=0\qquad(k=1,\ldots,n)
$$  

and  

$$
h_{i i}^{\prime}(a)=1,\qquadh_{i k}^{\prime}(a)=0\qquad(k\neq i).
$$  

Then the point $\Tilde{a}\ (\neq a)$ is said to be conjugate to the point a if the deter­ minant  

$$
\begin{array}{r}{\left|\begin{array}{l}{h_{11}(x)\:h_{12}(x)\:\cdot\:\cdot\:h_{1n}(x)}\\ {h_{21}(x)\:h_{22}(x)\:\cdot\:\cdot\:h_{2n}(x)}\\ {\cdot\:\cdot\:\cdot\:\cdot}\\ {h_{n1}(x)\:h_{n2}(x)\:\cdot\:\cdot\:h_{n n}(x)}\end{array}\right|}\end{array}
$$  

vanishes for $x=\tilde{a}$ .  

THEOREM 2. IfP is a positive definite symmetric matrix, and if the inter­ val $[a,b]$ contains no points conjugate to $a$ , then the quadratic functional (54) is positive definite for all $h(x)$ such that $h(a)=h(b)=0.$  

Proof The proof of this theorem follows the same plan as the proof of Theorem 1 of Sec. 26. Let $W$ be an arbitrary differentiable sym­ metric matrix. Then  

$$
0=\int_{a}^{b}{\frac{d}{d x}}\left(W h,h\right)d x=\int_{a}^{b}\left(W^{\prime}h,h\right)d x+2\int_{a}^{b}\left(W h,h^{\prime}\right)d x
$$  

for every vector $\pmb{h}$ satisfying the boundary conditions (58). Therefore, we can add the expression  

$$
(W^{\prime}h,h)+2(W h,h^{\prime})
$$  

to the integrand of (54), obtaining  

$$
\int_{a}^{b}\left[(P h^{\prime},h^{\prime})+2(W h,h^{\prime})+(Q h,h)+(W^{\prime}h,h)\right]d x,
$$  

without changing the value of (54).  

We now try to select a matrix $W$ such that the integrand of (6 1 ) is a perfect square. This will be the case if $W$ is chosen to be a solution of the equation21  

$$
Q\:+\:W^{\prime}=W P^{-1}W,
$$  

which we call the matrix Riccati equation (cf. p. 1 08). In fact, if we use (62), the integrand of (6 1 ) becomes  

$$
(P h^{\prime},h^{\prime})+2(W h,h^{\prime})+(W P^{-1}W h,h).
$$  

Since $P$ is a positive definite symmetric matrix, the square root $P^{1/2}$ exists, is itself positive definite and symmetric, and has the inverse $P^{-1/2}$ . Therefore, we can write (63) as the " perfect square "  

$$
(P^{1/2}h^{\prime}+P^{-1/2}W h,P^{1/2}h^{\prime}+P^{-1/2}W h).
$$  

[Recall that if $T$ is a symmetric matrix, $(T y,z)\:=\:(y,T z)$ for any vectors $y$ and z. ] Repeating the argument given in the case of a scalar function $\pmb{h}$ (see p. 1 07), we can show that  

$$
P^{1/2}h^{\prime}+P^{-1/2}W h
$$  

cannot vanish for all $x$ i n $[a,b]$ unless $\boldsymbol{h}\equiv\boldsymbol{0}$ . It follows that if the matrix Riccati equation (62) has a solution $W$ defined on the whole interval $[a,b],$ then, with this choice of $W$ , the functional (6 1 ), and hence the functional (54), is positive definite.  

Thus, the proof of the theorem reduces to showing that the absence of points in $[a,b]$ which are conjugate to $\pmb{a}$ guarantees that (62) has a solution defined on the whole interval $[a,b]$ . Making the substitution  

$$
\begin{array}{r}{W=-P U^{\prime}U^{-1}}\end{array}
$$  

in (62), where $U$ is a new unknown matrix [cf. (32)], we obtain the equation  

$$
-\frac{d}{d x}(P U^{\prime})+Q U=0,
$$  

which is j ust the matrix form of equation (56). The solution of (65) satisfying the initial conditions  

$$
U(0)=\Theta,\qquadU^{\prime}(0)=I,
$$  

where 8 is the zero matrix and $\boldsymbol{{\cal I}}$ the unit matrix of order $n,$ is precisely the set of solutions (57) of the system (55) which satisfy the initial conditions (58) and (59) [cf. footnote 1 9, p. 1 1 9] . If $[a,b]$ contains no points conjugate to $\pmb{a}$ , we can show that (65) has a solution $U(x)$ whose determinant does not vanish anywhere in $[a,b],^{22}$ and then there exists a solution of (62), given by (64), which is defined on the whole interval $[a,b]$ . In other words, we can actually find a matrix $W$ which converts the integrand of the functional (6 1 ) into a perfect square, in the way described. This completes the proof of the theorem.  

Next we show, as in Sec. 26, that the absence of points conjugate to $\pmb{a}$ in the interval $[a,b]$ is not only sufficient but also necessary for the functional (53) to be positive definite.  

LEMMA. I  

$$
h(x)=(h_{1}(x),\ldots,h_{n}(x))
$$  

satisfies the system (55) and the boundary conditions  

$$
h(a)=h(b)=0,
$$  

then  

$$
\int_{a}^{b}\left[(P h^{\prime},h^{\prime})+(Q h,h)\right]d x=0.
$$  

Proof. The lemma is an immediate consequence of the formula  

$$
0=\int_{a}^{b}\left(-\frac{d}{d x}(P h^{\prime})+Q h,h\right)d x=\int_{a}^{b}\left[(P h^{\prime},h^{\prime})+(Q h,h)\right]d x,
$$  

which is obtained by integrating by parts and using (66).  

THEOREM 3. If the quadratic functional  

$$
\int_{a}^{b}\left[\left(P h^{\prime},h^{\prime}\right)+\left(Q h,h\right)\right]d x,
$$  

where $P$ is a positive definite symmetric matrix, is positive definite for all $h(x)$ such that $h(a)=h(b)=0$ , then the interval $[a,b]$ contains no points conjugate to $\pmb{a}$ .  

Proof. The proof of this theorem follows the same plan as the proof of the corresponding theorem for the case of one unknown function (Theorem 2 of Sec. 26). We consider the positive definite quadratic functional  

$$
\int_{a}^{b}\{t[(P h^{\prime},h^{\prime})+(Q h,h)]+(1-t)(h^{\prime},h^{\prime})\}d x.
$$  

The system of Euler equations corresponding to (68) is  

$$
-\frac{d}{d x}\left[t\sum_{i=1}^{n}P_{i k}h_{i}^{\prime}+(1-t)h_{k}^{\prime}\right]+t\sum_{i=1}^{n}Q_{i k}h_{i}=0\quad(k=1,...,n)
$$  

[cf. (37)], which for $t=1$ reduces to the system (55), and for $\pmb{t}=0$ red uces to the system  

$$
h_{k}^{\prime}=0\qquad(k=1,...,n).
$$  

Suppose the interval $[a,b]$ contains a point $\tilde{a}$ conjugate to $a$ , i.e. , suppose the determinant (60) vanishes for $x=\tilde{a}$ . Then there exists a linear combination $h(x)$ of the solutions (57) which is not identically zero such that $h(\tilde{a})=0$ . Moreover, there exists a nontrivial solution $h(x,t)$ of the system (69) which depends continuously on $t$ and reduces to $h(x)$ for $t=1$ .  It s clear that ${\tilde{a}}\neq b$ , since otherwise, according to the lemma, the positive definite functional (67) would vanish for $h(x)\neq0$ , which is impossible. The fact that $\tilde{a}$ cannot be an interior point of $[a,b]$ is proved by the same kind of argument as used in Theorem 2 of Sec. 26, for the case of a scalar function $h(x)$ . Further details are left to the reader.  

Suppose now that we only require that the functional (67) be nonnegative. Then, by the same argument as used to prove Theorem $2^{\prime}$ of Sec. 26, we have  

THEOREM $3^{\prime}$ . If the quadratic functional  

$$
\int_{a}^{b}\left[\left(P h^{\prime},h^{\prime}\right)+\left(Q h,h\right)\right]d x,
$$  

where $P$ is a positive definite symmetric matrix, is nonnegativefor all $h(x)$ such that $h(a)=h(b)=0$ , then the interval $[a,b]$ contains no interior points conjugate to a.  

Finally, combining Theorems 2 and 3, we obtain  

THEOREM 4. The quadratic functional  

$$
\int_{a}^{b}\left[\left(P h^{\prime},h^{\prime}\right)+\left(Q h,h\right)\right]d x,
$$  

where $P$ is a positive definite symmetric matrix, is positive definite for al $h(x)$ such that $h(a)=h(b)=0$ if and only if the interval $[a,b]$ contains no point conjugate to $a$ .  

29.3. Jacobi's necessary condition. More on conjugate points. We now apply the results just obtained to the original functional  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x,\qquady(a)=M_{0},~y(b)=M_{1},
$$  

where $M_{0}$ and $M_{1}$ are two fixed points, recalling that the second variation of (70) is given by  

$$
\int_{a}^{b}\left[(P h^{\prime},h^{\prime})+(Q h,h)\right]d x,
$$  

where  

$$
P={\frac{1}{2}}F_{y^{\prime}y^{\prime}},Q={\frac{1}{2}}\Bigl(F_{y y}-{\frac{d}{d x}}F_{y y^{\prime}}\Bigr).
$$  

DEFINITION 2. The system of Euler equations  

$$
-\frac{d}{d x}\sum_{i=1}^{n}P_{i k}h_{i}^{\prime}+\sum_{i=1}^{n}Q_{i k}h_{i}=0(k=1,...,n),
$$  

or more concisely  

$$
-\ {\frac{d}{d x}}\left(P h^{\prime}\right)+\ Q h=0,
$$  

of the quadratic functional (7 1 ) is called the Jacobi system of the original functional (70). 23  

DEFINITION 3. The point $\pmb{\tilde{a}}$ is said to be conjugate to the point a with respect to the functional (70) if it is conjugate to a with respect to the quadratic functional (7 1 ) which is the second variation of the functional (70), i. e. , if it is conjugate to a in the sense of Definition I , p. 1 1 9 .  

Since nonnegativity of the second variation is a necessary condition for the functional (70) to have a minimum (see Theorem 1 of Sec. 24), Theorem $3^{\prime}$ immediately implies  

THEOREM 5 (Jacobi's necessary condition). If the extremal  

$$
y_{1}=y_{1}(x),...,y_{n}=y_{n}(x)
$$  

corresponds to a minimum of the functional (70), and if the matrix  

$$
F_{y^{\prime}y^{\prime}}[x,y(x),y^{\prime}(x)]
$$  

is positive definite along this extremal, then the open interval $(a,b)$ contains no points conjugate to $\mathbf{\Delta}_{a}$ .  

So far, we have said that the point $\tilde{a}$ is conjugate to $a$ if the determinant formed from $\pmb{n}$ linearly independent solutions of the Jacobi system, satisfying certain initial conditions, vanishes for $x=\tilde{a}$ .. As in the case $n=1$ , thi s basic definition is equivalent to two others, which involve only extremals of the functional (70), and not solutions of the Jacobi system :  

DEFINITION 4. Suppose n neighboring extremals  

$$
y_{1}=y_{i1}(x),...,y_{n}=y_{i n}(x)\qquad(i=1,...,n)
$$  

start from the same n-dimensional point, with directions which are close together but linearly independent. Then the point $\tilde{a}$ is said to be conjugate to the point a if the value of the determinant  

$$
\left|\begin{array}{l l l l}{y_{11}(x)}&{y_{12}(x)}&{\cdot\cdot\cdot}&{y_{1n}(x)}\\ {y_{21}(x)}&{y_{22}(x)}&{\cdot\cdot\cdot}&{y_{2n}(x)}\\ {\cdot}&{\cdot}&{\cdot\cdot}&{\cdot}\\ {y_{n1}(x)}&{y_{n2}(x)}&{\cdot\cdot\cdot}&{y_{n n}(x)}\end{array}\right|
$$  

for $x=\tilde{a}$ is an infinitesimal whose order is higher than that of its values for $a<x<\tilde{a}$ ..  

In the next definition, we enlarge the meaning of a conjugate point to apply to points lying on extremals (cf. footnote 1 4, p. 1 1 4).  

DEFINITION 5. Given an extremal $\upgamma$ with equations  

$$
y_{1}=y_{1}(x),...,y_{n}=y_{n}(x),
$$  

the point  

$$
\tilde{M}=(\tilde{a},y_{1}(\tilde{a}),...,y_{n}(\tilde{a}))
$$  

is said to be conjugate to the point  

$$
M=(a,y_{1}(a),\dotsc,y_{n}(a))
$$  

$i f\Upsilon$ has a sequence of neighboring extremals drawn from the same initial point $M$ , such that each neighboring extremal intersects $\upgamma$ and the points of intersection have $\tilde{M}$ as their limit .  

The equivalence of all these definitions of a conjugate point is proved by using considerations similar to those given for the case of a single un known function (see Sec. 27).  

29.4. Sufficient conditions for a weak extremum. Theorem 2 and an argument like that used to prove the corresponding theorem of Sec. 28 (for the scalar case) imply  

THEOREM 6. Suppose that for some admissible curve $\upgamma$ with equations  

$$
y_{1}=y_{1}(x),...,y_{n}=y_{n}(x),
$$  

the functional (70) satisfies the following conditions :  

I . The curve $\upgamma$ is an extremal, i.e. , satisfies the system ofEuler equations  

$$
F_{y_{i}}-{\frac{d}{d x}}F_{y_{i}^{}}=0\qquad(i=1,...,n);
$$  

2. A long $\upgamma$ the matrix  

$$
\begin{array}{r}{P(x)=\frac{1}{2}F_{y^{\prime}y^{\prime}}[x,y(x),y^{\prime}(x)]}\end{array}
$$  

is positive definite ;  

3. The interval $[a,b]$ contains no points conjugate to the point $a$ .  

Then the functional (70) has a weak minimum for the curve $\upgamma$ .  

30. Con n ection betwee n J aco b i ' s Co n d ition and the Theory of Q u ad rat i c Fo r m s 24  

According to Theorem 3 of Sec. 26, the quadratic functional  

$$
\int_{a}^{b}\left(P h^{\prime2}+Q h^{2}\right)d x,
$$  

where  

$$
P(x)>0\qquad(a\leqslant x\leqslant b),
$$  

is positive definite for all $h(x)$ such that $h(a)=h(b)=0$ if and only if the interval $[a,b]$ contains no points conjugate to $a.^{\ 25}$ The functional (74) is the infinite-dimensional analog of a quadratic form. Therefore, to obtain conditions for (74) to be positive definite, it is natural to start from the conditions for a quadratic form defined on an $\pmb{n}$ -dimensional space to be positive definite, and then take the limit as $n\rightarrow\infty$ .  

This may be done a s follows : By introducing the points  

$$
a=x_{0},x_{1},...,x_{n},x_{n+1}=b,
$$  

we divide the interval $[a,b]$ i nto $n+1$ equal parts of length  

$$
\Delta x=x_{i+1}-x_{1}={\frac{b-a}{n+1}}\qquad(i=0,1,\ldots,n).
$$  

Then we consider the quadratic form  

$$
\sum_{i=0}^{n}\left[P_{i}\Big(\frac{h_{i+1}-h_{i}}{\Delta x}\Big)^{2}+Q_{i}h_{i}^{2}\right]\Delta x,
$$  

where $P_{i},\ Q_{i}$ and $h_{i}$ re the values of the functions $P(x),Q(x)$ and $h(x)$ at the point $x=x_{i}$ . This quadratic form is a " finite-dimensional approxi­ mation " to the functional (74). Grouping similar terms and bearing in mind that  

$$
h_{0}=h(a)=0,\qquadh_{n+1}=h(b)=0,
$$  

we can write (75) as  

$$
\sum_{i=1}^{n}\bigg[\bigg(Q_{i}\Delta x+\frac{P_{i-1}+P_{i}}{\Delta x}\bigg)h_{i}^{2}-2\frac{P_{i-1}}{\Delta x}h_{i-1}h_{i}\bigg].
$$  

In other words, the quadratic functional (74) can be approximated by a quadratic form in $\pmb{n}$ variables $h_{1},...,h_{n}$ , with the $\textbf{\em n}\times\textbf{\em n}$ matrix  

$$
\left|\begin{array}{c c c c c c c}{a_{1}}&{b_{1}}&{0}&{\cdots}&{0}&{0}&{0}\\ {b_{1}}&{a_{2}}&{b_{2}}&{\cdots}&{0}&{0}&{0}\\ {0}&{b_{2}}&{a_{3}}&{\cdots}&{0}&{0}&{0}\\ {\cdot}&{\cdot}&{\cdot}&{\cdot\cdot}&{\cdot}&{\cdot}&{\cdot}\\ {0}&{0}&{0}&{\cdots}&{b_{n-2}}&{a_{n-1}}&{b_{n-1}}\\ {0}&{0}&{0}&{\cdots}&{0}&{b_{n-1}}&{a_{n}}\end{array}\right|,
$$  

where  

$$
a_{i}=Q_{1}\Delta x+{\frac{P_{*-1}+P_{i}}{\Delta x}}\quad\quad(i=1,...,n)
$$  

and  

$$
b_{i}=\mathrm{~-~}\frac{P_{i}}{\Delta x}\qquad(i=1,\ldots,n-1).
$$  

A symmetric matrix like (77), all of whose elements vanish except those appearing on the principal diagonal and on the two adjoining diagonals, is called a Jacobi matrix, and a quadratic form with such a matrix is called a Jacobiform. For any Jacobi matrix, there is a recurrence relation between the descending principal minors, i.e., between the determinants  

$$
D_{i}=\left|\begin{array}{c c c c c c c}{{a_{1}}}&{{b_{1}}}&{{0}}&{{\cdots}}&{{0}}&{{0}}&{{0}}\\ {{b_{1}}}&{{a_{2}}}&{{b_{2}}}&{{\cdots}}&{{0}}&{{0}}&{{0}}\\ {{0}}&{{b_{2}}}&{{a_{3}}}&{{\cdots}}&{{0}}&{{0}}&{{0}}\\ {{.}}&{{.}}&{{.}}&{{...}}&{{.}}&{{.}}&{{.}}\\ {{0}}&{{0}}&{{0}}&{{...}}&{{b_{i-2}}}&{{a_{i-1}}}&{{b_{i-1}}}\\ {{0}}&{{0}}&{{0}}&{{...}}&{{0}}&{{b_{i-1}}}&{{a_{i}}}\end{array}\right|,
$$  

where $i=1,...,n$ . In fact, expanding $D_{i}$ with respect to the elements of the last row, we obtain the recursion relation  

$$
D_{i}=a_{i}D_{i-1}-b_{i-1}^{2}D_{i-2},
$$  

which allows us t o determine the minors $D_{3},...,D_{n}$ in terms o f the first two minors $D_{1}$ and $D_{2}$ • Moreover, if we set $D_{0}=1$ , $D_{-1}=0$ , then (8 1 ) is valid for all $i=1,...,n,$ and uniquely determines $D_{1},...,D_{n}$ .  

According to a familiar result, sometimes called the Sylvester criterion, a quadratic form  

$$
\sum_{i,k=1}^{n}a_{i k}\xi_{i}\xi_{k}\qquad(a_{k i}=a_{i k})
$$  

is positive definite if and only if the descending principal minors  

$$
a_{11},\quad{\left|\begin{array}{l l}{a_{11}}&{a_{12}}\\ {a_{21}}&{a_{22}}\end{array}\right|},\quad{\left|\begin{array}{l l l}{a_{11}}&{a_{12}}&{a_{13}}\\ {a_{21}}&{a_{22}}&{a_{23}}\\ {a_{31}}&{a_{32}}&{a_{33}}\end{array}\right|},\ \ldots,\operatorname*{det}\ \left\|a_{i k}\right\|
$$  

of the matrix $\left\|a_{i k}\right\|$ are all positive.26 Applied to the present problem, this criterion states that the Jacobi form (76), with matrix (77), is positive definite if and only if all the quantities defined by (8 1 ) are positive, where $i=1,...,n$ and $D_{0}=1,D_{-1}=0$ .  

We now use this result to obtain a criterion for the quadratic functional (74) to be positive definite. Thus, we examine what happens to the recur­ rence relation (8 1 ) as ${\pmb n}\rightarrow\infty$ .  Substituting for the coefficients $a_{i}$ and $b_{i}$ from (78) and (79), we can write (8 1 ) in the form  

$$
D_{i}=\Big(Q_{i}\Delta x+\frac{P_{i-1}+P_{i}}{\Delta x}\Big)D_{i-1}-\frac{P_{i-1}^{2}}{(\Delta x)^{2}}D_{i-2}\qquad(i=1,...,n).
$$  

It is obviously impossible to pass directly to the limit $n\rightarrow\infty$ (i . e . , $\Delta x\rightarrow0$ ) in (82), since then the coefficients of $D_{i-1}$ and $D_{i-2}$ become infinite. To avoid this difficulty, we make the "change of variables " 27  

$$
\begin{array}{l}{{D_{i}=\displaystyle\frac{P_{1}\cdot\cdot\cdot P_{i}Z_{i+1}}{(\Delta x)^{i+1}}\qquad(i=1,...,n),}}\\ {{\ }}\\ {{D_{0}=\displaystyle\frac{Z_{1}}{\Delta x}=1,}}\\ {{\ }}\\ {{D_{-1}=Z_{0}=0.}}\end{array}
$$  

In terms of the variables $Z_{i}$ ' the recurrence relation (82) becomes  

$$
\begin{array}{r l}&{\frac{\boldsymbol{P}_{1}\cdot\cdot\cdot\cdot P_{i}Z_{i+1}}{(\Delta x)^{i+1}}=\left(Q_{i}\Delta x+\frac{P_{i-1}+P_{i}}{\Delta x}\right)\frac{\boldsymbol{P}_{1}\cdot\cdot\cdot\cdot P_{i-1}Z_{i}}{(\Delta x)^{i}}}\\ &{\qquad-\frac{P_{i-1}^{2}}{(\Delta x)^{2}}\frac{\boldsymbol{P}_{1}\cdot\cdot\cdot\cdot P_{i-2}Z_{i-1}}{(\Delta x)^{i-1}},}\end{array}
$$  

i . e . ,  

$$
Q_{i}Z_{i}(\Delta x)^{2}+P_{i-1}Z_{i}+P_{i}Z_{i}-P_{i}Z_{i+1}-P_{i-1}Z_{i-1}=0
$$  

or  

$$
Q_{i}Z_{i}-\frac{1}{\Delta x}\left(P_{i}\frac{Z_{i+1}-Z_{i}}{\Delta x}-P_{i-1}\frac{Z_{i}-Z_{i-1}}{\Delta x}\right)=0(i=1,...,n).
$$  

Passing to the limit $\Delta x\to0$ in (84), we obtain the differential equation  

$$
-\frac{d}{d x}\left(P Z^{\prime}\right)+\ Q Z=0,
$$  

which is just the Jacobi equation !  

The condition that the quantities $D_{i}$ satisfying the relation (82) be positive is equivalent to the condition that the quantities $Z_{i}$ satisfying the difference equation (84) be positive, since the factor  

$$
\frac{P_{1}\cdot\cdot\cdot P_{i}}{(\Delta x)^{i+1}}
$$  

is always positive [because of the condition $P(x)>0]$ . Thus, we have proved that the quadratic form (76) is positive definite if and only if all but the first of the $n+2$ quantities $Z_{0},Z_{1},...,Z_{n+1}$ satisfying the difefrence equation (84) are positive. 28  

If we consider the polygonal line $\Pi_{n}$ with vertices  

$$
(a,Z_{0}),(x_{1},Z_{1}),\cdot\cdot\cdot,(b,Z_{n+1})
$$  

recall that $a=x_{0}$ , $b=x_{n+1})$ , the condition that $Z_{\circ}=0$ and $Z_{i}>0$ for $i=1,...,n+1$ means that $\Pi_{n}$ does not intersect the interval $[a,b]$ except at the end point $\pmb{a}$ . As $\Delta x\rightarrow0$ , the difference equation (84) goes into the J acobi differential equation (85), and the polygonal line $\Pi_{n}$ goes into a nontrivial solution of (85) which satisfies the initial condition  

$$
Z(a)=Z_{0}=0,\:\:\:\:\:\:Z^{\prime}(a)=\operatorname*{lim}_{\Delta x\rightarrow0}\frac{Z_{1}-Z_{0}}{\Delta x}=\operatorname*{lim}_{\Delta x\rightarrow0}\frac{\Delta x}{\Delta x}=1
$$  

and does not vanish for $a<x\leqslant b$ . In other words, as $n\rightarrow\infty$ , tHe Jacobi form (76) goes into the quadratic functional (74), and the condition that (76)  

be positive definite goes into precisely the condition for (74) to be positive definite given in Theorem 3 of Sec. 26, i.e., the condition that $[a,b]$ contain no points conj ugate to $a$ . The legitimacy of this passage to the limit can be made completely rigorous, but we omit the details.  

# PROBLEMS  

1 . Calculate the second variation o f each o f the following functionals :  

$$
\begin{array}{l}{J[y]=\displaystyle\int_{a}^{b}F(x,y)d x;}\\ {J[y]=\displaystyle\int_{a}^{b}F(x,y,y^{\prime},...,y^{(n)})d x;}\\ {J[u]=\displaystyle\int_{a}^{b}F(x,y,u,u_{x},u_{y})d x d y.}\end{array}
$$  

2. Show that the second variation of a linear functional is zero. State and prove a converse result.  

3. Prove that a quadratic functional is twice differentiable, and find its first and second variations.  

4. Calculate the second variation of the functional  

$$
e^{\boldsymbol{J}[\boldsymbol{y}]},
$$  

where $J[y]$ is a twice differentiable functional.  

$$
\S^{2}e^{J[y]}=[(\delta J)^{2}+\delta^{2}J]e^{J[y]}.
$$  

5. Give an example showing that in Theorem 2 of Sec. 24, we cannot replace the condition that $\updelta^{2}J[h]$ be strongly positive by the condition that $\delta^{2}J[h]>0$ .  

6. Derive the analog of Legendre's necessary condition for functionals of the form  

$$
J[u]=\int\int_{R}F(x,y,u,u_{x},u_{y})d x d y,
$$  

where $\pmb{u}$ vanishes on the boundary of $R$ .  

Ans. The matrix  

$$
\left\|\begin{array}{l l}{F_{u_{x}u_{x}}}&{F_{u_{x}u_{y}}}\\ {F_{u_{y}u_{x}}}&{F_{u_{y}u_{y}}}\end{array}\right\|
$$  

should be nonnegative definite (cf. p. 1 1 9).  

7. For which values of $\pmb{a}$ and $\boldsymbol{b}$ is the quadratic functional  

$$
\int_{0}^{a}{[f^{\prime}{}^{2}(x)\ -\ b f{}^{2}(x)]\ d x}
$$  

nonnegative for all $f(x)$ such that $f(0)=f(a)=0?$ Deduce a n inequality from the answer.  

S. Show that the extrema s of any fu nctional of the form  

$$
\int_{a}^{b}F(x,y^{\prime})d x
$$  

have no conj ugate points.  

9. Prove that if a family of extremals drawn from a given point $\pmb{A}$ has an envelope $E_{\cdot}$ , then the point where a given extremal touches $\boldsymbol{E}$ is a conjugate point of $\pmb{A}$ .  

10. Investigate the extremals o f the functional  

$$
J[y]=\int_{0}^{a}\frac{y}{y^{\prime2}}d x,\qquady(0)=1,y(a)=A,
$$  

where $0<a,$ $0<A<1$ .  Show that two extremals go through every pair of points (0, 1 )  and $(a,A)$ . Which of these two extremals corresponds to a weak minimum ?  

Hint. The line $x=0$ is an envelope of the family of extremals.  

1 1 .  Prove that the extremal $y=y_{1}x/x_{1}$ corresponds to a weak minimum of both functionals  

$$
\int_{0}^{z_{1}}\frac{d x}{y^{\prime}},\qquad\int_{0}^{z_{1}}\frac{d x}{y^{\prime2}},
$$  

where $y(0)=0,y(x_{1})=y_{1},x_{1}>0,y_{1}>0.$  

1 2. What is the restriction on $\pmb{a}$ if the functional  

$$
\int_{0}^{a}\left(y^{\prime2}-y^{2}\right)d x,\qquady(0)=0,\quad y(a)=0
$$  

is to satisfy the strengthened Jacobi condition ? Use two approaches, one based on Jacobi's equation (42) and the other based on Definition 4 (p. 1 1 4) of a conj ugate point.  

13. Is the strengthened Jacobi condition satisfied by the functional  

$$
J[y]=\int_{0}^{a}\left(y^{\prime2}+y^{2}+x^{2}\right)d x,\qquady(0)=0,\quad y(a)=0
$$  

for arbitrary a ?  

Ans. Yes.  

14. Let $y=y(x,\alpha,\beta)$ be a general solution of Euler's equation, depending on two parameters $\alpha$ and $\beta$ [3. Prove that if the ratio  

$$
\frac{{\partial y}/{\partial\alpha}}{{\partial y}/{\partial\beta}}
$$  

is the same at two points, the points are conj ugate.  

15. Consider the catenary  

$$
y=c\cosh{\bigg(}{\frac{x+b}{c}}{\bigg)},
$$  

where $\pmb{b}$ and $\boldsymbol{\mathbf{\mathit{c}}}$ are constants. Show that any point on the catenary except the vertex $(-b,c)$ has one and only one conj ugate, and show that the tangents to any pair of conjugate points intersect on the $x$ -axis.  

6  

# FIELDS. SUFFI CIENT CONDITIONS FOR A STRON G EXTREMUM  

I n our study o f sufficient conditions for a weak extremum, w e introduced the important concept of a conjugate point. The simplest and most natural way to introduce this concept is based on the use of families of neighboring extremals (see Sec. 27). Then the conjugate of a point $M$ lying on an extremal $\upgamma$ is defined as the imit of the points of ntersection of $\upgamma$ with the neighboring extremals drawn from $M$ .  

The utility of studying families of extremals rather than individual extremals is particularly apparent when we turn our attention to the problem of finding sufficient conditions for a strong extremum . The study of such families of extremals is intimately connected with the important concept of a field, which we introduce in the next section. Since the concept of a field is useful in many problems, we first give a general definition of a field, which is not directly related to variational problems.  

# 3 1 .  Con s i stent Bou n d ary Co n d i t i o n s . G e n e ral Defi n i t i o n o f a F i e l d  

Consider a system o f second-order differential equations  

$$
y_{i}^{\prime\prime}=f_{i}(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})\qquad(i=1,...,n),
$$  

solved explicitly for the second derivatives. In order to single out a definite  

solution of this system, we have to specify $2n$ conditions, e.g., boundary conditions of the form  

$$
y_{i}^{\prime}=\psi_{i}(y_{1},...,y_{n})\qquad(i=1,...,n)
$$  

for two values of $x$ , say $x_{1}$ and $x_{2}$ ' Boundary conditions of this kind are commonly encountered in variational problems. If we require that the boundary conditions (2) hold only at one point, they determine a solution of the system ( 1 ) which depends on $n$ parameters.  

We now introduce the following definitions :  

DEFINITION I .  The boundary conditions  

$$
y_{i}^{\prime}=\Psi_{i}^{(1)}(y_{1},...,y_{n})\qquad(i=1,...,n),
$$  

prescribedfor $x=x_{1}$ . and the boundary conditions  

$$
y_{i}^{\prime}=\Psi_{i}^{(2)}(y_{1},...,y_{n})\qquad(i=1,...,n),
$$  

prescribedfor $x=x_{2}$ , are said to be (mutually) consistent if every solution of the system ( \ )  satisfying the boundary conditions (3) at $x=x_{1}$ also satisfies the boundary conditions (4) at $x=x_{2}$ , and conversely.  

DEFINITION 2. Suppose the boundary conditions  

$$
y_{i}^{\prime}=\Psi_{i}(x,y_{1},...,y_{n})\qquad(i=1,...,n)
$$  

(where the $\downarrow_{i}$ are continuously difefrentiable functions) are prescribedfor every $x$ in the interval $[a,b]$ , and suppose they are consistent for every pair of points $x_{1},x_{2}$ in $[a,b]$ . Then the family of mutually consistent boundary conditions (5) is called $\pmb{a}$ field (of directions) for the given system ( 1 ).  

As is clear from (5), boundary conditions prescribed for every value of $x$ define a system of first-order differential equations. The requirement that the boundary conditions be consistent for different values of $x$ means that the solutions of the system (5) must also satisfy the system ( I ), i . e . , that ( I ) i s implied b y (5) .  

Because of the existence and uniqueness theorem for systems of differential equations,2 one and only one integral curve of the system (5) passes through each point $(x,y_{1},\ldots,y_{n})$ of the region $R$ where the functions $\psi_{i}(x,y_{1},...,y_{n})$ are defined. According to what has j u st been said, each of these curves is at the same time a solution of the system ( I ). Thus, specifying a field (5) of the system ( I ) in some region $R$ defines an $\pmb{n}$ -parameter family of solutions of ( 1 ), such that one and only one curve from the family passes through each point of $R$ . The curves of the family will be called trajectories of the field.3  

The following theorem gives conditions which must be satisfied by the functions $\psi_{i}(x,y_{1},...,y_{n}),$ , $1\leqslant i\leqslant n$ , if the system (5) is to be a field for the system ( I ) :  

THEOREM. The first-order system  

$$
y_{i}^{\prime}=\psi_{i}(x,y_{1},...,y_{n})\qquad(a\leqslant x\leqslant b;1\leqslant i\leqslant n)|
$$  

is a fieldfor the second-order system  

$$
y_{i}^{\prime\prime}=f_{i}(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})
$$  

if and only if the functions $\psi_{i}(x,y_{1},...,y_{n})$ satisfy the following system of partial difefrential equations, called the Hamilton-Jacobi system4 for the original system (7) :  

$$
\frac{\partial\Psi_{i}}{\partial x}+\sum_{k=1}^{n}\frac{\partial\Psi_{i}}{\partial y_{k}}\Psi_{k}=f_{i}(x,y_{1},...,y_{n},\Psi_{1},...,\Psi_{n}).
$$  

Thus, every solution of the Hamilton-Jacobi system (8) gives a field for the original system (7)  

Proof Differentiating (6) with respect to $x$ , we obtain  

$$
y_{i}^{\prime\prime}={\frac{\partial\Psi_{i}}{\partial x}}+\sum_{k=1}^{n}{\frac{\partial\Psi_{i}}{\partial y_{k}}}{\frac{d y_{k}}{d x}},
$$  

i . e . ,  

$$
y_{i}^{\prime\prime}={\frac{\partial\Psi_{i}}{\partial x}}+\sum_{k=1}^{n}{\frac{\partial\Psi_{\imath}}{\partial y_{k}}}\Psi_{k}.
$$  

Thus, the system (7) is a consequence of the system (6) if and only if (8) holds .  

Example 1. Consider a single linear differential equation  

$$
y^{\prime\prime}=p(x)y.
$$  

The corresponding Hamilton-Jacobi system reduces to a single equation  

$$
\frac{\partial\Psi}{\partial x}+\frac{\partial\Psi}{\partial y}\Psi=p(x)y,
$$  

i . e . ,  

$$
\frac{\partial\Psi}{\partial x}+\frac{1}{2}\frac{\partial\Psi^{2}}{\partial y}=p(x)y.
$$  

The set of solutions of ( 1 0) depends on an arbitrary function, and according to the theorem, each of these solutions is a field for equation (9).  

The simplest solutions of ( 1 0) are those that are linear in $y$ :  

$$
\Psi(x,y)=\alpha(x)y.
$$  

Substituting ( I I ) into ( 1 0), w e obtain  

$$
\alpha^{\prime}(x)y+\alpha^{2}(x)y=p(x).
$$  

Thus, $\pmb{\alpha}(\pmb{x})$ satisfies the Riccati equation  

$$
\alpha^{\prime}(x)+\alpha^{2}(x)=p(x).
$$  

Solving ( 1 2) and setting  

$$
y^{\prime}=\alpha(x)y,
$$  

we obtain a field (which is linear in $y$ ) for the differential equation (9).  

Example 2. In the same way, we can find the simplest field for a system of linear differential equations  

$$
Y^{\prime\prime}=P(x)Y,
$$  

where $Y=(y_{1},...,y_{n})$ and $P(x)=\|p_{i k}(x)\|$ is a matrix. The system of Hamilton-Jacobi equations corresponding to ( 1 3) is  

$$
{\frac{\partial\Psi_{i}}{\partial x}}+\sum_{k=1}^{n}{\frac{\partial\Psi_{i}}{\partial y_{k}}}\Psi_{k}=\sum_{k=1}^{n}p_{i k}(x)y_{k}\qquad(i=1,...,n).
$$  

Let us look for a solution of ( 1 4) which is linear in $\textstyle\Y,$ , i . e . ,  

$$
\psi_{1}(x,y_{1},...,y_{n})=\sum_{k=1}^{n}\alpha_{1k}(x)y_{k},
$$  

or in vector notation,  

$$
\Psi=A Y.
$$  

Substituting ( 1 5) into ( 1 4), we obtain  

$$
\sum_{k=1}^{n}{\alpha}_{i k}^{\prime}(x)y_{k}+\sum_{k=1}^{n}{\alpha}_{{\mathrm{i}}k}(x)\sum_{j=1}^{n}{\alpha}_{k j}(x)y_{j}=\sum_{k=1}^{n}p_{\mathrm{i}k}(x)y_{k},
$$  

o r i n matrix form  

$$
\left[\frac{d}{d x}A(x)\right]Y+A^{2}(x)Y=P(x)Y,\cdot
$$  

where $A=\|\alpha_{i k}\|$ Thus, if the matrix $A(x)$ satisfies the equation  

$$
\frac{d}{d x}A(x)+A^{2}(x)=P(x),
$$  

which it is natural to call a matrix Riccati equation (cf. p. 1 20), the functions ( I S) define a field for the system ( 1 3), and this field is linear i n $y$ .  

It is worth noting, although this observation will not be needed later, that the concept of a field is intimately related to the solution of boundary value problems for systems of second-order differential equations by the so-called " sweep method." We illustrate this method by considering the very simple case where the system consists of a single linear differential equation  

$$
y^{\prime\prime}(x)=p(x)y(x)+f(x),
$$  

with the boundary conditions  

$$
\begin{array}{r}{y^{\prime}(a)=c_{0}y(a)+d_{0},}\\ {y^{\prime}(b)=c_{1}y(b)+d_{1}.}\end{array}
$$  

We begin by constructing the first-order differential equation  

$$
y^{\prime}(x)=\alpha(x)y(x)+\beta(x)
$$  

and requiring that all its solutions satisfy the boundary condition ( 1 7) and the original equation ( 1 6) . Obviously, to meet the first requirement, we must set  

$$
\alpha(a)=c_{0},\beta(a)=d_{0}.
$$  

To meet the second requirement, we differentiate ( 1 9), obtaining  

$$
y^{\prime\prime}(x)=\alpha^{\prime}(x)y(x)+\alpha(x)y^{\prime}(x)+\beta^{\prime}(x).
$$  

Substituting ( 1 9) for $y^{\prime}(x)$ in the right-hand side, we find that  

$$
y^{\prime\prime}(x)=[\alpha^{\prime}(x)+\alpha^{2}(x)]y(x)+\beta^{\prime}(x)+\alpha(x)\beta(x),
$$  

from which it is clear that ( 1 9) implies ( 1 6) if  

$$
\begin{array}{r}{\alpha^{\prime}(x)+\alpha^{2}(x)=p(x),}\\ {\beta^{\prime}(x)+\alpha(x)\beta(x)=f(x).}\end{array}
$$  

Now let $\alpha(x)$ and $\beta(x)$ b e a solution o f the system (2 1 ), satisfying the initial conditions (20). Once we have found $\alpha(x)$ and $\beta(x)$ , we can write a " boundary condition "  

$$
y^{\prime}(x_{0})=\alpha(x_{0})y(x_{0})+\beta(x_{0})
$$  

for every point $x_{0}$ in $[a,b]$ . This process of shifting the boundary condition originally prescribed for $x=a$ over to every other point in the interval  

$[a,b]$ is called the " forward sweep. " I n particular, setting $x=b$ , we obtain the equation  

$$
y^{\prime}(b)=\alpha(b)y(b)+\beta(b),
$$  

which, together with the boundary condition ( 1 8), forms a system determining $y(b)$ and $y^{\prime}(b)$ . If these values are uniquely determined, our original boundary value problem has a unique solution, i.e., the solution ofequation ( 1 9) which for $x=b$ takes the value $y(b)$ just found. This second stage in the solution of the boundary value problem is called the " backward sweep. " These consider­ ations apply to the case of a single equation, but a similar method can be used to deal with systems of second-order differential equations.  

The use of the sweep method to solve the boundary value problem con­ sisting of the differential equation ( 1 6) and the boundary conditions ( 1 7) and ( 1 8) has decided advantages over the more traditional method. [In the latter method, we first find a general solution of equation ( 1 6) and then choose the values of the arbitrary constants appearing in this sol ution in such a way that the boundary conditions ( 1 7) and ( 1 8) are satisfied.] These advantages are particularly marked in cases where one must resort to some kind of approximate numerical method in order to solve the problem. 5  

The connection between the sweep method and the concept (introduced earlier) of the field of a system of second-order differential equations is now entirely clear. In fact, in the simple case j u st considered, the forward sweep is nothing but the construction of a field linear in y for equation ( 1 6). More­ over, (2 1 ) is j ust the system of ordinary differential equations to which the Hamilton-Jacobi system reduces in the case where we are looking for a field linear in $y$ of a single second-order differential equation.6  

We might have constructed a field starting from the right-hand end point of the interval $[a,b],$ , rather than from the left-hand end point. Thus, our boundary value problem actually involves two fields for equation ( 1 6), one of which is determined by shifting the boundary condition ( 1 7) from $a$ to $b_{;}$ , and the other by shifting the boundary condition ( 1 8) from $b$ to $a$ . The solution of the boundary value problem consisting of the differential equation ( 1 6) and the boundary cond itions ( 1 7.) and ( 1 8) is a curve which is a common trajectory of these two fields. Thus, in the sweep method, we construct one field (the forward sweep) and then choose one of its trajectories which is simultaneously a trajectory of a second field (the backward sweep).  

# 32. The Field of a F u n ctional  

32.1. We now apply the considerations ofthe preceding section to variational problems. The Euler equations  

$$
F_{y_{i}}-{\frac{d}{d x}}F_{y_{i}^{'}}=0\qquad(i=1,...,n),
$$  

corresponding to the functional  

$$
\int_{a}^{b}F(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})d x,
$$  

form a system of $\pmb{n}$ second-order differential equations. In order to single out a definite solution of this system, we have to specify $2n$ supplementary conditions, which are usually given in the form of boundary conditions, i.e., relations connecting the values of $y_{i}$ and $y_{i}^{\prime}$ at the end points of the interval $[a,b]$ (there are $\pmb{n}$ such relations at each end point). In many cases, of course, the boundary conditions are determined by the very functional under consideration. For example, consider the variable end point problem for the functional  

$$
\int_{a}^{b}F(x,y_{1},...,y_{n},y_{1}^{\prime},...,y_{n}^{\prime})d x+g^{(1)}(a,y_{1},...,y_{n})+g^{(2)}(b,y_{1},...,y_{n})
$$  

differing from (22) by two fu nctions $g^{(1)}$ and $g^{(2)}$ of the coordinates of the end points of the path along which the functional is considered. Calculating the variation of the functional (23), we obtain  

$$
\begin{array}{l}{\displaystyle\int_{a}^{b}\displaystyle\sum_{i=1}^{n}\Big(F_{y_{i}}-\frac{d}{d x}F_{y_{i}}\Big)h_{i}d x+\displaystyle\sum_{i=1}^{n}F_{y_{i}}h_{i}\displaystyle\Big|_{x=a}^{x=b}}\\ {\displaystyle\qquad+\displaystyle\sum_{i=1}^{n}g_{y_{i}}^{(1)}h_{i}(a)+\sum_{i=1}^{n}g_{y_{i}}^{(2)}h_{i}(b).}\end{array}
$$  

Setting (24) equal to zero, and assuming that the curve $y_{i}=y_{i}(x),1\leqslant i\leqslant n$ is an extremal, we find that  

$$
\sum_{i=1}^{n}F_{y_{i}^{\prime}}h_{i}\Big|_{x=a}^{x=b}+\sum_{i=1}^{n}g_{y_{i}}^{(1)}h_{i}(a)+\sum_{i=1}^{n}g_{y_{i}}^{(2)}h_{i}(b)=0.
$$  

Since $h_{i}(a)$ and $h_{\mathrm{i}}(b)$ are arbitrary, (2 5) im plies that  

$$
(F_{y_{i}}-g_{y_{i}}^{(1)})|_{x=a}=0\qquad(i=1,...,n)
$$  

and  

$$
(F_{y_{i}}-g_{y_{i}}^{(2)})|_{x=b}=0\qquad(i=1,...,n).
$$  

I f $g^{\scriptscriptstyle(1)}=g^{\scriptscriptstyle(2)}\equiv0$ , (25) implies  

$$
F_{y_{i}^{'}}|_{x=a}=F_{y_{i}^{'}}|_{x=b}=0,
$$  

i.e., the natural boundary conditions for a variable end point problem like the one considered in Sec. 6 [cf. Chap. I , formula (29)].7  

Next, we examine in more detail the boundary conditions corresponding to one end point, say $x=a$ . For simplicity, we write $\pmb{g}$ instead of ${\pmb g}^{(1)}$ , and adopt the vector notation  

$$
y=(y_{1},...,y_{n}),\qquady^{\prime}=(y_{1}^{\prime},...,y_{n}^{\prime}),
$$  

etc., in arguments of functions (cf. Sec. 29). As usual, we introduce the " momenta " (see footnote 1 5, p. 86)  

$$
p_{\mathrm{i}}(x,y,y^{\prime})=F_{y_{\mathrm{i}}}(x,y,y^{\prime})\qquad(i=1,...,n),
$$  

and then write the boundary conditions (26) in the form  

$$
p_{i}(x,y,y^{\prime})|_{x=a}=g_{y_{i}}(x,y)|_{x=a}\qquad(i=1,...,n).
$$  

The relations (28) determine $y_{1}^{\prime}(a),...,y_{n}^{\prime}(a)$ as functions of $y_{1}(a),...,y_{n}(a)$ : B  

$$
y_{i}^{\prime}(a)=\Psi_{1}(y)|_{x=a}\qquad(i=1,...,n).
$$  

Boundary conditions that can be derived in this way merit a special name :  

DEFINITION I . Given $a$ functional  

$$
\int_{a}^{b}F(x,y,y^{\prime})d x,
$$  

with momenta (28), the boundary conditions (30), prescribed for $x=a;$ , are said to be self-adjoint if there exists $a$ function $g(x,y)$ such that  

$$
p_{i}[x,y,\psi(y)]|_{x=a}\equiv g_{y_{i}}(x,y)|_{x=a}\qquad(i=1,...,n).
$$  

THEOREM I. The boundary conditions (30) are self-adjoint if and only if they satisfy the conditions  

$$
\left.\frac{\partial p_{i}[x,y,\Psi(y)]}{\partial y_{k}}\right|_{x=a}=\left.\frac{\partial p_{k}[x,y,\Psi(y)]}{\partial y_{i}}\right|_{x=a}(i,k=1,...,n),
$$  

called the self-adjointness conditions.  

7 t should also be noted that the boundary conditions corresponding to fixed end points can be regarded as a limiting case of the boundary conditions (26) and (27), although the latter involve the additional functions ${\pmb g}^{(1)}$ and ${\pmb g}^{({\pmb2})}$ . For example, in the case of the functional  

$$
\int_{a}^{b}F(x,y,y^{\prime})\ d x-k[y(a)-A]^{2},
$$  

the boundary condition at the left-hand end point is  

$$
[F_{y^{\prime}}(x,y,y^{\prime})-2k(y-A)]|_{x=a}=0
$$  

or  

$$
y(a)=A+{\frac{F_{y^{\prime}}(x,y,y^{\prime})}{2k}}{\bigg|}_{x=a}.
$$  

If we now let $k\to\infty$ ,  we obtain in the limit the boundary condition $y(a)=\mathbf{A}$ . S i m i lar considerations apply to the case of several functions $y_{1},\ldots,y_{n}$ '  

8 The conditions (30) can be thought of as assigning a direction to every point of the hyperplane $x=a$ . [Cf. formula (2) . ]  

Proof. If the boundary conditions (30) are self-adj oint, then (3 1 ) holds, and hence  

$$
\frac{\partial p_{\mathrm{i}}[x,y,\Psi(y)]}{\partial y_{k}}=\frac{\partial^{2}g(x,y)}{\partial y_{i}\partial y_{k}}=\frac{\partial p_{k}[x,y,\Psi(y)]}{\partial y_{i}},
$$  

which is just (32). Conversely, if the boundary conditions (30) are such that the functions $p_{i}[x,y,\Psi(y)]$ satisfy (32), then, for $x=a$ , the $\boldsymbol{p}_{i}$ are the partial derivatives with respect to $y_{i}$ of some function $g(y),{\overset{\circ}{\operatorname{\delta}}}$ so that the boundary conditions (30) are self-adj oint in the sense of Definition 1 .  

Remark. It is immediately clear that for $n=1$ , i . e . , in the case of variational problems involving a single unknown function, any boundary con­ dition is self-adj oint, and in fact, the self-adjointness conditions (32) disappear for $n=1$ .  

32.2. In the preceding section, we introduced the concept of a field for a system of second-order differential equations. We now define the field of a functional :  

DEFINITION 2. Given a functional  

$$
\int_{a}^{b}F(x,y,y^{\prime})d x,
$$  

with the system of Euler equations  

$$
F_{y_{i}}-{\frac{d}{d x}}F_{y_{i}^{\prime}}=0\qquad(i=1,...,n),
$$  

we say that the boundary conditions  

$$
y_{i}^{\prime}=\Psi_{i}^{(1)}(y)\qquad(i=1,...,n),
$$  

prescribedfor $x=x_{1}$ > and the boundary conditions  

$$
y_{i}^{\prime}=\Psi_{i}^{(2(}y)\qquad(i=1,...,n),
$$  

prescribed for $x=x_{2}$ , are (mutually) consistent with respect to the functional (33) if they are consistent with respect to the system (34), i.e. , if every extremal satisfying the boundary conditions (35) a t $x=x_{1}$ , also satisfies the boundary conditions (36) at $x=x_{2}$ , and conversely.  

DEFINITION 3. The family of boundary conditions  

$$
y_{\mathfrak{i}}^{\prime}=\Psi_{i}(x,y)\qquad(i=1,...,n),
$$  

prescribed for every $x$ in the interval $[a,b]$ , is said to be a field of the functional (33) if  

1 .  The conditions (37) are self-adjoint for every $x$ in $[a,b]$ ; 2. The conditions (37) are consistent for every pair of points $x_{1},x_{2}$ in $[a,b]$ .  

In other words, by a field of the functional (33) is meant a field for the corresponding system of Euler equations (34) which satisfies the self­ adjointness conditions at every point $x.$ The equations (37) represent a system of first-order differential equations. Its general solution (the family of trajectories of the field) is an $n$ -parameter family of extremals such that one and only one extremal passes through each point $(x,y_{1},...,y_{n})$ of the region where the field is defined. 10  

We now give an effective criterion for a given family of boundary con­ ditions to be the field of a functional :  

THEOREM 2.11 $A$ necessary and sufficient condition for the family of boundary conditions (37) to be a field of the functional (33) is that the self-adjointness conditions  

$$
{\frac{\partial p_{i}[x,y,\psi(x,y)]}{\partial y_{k}}}={\frac{\partial p_{k}[x,y,\psi(x,y)]}{\partial y_{i}}}
$$  

and the consistency conditions  

$$
{\frac{\partial p_{i}[x,y,\psi(x,y)]}{\partial x}}=-\ {\frac{\partial H[x,y,\psi(x,y)]}{\partial y_{\mathfrak{i}}}}
$$  

be satisfied at every point $x$ in $[a,b]$ , where  

$$
\begin{array}{r}{p_{i}(x,y,y^{\prime})=F_{y_{i}^{\prime}}(x,y,y^{\prime}),}\end{array}
$$  

and $H$ is the Hamiltonian corresponding to the functional (33) :  

$$
H(x,y,y^{\prime})=-F(x,y,y^{\prime})+\sum_{i=1}^{n}p_{i}(x,y,y^{\prime})y_{i}^{'}.
$$  

Proof We have already shown in Theorem I that the conditions (38) are necessary and sufficient for the boundary conditions  

$$
y_{i}^{\prime}=\Psi_{i}(x,y)\qquad(i=1,...,n)
$$  

to be self-adj oint at every point $x$ i n $[a,b]$ . Therefore, it only remains to show that if (38) holds at every point $x$ i n $[a,b],$ then the conditions (39) are necessary and sufficient for the boundary conditions (42) to be con­ sistent for $a\leqslant x\leqslant b$ . To prove this, we set  

$$
y_{i}^{\prime}=\Psi_{i}(x,y),\qquady^{\prime}=\Psi(x,y)
$$  

in (40) and (4 1 ), and substitute the right-hand sides of the resulting equations into (39). Performing the indicated differentiations and dropping arguments (to keep the notation concise), we obtain  

$$
\begin{array}{l}{{\displaystyle F_{y_{i}x}+\sum_{k=1}^{n}F_{y_{i}^{\prime}y_{k}^{\prime}}\frac{\partial\Psi_{k}}{\partial x}=F_{y_{i}}+\sum_{k=1}^{n}F_{y_{k}}\frac{\partial\Psi_{k}}{\partial y_{i}}}}\\ {{\displaystyle~-\sum_{k=1}^{n}\psi_{k}\frac{\partial F_{y_{k}}}{\partial y_{i}}-\sum_{k=1}^{n}F_{y_{k}^{\prime}}\frac{\partial\Psi_{k}}{\partial y_{i}}.}}\end{array}
$$  

Using the self-adj ointness conditions  

$$
\frac{\partial F_{y_{k}^{\prime}}}{\partial y_{i}}=\frac{\partial F_{y_{i}^{\prime}}}{\partial y_{k}},
$$  

we can write (43) in the form  

$$
F_{y_{i}}=F_{y_{i}^{\prime}x}+\sum_{k=1}^{n}F_{y_{i}^{\prime}y_{k}^{\prime}}{\frac{\partial\Psi_{k}}{\partial x}}+\sum_{k=1}^{n}\Psi_{k}{\frac{\partial F_{y_{i}^{\prime}}}{\partial y_{k}}}
$$  

Since  

$$
\frac{\partial F_{y_{i}^{'}}}{\partial y_{k}}=F_{y_{i}^{'}y_{k}}+\sum_{j=1}^{n}F_{y_{i}^{'}y_{j}^{'}}\frac{\partial\Psi_{j}}{\partial y_{k}},
$$  

(44) becomes  

$$
F_{y_{i}}=F_{y_{i}^{\prime}x}+\sum_{k=1}^{n}F_{y_{i}^{\prime}y_{k}}\Psi_{k}+\sum_{k=1}^{n}F_{y_{i}^{\prime}y_{k}^{\prime}}\bigg({\frac{\partial\Psi_{k}}{\partial x}}+\sum_{j=1}^{n}{\frac{\partial\Psi_{k}}{\partial y_{j}}}\Psi_{j}\bigg).
$$  

Along the trajectories of the field, we have  

$$
{\frac{d y_{k}}{d x}}=\Psi_{k},
$$  

so that  

$$
\frac{d^{2}y_{k}}{d x^{2}}=\frac{\hat{c}\Psi_{k}}{\hat{\sigma}x}+\sum_{j=1}^{n}\frac{\partial\Psi_{k}}{\partial y_{j}}\Psi_{j}.
$$  

Therefore, (45) reduces to  

$$
F_{y_{i}}=F_{y_{i}^{\prime}x}+\sum_{k=1}^{n}F_{y_{i}^{\prime}y_{k}}{\frac{d y_{k}}{d x}}+\sum_{k=1}^{n}F_{y_{i}^{\prime}y_{k}^{\prime}}{\frac{d^{2}y_{k}}{d x^{2}}}
$$  

along the trajectories of the field , or  

$$
F_{y_{i}}-{\frac{d}{d x}}F_{y_{i}^{\prime}}=0,
$$  

where $1\leqslant i\leqslant n$ . This means that the trajectories of the field of directions (42) are extremals, i.e., (42) is a field of the functional  

$$
\int_{a}^{b}F(x,y,y^{\prime})d x,
$$  

and hence the conditions (39) are sufficient. Since the calculations leading from (39) to (46) are reversible, the conditions (39) are also necessary, and the theorem is proved.  

THEOREM 3. The expression  

$$
\begin{array}{r}{\frac{\partial p_{i}(x,y,y^{\prime})}{\partial y_{k}}-\frac{\partial p_{k}(x,y,y^{\prime})}{\partial y_{i}}}\end{array}
$$  

has a constant value along each extremal.  

Proof. Using (46), we find that  

$$
{\frac{d}{d x}}\left({\frac{\partial p_{i}}{\partial y_{k}}}-{\frac{\partial p_{k}}{\partial y_{i}}}\right)={\frac{\partial F_{y_{i}}}{\partial y_{k}}}-{\frac{\partial F_{y_{k}}}{\partial y_{i}}}=0.
$$  

COROLLARY. Suppose the boundary conditions  

$$
y_{i}^{\prime}=\Psi_{i}(x,y)(a\leqslant x\leqslant b;1\leqslant i\leqslant n)
$$  

are consistent, i.e. , suppose the solutions of the system (49) are extremals of the functional (47). Then. to prove that the conditions (49) define $\pmb{a}$ field of the functional (47), it is only necessary to verify that they are self­ adjoint at a single (arbitrary) point in $[a,b]$ .  

According to Definition 1 , the boundary conditions (49) are self-adjoint i f there exists a function $g(x,y)$ such that  

$$
p_{i}[x,y,\Psi(x,y)]=g_{y_{i}}(x,y)\qquad(i=1,...,n)
$$  

for $a\leqslant x\leqslant b$ . We now ask the following question : What condition has to be imposed on the function $g(x,y)$ in order for the boundary conditions (49), defined by the relations (50), to be not only self-adjoint, but also consistent, at every point of $[a,b],$ i.e., for the boundary conditions (49) to be a field of the functional (47) ? The answer is given by  

THEOREM 4. The boundary conditions (49) defined by the relations (50) are consistent $i f$ and only if the function $g(x,y)$ satisfies the Hamilton­ Jacobi equation12  

$$
{\frac{\partial g}{\partial x}}+H{\Big(}x,y_{1},...,y_{n},{\frac{\partial g}{\partial y_{1}}},...,{\frac{\partial g}{\partial y_{n}}}{\Big)}=0.
$$  

Proof It follows from (50) that the Hamilton-Jacobi equation (5 1 ) can be written i n the form  

$$
\frac{\partial g}{\partial x}=-H(x,y_{1},...,y_{n},p_{1},...,p_{n}),
$$  

where $p_{i}=p_{i}[x,y,\downarrow(x,y)]$ . Differentiating (52) with respect to $y_{i},$ we obtain  

$$
{\frac{\partial^{2}g}{\partial x\ \partial y_{i}}}=-{\frac{\partial H[x,y_{1},...,y_{n},\psi_{1}(x,y),...,\psi_{n}(x,y)]}{\partial y_{i}}},
$$  

i . e . ,  

$$
\frac{\partial p_{i}}{\partial x}=-\frac{\partial H[x,y_{1},...,y_{n},\psi_{1}(x,y),...,\psi_{n}(x,y)]}{\partial y_{i}},
$$  

which is just the set of consistency conditions (39).  

Remark. The connection between the Hamilton-Jacobi system intro­ duced in Sec. 3 1  and the Hamilton-Jacobi equation introduced in Sec. 23 is now apparent. As we saw in Sec. 3 1 ,  in the case of an arbitrary system of n second-order differential equations, a field is a system of $n$ first-order differential equations of the form (49), where the functions $\psi_{i}(x,y)$ sati sfy the Hamilton-Jacobi system (8). When we deal with the field of a functional, the system (8) turns into the consistency conditions (39), and in this case, we impose the additional requirement that the boundary conditions defining the field be self-adjoint at every point. This means that the field of a functional is not really determined by $\pmb{n}$ functions $\psi_{i}(x,y)$ , but rather by a single function $g(x,y)$ from which the functions $\Psi_{i}(x,y)$ are derived by using the relations (50). In other words, the function $g(x,y)$ is a kind of potential for the field of a functional. Since the field of a functional is determined by a single function, instead of by $n$ functions, it is entirely natural that the set of $\pmb{n}$ consistency conditions for such a field should reduce to a single equation, i.e., that the Hamilton-Jacobi system should be replaced by the Hamilton­ Jacobi equation.  

32.3. Once more, we consider a functional  

$$
\int_{a}^{b}F(x,y,y^{\prime})d x,
$$  

whose extremals are curves in the $(n+1)$ -dimensional space of points $(x,y)=(x,y_{1},...,y_{n})$ . Let $R$ be a simply connected region in this space, and let $c=(c_{0},c_{1},...,c_{n})$ be a point lying outside $R$ .  

DEFINITION 4. Let $(x,y)$ be an arbitrary point of $R$ , and suppose that one and only one extremal of the functional (53) leaves $c$ and passes through $(x,y)$ thereby defining a direction  

$$
y_{i}^{\prime}=\Psi_{i}(x,y)\qquad(i=1,...,n)
$$  

at every point of $R$ . Then thefield ofdirections (54) is called a centralfield.  

THEOREM 5 . Every central field (54) is a field of the functional (53), i.e. , satisfies the consistency and self-adjointness conditions.  

Proof Consider the function  

$$
g(x,y)=\int_{c}^{(x,y)}F(x,y,y^{\prime})d x,
$$  

where the integral is taken along the extremal of (53) joining the point $c$ to the point $(x,y)$ . We define a field of directions in $R$ by setting  

$$
F_{y_{i}}(x,y,y^{\prime})\equiv p_{i}(x,y,y^{\prime})=g_{y_{i}}(x,y)(i=1,...,n).
$$  

The theorem will be proved if it can be shown that this field coincides with the original field (54), since then the original field will satisfy the consis­ tency conditions [since its trajectories are extremals] and also the self­ adjointness conditions [this follows from Theorem I applied to the field defined by (56) ] . But (55) is just the function $S(x,y_{1},\ldots,y_{n})$ of Sec. 23, and hence  

$$
g_{y_{i}}(x,y)=p_{i}(x,y,z),
$$  

where $z$ denotes the slope of the extremal joining $c$ to $(x,y)$ , evaluated at $(x,y)$ . 13 This shows that the field of directions (56) actually coincides with the original field (54).  

DEFINITION 5. Given an extremal $\upgamma$ of thefunctional (53), suppose there exists a simply connected (open) region $R$ containing $\upgamma$ such that  

l .  A field of the functional (53) covers $R$ , i.e. , is defined at every point of $R$ ;   
2 .  One of the trajectories of the field is $\upgamma$ .  

Then we say that $\upgamma$ can be imbedded in afield [of the functional (53)].  

THEOREM 6. Let $\upgamma$ be an extremal of the functional (53), with equation  

$$
y=y(x)\qquad(a\leqslant x\leqslant b),
$$  

in vector form. Moreover, suppose that  

$$
\|F_{y_{\imath}^{\prime}y_{k}^{\prime}}\|
$$  

is nonvanishing in $[a,b]$ , and that no points conjugate to $(a,y(a))$ lie $o n\Upsilon$ .   
Then $\upgamma$ can be imbedded in a field.  

Proof By hypothesis, the following two conditions are satisfied for sufficiently small $\mathfrak{s}>0$ :  

l .  The extremal $\upgamma$ can be extended onto the whole interval $[a-\varepsilon,b]$ ; 2. The interval $[a-\varepsilon,b]$ contains no poi nts conjugate to $a$ (cf. foot­ note 20, p . 1 2 1 ) .  

Now consider the family of extremals leaving the point $(a-{\mathfrak{s}},y(a-{\mathfrak{s}}))$ . Since there are no points conj ugate to $a-\varepsilon$ i n the i nterval $[a\mathrm{~-~}\varepsilon,b]$ , i t follows that for $a\leqslant x\leqslant b$ no two extremals i n this family which are sufficiently close to the original extremal $\upgamma$ can i ntersect. Thus, in some region $R$ containing $\upgamma$ , the extremals s u fficiently close to $\upgamma$ define a central field in which $\upgamma$ is imbedded. The proof is now completed by using Theorem 5.  

# 33. H i l bert ' s I n va r i a n t I n teg ral  

As before, let $R$ be a simply connected region in the $(n+1)$ -dimensional space of points $(x,y)=(x,y_{1},...,y_{n})$ , and l et  

$$
y_{i}=\Psi_{i}(x,y)\qquad(i=1,...,n)
$$  

define a field of the functional  

$$
\int_{a}^{b}F(x,y,y^{\prime})d x
$$  

i n $R$ . It was proved in the preceding section (see Theorem 2) that the field of directions (57) is a field of the functional (58) if and only if the functions $\psi_{i}(x,y)$ satisfy the self-adj ointness conditions  

$$
{\frac{\dot{c}p_{i}[x,y,\Psi(x,y)]}{\dot{c}y_{k}}}={\frac{\dot{c}p_{k}[x,y,\Psi(x,y)]}{\hat{c}y_{i}}}
$$  

and the consistency conditions  

$$
\frac{\hat{c}H[x,y,\dot{\psi}(x,y)]}{\dot{c}y_{i}}=-\frac{\hat{c}p_{\mathrm{\scriptsize{1}}}[x,y,\Psi(x,y)]}{\hat{c}x}.
$$  

Taken together, the conditions (59) and (60) imply that the quantity  

$$
-H[x,y,\psi(x,y)]d x+\sum_{i=1}^{n}p_{\scriptscriptstyle i}[x,y,\psi(x,y)]d y_{i}
$$  

is the exact differential of some fu nction (see footnote 9 , p. 1 39)  

$$
g(x,y)=g(x,y_{1},...,y_{n}).
$$  

As is fam i l iar fro m elementary analysis, 1 4 this fu ncti o n , which is determined to within an additive con sta nt, can be written as a line i ntegral  

$$
g(x,y)=\int_{\Gamma}\Bigl(-H d x+\sum_{i=1}^{n}p_{\imath}d y_{\imath}\Bigr),
$$  

evaluated along the curve $\Gamma$ going from some fixed point $M_{0}=(x_{0},y(x_{0}))$ to the variable point $M=(x,y)$ . Si nce the i n tegra nd of (6 1 )  is an exact  

differential, the choice of the curve $\Gamma$ does not matter ; in fact, the value of the integral depends only on the points $M_{0},M_{1}$ , and not on the curve $\Gamma$ . The right-hand side of (6 1 )  is known as Hilbert s invariant integral.  

Using the equations (57) defining the field, and explicitly introducing the integrand $F$ f the functional (58), we can write the integral in (6 1 ) as  

$$
\begin{array}{l}{\displaystyle\int_{\Gamma}\Big(\Big\{{\cal F}[x,y,\psi(x,y)]-\sum_{i=1}^{n}\psi_{i}(x,y){\cal F}_{y;}[x,y,\psi(x,y)]\Big\}d x}\\ {+\sum_{i=1}^{n}{\cal F}_{y;}[x,y,\psi(x,y)]d y_{i}\Big).}\end{array}
$$  

This expression is Hilbert's invariant integral , in the form corresponding to the field defined by the functions $\psi_{i}(x,y)$ . If the curve $\Gamma$ along which the integral (62) is evaluated is one of the trajectories of the field, then  

$$
d y_{i}=\psi_{i}(x,y)d x
$$  

along $\Gamma$ , and hence (62) reduces to  

$$
\int_{\Gamma}F(x,y,y^{\prime})d x
$$  

evaluated along this trajectory.  

Remark. If $\upgamma$ is an extremal which is a trajectory of the field, Hilbert's invariant integral can be used to write the value of the functional for this extremal as an integral eval uated along any curve joining the end points of $\upgamma$ . This impo rtant fact will be used in the next section.  

34. T h e We i e rst rass E-F u n ct i o n . S u ffi c i e n t Co n d i t i o n s for a Strong Extre m u m  

DEFINITION. $B y$ the Weierstrass $E$ -function of the functional15  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x,~y(a)=A,~y(b)=B
$$  

we mean the following function of $3n+1$ variables :  

$$
E(x,y,z,w)=F(x,y,w)-F(x,y,z)-\sum_{i=1}^{n}(w_{i}-z_{i})F_{y_{i}^{*}}(x,y,z).
$$  

In other words, $E(x,y,z,w)$ is the difference between the value of the  

function $F$ regarded as a function of its last $\pmb{n}$ arguments) at the point $w$ and the first two terms of its Taylor's series expansion about the point $z$ . Thus, $E(x,y,z,w)$ can also be written as the remainder of a Taylor's series :  

$$
E(x,y,z,w)=\frac{1}{2}\sum_{i,k=1}^{n}(w_{i}-z_{i})(w_{k}-z_{k})F_{y_{i}y_{k}^{*}}[x,y,z+\theta(w-z)]
$$  

For $n=1$ , the Weierstrass $E$ -function has a simple geometric interpretation, since if we regard $F(x,y,z)$ as a function of $z$ ,  

$$
F(x,y,w)-F(x,y,z)-(w-z)F_{y^{\prime}}(x,y,z)
$$  

is j ust the vertical distance from the curve $\Gamma$ representing $F(x,y,z)$ to the tangent to $\Gamma$ drawn through a fixed point of $\Gamma$ .  

Our goal in this section is to derive sufficient conditions for the functional (63) to have a strong extremum. It will be recalled from Secs. 28 and 29 that the following set of conditions is sufficient for the functional (63) to have a weak minimum16 for the admissible curve $\upgamma$ :  

Condition 1 .  The curve $\upgamma$ is an extremal ;   
Condition 2. The matrix $\|F_{y,^{\prime}y_{k}^{\prime}}\|$ is positive definite along $\upgamma$ ;   
Condition 3. The i nterval $[a,b]$ contains no points conjugate to $\pmb{a}$ .  

Every strong extremum is simultaneously a weak extremum, but the converse is in general false (see p. 1 3). Therefore, in looking for sufficient conditions for a strong extremum, it is natural to assume from the outset that the three conditions just listed are satisfied. We then try to supplement them in such a way as to obtain a set of conditions guaranteeing a strong extremum as well as a weak extremum. To find such supplementary con­ ditions, we first recall that Conditions 2 and 3 imply that the given extremal $\upgamma$ can be imbedded in a field  

$$
y_{i}^{\prime}=\Psi_{i}(x,y)\qquad(i=1,...,n)
$$  

of the functional (63) [see Theorem 6 of Sec. 32]. 17 Let $\upgamma$ have the equations  

$$
y_{i}=y_{i}(x)\qquad(i=1,...,n),
$$  

and let $\upgamma^{\ast}$ be an arbitrary curve with the same end points ${\tt a s\gamma}$ , lying in the $(n+1)$ -dimensional region $R$ containing $\upgamma$ and covered by the field (see  

Definition 5 of Sec. 32). Then, according to equation (62) and the remark at the end of Sec. 33, we have  

$$
\int_{\mathbb{v}}F(x,y,y^{\prime})=\int_{\mathbb{v}^{*}}\Big(\Big\{F(x,y,\uppsi)-\sum_{i=1}^{n}\psi_{i}F_{y_{i}^{*}}(x,y,\uppsi)\Big\}d x+\sum_{i=1}^{n}F_{y_{i}^{*}}(x,y,\uppsi)d y
$$  

where for simplicity we omit the arguments of the functions $\phi$ and $\Psi_{i}$ ' The right-hand side of (66) is j ust Hilbert's invariant i ntegral, in the form corre­ sponding to the field (65). As usual, we are interested in the increment  

$$
\Delta J=\int_{\gamma*}F(x,y,y^{\prime})d x-\int_{\gamma}F(x,y,y^{\prime})d x.
$$  

Using (66), we find that  

$$
\begin{array}{l}{\displaystyle\Delta J=\int_{\mathbb{V}^{*}}F(x,y,y^{\prime})d x}\\ {\displaystyle\quad-\int_{\mathbb{V}^{*}}\Big(\Big\{F(x,y,\psi)-\sum_{i=1}^{n}\Psi_{i}F_{i}(x,y,\psi)\Big\}d x+\sum_{i=1}^{n}F_{y_{i}}(x,y,\psi)d y_{i}\Big)}\\ {=\int_{\mathbb{V}^{*}}\Big(F(x,y,y^{\prime})-F(x,y,\psi)-\sum_{i=1}^{n}\big(y_{i}^{\prime}-\Psi_{i}\big)F_{y_{i}}(x,y,\psi)\Big)d x,}\end{array}
$$  

or in terms of the Weierstrass $E$ -function. 1 8  

$$
\Delta J=\int_{\gamma*}E(x,y,\psi,y^{\prime})d x.
$$  

We are now in a position to state sufficient conditions for a strong extremum.  

THEOREM I .  Let y be an extremal, and let  

$$
y_{i}^{\prime}=\Psi_{i}(x,y)\qquad(i=1,...,n)
$$  

be a field of the functional  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x,\qquady(a)=A,\qquady(b)=B.
$$  

Suppose that at every point $(x,y)=(x,y_{1},...,y_{n})$ ofsome (open) region containing $\upgamma$ and cOl'ered by the field (68), 9 the condition  

$$
E(x,y,\psi,w)\geqslant0
$$  

is satisfied for el'ery finite l'ector $\boldsymbol{w}=(\boldsymbol{w}_{1},\ldots,\boldsymbol{w}_{n})$ . Then $J[y]$ has $\pmb{a}$ strong minimum for the extremal $\upgamma$ .  

$$
\Delta J=\int_{a}^{b}E(x,y^{\ast},\dot{\psi},y^{\ast\prime})d x,
$$  

Proof To say that the functional $J[y]$ has a strong minimum for the extremal $\upgamma$ means that $\Delta J$ is nonnegative for any admissible curve $\upgamma^{\ast}$ which is sufficiently close to $\upgamma$ in the norm of the space $\mathcal{C}(\boldsymbol{a},\boldsymbol{b})$ . But the condition (70) guarantees that the increment $\Delta J$ , given by (67), is non­ negative for all such curves. Note that we do not impose any restrictions at all on the slope of the curve $\upgamma^{\ast}$ , i . e . , $\upgamma^{\ast}$ need not be close to $\upgamma$ i n the norm of the space $\mathcal{D}_{1}(a,b)$ . I n fact, $\upgamma^{\ast}$ need not even belong to $\mathcal{D}_{1}(a,b)$ . 20  

Remark $\boldsymbol{{\mathit{1}}}$ .  As already noted, the hypothesis that the extremal $\upgamma$ can be imbedded in a field can be replaced by Conditions 2 and 3 .  

Remark 2 . Since the Weierstrass $E$ -function can b e written in the form  

$$
E(x,y,\uppsi,w)=\frac{1}{2}\sum_{i,k=1}^{n}(w_{i}-\uppsi_{i})(w_{k}-\uppsi_{k})F_{y_{1}y_{k}^{-}}[x,y,\uppsi+\uptheta(w-\uppsi)]
$$  

$$
(0<\Theta<1)
$$  

(see p . 1 47), we can replace (70) b y the condition that a t every point o f some region $R$ containing $\upgamma$ , the matrix $\|F_{y_{1}^{\prime}y_{k}^{\prime}}(x,y,z)\|$ be nonnegative definite for every finite $z$ .  

We conclude this section by indicating the following necessary condition for a strong extremum :  

THEOREM 2 ( Weierstrass' necessary condition). If the functional  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x,\qquady(a)=A,\qquady(b)=B
$$  

has a strong minimum for the extremal $\upgamma$ , then  

$$
E(x,y,y^{\prime},w)\geqslant0
$$  

along y for every finite $w$ .  

The idea o f the proof i s the following : I f (7 1 ) i s not satisfied, there exists a point $\xi$ in $[a,b]$ and a vector $q$ such that  

$$
E[\xi,y(\xi),y^{\prime}(\xi),q]<0,
$$  

where $y=y(x)$ is the equation of the extremal $\upgamma$ . It can then be shown that a suitable modification of $\upgamma$ leads to an admissible curve $\upgamma^{\ast}$ close to $\upgamma$ in the norm of the space $\mathcal{C}(\boldsymbol{a},\boldsymbol{b})$ such that  

$$
\Delta J=\int_{\gamma_{*}}F(x,y,y^{\prime})d x-\int_{\gamma}F(x,y,y^{\prime})d x<0,
$$  

which contradicts the hypothesis the $J[y]$ has a strong minimum for $\upgamma$ . However, the construction of $\upgamma^{\ast}$ must be carried out carefully, since all we know is that (72) holds for a suitable $q$ (see Probs. 9 and 1 0).  

# PROBLEMS  

1. Find the curve joining the points $(-1,-1)$ and ( 1 , 1 ) which minimizes the functional  

$$
J[y]=\int_{-1}^{1}\left(x^{2}y^{\prime2}+12y^{2}\right)d x.
$$  

What is the nature of the minimum ?  

Hint. $\Delta J=J[y+h]-J[y]=\int_{-1}^{1}\left(x^{2}h^{\prime2}+12h^{2}\right)d x>0.$   
Ans. $J[y]$ has a strong minimum for $y=x^{3}$ .  

2. Find the curve joining the points ( 1 , 3) and (2, 5) which minimizes the func­ tional  

$$
J[y]=\int_{1}^{2}y^{\prime}(1+x^{2}y^{\prime})d x.
$$  

What is the nature of the minimum ?  

Hint. Again calculate $\Delta J.$ .  

3. Prove that the segment of the $\pmb{x}$ -axis j oining $\scriptstyle{\pmb{x}}={\pmb{0}}$ to $x=\pi$ corresponds to a weak minimum but not a strong minimum of the functional  

$$
J[y]=\int_{0}^{\pi}y^{2}(1-y^{\prime2})d x,\qquady(0)=0,\quad y(\pi)=0.
$$  

Hint. Calculate $J[y]$ for  

$$
y={\frac{1}{\sqrt{n}}}\sin n x.
$$  

4. Prove that the extrema of the functional  

$$
\int_{a}^{b}n(x,y){\sqrt{1+y^{\prime2}}}d x
$$  

are always strong minima if $\begin{array}{r}{\pmb{n}(x,y)\geqslant0}\end{array}$ for all $\pmb{x}$ and $_y$ .  

5. Investigate the extrema of the following functionals :  

$$
\begin{array}{l}{{J[y]=\displaystyle\int_{-1}^{2}y^{\prime}(1+x^{2}y^{\prime})d x,\qquady(-1)=1,y(2)=1;}}\\ {{\displaystyle J[y]=\displaystyle\int_{0}^{\pi/4}(4y^{2}-y^{\prime2}+8y)d x,\qquady(0)=-1,y(\pi/4)=0;}}\\ {{\displaystyle J[y]=\displaystyle\int_{1}^{2}(x^{2}y^{\prime2}+12y^{2})d x,\qquady(1)=1,y(2)=8;}}\\ {{\displaystyle J[y]=\displaystyle\int_{0}^{1}(y^{\prime2}+y^{2}+2y e^{2x})d x,\qquady(0)=\frac{1}{3},\quad y(1)=\frac{1}{3}e^{2}.}}\end{array}
$$  

Ans. b) A strong maximum for $y=\sin2x-1;{\mathsf{d}})$ A strong minimum for y = te2X.  

6. Prove that $y\:=\:b x/a$ is a weak minimum but not a strong minimum of the functional  

$$
J[y]=\int_{0}^{a}y^{\prime3}d x,
$$  

where $y(0)=0,y(a)=b,a>0,b>0.$ .  

Hint. Examine the corresponding Weierstrass $\scriptstyle{E}$ -funct ion.  

7. Show that the extremals which give weak minima i n Chap. 5, Prob. 1 0 do not give strong minima.  

8. Show that the extremal $y\equiv0$ of the functional  

$$
J[y]=\int_{0}^{1}\left(a y^{\prime2}-4b y y^{\prime3}+2b x y^{\prime4}\right)d x,
$$  

where  

$$
y(0)=0,~y(1)=0,~a>0,~b>0,
$$  

satisfies both the strengthened Legendre condition and Weierstrass' necessary condition . Also verify that $y\equiv0$ can be imbedded in a field of the func­ tional $J[y].$ Does $y\equiv0$ correspond to a strong minimum of $J[y]{\mathord{?}}$  

Hint. Choose  

$$
y=y_{0}(x)={\left\{\begin{array}{l l}{\displaystyle{\frac{k}{h}}x}&{{\mathrm{for}}\quad0\leqslant x\leqslant h,}\\ {\displaystyle k{\frac{1-x}{1-h}}}&{{\mathrm{for}}\quad h\leqslant x\leqslant1.}\end{array}\right.}
$$  

Then, given any $k>0$ however small, there is an $\pmb{h}>0$ such that $J[y_{0}]<0$ . Ans. No.  

9. Complete the proof of Weierstrass' necessary condition, begun on p. 149. Hint. By continuity of the $E$ -function, we can always arrange for the point $\boldsymbol{\xi}$ to be an interior point of $[a,b]$ . Choose $\pmb{h}>0$ such that $\xi-h>a$ , and construct the function  

$$
y=y_{h}(x)={\left\{\begin{array}{l l}{y(x)+(x-a)Q}&{{\mathrm{for}}\quad a\leqslant x\leqslant\xi-h,}\\ {(x-\xi)q+y(\xi)}&{{\mathrm{for}}\quad\xi-h\leqslant x\leqslant\xi,}\\ {y(x)}&{{\mathrm{for}}\quad\xi\leqslant x\leqslant b,}\end{array}\right.}
$$  

where $y=y(x)$ is the equation of the extremal $\upgamma$ , and $\scriptstyle Q$ is the vector deter­ mined by the condition  

$$
y(\xi-h)+(\xi-a-h)Q=-q h+y(\xi).
$$  

Then let $\Delta(h)=J[y_{h}]-J[y]$ . Prove that $\Delta^{\prime}(0)=E[\xi,y(\xi),y^{\prime}(\xi),q]<0,$ , which, together with $\Delta(0)=0$ , im plies that $J[y_{h}]-J[y]<0$ for small enough $\pmb{h}$ .  

10. Give another proof of Weierstrass' necessary condition, based on the direct use of Hilbert's invariant integral .  

Hin t. Let $\pmb{M}_{1}$ be the point $(\xi,y(\xi))$ . From a point $M_{0}$ on $\upgamma$ sufficiently close to $M$ , construct a central field of the functional. Let $R$ be the region covered by this field, and let $\Phi(M)$ be the value of Hilbert's in variant in tegral evaluated along any curve in $R$ j oining $M_{0}$ to the variable point $M$ i n $R$ . Draw two surfaces ${\upsigma}_{2}$ and ${\pmb{\upsigma}}_{1}$ of the one-parameter family $\Phi(M)=$ const, the first intersecting $\upgamma$ in a point $M_{2}$ lying between $M_{0}$ and $M_{1}$ , the second intersecting $\upgamma$ i n the point $M_{1}$ . Moreover, from $M_{1}$ draw the straight line with direction $\pmb q$ , and let this line in tersect ${\upsigma}_{2}$ in a p o i n t $M_{3}$ • Finally, let $\upgamma^{\ast}$ be obtained from $\upgamma$ by replacing the part of $\upgamma$ from $M_{0}$ to $M_{1}$ by the curve $M_{0}M_{3}M_{1}$ where $M_{0}M_{3}$ is the extremal from $M_{0}$ to $M_{3}$ and $M_{3}M_{1}$ is the straight line segment from $M_{3}$ to $M_{1}$ . Again using Hilbert's invariant integral, prove that $\upgamma^{\ast}$ satisfies the inequality (72).  

7  

I n this chapter, we d iscuss a variety of topics pertaining to functionals which depend on functions of two or more variables. Such functionals arise, for example, in mechanical problems i nvolving systems with infinitely many degrees of freedom (strings, membranes, etc.). In our treatment of systems consisting of a fi nite n u m ber of particles (see Chapter 4), we derived the principle of least action and a general method for obtaining conservation laws (Noether's theorem). These methods will now be applied to systems with infinitely many degrees of freedom.  

# 35. Var i at i o n of a F u n ctional Defi n ed on a Fixed Reg ion  

Consider t h e functional  

$$
J[u]=\int\cdot\cdot\cdot\int_{R}F(x_{1},\cdot\cdot\cdot,x_{n},u,u_{x_{1}},\cdot\cdot\cdot,u_{x_{n}})d x_{1}\cdot\cdot\cdot d x_{n},
$$  

depending on $n$ independent variables $x_{1},...,x_{n}$ , an unknown function $\pmb{u}$ of these variables, and the partial derivatives $u_{x_{1}},\ldots,u_{x_{n}}$ of $\pmb{u}$ . (As usual, it is assumed that the i n tegrand $F$ has conti nuous first and second derivatives with respect to all its a rgu ments.) We now calculate the variation of ( I ), assuming that the region $R$ stays fixed, while the function $u(x_{1},....,x_{n})$ goes i nto  

$$
u^{*}(x_{1},...,x_{n})=u(x_{1},...,x_{n})+\mathfrak{s}_{\forall}^{\prime}(x_{1},...,x_{n})+\cdot\cdot\cdot,
$$  

where the dots denote terms of order higher than 1 relative to E. By the variation $\updelta J$ of the fu nctional ( I ), corresponding to the transformation (2), we mean the principal linear part (in E) of the difference  

$$
J[u^{*}]-J[u].
$$  

For simplicity, we write $u(x),\Psi(x)$ instead of $u(x_{1},...,x_{n}),\psi(x_{1},...,x_{n}),$ $d x$ instead of $d x_{1}\dotsm d x_{n},$ , etc. Then, using Taylor's theorem , we find that  

$$
\begin{array}{l}{J[u^{*}]-J[u]=\displaystyle\int_{R}\left\{F[x,u(x)+\mathfrak{e}\psi(x),u_{x_{1}}(x)+\mathfrak{e}\updownarrow_{x_{1}}(x),...,u_{x_{n}}(x)+\mathfrak{e}\updownarrow_{x_{n}}(x)}\\ {\quad\quad\quad-F[x,u(x),u_{x_{1}}(x),...,u_{x_{n}}(x)]\right\}d x}\\ {\displaystyle=\mathfrak{e}\int_{R}\left(F_{u}+\sum_{i=1}^{n}F_{u_{x_{i}}\backslash\xi_{x_{i}}}\right)d x+\cdot\cdot\cdot,}\end{array}
$$  

where the dots again denote terms of order higher than 1 relative to E. It follows that  

$$
\updelta J=\upvarepsilon\int_{R}\left(F_{u}+\sum_{i=1}^{n}F_{u_{z_{i}}}\grave{\psi}_{x_{i}}\right)d x
$$  

is the variation of the functional ( 1 ).  

Next, we try to represent the variation of the functional ( 1 ) as an integral of an expression of the form  

$$
{\cal G}(x)\uppsi(x)+{\cal{\mathrm{div}}}(\cdot\cdot\cdot),
$$  

i.e., we try to transform the expression (3) in such a way that the derivatives $\psi_{x_{i}}$ only appear in a combination of terms which can be written as a diver­ gence. To achieve this, we replace  

by  

$$
\begin{array}{c}{F_{u_{z_{i}}\downarrow\psi_{x_{i}}}(x)}\\ {\displaystyle}\\ {\displaystyle\frac{\partial}{\partial x_{i}}{}\cdot{}[F_{u_{z_{i}}\downarrow}\psi(x)]-\frac{\partial F_{u_{z_{i}}}}{\partial x_{i}}\downarrow(x)}\end{array}
$$  

in (3), obtaining  

$$
\delta J={\mathfrak{c}}\int_{R}\Big(F_{u}-\sum_{i=1}^{n}{\frac{\partial}{\partial x_{i}}}F_{u_{z_{i}}}\Big)\uppsi(x)d x+{\mathfrak{c}}\int_{R}\sum_{i=1}^{n}{\frac{\partial}{\partial x_{i}}}[F_{u_{z_{i}}}\uppsi(x)]d x.
$$  

This expression for the variation $\delta J$ has the important feature that its second term is the integral of a divergence, and hence can be red uced to an integral over the boundary $\Gamma$ of the region $R$ . In fact, let $d\sigma$ be the area of a variable element of $\Gamma$ , regarded as an $(n\mathrm{~-~}1)$ -dimensional surface. Then the $n$ -dimensional version of Green's theorem states that  

$$
\int_{R}\sum_{i=1}^{n}{\frac{\partial}{\partial x_{i}}}\left[F_{u_{z_{i}}}\Psi(x)\right]d x=\int_{\Gamma}\Psi(x)(G,\circ)d\sigma,
$$  

where  

$$
G=(F_{u_{z_{1}}},...,F_{u_{z_{n}}})
$$  

is the n-dimensional vector whose components are the derivatives FU'I ' $\textsf{v}=(\textsf{v}_{1},\ldots\ldots\textsf{v}_{n})$ is the unit outward normal to $\Gamma_{\/{\/}}$ , and $(G,\upnu)$ denotes the scalar product of $G$ and $\blacktriangledown\blacktriangledown\blacktriangledown\blacktriangledown\blacktriangledown\$ . Using (5), we can write (4) in the form  

$$
\delta J=\varepsilon\int_{R}{\Big(}F_{u}-\sum_{i=1}^{n}{\frac{\partial}{\partial x_{i}}}F_{u_{z_{i}}}{\Big)}\uppsi(x)d x+\varepsilon\int_{\Gamma}\uppsi(x)(G,\uppsi)d\sigma,
$$  

where the integral over $R$ no longer involves the derivatives of $\psi(x)$ .  

In order for the functional ( 1 ) to have an extremum, we must require that $\ \delta J=0$ for all admissible $\psi(x)$ , in particular, that $\ \delta J=0$ for all admissible $\Psi(x)$ which vanish on the boundary $\Gamma$ . For such functions, (6) reduces to  

$$
\updelta J=\int_{\mathcal{M}}\bigg(F_{u}-\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}F_{u_{x_{i}}}\bigg)\uppsi(x)d x,
$$  

and then, because of the arbitrariness of $\boldsymbol{\Psi}(\boldsymbol{x})$ in side $R,\delta J=0$ implies that  

$$
F_{u}-\sum_{i=1}^{n}{\frac{\partial}{\partial x_{i}}}F_{u_{x_{i}}}=0
$$  

for all $x\in R$ . This is the Euler equation of the functional (1), and is the $n$ -dimensional generalization of formula (24) of Sec. 5. 1  

Remark. In deriving (7), we assumed that the region of integration $R$ appearing in the functional ( 1 ) is fixed. Generalization of (7) to the case where the region of ntegration is variable will be made in Sec. 36.  

# 36. Va riational Derivat i o n of t h e Eq u at i o n s of M otion of Cont i n u o u s M ech a n i cal Systems  

A s w e saw in Sec. 2 1 , the equations o f motion o f a mechanical system consisting of $\pmb{n}$ particles can be derived from the principle of least action, which states that the actual trajectory of the system in phase space mini­ mizes the action functional  

$$
\int_{t_{0}}^{t_{1}}\left(T-\ U\right)d t,
$$  

where $T$ is the kinetic energy and $U$ the potential energy of the system of particles. We now use this principle, together with our basic formula for the first variation, to derive the equations of motion and the appropriate boundary conditions for some simple mechanical systems with infinitely many degrees of freedom, namely, the vibrating string, membrane and plate.  

36.1. The vibrating string. Consider the transverse motion of a string (i.e. , a homogeneous flexible cord) of length $\iota$ and linear mass density $p$ . Suppose the ends of the string (at $x=0$ and $x=l)$ are fastened elastically, which means that if either end is displaced from its equilibriu m position, a restoring force proportional to the displacement appears. This can be achieved, for example, by fastening the ends of the string to two rings which are constrained to move along two parallel rods, while the rings them selves are held in their initial positions by two ideal springs, 2 as shown in Fig. 8. Let the eq uilibrium position of the string lie along the $x$ -axis, and let $u(x,t)$ denote the dis­ placement of the string at the point $x$ and time t from its equilibrium position. Then, at time $t$ , the kinetic energy of the element of string which initially lies between $x_{0}$ and $x_{0}+\Delta x$ is clearly  

![](https://cdn-mineru.openxlab.org.cn/extract/c29daec4-3bde-4c07-a565-58de41e65c3b/d61dc51d26803cb18d64aed8fea95b114a1ebb9540c3b84c891a3c065b8ed0e7.jpg)  
FIG URE 8  

$$
\begin{array}{r}{\frac{1}{2}\rho u_{t}^{2}(x_{0},t)\Delta x.}\end{array}
$$  

Integrating (9) from 0 to $l.$ , we find that the kinetic energy of the whole string at time $t$ equals  

$$
T=\frac{1}{2}\:\rho\int_{0}^{l}u_{t}^{2}(x,t)\:d x.
$$  

To find the potential energy of the string, we use the following argument : The potential energy of the string in the position described by the function $u(x,t)$ , where $t$ is fixed, is j ust the work req ui red to m ove the string from its equilibri u m position $u\equiv0$ into the given position $u(x,t)$ . Let $\tau$ denote the tension in the spring, and consider the element of string indicated by $\scriptstyle A B$ in Figure 9, which initially ' occupies t h e position $D E$ along the $x$ -axis, i . e . , the nterval $[x_{0},x_{0}+\Delta x]$ v To calculate the amount ofwork needed to move $D E$ o $\scriptstyle A B$ , we first m ove $D E$ to the position $_{A C}$ . This requires no work at all, si nce the force (the tension in the stri ng) is perpendicular to the dis­ placement. 4 Next, we stretch the string from the position $_{A C}$ to the position $\pmb{A}\pmb{C}^{\prime}$ , where the length of $\pmb{A}\pmb{C}^{\prime}$ equals the length of $\ A B$ . This obviously requires an amount of work equal to $\tau\beta$ , where $\beta$ is the length of $C C^{\prime}$ . Finally, we rotate $A C^{\prime}$ about the point $A$ into the final position $\pmb{A}\pmb{B}.$ . Like the first step, this requires no work at all, since at each stage of the rotation the force is perpendicular to the displacement. Thus, the total amount of work requi red to move $D E$ to $\pmb{A}\pmb{B}$ is j ust the product of $\bar{\boldsymbol{\uptau}}$ and the increase in length of the element of string, i.e. , the quantity  

$$
\tau\sqrt{(\Delta x)^{2}+(\Delta u)^{2}}-\tau\Delta x=\frac{1}{2}\tau\Big(\frac{\Delta u}{\Delta x}\Big)^{2}\Delta x+\cdot\cdot\cdot=\frac{1}{2}\tau u_{x}^{2}(x_{0},t)\Delta x+\cdot\cdot\cdot,
$$  

where the dots indicate terms o f order higher than those written $(\Delta u/\Delta x\ll1$ for all $t$ , since the vibrations are small).  

![](https://cdn-mineru.openxlab.org.cn/extract/c29daec4-3bde-4c07-a565-58de41e65c3b/ed06d33c238532e25dbb60fb3bb9eb15f25ee5a1e42e06247c7c406f8cf8cb11.jpg)  
FIGURE 9  

Integrating ( I I )  from ° to $l_{s}$ we find that the potential energy of the whole string is  

$$
U_{1}=\frac{1}{2}\thinspace\thinspace\tau\int_{0}^{l}u_{x}^{2}(x,t)\thinspace d x,
$$  

except for the work expended in displacing the elastically fastened ends of the string from their e9uilibrium positions. This work equals  

$$
U_{2}=\frac{1}{2}\varkappa_{1}u^{2}(0,t)+\frac{1}{2}\varkappa_{2}u^{2}(l,t),
$$  

where $\varkappa_{1}$ and $x_{2}$ are positive constants (the elastic moduli of the springs). [In fact, the force $f_{1}$ acting on the end point $P_{1}$ (see Figure 8) is proportional to the displacement $\boldsymbol{\xi}$ of ${\pmb P}_{1}$ from its equilibrium position $x=0,u=0$ , i . e . ,  

$$
|f_{1}|=\varkappa_{1}\xi,
$$  

where $x_{1}>0$ is a constant ; integration of ( 1 4) shows that the work req uired to move $P_{1}$ fro m (0, 0) to $(0,u(0,t))$ , its position at time $t$ , is given by  

$$
\int_{0}^{u(0,t)}\varkappa_{1}\xi d\xi=\frac{1}{2}\varkappa_{1}u^{2}(0,t),
$$  

and similarly for the other end point $P_{2}$ .] Then, adding ( 1 2) and ( 1 3), we find that the total potential energy of the string in the position described by the function $u(x,t)$ i s  

$$
U=U_{1}+U_{2}=\frac{1}{2}\uptau\int_{0}^{\imath}u_{\mathrm{r}}^{2}(x,t)d x+\frac{1}{2}\upvarkappa_{1}u^{2}(0,t)+\frac{1}{2}\upvarkappa_{2}u^{2}(l,t).
$$  

Finally, using ( 1 0) and ( 1 5) , we write the action (8) for the vibrating string, obtaining the functional  

$$
\begin{array}{l}{{\displaystyle{J[u]}=\frac{1}{2}\int_{t_{0}}^{t_{1}}\int_{0}^{l}\left[\rho{u_{t}^{2}}(x,t)-\tau{u_{x}^{2}}(x,t)\right]d x d t}}\\ {{\displaystyle{~-\frac{1}{2}\times_{1}\int_{t_{0}}^{t_{1}}u^{2}(0,t)d t-\frac{1}{2}\times_{2}\int_{t_{0}}^{t_{1}}u^{2}(l,t)d t}.}}\end{array}
$$  

According to the principle of least action, $\delta J$ must vanish for the function $u(x,t)$ which describes the actual motion of the string. Thus, we now calculate the variation $\delta J$ of the functional ( 1 6). Suppose we go from the function $u(x,t)$ to the " varied " function  

$$
u^{*}(x,t)=u(x,t)+\mathfrak{s}\Psi(x,t)+\cdot\cdot\cdot
$$  

Then, using formula (4) and the fact that the variation of a sum equals the sums of the variations of the separate terms, we find that  

$$
\begin{array}{l}{\displaystyle\bar{\delta}J=\ensuremath{\varepsilon}\Biggl\{\int_{t_{0}}^{t_{1}}\int_{0}^{l}\ensuremath{\v{D}}[-\rho\boldsymbol{u}_{t t}(\boldsymbol{x},t)+\tau\boldsymbol{u}_{x x}(\boldsymbol{x},t)]\dot{\boldsymbol{\psi}}(x,t)d x d t}\\ {\displaystyle\quad-\scriptsize{\*}_{1}\int_{t_{0}}^{t_{1}}u(0,t)\ \dot{\boldsymbol{\psi}}(0,t)d t-\varkappa_{2}\int_{t_{0}}^{t_{1}}u(l,t)\dot{\boldsymbol{\psi}}(l,t)d t\Biggr\}}\\ {\displaystyle\quad+\ \varepsilon\int_{t_{0}}^{t_{1}}\int_{0}^{l}\frac{\partial}{\partial\boldsymbol{x}}\left[-\tau\boldsymbol{u}_{x}(\boldsymbol{x},t)\ \boldsymbol{\psi}(\boldsymbol{x},t)\right]d\boldsymbol{x}d t}\\ {\displaystyle\quad+\ \varepsilon\int_{t_{0}}^{t_{1}}\int_{0}^{l}\frac{\partial}{\partial t}\left[\rho\boldsymbol{u}_{t}(\boldsymbol{x},t)\boldsymbol{\psi}(\boldsymbol{x},t)\right]d\boldsymbol{x}d t.}\end{array}
$$  

If we assume that the admissible functions $\boldsymbol{\Psi}(\boldsymbol{x},t)$ are such that  

$$
\begin{array}{r}{\psi(x,t_{0})=0,\psi(x,t_{1})=0(0\leqslant x\leqslant l),}\end{array}
$$  

i.e., that $u(x,t)$ is not varied at the initial and final times, then the last term in ( 1 7) vanishes and the next to the last term reduces to  

$$
\varepsilon\int_{t_{0}}^{t_{1}}\left[\tau u_{x}(0,t)\psi(0,t)-\tau u_{x}(l,t)\psi(l,t)\right]d t.
$$  

I t follows that the variation ( \ 7) can be written in the form  

$$
\begin{array}{c}{{\displaystyle\delta J=\mathsf{\varepsilon}\biggl\{\int_{t_{0}}^{t_{1}}\int_{0}^{l}\big[-\mathsf{\varepsilon}u_{t t}+\mathsf{\varepsilon}u_{x x}(x,t)\big]\uppsi(x,t)d x d t}}\\ {{\displaystyle-\int_{t_{0}}^{t_{1}}\big[\mathsf{x}_{1}u(0,t)-\mathsf{\varepsilon}u_{x}(0,t)\big]\uppsi(0,t)d t}}\\ {{\displaystyle-\int_{t_{0}}^{t_{1}}\big[\mathsf{x}_{2}u(l,t)+\mathsf{\varepsilon}\boldsymbol{u}_{x}(l,t)\big]\uppsi(l,t)d t\biggr\}.}}\end{array}
$$  

According to the principle of least action, the expression ( 1 8) must vanish for the function $u(x,t)$ corresponding to the actual motion of the string. Suppose first that $\boldsymbol{\Psi}(\boldsymbol{x},t)$ vanishes at the end of the string,5 i . e . , that  

$$
\Psi(0,t)=0,\Psi(l,t)=0\qquad(t_{0}\leqslant t\leqslant t_{1}).
$$  

Then ( 1 8) reduces to j ust  

$$
\delta J=\varepsilon\int_{t_{0}}^{t_{1}}\int_{0}^{l}\left[-\rho u_{t t}(x,t)+\tau u_{x x}(x,t)\right]\psi(x,t)d x d t.
$$  

Setting (20) equal to zero, and using the arbitrariness of the interval $[t_{0},t_{1}]$ and of the function $\boldsymbol{\Psi}(\boldsymbol{x},t)$ for $0<x<l,$ $t_{0}<t<t_{1}$ (cf. the lemma of Sec. 5), we find that  

$$
u_{t t}(x,t)=a^{2}u_{x x}(x,t)\qquad\left(a^{2}=\frac{\tau}{\rho}\right)
$$  

for $0\leqslant x\leqslant l$ and all $t.$ . This result, called the equation of the vibrating string, is the Euler equation of the functional  

$$
\frac{1}{2}\int_{t_{0}}^{t_{1}}\int_{0}^{l}\left[u_{t}^{2}(x,t)-\tau u_{x}^{2}(x,t)\right]d x d t.
$$  

Next, we remove the restriction ( 1 9). Since ${u}(x,t)$ must satisfy (2 1 ) , the first term in ( 1 8) vanishes, and we have  

$$
\begin{array}{r}{\displaystyle\mathfrak{J}J=-\mathfrak{e}\Big\{\int_{t_{0}}^{t_{1}}\lbrack\varkappa_{1}u(0,t)-\tau u_{x}(0,t)\rbrack\boldsymbol{\psi}(0,t)d t}\\ {\displaystyle+\int_{t_{0}}^{t_{1}}\lbrack\varkappa_{2}u(l,t)+\tau u_{x}(l,t)\rbrack\boldsymbol{\psi}(l,t)d t\Big\}.}\end{array}
$$  

This expression must also vanish for the function ${u}(x,t)$ corresponding to the actual motion of the string. Since $[t_{0},t_{1}]$ is arbitrary and $\Psi(0,t),\Psi(l,t)$ are arbitrary admissible functions, equating (22) to zero leads to the relations  

$$
\varkappa_{1}u(0,t)-\tau u_{x}(0,t)=0
$$  

and  

$$
\varkappa_{2}u(l,t)+\tau u_{x}(l,t)=0
$$  

for all $t$ . Thus, finally, the function $u(x,t)$ which describes the oscillations of the string must satisfy (2 1 ) and the boundary conditions  

$$
\alpha u(0,t)+u_{x}(0,t)=0\qquad\left(\alpha=-\frac{\varkappa_{1}}{\tau}\right)
$$  

and  

$$
\beta u(l,t)+u_{x}(l,t)=0\qquad\bigg(\beta=\frac{\varkappa_{2}}{\tau}\bigg),
$$  

which connect the displacement from equilibrium and the direction of the tangent at each end of the string.  

Next, suppose the ends of the string are free, which means that the springs shown in Fig. 8 are absent and the rings fastening the string to the lines $x=0$ , $x=l$ can move up and down freely. Then $\varkappa_{1}=\varkappa_{2}=0$ , and the boundary conditions (23), (24) become  

$$
u_{x}(0,t)=0,\qquadu_{x}(l,t)=0.
$$  

Thus, at a free end point, the tangent to the string always preserves the same slope (zero) as it had in the equilibriu m position.  

The case where the ends of the string are fixed, corresponding to the boundary conditions  

$$
u(0,t)=0,\qquadu(l,t)=0,
$$  

can be regarded as a limit of the case of elastically fastened ends. In fact, let the stiffness of the springs binding the ends of the string to their initial positions increase without limit, i . e . , let $\varkappa_{1}\to\infty$ 0, ${\pmb x}_{2}\rightarrow\infty$ .  Then, dividing (23) by $x_{1}$ and (24) by ${\pmb x}_{2}$ , and taking this limit, we obtain the conditions (27).  

36.2. Least action vs. stationary action. The principle of least action is widely used not only in mechanics, but also in other branches of physics, e.g. , in electrodynamics and field theory. However, as already noted (see Remark 2, p. 8 5), in a certain sense the principle is not quite true. For example, consider a simple harmonic oscillator, i.e., a particle of mass m oscillating about an equilibrium position under the action of an elastic restoring force (cf. Chap. 4, Prob. 2). The equation of motion of the par­ ticle is  

$$
m\ddot{x}+\varkappa x=0,
$$  

with solution  

$$
x=C\sin{(\omega t+\theta)},
$$  

where  

$$
\omega={\sqrt{\frac{\varkappa}{m}}},
$$  

and the values of the constants $c,\mathfrak{\theta}$ are determined from the initial conditions . Moreover, the particle has kinetic energy  

$$
\scriptstyle T={\frac{1}{2}}m{\dot{x}}^{2}
$$  

and potential energy  

$$
\begin{array}{r}{U=\frac{1}{2}\varkappa x^{2},}\end{array}
$$  

so that the action is  

$$
\frac{1}{2}\int_{t_{0}}^{t_{1}}\left(m\dot{x}^{2}-\varkappa x^{2}\right)d t.
$$  

Equation (28) is the Euler equation of the functional (30), but in general we cannot assert that its solution (29) actually minimizes (30). In fact, consider the solution  

$$
x={\frac{1}{\omega}}\sin\omega t,
$$  

which passes through the point $x=0,\ t=0$ and satisfies the condition $\dot{x}(0)=1$ .  The point $(\pi/\omega,0)$ is conjugate to the point (0, 0), since every  

extremal satisfying condition $x(0)=0$ intersects the extremal (3 1 ) at $(\pi/\omega,0)$ [see p . 1 1 4 ] . Since  

$$
F_{t t}=m>0
$$  

for the functional (30), the extremal (3 1 ) satisfies the sufficient conditions for a minimum (in fact, a strong minimum), provided that  

$$
0\leqslant t\leqslant t_{0}<\frac{\pi}{\omega}\cdot
$$  

However, if we consider time intervals greater than $\pi/\upomega$ ,  we can no longer guarantee that the extremal (3 1 ) minimizes the functional (30).  

Next, consider a system of $\pmb{n}$ coupled oscillators, with kinetic energy  

$$
T=\sum_{i,k=1}^{n}a_{i k}{\dot{x}}_{i}{\dot{x}}_{k}
$$  

(a quadratic form in the velocities $\dot{x}_{i}^{\cdot}$ ) and potential energy  

$$
U=\sum_{i,k=1}^{n}b_{i k}x_{i}x_{k}
$$  

(a quadratic form in the coordinates $x_{i}$ ). The quadratic form (32) is positive definite (since it is a kinetic energy) ; therefore, (32) and (33) can be simul­ taneously reduced to sums of squares by a suitable linear transformation6  

$$
x_{i}=\sum_{k=1}^{n}c_{i k}q_{k}\qquad(i=1,...,n),
$$  

i . e . , substitution of (34) into (32) and (33) gives  

$$
T=\sum_{i=1}^{n}\dot{q}_{i}^{2},~U=\sum_{i=1}^{n}\uplambda_{i}q_{i}^{2}.
$$  

Then the equations of motion of the system of oscillators are given by the Euler equations  

$$
\frac{d}{d t}\Big(\frac{\partial T}{\partial\dot{q}_{i}}\Big)+\frac{\partial U}{\partial q_{i}}=\ddot{q}_{i}+\uplambda_{i}q_{i}=0\qquad(i=1,...,n),
$$  

corresponding to the action functional  

$$
\int_{t_{0}}^{t_{1}}\sum_{i=1}^{n}({\dot{q}}_{i}^{2}-\lambda_{1}q_{i}^{2})d t.
$$  

Suppose all the $\lambda_{i}$ are positive, which means that we are considering oscillations of the system about a position of stable equilibrium . Then the solution of the system (35) has the form  

$$
q_{i}=C_{i}\sin\omega_{i}(t+\theta_{i})(i=1,...,n),
$$  

where  

$$
\omega_{i}=\sqrt{\overline{{\lambda_{i}}}},
$$  

and the values of the constants $C_{i},\ \theta_{i}$ are determined from the initial con­ ditions. An argument like that made for the simple harmonic oscillator $(n=1)$ shows that a trajectory of the system [i. e . , a curve given by (36) in a space of $n+1$ dimensions] whose projection on the time axis is of length no greater than $\pi/\omega$ , where  

$$
\omega=\operatorname*{max}_{1\leqslant i\leqslant n}\omega_{i},
$$  

contains no conjugate points and satisfies the sufficient conditions for a minimum. However, just as before, we cannot guarantee that a trajectory whose projection on the time axis is of length greater than ${\pi}/{\omega}$ actually minimizes the action.  

Finally, consider a vibrating string of length I with fixed ends.7 As shown above, the function $u(x,t)$ describing the oscillations of the string satisfies the equation  

$$
u_{t t}(x,t)=a^{2}u_{x x}(x,t)
$$  

and the boundary conditions  

$$
u(0,t)=0,\qquadu(l,t)=0.
$$  

It follows thatB  

$$
u(x,t)=\sum_{k=1}^{\infty}C_{k}(x)\sin\upomega_{k}(t+\uptheta_{k}),
$$  

where  

$$
\omega_{k}=\frac{k a\pi}{l},
$$  

and $C_{k}(x)$ , $\uptheta_{\boldsymbol{k}}$ are determined from the initial conditions. Thus, in a certain sense, a vibrating string can be regarded as a system of infinitely many coupled oscillators, with natural frequencies (37). However, the numbers (37) have no finite upper bound, and hence the analogy with the case of $n$ coupled oscillators leads us to believe that for a vibrating string, there is no time ihӢerval short enough to guarantee that ${u}(x,t)$ actually mlmmlzes the action functional. Similar arguments can be carried out for other systems with infinitely many degrees of freedom.  

Guided by the above considerations, we shall henceforth replace the principle of least action by the principle of stationary action. In other words, the actual trajectory of a given mechanical system will not be required to minimize the action but only to cause its first variation to vanish.  

36.3. The vibrating membrane. Consider the transverse motion of a membrane (i.e., a homogeneous flexible sheet) of surface mass density $p$ . Let $u(x,y,t)$ denote the displacement from equilibrium of the point $(x,y)$ of the membrane, at time $t$ . The kinetic energy of the membrane at time $t$ is given by  

$$
T=\frac{1}{2}\:\rho\int\int_{R}u_{t}^{2}(x,y,t)\:d x\:d y,
$$  

where $R$ is the region of the $x y$ -plane occupied by the membrane at rest. The potential energy of the membrane in the position described by the function $u(x,y,t)$ , where $t$ is fixed, is just the work required to move the membrane from its equilibrium position $u\equiv0$ into the given position $u(x,y,t)$ . This work is the sum of the work $U_{\mathbf{1}}$ expended in deforming the membrane and the work $U_{\mathbf{2}}$ expended in moving the boundary of the mem­ brane, which we assume to be elastically fastened to its equilibrium position.  

To calculate $U_{\mathbf{1}}$ , let $\bar{\boldsymbol{\uptau}}$ denote the tension in the membrane, and consider the element $\Delta A$ of the membrane initially occupying the region $x_{0}\leqslant x\leqslant x_{0}+\Delta x.$ $y_{0}\leqslant y\leqslant y_{0}+\Delta y$ . Then, j ust as in the case of the string, the work needed to deform $\Delta A$ equals the product of $\bar{\boldsymbol{\uptau}}$ and the increase in the area of $\Delta A$ under deformation, i.e.,  

$$
\begin{array}{l}{\displaystyle\tau\sqrt{(\Delta x)^{2}+(\Delta u)^{2}}\ \sqrt{(\Delta y)^{2}+(\Delta u)^{2}}-\tau\Delta x\Delta y}\\ {\displaystyle=\frac{1}{2}\ \tau\Big[\Big(\frac{\Delta u}{\Delta x}\Big)^{2}+\Big(\frac{\Delta u}{\Delta y}\Big)^{2}\Big]\Delta x\Delta y+\cdot\cdot\cdot,}\\ {\displaystyle=\frac{1}{2}\thinspace\tau[u_{x}^{2}(x_{0},y_{0},t)+u_{y}^{2}(x_{0},y_{0},t)]\Delta x\Delta y+\cdot\cdot\cdot,}\end{array}
$$  

where the dots indicate terms of order higher than those written. Integrating (39) over $R$ , we find that the work required to deform the whole membrane is  

$$
U_{1}=\frac{1}{2}\thinspace\thinspace\thinspace\thinspace\tau\int\int_{R}\left[u_{x}^{2}(x,y,t)+\left.u_{y}^{2}(x,y,t)\right]{d x}{d y}.
$$  

To calculate $U_{\mathbf{2}}$ , we generalize the argument used to derive ( 1 4). If $\Gamma$ is the boundary of the region $R$ , and $s$ is arc length measured along $\Gamma$ from some fixed point on $\Gamma$ , then  

$$
U_{2}=\frac{1}{2}\int_{\Gamma}\varkappa(s)u^{2}(s,t)d s,
$$  

where $u(s,t)$ is the displacement of the membrane from equilibrium at the point $\pmb{s}$ and time $t$ , and $\varkappa(s)$ is the linear density of the elastic modulus of the forces retaining the boundary of the membrane.9 Combining (38), (40) and (4 1), we find that the action functional for the vibrating membrane is  

$$
\begin{array}{l}{{\displaystyle{J[u]=\int_{t_{0}}^{t_{1}}\left(T-U_{1}-U_{2}\right)d t}}}\\ {{\displaystyle~=\frac12\int_{t_{0}}^{t_{1}}\int\int_{R}\left\{\varphi u_{t}^{2}(x,y,t)-\tau[u_{x}^{2}(x,y,t)+u_{y}^{2}(x,y,t)]\right\}d x d y d t}}\\ {{\displaystyle~-\frac12\int_{t_{0}}^{t_{1}}\int_{\Gamma}\varkappa(s)u^{2}(s,t)d s d t.}}\end{array}
$$  

Suppose we go from the function $u(x,y,t)$ to the " varied " function  

$$
u^{*}(x,y,t)=u(x,y,t)+\mathfrak{s}\psi(x,y,t)+\cdot\cdot\cdot
$$  

Then, using formula (4) of Sec. 35 and dropping arguments of functions, we find that the variation $\otimes J$ of the functional (42) is  

$$
\begin{array}{l}{{\displaystyle\left.\begin{array}{l}{{\displaystyle\left.\left\{\begin{array}{l}{{\displaystyle\partial J=\varepsilon\int_{t_{0}}^{t_{1}}\int\int_{R}\left[-\rho{u_{t t}}+\tau(u_{x x}+u_{y y})\right]\right\}\psi\ d x\ d y\ d t}}}\\ {{\displaystyle-\varepsilon\int_{t_{0}}^{t_{1}}\int_{\Gamma}\varkappa u\overline{{\psi}}\ d s\ d t-\varepsilon\tau\int_{t_{0}}^{t_{1}}\iint_{R}\left[\frac{\partial}{\partial x}\left(u_{x}\overline{{\psi}}\right)+\frac{\partial}{\partial y}\left(u_{y}\overline{{\psi}}\right)\right]d x d y d t}}\\ {{\displaystyle+\varepsilon\int_{t_{0}}^{t_{1}}\int\int_{R}\frac{\partial}{\partial t}\left(u_{t}\overline{{\psi}}\right)d x d y d t.}}\end{array}\right.}}\end{array}
$$  

Just as in the case of the vibrating string, we assume that the function $u(x,y,t)$ is not varied at the initial and final times, i . e . , that  

$$
\begin{array}{r}{\Psi(x,y,t_{0})=\Psi(x,y,t_{1})\equiv0.}\end{array}
$$  

Because of (44), the last integral in (43) vanishes. Moreover, using Green's theorem in two dimensions (see p. 23), we have  

$$
\begin{array}{r l}&{\displaystyle\int\int_{R}\left[\frac{\partial}{\partial x}\left(u_{x}\uppsi\right)+\frac{\partial}{\partial y}\left(u_{y}\uppsi\right)\right]d x d y=\int_{\Gamma}\left(u_{x}\uppsi\ d y-u_{y}\uppsi d x\right)}\\ &{\quad=\int_{\Gamma}\left[\frac{\partial u}{\partial n}\cos\mathfrak{d}\cdot\uppsi d s\sin\left(\frac{\uppi}{2}+\mathfrak{s}\right)-\frac{\partial u}{\partial n}\sin\mathfrak{d}\cdot\uppsi d s\cos\left(\frac{\uppi}{2}+\mathfrak{s}\right)\right]}\\ &{\quad=\int_{\Gamma}\frac{\partial u}{\partial n}\uppsi d s,}\end{array}
$$  

where $\partial/\partial n$ denotes differentiation with respect to $n$ , the outward normal to $\Gamma_{\/{\leftmoon}\right.}$ , and $\mathfrak{g}$ is the angle between $n$ and the $x$ -axis. Thus, we can finally write (43) in the form  

$$
\begin{array}{c}{{\displaystyle\displaystyle\delta J=\varepsilon\int_{t_{0}}^{t_{1}}\int\int_{R}^{}[-\rho u_{t t}+\tau(u_{x x}+u_{y y})]\psi d x d y d t}}\\ {{-\displaystyle\varepsilon\int_{t_{0}}^{t_{1}}\int_{\Gamma}\Big(\varkappa u+\tau\frac{\partial u}{\partial n}\Big)\big\}d s d t.}}\end{array}
$$  

9 More precisely, let the parametric equations of $\Gamma$ be  

$$
x=x(s),\qquady=y(s),\qquads_{0}\leqslant s\leqslant s_{1}.
$$  

Then $u(s,t)$ means $u[x(s),y(s),t]$ , and " the point $\boldsymbol{s}^{\flat}$ means the point $(x(s),y(s))$ .  

We first assume that  

$$
\begin{array}{r}{\Psi(s,t)=0\qquad(s\in\Gamma),}\end{array}
$$  

where $t$ is arbitrary, i . e . , that $\pmb{u}$ does not vary on the boundary of the mem­ brane. Then (45) reduces to just  

$$
\displaystyle\delta J=\int_{t_{0}}^{t_{1}}\int\int_{R}\left[-\rho u_{t t}+\tau(u_{x x}+u_{y y})\right]d x d y d t.
$$  

Setting (47) equal to zero, and using the arbitrariness of the interval $[t_{0},t_{1}]$ and of the function $\Psi=\Psi(x,y,t)$ inside $R\times[t_{0},t_{1}]_{\cdot}$ , we find that  

$$
u_{t t}(x,y,t)=a^{2}[u_{x x}(x,y,t)+u_{y y}(x,y,t)]\qquad\left(a^{2}=\frac{\tau}{\Theta}\right)
$$  

for $(x,y)\in R$ and all $t$ , a result known as the equation of the vibrating mem­ brane. 1 Equation (48) can also be written as  

$$
u_{t t}(x,y,t)=a^{2}\nabla^{2}u(x,y,t),
$$  

in terms of the Laplacian (operator)  

$$
\nabla^{2}=\frac{\partial^{2}}{\partial x^{2}}+\frac{\partial^{2}}{\partial y^{2}}\cdot
$$  

Next, we remove the restriction (46) . Since $u(x,y,t)$ must satisfy (48), the first term in (45) vanishes, and we are left with  

$$
\delta J=-\varepsilon\int_{t_{0}}^{t_{1}}\int_{\Gamma}\Big[x(s)u(s,t)+\tau\frac{\partial u(s,t)}{\partial n}\Big]\psi(s,t)d s d t.
$$  

Then, since $\boldsymbol{\Psi}(s,t)$ is an arbitrary admissible function, equating (50) to zero leads to the formulal l  

$$
\varkappa(s)u(s,t)+\tau\frac{\partial u(s,t)}{\partial n}=0\qquad(s\in\Gamma).
$$  

This is the boundary condition satisfied b y a vibrating membrane when its boundary is elastically fastened to its eq uilibrium position. In particular, if the boundary of the membrane is free, $\varkappa(s)=0$ and (5 1 ) becomes  

$$
\frac{\partial u(s,t)}{\partial n}=0\qquad(s\in\Gamma),
$$  

while if the boundary of the membrane is fixed, $\varkappa(s)=\infty$ and (5 1 ) becomes  

$$
u(s,t)=0\qquad(s\in\Gamma).
$$  

36.4. The vibrating plate. Finally, we use the principle of stationary action to derive the equation of motion and the boundary conditions for the transverse vibrations of a plate (i.e., a homogeneous two-dimensional elastic body) with surface mass density $p$ . As in the case of the vibrating membrane, let $u(x,y,t)$ denote the displacement from equilibrium of the point $(x,y)$ of the plate, at time $t$ . Then the kinetic energy of the plate at time $t$ is given by  

$$
T=\frac{1}{2}\:\rho\int\int_{R}u_{t}^{2}(x,y,t)\:d x\:d y,
$$  

where $R$ is the region of the $x y.$ -plane occupied by the plate at rest [cf. (38)].  

The potential energy of deformation of the plate, which we denote by $U_{1;}$ > depends on how the plate is bent, and hence involves the second derivatives $u_{x x},u_{x y}$ and $u_{y y}$ • Unlike the case of the membrane, it is assumed that no work is done in stretching the plate, so that $U_{1}$ does not involve $u_{x}$ and $u_{y}$ • Moreover, we require $U_{1}$ to be a quadratic functional in $u_{x x},u_{x y}$ and $u_{y y}$ , 1 2 which does not depend on the orientation of the coordinate system. Then, since the matrix  

$$
\begin{array}{r l}{\left\|u_{x x}\quad u_{x y}\right\|}&{{}}\\ {u_{y x}}&{{}u_{y y}\right\|}\end{array}
$$  

has just two invariants under rotations, i.e., its trace and its determinant, 13 it follows that  

$$
U_{1}=\int\int_{R}\left[A(u_{x x}+u_{y y})^{2}+B(u_{x x}u_{y y}-u_{x y}^{2})\right]d x d y,
$$  

where $A$ and $\pmb{B}$ are constants. Equation (55) is usually written in the form  

$$
U_{1}=\frac{1}{2}c\int\int_{R}{[(u_{x x}^{2}+u_{y y}^{2})-2(1-\mu)(u_{x x}u_{y y}-u_{x y}^{2})]d x d y},
$$  

where $c$ is a constant depending on the choice of units, and $\mu$ is an absolute constant (Poisson's ratio) characterizing the material from which the plate is made. For simplicity, we set $c=1$ .  

In addition to the potential energy of deformation $U_{1}$ , the total potential energy of the plate may also contain a contribution $U_{\mathbf{2}}$ due to bending moments with density $m(s,t)$ , prescribed on the boundary $\Gamma$ of $R$ , and a contribution $U_{3}$ due to external forces acting on $R$ with surface density $f(x,y,t)$ and on $\Gamma$ with linear density $p(s,t)$ . This would give  

$$
U_{2}=\int_{\Gamma}{m(s,t){\frac{\partial u(s,t)}{\partial n}}d s},
$$  

where $\partial/\partial n$ enotes differentiation with respect to $n,$ the outward normal to $\Gamma$ , and14  

$$
U_{3}=\int\int_{R}f(x,y,t)u(x,y,t)d x d y+\int_{\Gamma}p(s,t)d s.
$$  

Combining (54), (56), (57) and (58), we find that the action functional for the vibrating plate is  

$$
\begin{array}{l}{\displaystyle{J[u]=\int_{t_{0}}^{t_{1}}\left(T-U_{1}-U_{2}-U_{3}\right)d t}}\\ {\displaystyle{\quad=\frac{1}{2}\int_{t_{0}}^{t_{1}}\int\int_{R}\left[\rho u_{t}^{2}-(u_{x x}+u_{y y})^{2}+2(1-\mu)(u_{x z}u_{y y}-u_{z y}^{2})-2f u\right]d x d y}}\\ {\displaystyle{\quad\quad-\int_{t_{0}}^{t_{1}}\int_{\Gamma}\left(p u+m\frac{\partial u}{\partial n}\right)d s d t.}}\end{array}
$$  

Unlike the corresponding expressions for the vibrating string and the vibrating membrane, (59) contains second derivatives of the unknown function $\pmb{u}$ . The variation of (59) corresponding to the transition from $u(x,y,t)$ to  

$$
u^{*}(x,y,t)=u(x,y,t)+\mathfrak{s}\psi(x,y,t)+\cdot\cdot\cdot
$$  

turns out to be (see Problems 4 and 5, p. 1 90)  

$$
\begin{array}{l}{\displaystyle\delta{J=\varepsilon\int_{t_{0}}^{t_{1}}\int\int_{R}\left(-\rho{u_{t t}}-\nabla^{4}u-f)\psi d x d y d t\right.}}\\ {\displaystyle+\left.\varepsilon\int_{t_{0}}^{t_{1}}\int_{\Gamma}\left[(P-p)\psi+(M-m)\frac{\partial\psi}{\partial n}\right]d s d t.}\end{array}
$$  

Here,  

$$
M=\mathrm{~-~}[\mu\nabla^{2}u+(1-\mu)(u_{x x}x_{n}^{2}+2u_{x y}x_{n}y_{n}+u_{y y}y_{n}^{2})]
$$  

and  

$$
P=\frac{\partial}{\partial n}\nabla^{2}u+\left(1-\mu\right)\frac{\partial}{\partial s}\left[u_{x x}x_{n}x_{s}+u_{x y}(x_{n}y_{s}+x_{s}y_{n})+u_{y y}y_{n}y_{s}\right],
$$  

where $\partial/\partial n$ enotes differentiation in the direction of the outward normal to $\Gamma$ , with direction cosines $x_{n},y_{n}$ , and $\partial/\partial\pmb{s}$ enotes differentiation in the direction of the tangent to $\Gamma$ , with direction cosines $x_{s},y_{s}$ ' Moreover.  

$$
\nabla^{4}u=\nabla^{2}(\nabla^{2}u)=\frac{\partial^{4}u}{\partial x^{4}}+2\frac{\partial^{4}u}{\partial x^{2}\partial y^{2}}+\frac{\partial^{4}u}{\partial y^{4}},
$$  

according to (49).  

We first assume that  

$$
\begin{array}{r}{\boldsymbol{\Psi}(s,t)=0,\frac{\partial\boldsymbol{\Psi}(s,t)}{\partial\boldsymbol{n}}=0\qquad(s\in\Gamma),}\end{array}
$$  

where $t$ is arbitrary, i.e., that $\pmb{u}$ and its normal derivative do not vary on the boundary of the plate. Then (60) reduces to just  

$$
\delta J=\varepsilon\int_{t_{0}}^{t_{1}}\int\int_{R}\left(-\rho u_{t t}-\nabla^{4}u-f)\psi d x d y d t.\right.
$$  

Setting (64) equal to zero, and using the arbitrariness of the interval $[t_{0},~t_{1}]$ and of the function $\Psi=\Psi(x,y,t)$ inside $R\times[t_{0},t_{1}]_{\mathrm{:}}$ , we obtain the equation forforced vibrations of the plate : 15  

$$
\begin{array}{r}{\rho u_{t t}(x,y,t)+\nabla^{4}u(x,y,t)+f(x,y,t)=0.}\end{array}
$$  

If we set $\scriptstyle f\equiv0$ , so that there are no external forces acting on the plate, (65) reduces to the equation for free vibrations of the plate  

$$
\begin{array}{r}{\rho u_{t t}(x,y,t)+\nabla^{4}u(x,y,t)=0.}\end{array}
$$  

Finally, if we set ${\boldsymbol{u}}_{t t}\equiv0$ in (65) and assume that $f=f(x,y)$ is independent of time, we obtain an equation for the equilibrium position of the plate under the action of external forces :  

$$
\nabla^{4}u(x,y)+f(x,y)=0.
$$  

This equation could have been obtained directly from the condition for the potential energy of the plate to have a minimum (see Remark 2 below).  

Next, we remove the restriction (63). Since $u(x,y,t)$ must satisfy (65), the first term i n (60) vanishes, and we are left with  

$$
\delta J=\varepsilon\int_{t_{0}}^{t_{1}}\int_{\Gamma}\Big[(P-p)\psi+(M-m)\frac{\partial\psi}{\partial n}\Big]d s d t.
$$  

Then, since the functions $\uppsi,\partial\uppsi/\partial\pmb{n}$ and the interval $[t_{0},t_{1}]$ are arbitrary, equating (66) to zero leads to the natural boundary conditions  

$$
P(s,t)-p(s,t)=0,\ M(s,t)-m(s,t)=0\qquad(s\in\Gamma).
$$  

If the boundary of the plate is clamped, the conditions (67) are replaced by the " imposed " boundary conditions  

$$
u(s,t)=0,\frac{\partial u(s,t)}{\partial n}=0\qquad(s\in\Gamma).
$$  

If the plate is supported, i.e., if the boundary of the plate is held fixed while the tangent plane at the boundary can vary, we obtain the boundary con­ ditions  

$$
u(s,t)=0,M(s,t)-m(s,t)=0\qquad(s\in\Gamma).
$$  

Remark 1 .  It should be noted that the Euler equation (65) does not involve the coefficient $\mu$ . This is explained by the fact that the expression  

$$
u_{x x}u_{y y}\mathrm{~-~}u_{x y}^{2}
$$  

is the divergence of the vector  

$$
(u_{x}u_{y y},\mathrm{~-~}u_{x}u_{x y}),
$$  

and hence has no effect on (65). However, (68) does have a decisive effect on the boundary conditions, via the functions $M(s,t)$ and $P(s,t)$ .  

Remark 2. For a mechanical system to be in equilibrium, its kinetic energy $T$ must vanish and its potential energy $U$ must be independent of time. Under these conditions, the principle of stationary action reduces to the assertion that $\mathbf{\delta}\mathbf{\delta}U=0$ . Thus, the equilibrium position of the system corresponds to a stationary value of $U_{\sun}$ . M oreover, it can be shown that this stationary value must be a minimum if the equilibrium is to be stable and hence physically realizable. In elasticity theory, this principle of minimum potential energy is often replaced by Castig/iano's principle, which states that the equilibrium position of an elastic body corresponds to a minimum of the work of deformation. 16  

# 37. Variat i o n of a Fu nctional Defi n ed o n a Variable Reg ion  

37.1 . Statement o f the problem. In Sec. 3 5, we derived a formula for the variation of the functional  

$$
J[u]=\int\cdot\cdot\cdot\int_{R}F(x_{1},\cdot\cdot\cdot,x_{n},u,u_{x_{1}},\cdot\cdot\cdot,u_{x_{n}})d x_{1}\cdot\cdot\cdot d x_{n},
$$  

allowing only the function $\boldsymbol{u}$ (and hence its derivatives) to vary, while leaving the independent variables (and hence the region of integration $R$ ) unchanged. We now find the variation of the functional (69) in the general case where the independent variables $x_{1},...,x_{n}$ are varied , as well as the function $\boldsymbol{u}$ and its derivatives. For simplicity, we use vector notation, writing $x=(x_{1},\ldots,x_{n})$ , $d x=d x_{1}\cdot\cdot\cdot d x_{n}$ and  

$$
\operatorname{grad}u\equiv\nabla u=(u_{\tau_{1}},\dots,u_{\tau_{n}}).
$$  

With this notation, (69) becomes  

$$
J[u]=\int_{R}F(x,u,\nabla u)d x.
$$  

Now consider the family of transformations17  

$$
\begin{array}{r l}&{x_{i}^{*}=\Phi_{i}(x,u,\nabla u;\mathfrak{c}),}\\ &{u^{*}=\Psi(x,u,\nabla u;\mathfrak{c}),}\end{array}
$$  

depending on a parameter e ,  where the functions $\Phi_{i}(i=1,...,n)$ and $\Psi$ are differentiable with respect to $\varepsilon,$ and the value $\mathfrak{s}=0$ corresponds to the identity transformation :  

$$
\begin{array}{l}{\Phi_{i}(x,u,\nabla u;0)=x_{i},}\\ {\Psi(x,u,\nabla u;0)=u.}\end{array}
$$  

The transformation (7 1 )  carries the surface $\pmb{\sigma}$ , with the equation  

$$
u=u(x)\qquad(x\in R),
$$  

into another surface $\upsigma^{*}$ . I n fact, replacing $\boldsymbol{u},\ \nabla\boldsymbol{u}$ in (7 1 ) by $\boldsymbol{u}(\boldsymbol{x}),\ \Gamma\boldsymbol{u}(\boldsymbol{x}),$ , and eliminating $x$ from the resulting $n+1$ equations, we obtain the equation  

$$
u^{*}=u^{*}(x^{*})\qquad(x^{*}\in R^{*})
$$  

for $\upsigma^{*}$ , where $x^{*}=(x_{1}^{*},\ldots,x_{n}^{*})$ , and $R^{*}$ is a new $\pmb{n}$ -dimensional region. Thus, the transformation (7 1 )  carries the functional $J[u(x)]$ into  

$$
J[u^{*}(x^{*})]=\int_{R^{*}}F(x^{*},u^{*},\nabla^{*}u^{*})d x^{*},
$$  

where  

$$
\nabla^{*}u^{*}=(u_{x_{1}}^{*},\ldots,u_{x_{n}}^{*}).
$$  

Our goal in this section is to calculate the variation of the functional (70) corresponding to the transformation from $x,u(x)$ to $x^{*},u^{*}(x^{*})$ , i . e . , the principal li near part (relative to $\varepsilon$ ) of the difference  

$$
J[u^{*}(x^{*})]-J[u(x)].
$$  

37.2. Calculation of $\updelta x_{i}$ and $\updelta\boldsymbol{u}$ o As in the proof of Noether's theorem for one-dimensional regions (see p. 82), suppose e is a small quantity. Then, by Taylor's theorem, we have  

$$
\begin{array}{r l}&{x_{i}^{*}=\Phi_{1}(x,u,\nabla u;\mathfrak{e})=\Phi_{i}(x,u,\nabla u;0)+\mathfrak{e}\frac{\partial\Phi_{i}(x,u,\nabla u;\mathfrak{e})}{\partial\mathfrak{e}}\bigg\vert_{\mathfrak{e}=0}+o(\mathfrak{e}),}\\ &{u^{*}=\Psi(x,u,\nabla u;\mathfrak{e})=\Psi(x,u,\nabla u;0)+\mathfrak{e}\frac{\partial\Psi(x,u,\nabla u;\mathfrak{e})}{\partial\mathfrak{e}}\bigg\vert_{\mathfrak{e}=0}+o(\mathfrak{e}),}\end{array}
$$  

or using (72),  

$$
\begin{array}{r}{x_{i}^{*}=x_{i}+\varepsilon\varphi_{i}(x,u,\nabla u)+o(\varepsilon),}\\ {u^{*}=u+\varepsilon\psi(x,u,\nabla u)+o(\varepsilon),}\end{array}
$$  

where  

$$
\begin{array}{l}{\displaystyle\varphi_{i}(x,u,\nabla u)=\frac{\partial\Phi_{i}(x,u,\nabla u;\mathfrak{c})}{\partial\mathfrak{c}}\bigg\vert_{\mathfrak{c}=0},}\\ {\displaystyle\psi(x,u,\nabla u)=\frac{\partial\Psi(x,u,\nabla u;\mathfrak{c})}{\partial\mathfrak{c}}\bigg\vert_{\mathfrak{c}=0}.}\end{array}
$$  

For a given surface $\pmb{\sigma}$ ', with equation $\boldsymbol{u}=\boldsymbol{u}(\boldsymbol{x})$ , (74) leads to the increments  

$$
\Delta x_{\mathrm{i}}=x_{\mathrm{i}}^{\ast}-x_{\mathrm{i}}=\varepsilon\varphi_{\mathrm{i}}(x)+o(\varepsilon)
$$  

and  

$$
\Delta u=u^{*}(x^{*})-u(x)=\mathfrak{s}\uppsi(x)+o(\mathfrak{e}),
$$  

where we explicitly indicate the arguments $x$ and $x^{*}$ at which the functions $\pmb{u}$ and ${{\pmb u}^{*}}$ are evaluated, and $\varphi_{i}(x),\psi(x)$ denote the functions (75) with $\boldsymbol{u}$ , $\boldsymbol{\nabla}u$ replaced by $\boldsymbol{u}(\boldsymbol{x}),\boldsymbol{\nabla}\boldsymbol{u}(\boldsymbol{x})$ . Formula (77) gives an expression for the change in $\boldsymbol{u}$ -coordinate as we go from the point $(x,u(x))$ on the surface $\pmb{\sigma}$ to its image $(x^{*},u^{*}(x^{*}))$ under the transformation (74). The variations $\mathfrak{F}x_{\mathfrak{i}}$ and $\updelta\boldsymbol{u}$ corresponding to (74) are defined as the principal linear parts (relative to $\varepsilon$ ) of the increments (76) and (77), i.e.,  

$$
\updelta x_{i}=\upvarepsilon\uprho_{i}(x),\qquad\updelta u=\upvarepsilon\uppsi(x).
$$  

We must also consider the increment  

$$
\overline{{\Delta u}}=u^{*}(x)-u(x),
$$  

i.e., the change in $\pmb{u}$ -coordinate as we go from the point $(x,u(x))$ to the point $(x,u^{*}(x))$ on the surface $\pmb{\sigma}^{\ast}$ with the same $x$ -coordinate, where ${\pmb{\sigma}}^{*}$ is the image of the surface $\pmb{\sigma}$ under the transformation (74). Imitating (77) and (78), we introduce a new function $\bar{\Psi}(x)$ and a corresponding variation $\overline{{\hat{\mathbf{\omega}}}}_{u}$ :  

$$
\begin{array}{l}{\overline{{\Delta u}}=u^{\ast}(x)-u(x)=\mathfrak{E}\bar{\Psi}(x)+o(\mathfrak{e}),}\\ {\overline{{\mathfrak{d}u}}=\mathfrak{e}\bar{\Psi}(x).}\end{array}
$$  

To find the relation between $\boldsymbol{\Psi}$ and $\bar{\psi}$ , or equivalently, between $\updelta\boldsymbol{u}$ and $\overline{{\delta u}}$ , we write  

$$
\begin{array}{l}{{\Delta u=u^{*}(x^{*})-u(x)=[u^{*}(x^{*})-u^{*}(x)]+[u^{*}(x)-u(x)]}}\\ {{\ =\ \displaystyle\sum_{-1}^{n}\frac{\partial u^{*}}{\partial x_{i}}\left(x_{i}^{*}-x_{i}\right)+\overline{{{\widetilde{\delta u}}}}+o(\varepsilon)}}\\ {{\ =\ \displaystyle\sum_{i=1}^{n}\frac{\partial u^{*}}{\partial x_{i}}\widetilde{\otimes}x_{i}+\overline{{{\widetilde{\delta u}}}}+o(\varepsilon).}}\end{array}
$$  

Since ${\partial}u^{*}/d x_{*}$ and $\partial u/\partial{x_{i}}$ differ only by a quantity of order $\varepsilon,$ , (79) becomes  

$$
\Delta u\sim\sum_{i=1}^{n}{\frac{\partial u}{\partial x_{i}}}\delta x_{i}+{\overline{{\delta u}}},
$$  

where the symbol $\sim$ denotes equality except for terms of order higher than 1 relative to &. But $\Delta u\sim\8u$ , since $\updelta\boldsymbol{u}$ is the principal part of $\Delta u$ , and hence  

$$
\updelta{u}=\overline{{\updelta u}}+\sum_{i=1}^{n}u_{x_{i}}\updelta{x_{i}}.
$$  

Moreover, since  

(80) also implies  

$$
\begin{array}{c}{{\displaystyle\delta u=\varepsilon\psi,\overline{{{\delta u}}}=\varepsilon\bar{\psi},\qquad\delta x_{i}=\varepsilon\varphi_{i},}}\\ {{}}\\ {{\psi=\bar{\Psi}+\displaystyle\sum_{i=1}^{n}u_{x_{i}\varphi_{i}}.}}\end{array}
$$  

Example. Let $\pmb{u}$ be a function of a single independent variable $x$ , and let (7 1 ) be the transformation  

$$
\begin{array}{r}{x^{*}=x\cos\mathfrak{e}-u(x)\sin\mathfrak{e}=x-\mathfrak{e}u(x)+o(\mathfrak{e}),}\\ {u^{*}(x^{*})=x\sin\mathfrak{e}+u(x)\cos\mathfrak{e}=\mathfrak{e}x+u(x)+o(\mathfrak{e}),}\end{array}
$$  

i.e., a counterclockwise rotation of the $x u$ -plane about the small angle $\alpha=\varepsilon$ . As shown in Figure 1 0, (82) carries the point $(x,u(x))$ on the curve $\upgamma$ with equation $u=u(x)$ into the point $(x^{*},u^{*}(x^{*}))$  

on its image $\upgamma^{\ast}$ with equation $u^{*}=u^{*}(x^{*})$ . It follows from (82) that  

$$
\updelta x=-\upvarepsilon u(x),\qquad\updelta u=\upvarepsilon x
$$  

and  

$$
\varphi(x)=-u(x),\quad\quad\psi(x)=x.
$$  

In fact, the expressions (83) can be read directly off the figure, as the components of the vector joining the point $(x,u(x))$ to the point $(x^{*},u^{*}(x^{*}))$ . Moreover,  

![](https://cdn-mineru.openxlab.org.cn/extract/c29daec4-3bde-4c07-a565-58de41e65c3b/cca6553ad167dec43a9e417821903d3d8a4e1229e180972fafe284d487468e73.jpg)  
FIGURE 10  

$$
u^{*}(x)=u^{*}[x^{*}+\mathfrak{e}u(x)]+o(\mathfrak{e})=u^{*}(x^{*})+\mathfrak{e}u(x)u^{*\prime}(x^{*})+o(\mathfrak{e}),
$$  

and since $u^{*}{}^{\prime}(x^{*})$ and ${\pmb u}^{\prime}({\pmb x})$ differ only by a quantity of order e, we have  

$$
u^{*}(x)=u^{*}(x^{*})+\mathfrak{s}u(x)u^{\prime}(x)+o(\mathfrak{e}).
$$  

On the other hand, according to the second of the formulas (82),  

$$
u^{*}(x^{*})=\mathfrak{s}x+u(x)+o(\mathfrak{s}).
$$  

It follows that  

$$
\overline{{{\Delta u}}}=u^{*}(x)-u(x)=\mathfrak{e}[x+u^{\prime}(x)u(x)]+o(\mathfrak{e})
$$  

and  

$$
\begin{array}{c}{{\overline{{{\widetilde{\delta u}}}}=\varepsilon[x+u(x)u^{\prime}(x)],}}\\ {{\bar{\Psi}(x)=x+u(x)u^{\prime}(x).}}\end{array}
$$  

Using (83) and (84), we can write (8 5) as  

$$
\begin{array}{c}{{\delta u=\overline{{{\delta u}}}+u^{\prime}\updelta x,}}\\ {{\uppsi=\Bar{\uppsi}+u^{\prime}\upphi,}}\end{array}
$$  

in complete agreement with (80) and (8 1).  

37.3. Calculation of $\updelta u_{x_{i}}$ . We now derive an expression for the quantity  

$$
\Delta u_{x_{i}}=\frac{\partial u^{*}(x^{*})}{\partial x_{i}^{*}}-\frac{\partial u(x)}{\partial x_{i}},
$$  

or more precisely, its principal part $\delta u_{x_{\imath}}$ which will be required later when we calculate the increment (73). First, we note that according to (74), 8  

$$
\frac{{\partial{x_{k}^{*}}}}{{\partial{x_{i}}}}\sim{\updelta_{i k}}+\upvarepsilon\frac{{\partial{\varphi_{k}}}}{{\partial{x_{i}}}},
$$  

where $\updelta_{\imath k}$ is the Kronecker delta, equal to I if $i=k$ and 0 otherwise. It follows that  

$$
\begin{array}{c}{\displaystyle\frac{\partial}{\partial x_{i}}=\sum_{k=1}^{n}\frac{\partial}{\partial x_{k}^{*}}\frac{\partial x_{k}^{*}}{\partial x_{1}}\sim\sum_{k=1}^{n}\frac{\partial}{\partial x_{k}^{*}}\left(\delta_{i k}+\varepsilon\frac{\partial\varphi_{k}}{\partial x_{i}}\right)}\\ {=\displaystyle\frac{\partial}{\partial x_{i}^{*}}+\varepsilon\sum_{k=1}^{n}\frac{\partial\varphi_{k}}{\partial x_{i}}\frac{\partial}{\partial x_{k}^{*}},}\end{array}
$$  

i . e . ,  

$$
\frac{\partial}{\partial{x}_{i}}-\frac{\partial}{\partial{x}_{i}^{*}}\sim\approx\sum_{k=1}^{n}\frac{\partial\varphi_{k}}{\partial{x}_{i}}\frac{\partial}{\partial{x}_{k}^{*}}\cdot
$$  

Next we write  

$$
\begin{array}{l}{\displaystyle\Delta u_{x_{i}}=\frac{\partial u^{*}({\boldsymbol x}^{*})}{\partial x_{i}^{*}}-\frac{\partial u({\boldsymbol x})}{\partial x_{i}}}\\ {=\frac{\partial[u^{*}({\boldsymbol x}^{*})-u({\boldsymbol x}^{*})]}{\partial x_{i}^{*}}+\frac{\partial[u({\boldsymbol x}^{*})-u({\boldsymbol x})]}{\partial x_{i}}+\Big(\frac{\partial}{\partial x_{i}^{*}}-\frac{\partial}{\partial x_{i}}\Big)u({\boldsymbol x}^{*}),}\end{array}
$$  

and analyze each of the three terms in the right-hand side separately. Using (87) and the fact that  

$$
u^{*}(x^{*})-u(x^{*})\sim\mathfrak{s}\bar{\Psi}(x^{*}),
$$  

we have  

$$
\frac{\partial[u^{*}(x^{*})-u(x^{*})]}{\partial x_{i}^{*}}\sim\frac{\partial[u^{*}(x^{*})-u(x^{*})]}{\partial x_{i}}\sim\mathfrak{s}\frac{\partial\bar{\Psi}(x^{*})}{\partial x_{i}}\sim\mathfrak{s}\frac{\partial\bar{\Psi}(x)}{\partial x_{i}}.
$$  

Moreover, it is easily verified that  

$$
\frac{\partial[u(x^{*})-u(x)]}{\partial x_{i}}\sim\frac{\partial}{\partial x_{i}}\sum_{k=1}^{n}\frac{\partial u(x)}{\partial x_{k}}\left(x_{k}^{*}-x_{k}\right)\sim\mathfrak{s}\frac{\partial}{\partial x_{i}}\sum_{k=1}^{n}\frac{\hat{c}u(x)}{\partial x_{k}}\varphi_{k}(x)
$$  

and  

$$
\Big({\cdot{\frac{\hat{c}}{\partial x_{i}^{*}}}-\frac{\partial}{\partial x_{i}}}\Big)u(x^{*})\sim\Big({\frac{\partial}{\partial x_{i}^{*}}-\frac{\partial}{\partial x_{i}}}\Big)u(x)\sim-\mathfrak{e}\sum_{k=1}^{n}{\frac{\partial\varphi_{k}}{\partial x_{i}}\frac{\partial u(x)}{\partial x_{k}^{*}}}\cdotp
$$  

Adding equations (88), (89) and (90), we obtain  

$$
\Delta u_{x_{i}}=\frac{\partial u^{*}(x^{*})}{\partial x_{i}^{*}}-\frac{\partial u(x)}{\partial x_{i}}\sim\mathfrak{e}\Big(\frac{\partial\bar{\Psi}}{\partial x_{i}}+\sum_{k=1}^{n}\frac{\hat{c}^{2}u}{\partial x_{i}\partial x_{k}}\varphi_{k}\Big).
$$  

Finally, recalling that  

$$
\Delta u_{x_{i}}\sim\ensuremath{\mathfrak{F}}_{k_{i}},\qquad\overline{{\mathfrak{F}}}=\mathfrak{E}\bar{\Psi},\qquad\mathfrak{F}x_{k}=\mathfrak{E}\varphi_{k},
$$  

we can write (9 ) as  

$$
\updelta u_{x_{i}}=(\overline{{\delta u}})_{x_{i}}+\sum_{k=1}^{n}u_{x_{i}x_{k}}\updelta x_{k}.
$$  

37.4. Calculation of $\delta J.$ We are now in a position to calculate the varia­ tion of a functional defi ned on a variable domain.  

THEOREM I .  The variation of the functional  

$$
J[u]=\int_{R}F(x,u,\nabla u)d x
$$  

corresponding to the transformation 19  

$$
\begin{array}{r l}&{x_{i}^{*}=\Phi_{i}(x,u,\nabla u;\varepsilon)\sim x_{i}+\varepsilon\varphi_{i}(x,u,\nabla u),}\\ &{u^{*}=\Psi(x,u,\nabla u;\varepsilon)\sim u+\varepsilon\psi(x,u,\nabla u)}\end{array}
$$  

$(i=1,...,n)$ is giL·en by the formula  

$$
\mathbb{\delta}J=\mathbb{\varepsilon}\int_{R}\Bigl(F_{u}-\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}F_{u_{x_{i}}}\Bigr)\mathbb{\bar{\psi}}d x+\mathbb{\varepsilon}\int_{R}\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}\bigl(F_{u_{x_{i}}}\mathbb{\bar{\psi}}+F\varphi_{i}\bigr)d x,
$$  

where  

$$
\bar{\Psi}=\Psi-\sum_{i=1}^{n}{u_{x_{i}}\varphi_{i}}.
$$  

Proof Here, $\otimes J$ means the principal linear part (relative to $\varepsilon$ ) of the increment  

$$
\Delta J=J[u^{*}(x^{*})]-J[u(x)],
$$  

where $u^{*}(x^{*})$ is the image of $u(x)$ under the transformation (94). By definition, (96) equals  

$$
\begin{array}{l}{\displaystyle\Delta J=\int_{R^{*}}F(x^{*},u^{*},\nabla^{*}u^{*})d x^{*}-\int_{R}F(x,u,\nabla u)d x}\\ {\displaystyle\quad=\int_{R}\left[F(x^{*},u^{*},\nabla^{*}u^{*})\frac{\partial(x_{1}^{*},...,x_{n}^{*})}{\partial(x_{1},...,x_{n})}-F(x,u,\nabla u)\right]d x,}\end{array}
$$  

where  

$$
\frac{\partial(x_{1}^{*},...,x_{n}^{*})}{\hat{c}(x_{1},...,x_{n})}
$$  

is the Jacobian of the transformation from the variables $x_{1},...,x_{n}$ to the variables $x_{1}^{*},...,x_{n}^{*}$ . According to (86), this Jacobian is  

$$
\begin{array}{r l}&{\left|1+\varepsilon\frac{\partial\varphi_{1}}{\partial x_{1}}\phantom{\frac{\partial\varphi_{1}}{\partial x_{1}}}\varepsilon\frac{\partial\varphi_{2}}{\partial x_{1}}\phantom{\frac{\partial\varphi_{2}}{\partial x_{1}}}\dots\qquad\varepsilon\frac{\partial\varphi_{n}}{\partial x_{1}}\right|}\\ &{\qquad\varepsilon\frac{\partial\varphi_{1}}{\partial x_{2}}\phantom{\frac{\partial\varphi_{1}}{\partial x_{2}}}1+\varepsilon\frac{\partial\varphi_{2}}{\partial x_{2}}\phantom{\frac{\partial\varphi_{2}}{\partial x_{2}}}\dots\qquad\varepsilon\frac{\partial\varphi_{n}}{\partial x_{2}}}\\ &{\qquad\cdot\ }\\ &{\qquad\varepsilon\frac{\partial\varphi_{1}}{\partial x_{n}}\phantom{\frac{\partial\varphi_{1}}{\partial x_{n}}}\varepsilon\frac{\partial\varphi_{2}}{\partial x_{n}}\phantom{\frac{\partial\varphi_{2}}{\partial x_{n}}}\dots\quad1+\varepsilon\frac{\partial\varphi_{n}}{\partial x_{n}}\ }\\ &{\qquad\sim\left(1+\varepsilon\frac{\partial\varphi_{1}}{\partial x_{1}}\right)\cdot\cdot\cdot\left(1+\varepsilon\frac{\partial\varphi_{n}}{\partial x_{n}}\right)\sim1+\varepsilon\sum_{i=1}^{n}\frac{\partial\varphi_{i}}{\partial x_{i}},}\end{array}
$$  

and hence we can write (97) as  

$$
\Delta J\sim\int_{R}\Big[F(x^{*},u^{*},\nabla^{*}u^{*})\Big(1+\mathfrak{e}\sum_{i=1}^{n}\frac{\partial\varphi_{i}}{\partial x_{*}}\Big)-F(x,u,\nabla u)\Big]d x.
$$  

Using Taylor's theorem to expand the integrand of (98), and retaining only terms of order I relative to $\varepsilon$ , we find that  

$$
\delta J=\int_{R}\bigg[\sum_{i=1}^{n}F_{x_{i}}\delta x_{i}+F_{u}\delta u+\sum_{i=1}^{n}F_{u_{x_{i}}}\delta u_{x_{i}}+\varepsilon F\sum_{i=1}^{n}\frac{\partial\varphi_{i}}{\partial x_{i}}\bigg]d x.
$$  

Then, since $\updelta x_{i}=\upvarepsilon\upvarphi_{i}$ h substitution of (80) and (92) into (99) gives  

$$
\begin{array}{r}{\displaystyle\mathfrak{J}J=\int_{R}\Big[\displaystyle\sum_{i=1}^{n}F_{x_{i}}\S\d\hat{s}x_{i}+F_{u}\overline{{\S u}}+F_{u}\sum_{i=1}^{n}u_{x_{i}}\S\d\hat{s}x_{i}+\sum_{i=1}^{n}F_{u_{z_{i}}}(\overline{{\widetilde{\delta}u}})_{x_{i}}(100\overline{{\o u}})}\\ {+\sum_{i,k=1}^{n}F_{u_{z_{i}}}u_{x_{i}x_{k}}\delta x_{k}+F\sum_{i=1}^{n}(\delta x_{i})_{x_{i}}\Big]\d d x.}\end{array}
$$  

As in the case of a fixed domain $R,$ we try to represent the integrand of ( 1 00) as an expression of the form20  

$$
G(x)\:\overline{{{\delta u}}}\:+\:\mathrm{div}\:(.\cdot\cdot)
$$  

(cf. p. 1 53). This can be achieved by noting that  

$$
\begin{array}{l}{{\displaystyle\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}\left(F\&x_{i}\right)=\sum_{i=1}^{n}F_{x_{i}}\&x_{i}+\sum_{i=1}^{n}F(\&x_{i})_{x_{i}}}}\\ {{\displaystyle\phantom{\sum_{i=1}^{n}\sum_{\ell=1}^{\ell}}+\sum_{i=1}^{n}F_{u}u_{x_{i}}\&x_{i}+\sum_{i,k=1}^{n}F_{u_{x_{i}}}u_{x_{i}x_{k}}\&}}\end{array}
$$  

and  

$$
\sum_{i=1}^{n}F_{u_{x_{i}}}(\overline{{\delta u}})_{x_{i}}=\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}\left(F_{u_{x_{i}}}\overline{{\delta u}}\right)-\sum_{i=1}^{n}\left(\frac{\partial}{\partial x_{i}}F_{u_{x_{i}}}\right)\delta u.
$$  

(The last formula resembles an integration by parts.) Thus, finally, we have  

$$
\delta J=\int_{R}\left(F_{u}-\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}F_{u_{z_{i}}}\right)\overline{{\tilde{\delta u}}}d x+\int_{R}\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}\left(F_{u_{z_{i}}}\overline{{\tilde{\delta u}}}+F\delta x_{i}\right)d x,
$$  

which is the same as formula (95), since $\overline{{\delta u}}=\mathfrak{s}\bar{\Psi}$ , $\updelta x_{k}=\upvarepsilon\upvarphi_{k}$ . This proves the theorem.  

Remark 1. In the special case where the function $\pmb{u}$ and its derivatives are varied, but not the independent variables $x_{i},$ we have  

$$
\varphi_{i}=0,\bar{\Psi}=\Psi-\sum_{i=1}^{n}{u_{x_{i}}\varphi_{i}}=\Psi,
$$  

and (95) becomes  

$$
\delta J=\varepsilon\int_{R}\Big(F_{u}-\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}F_{u_{x_{i}}}\Big)\psi(x)d x+\varepsilon\int_{R}\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}[F_{u_{x_{i}}}\psi(x)]d x,
$$  

which is identical with formula (4) of Sec. 35.  

Remark 2. The formula for the variation of the functionaI $J[u]$ i s ordinarily used in the case where $u=u(x)$ is an extremal surface of $J[u]$ , i . e . , satisfies the Euler equation  

$$
F_{u}-\sum_{i=1}^{n}{\frac{\partial}{\partial x_{i}}}F_{u_{x_{i}}}=0.
$$  

Then (95) reduces to  

$$
\delta J=\varepsilon\int_{R}\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}\left(F_{u_{z_{i}}}\bar{\Psi}+F\varphi_{\mathrm{i}}\right)d x
$$  

in the general case, and to  

$$
\updelta J=\upvarepsilon\int_{R}\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}\left(F_{u_{x_{1}}}\Bar{\Psi}\right)d x
$$  

in the case where the independent variables $x_{i}$ are not varied.  

Remark 3. Consider the functional  

$$
J[u_{1},\varrho...,u_{m}]=\int_{R}F\bigg(x,u_{1},...,u_{m},\frac{\partial u_{1}}{\partial x_{1}},...,\frac{\partial u_{m}}{\partial u_{n}}\bigg)d x,
$$  

involving $m$ unknown functions $u_{1},...,u_{m}$ and their derivatives  

$$
{\frac{\partial u_{j}}{\partial x_{i}}}\qquad(i=1,...,n;j=1,...,m).
$$  

Introducing the vector $\boldsymbol{u}=(u_{1},\ldots..,u_{m})$ and interpreting $\boldsymbol{\nabla}\boldsymbol{u}$ as the tensor with components ( 1 03), we can still write ( 1 02) in the form  

$$
J[u]=\int_{R}F(x,u,\nabla u)d x.
$$  

Then, if (94) is replaced by the transformation  

$$
\begin{array}{r l}&{x_{i}^{*}=\Phi_{i}(x,u,\nabla u;\varepsilon)\sim x_{i}+\varepsilon\varphi_{i}(x,u,\nabla u)\qquad(i=1,...,n),}\\ &{u_{j}^{*}=\Psi_{j}(x,u,\nabla u;\varepsilon)\sim u_{j}+\varepsilon\psi_{j}(x,u,\nabla u)\quad(j=1,...,m),}\end{array}
$$  

the formula (95) generalizes to  

$$
\begin{array}{l}{\displaystyle\mathfrak{d}J=\mathfrak{e}\int_{R}\sum_{j=1}^{m}\left(F_{u_{j}}-\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}\frac{\partial F}{\partial\left(\frac{\partial u_{j}}{\partial x_{i}}\right)}\bar{\Psi}_{j}\right)d x}\\ {\displaystyle+\mathfrak{e}\int_{R}\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}\left(\sum_{j=1}^{m}\frac{\partial F}{\partial\left(\frac{\partial u_{j}}{\partial x_{i}}\right)}\bar{\Psi}_{j}+F_{\bar{\Psi}_{i}}\right)d x,}\end{array}
$$  

where  

$$
\bar{\Psi}_{j}=\Psi_{j}-\sum_{i=1}^{n}\frac{\partial u_{j}}{\partial x_{i}}\varphi_{i}\qquad(j=1,\dots,m).
$$  

Remark 4. Let ( 1 04) be replaced by the more general transformation  

$$
\begin{array}{l l}{{x_{i}^{*}=\Phi_{i}(x,u,\nabla u;\varepsilon)\sim x_{i}+\displaystyle\sum_{k=1}^{r}\varepsilon_{k}\Phi_{i}^{(k)}(x,u,\nabla u)\qquad(i=1,...,n),}}\\ {{u_{j}^{*}=\Psi_{j}(x,u,\nabla u;\varepsilon)\sim u_{j}+\displaystyle\sum_{k=1}^{r}\varepsilon_{k}\Psi_{j}^{(k)}(x,u,\nabla u)\qquad(j=1,...,m),}}\end{array}
$$  

depending on $r$ parameters $\mathfrak{E}_{1},\ldots,\mathfrak{E}_{r}$ where e means the vector $(\mathfrak{e}_{1},...,\mathfrak{e}_{r})$ and the symbol $\sim$ denotes equality except for quantities of order higher than 1 relative to $\mathfrak{E}_{1},\ldots,\mathfrak{E}_{r}$ • Then, formula ( 1 05) generalizes further to  

$$
\begin{array}{r l}&{\displaystyle\delta J=\sum_{k=1}^{r}\mathsf{\bar{\varepsilon}}_{k}\int_{R}\sum_{j=1}^{m}\left(F_{u_{j}}-\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}\frac{\partial F}{\partial\left(\frac{\partial u_{j}}{\partial u_{i}}\right)}\bar{\psi}_{j}^{(k)}\right)d x}\\ &{\qquad+\displaystyle\sum_{k=1}^{r}\mathsf{\bar{\varepsilon}}_{k}\int_{R}\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}\left(\sum_{j=1}^{m}\frac{\partial F}{\partial\left(\frac{\partial u_{j}}{\partial x_{i}}\right)}\bar{\psi}_{j}^{(k)}+F\varphi_{i}^{(k)}\right)d x,}\end{array}
$$  

where  

$$
\bar{\Psi}_{j}^{(k)}=\oint_{j}^{(k)}-\sum_{i=1}^{n}\frac{\partial u_{j}}{\partial x_{i}}\varphi_{i}^{(k)}(k=1,...,r).
$$  

37.5. Noether's theorem. Using form ula (95) for the variation of a functional, we can deduce an important theorem due to Noether, concerning " invariant variational problems." This theorem has already been proved in Sec. 20 for the case of a single independent variable. Suppose we have a functional  

$$
J[u]=\int_{R}F(x,u,\nabla u)d x
$$  

and a transformation  

$$
\begin{array}{l}{{x_{i}^{*}=\Phi_{i}(x,u,\nabla u),}}\\ {{u^{*}=\Psi(x,u,\nabla u)}}\end{array}
$$  

$(i=1,\ldots,n)$ carrying the surface $\upsigma$ with equation $u=u(x)$ into the surface $\upsigma^{*}$ with equation $u^{*}=u^{*}(x^{*})$ , in the way described on p. 1 69.  

DEFINITION.21 The functional ( 1 06) is said to be invariant under the transformation ( 1 07) i ${}^{\cdot}J[\sigma^{*}]=J[\sigma]$ , i. e . , if  

$$
\int_{R^{*}}F(x^{*},u^{*},\nabla^{*}u^{*})d x^{*}=\int_{R}F(x,u,\nabla u)d x.
$$  

Example. The functional  

$$
J[u]=\int\int_{R}\left[\left({\frac{\partial u}{\partial x}}\right)^{2}+\left({\frac{\partial u}{\partial y}}\right)^{2}\right]d x d y
$$  

is invariant under the rotation  

$$
\begin{array}{r l}&{x^{*}=x\cos{\mathfrak{e}}-y\sin{\mathfrak{e}},}\\ &{y^{*}=x\sin{\mathfrak{e}}+y\cos{\mathfrak{e}},}\\ &{u^{*}=u,}\end{array}
$$  

where e is an arbitrary constant. In fact, since the inverse of the trans­ formation ( l 08) is  

$$
\begin{array}{l}{x=x^{*}\cos{\upvarepsilon}+y^{*}\sin{\upvarepsilon},}\\ {y=-x^{*}\sin{\upvarepsilon}+y^{*}\cos{\upvarepsilon},}\\ {u=u^{*},}\end{array}
$$  

it follows that, given a surface $\upsigma$ with equation $u=u(x,y)$ , the " transformed " surface $\upsigma^{*}$ has the equation  

$$
u^{*}=u(x^{*}\cos\mathfrak{c}+y^{*}\sin\mathfrak{c},-x^{*}\sin\mathfrak{c}+y^{*}\cos\mathfrak{c})=u^{*}(x^{*},y^{*}).
$$  

Consequently, we have  

$$
\begin{array}{l}{\displaystyle{J[\sigma^{*}]=\int\int_{R^{*}}\left[\left(\frac{\partial{u^{*}}}{\partial{x^{*}}}\right)^{2}+\left(\frac{\partial{u^{*}}}{\partial{y^{*}}}\right)^{2}\right]d x^{*}d y^{*}}}\\ {\displaystyle{\quad=\int\int_{R^{*}}\left[\left(\frac{\partial{u}}{\partial x}\cos\varepsilon-\frac{\partial{u}}{\partial{y}}\sin\varepsilon\right)^{2}+\left(\frac{\partial{u}}{\partial{x}}\sin\varepsilon+\frac{\partial{u}}{\partial{y}}\cos\varepsilon\right)^{2}\right]d x^{*}d y^{*}}}\\ {\displaystyle{\quad=\int\int_{R}\left[\left(\frac{\partial{u}}{\partial x}\right)^{2}+\left(\frac{\partial{u}}{\partial{y}}\right)^{2}\right]\frac{\partial{(x^{*},y^{*})}}{\partial{(x,y)}}d x d y=\int\int_{R}\left[\left(\frac{\partial{u}}{\partial{x}}\right)^{2}+\left(\frac{\partial{u}}{\partial{y}}\right)^{2}\right]d x d y.}}\end{array}
$$  

THEOREM 2 (Noether). If the functional  

$$
J[u]=\int_{R}F(x,u,\nabla u)d x
$$  

is invariant under the family of transformations  

$$
\begin{array}{r l}&{x_{i}^{*}=\Phi_{i}(x,u,\nabla u;\mathfrak{e})\sim x_{i}+\mathfrak{e}\varphi_{i}(x,u,\nabla u),}\\ &{u^{*}=\Psi(x,u,\nabla u;\mathfrak{e})\sim u+\mathfrak{e}\psi(x,u,\nabla u)}\end{array}
$$  

$(i=1,\ldots,n)$ for an arbitrary region $R$ , then  

$$
\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}\left(F_{u_{x_{i}}}\bar{\psi}+F\varphi_{i}\right)=0
$$  

on each extremal surface of $J[u]$ , where  

$$
\bar{\Psi}=\Psi-\sum_{i=1}^{n}{u_{x_{i}}\varphi_{i}}.
$$  

Proof. According to formula (95),  

$$
\updelta J=\upvarepsilon\int_{R}\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}\left(F_{u_{x_{i}}}\bar{\Psi}+F\varphi_{i}\right)d x,
$$  

if $u=u(x)$ is an extremal surface. Since $J[u]$ is invariant under ( 1 1 0), $\ \pmb{\delta J}=\ 0$ , and since $R$ is arbitrary, this implies ( I l l ), as asserted.  

Remark $\boldsymbol{{I}}$ .  If we drop the requirement that $u=u(x)$ be an extremal surface of $J[u],$ , then, using (95) again, we find that ( I I I ) is replaced by  

$$
\bigg(F_{u}-\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}F_{u_{x_{i}}}\bigg)\bar{\Psi}+\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}(F_{u_{x_{i}}}\bar{\Psi}+F\varphi_{i})=0.
$$  

Remark 2. If there are $m$ unknown functions $u_{1},...,u_{m}$ we introduce the vector $\pmb{u}=(u_{1},\ldots{},u_{m})$ and continue to write ( 1 09), as in Remark 3, p. 1 75. Then invariance of $J[u]$ under the family of transformations  

$$
\begin{array}{l l}{x_{i}^{*}=\Phi_{i}(x,u,\nabla u;\varepsilon)\sim x_{i}+\varepsilon\varphi_{i}(x,u,\nabla u)\quad}&{(i=1,...,n),}\\ {u_{j}^{*}=\Psi_{j}(x,u,\nabla u;\varepsilon)\sim u_{j}+\varepsilon\psi_{j}(x,u,\nabla u)\quad}&{(j=1,...,m)}\end{array}
$$  

implies that  

$$
\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}\left(\sum_{j=1}^{m}\frac{\partial F}{\partial\left(\frac{\partial u_{j}}{\partial x_{i}}\right)}\bar{\Psi}_{j}+F\varphi_{i}\right)=0,
$$  

where  

$$
\bar{\Psi}_{j}=\Psi_{j}-\sum_{i=1}^{n}\frac{\partial u_{j}}{\partial x_{i}}\varphi_{i}.
$$  

When $n=1$ , 1 1 2) reduces to  

$$
\frac{d}{d x}\Bigl(\sum_{j=1}^{m}F_{u_{j}^{\prime}}\bar{\Psi}_{j}+F\varphi\Bigr)=0
$$  

or  

$$
\sum_{j=1}^{m}F_{u_{j}^{\prime}}\Psi_{j}+\biggl(F-\sum_{j=1}^{m}u_{j}^{\prime}F_{u_{j}^{\prime}}\biggr)\varphi=\mathrm{const}
$$  

along each extremal. This is precisely the version of Noether's theorem proved in Sec. 20. In other words, the left-hand side of ( 1 1 3) is a first integral of the system of Euler equations  

$$
F_{u_{j}}-\frac{d}{d x}F_{u_{j}^{\prime}}=0(j=1,...,m).
$$  

Remark 3. Invariance of the functional ( 1 09) under the $r$ -parameter family of transformations (see Remark 4, p. 1 76)  

$$
\begin{array}{l l}{{\displaystyle x_{i}^{*}=\Phi_{i}(x,u,\nabla u;\mathfrak{c})\sim x_{i}+\sum_{k=1}^{r}\mathfrak{E}_{k}\varphi_{i}^{(k)}(x,u,\nabla u)\quad}}&{{(i=1,...,n),}}\\ {{\displaystyle u_{j}^{*}=\Psi_{j}(x,u,\nabla u;\mathfrak{c})\sim u_{j}+\sum_{k=1}^{r}\mathfrak{E}_{k}\Psi_{j}^{(k)}(x,u,\nabla u)\quad}}&{{(j=1,...,m)}}\end{array}
$$  

implies the existence of $r$ linearly independent relations  

$$
\sum_{i=1}^{n}\frac{\partial}{\partial x_{i}}\left(\sum_{j=1}^{m}\frac{\partial F}{\partial\left(\frac{\partial u_{j}}{\partial x_{i}}\right)}\bar{\Psi}_{j}^{(k)}+F\varphi_{i}^{(k)}\right)=0\qquad(k=1,...,r),
$$  

where  

$$
\bar{\Psi}_{j}^{(k)}=\Psi_{j}^{(k)}-\sum_{i=1}^{n}\frac{\partial u_{j}}{\partial x_{i}}\varphi_{i}^{(k)}.
$$  

Remark 4. Suppose the functional $\boldsymbol{J}[\boldsymbol{u}]$ is invariant under a family of transformations depending on $r$ arbitrary functions instead of $r$ arbitrary parameters. Then, according to another theorem of Noether (which will not be proved here), there are $r$ identities connecting the left-hand sides of the Euler equations corresponding to $J[u]$ . For example, consider the simplest variational problem in parametric form, involving a functional  

$$
J[x,y]=\int_{t_{0}}^{t_{1}}\Phi(x,y,\dot{x},\dot{y})d t,
$$  

where $\Phi$ is a positive-homogeneous function of degree 1 in $x(t)$ and $y(t)$ (see Sec. 1 0). Then, as already noted on p. 39, $J[x,y]$ does not change if we introduce a new parameter $\ulcorner$ by setting $t=t(\tau)$ , where $d t/d\tau>0$ , and in fact, the left-hand sides of the Euler equations  

$$
\Phi_{x}-\frac{d}{d t}\Phi_{\dot{x}}=0,\qquad\Phi_{y}-\frac{d}{d t}\Phi_{\dot{y}}=0
$$  

corresponding to ( 1 1 5) are connected by the identity  

$$
\dot{x}\Bigl(\Phi_{x}-\frac{d}{d t}\Phi_{z}\Bigr)+\dot{y}\Bigl(\Phi-\frac{d}{d t}\Phi_{\dot{y}}\Bigr)=0.
$$  

Another interesting example of a family of transformations depending on an arbitrary function, i.e. , the gauge transformations of electrodynamics, will be given in Sec. 39.  

# 38. A p p l i cat ions to Field Theory  

38. 1. The principle of stationary action for fields. In Sec. 36, we discussed the application of the principle of stationary action to vibrating systems with infinitely many degrees of freedom. These systems were characterized by a function $u(x,t)$ or $u(x,y,t)$ giving the transverse displacement of the system from its equilibrium position. More generally, consider a physical system (not necessarily mechanical) characterized by one function  

$$
u(t,x_{1},...,x_{n})
$$  

or by a set of functions  

$$
u_{j}(t,x_{1},...,x_{n})\qquad(j=1,...,m),
$$  

depending on the time $t$ and the space coordinates $x_{1},...,x_{n}.$ . 22 Such a system is called a field [not to be confused with the concept of a field (of directions) treated in Chap. 6], and the functions $\boldsymbol{u}_{j}$ are called the field functions. As usual, we can simplify the notation by interpreting ( 1 1 6) as a vector function $\pmb{u}=(u_{1},\ldots{},u_{m})$ in the case where $m>1$ .  It is also convenient to write  

$$
t=x_{0},\quad x=(x_{0},x_{1},...,x_{n}),\quad d x=d x_{0}d x_{1}\cdot\cdot\cdot d x_{n}.
$$  

Then the field function ( 1 1 6) becomes simply $u(x)$ .  

In the case of the simple vibrating systems studied in Sec. 36, the equations of motion for the system were derived by first calculating the action functional  

$$
\int_{a}^{b}\left(T-U\right)d t,
$$  

where $T$ is the kinetic energy and $U$ the potential energy of the system, and then invoking the principle of stationary action. Similarly, many other physical fields can be derived from a suitably defined action functional. By analogy with the vibrating string and the vibrating membrane, we write the action in the form23  

$$
J[u,\nabla u]=\int_{a}^{b}d x_{0}\int\cdot\cdot\cdot\int_{R}L(u,\nabla u)d x_{1}\cdot\cdot\cdot d x_{n}=\int_{\Omega}{\mathcal{L}}(u,\nabla u)d x,
$$  

where $\nabla$ is the operator  

$$
{\biggl(}{\frac{\partial}{\partial x_{0}}},{\frac{\partial}{\partial x_{1}}},\ldots,{\frac{\partial}{\partial x_{n}}}{\biggr)},
$$  

$R$ is some $\pmb{n}$ -dimensional region, and $\Omega$ is the " cylindrical space-time region " $R\times[a,b],$ , i.e., the Cartesian product of $R$ and the interval $[a,b]$ (see footnote 1 0, p. 1 64) . The functions $L(u,\nabla u)$ and $\mathcal{L}(u,\nabla u)$ are called the Lagrangian and Lagrangian density of the field, respectively. Applying the principle of stationary action to ( 1 1 7), we require that $\ \delta J=0$ . This leads to the Euler equations  

$$
\frac{\partial\mathcal{L}}{\partial u_{j}}-\sum_{i=0}^{3}\frac{\partial}{\partial x_{i}}\frac{\partial\mathcal{L}}{\partial\Big(\frac{\partial u_{j}}{\partial x_{i}}\Big)}=0\qquad(j=1,\dots,m),
$$  

which are the desired field equations.  

Example 1 . For the vibrating string with free e n d s $({\varkappa_{1}}={\varkappa_{2}}=0.$ ), we have $m=n=1$ ,  and  

$$
\mathcal{L}=\textstyle\frac{_1}{^2}(\rho u_{t}^{2}-\tau u_{x}^{2})=\frac{_1}{^2}(\rho u_{x_{0}}^{2}-\tau u_{x_{1}}^{2})
$$  

[cf. formula ( 1 6) ] .  

Example 2. For the vibrating membrane with a free boundary $[{\varkappa(s)=0}]$ we have $m=1,n=2$ , and  

$$
\mathcal{L}=\textstyle\frac{_1}{2}[\rho u_{t}^{2}-\tau(u_{x}^{2}+u_{y}^{2})]=\frac{_1}{2}[\circ u_{x_{0}}^{2}-\tau(u_{x_{1}}^{2}+u_{x_{2}}^{2})]
$$  

[cf. formula (42)].  

Example 3. Consider the Klein-Gordon equation  

$$
(\square-M^{2})u(x)=0,
$$  

describing the scalar field corresponding to uncharged particles of mass $M$ with spin zero (e . g . , $\pi^{0}$ -mesons). Here, 0 denotes the $D^{\prime}$ A lembertian (operator)  

$$
\bigtriangledown=-\frac{{\partial}^{2}}{{\partial}x_{0}^{2}}+\frac{{\partial}^{2}}{{\partial}x_{1}^{2}}+\frac{{\partial}^{2}}{{\partial}x_{2}^{2}}+\frac{{\partial}^{2}}{{\partial}x_{3}^{2}}\cdot
$$  

It is easy to see that ( 1 1 9) is the E u ler equation corresponding to the Lagran­ gian density  

$$
\mathcal{L}=\textstyle{\frac{1}{2}}(u_{x_{0}}^{2}-u_{x_{1}}^{2}-u_{x_{2}}^{2}-u_{x_{3}}^{2}-M^{2}u^{2}).
$$  

38.2. Conservation laws for fields. Noether's theorem (derived in Sec.   
37.5) affords a general method of deriving conserl'ation lall's for fields, i.e.,  

for constructing combinations of field functions, called field invariants, which do not change in time. Thus, suppose the integral  

$$
\int_{\Omega}\mathcal{L}(u,\nabla u)d x
$$  

is invariant under an $r$ -parameter family of transformations24  

$$
\begin{array}{l l}{x_{i}^{*}=\Phi_{i}(x,u,\nabla u;\mathfrak{c})\sim x_{i}+\displaystyle\sum_{k=1}^{r}\mathfrak{s}_{k}\varphi_{i}^{(k)}}&{\quad(i=0,1,2,3),}\\ {u_{j}^{*}=\Psi_{j}(x,u,\nabla u;\mathfrak{c})\sim u_{j}+\displaystyle\sum_{k=1}^{r}\mathfrak{s}_{k}\Psi_{j}^{(k)}}&{\quad(j=1,\dots,m),}\end{array}
$$  

where $\boldsymbol\mathfrak{E}=(\mathfrak{e}_{1},...,\mathfrak{e}_{r})$ . Then, according to Remark 3, p. 1 79, we have $r$ relations of the form  

$$
\Dot{\mathrm{div}}I^{(k)}\equiv\sum_{i=0}^{3}\frac{\partial I_{i}^{(k)}}{\partial x_{i}}-0,
$$  

where  

$$
I_{i}^{(k)}=\sum_{j=1}^{m}\frac{\partial\mathcal{L}}{\partial\bigg(\frac{\partial u_{j}}{\partial x_{i}}\bigg)}\bar{\Psi}_{j}^{(k)}+\mathcal{L}\varphi_{i}^{_{(k)}}(k=1,...,r)
$$  

and  

$$
\bar{\Psi}_{j}^{(k)}=\Psi_{j}^{(k)}-\sum_{i=1}^{n}\frac{\partial u_{j}}{\partial x_{i}}\varphi_{i}^{(k)}.
$$  

These equations have the following interesting consequence : Suppose the cylinder $\Omega=R\times[a,b],$ where $R$ is the three-dimensional sphere defined by  

$$
x_{1}^{2}+x_{2}^{2}+x_{3}^{2}\leqslant c^{2}.
$$  

Let $\Gamma$ be the boundary of $\Omega$ , and let $\blacktriangledown\blacktriangledown\blacktriangledown\blacktriangledown\blacktriangledown\$ be the unit outward normal to $\Gamma$ . Then, integrating each of the relations ( 1 22) over $\Gamma$ and using Green's theorem [formula (5) of Sec. 35], we obtain  

$$
\int_{\Omega}\mathrm{div}I^{(k)}d x=\int_{\Gamma}\left(I^{(k)},\mathrm{v}\right)d\sigma=0\qquad(k=1,...,r).
$$  

The surface integral in ( 1 23) is the sum of an integral over the lateral surface of the cylinder $\Gamma$ and an integral over the two end surfaces cut off by the planes $x_{0}=a$ , $x_{0}=b$ . As $c\to\infty$ ,  the integral over the lateral surfaces goes to zero (by the usual argument requiring that the field fall off at infinity " sufficiently rapidly "), and we are left with the integral over the end surfaces.  

On these surfaces, the scalar product $(I^{(k)},\mathsf{v})$ reduces to $I_{0}^{(k)}$ , where the plus sign refers to the " top " surface and the minus sign to the " bottom " surface. Therefore, taking the limit as $c\to\infty$ in ( 1 23), we find that  

$$
\begin{array}{r l}{\lefteqn{\int I_{0}^{(k)}\left(a,x_{1},x_{2},x_{3}\right)d x_{1}d x_{2}d x_{3}}\ ~}&{}\\ {=\int I_{0}^{(k)}\left(b,x_{1},x_{2},x_{3}\right)d x_{1}d x_{2}d x_{3}~}&{(k=1,...,r),}\end{array}
$$  

where $I_{0}^{(k)}$ denotes the $\scriptstyle x_{0}$ -component of the vector ${\cal I}^{(k)}$ , and the integrations extend over all of three-dimensional space, as will always be assumed if no region of integration is indicated. Since $\pmb{a}$ and $\pmb{b}$ are arbitrary, it follows from ( 1 24) that the quantities  

$$
\begin{array}{r l}{\lefteqn{\int I_{0}^{\scriptscriptstyle(k)}d x_{1}d x_{2}d x_{3}}\quad}&{{}}\\ {=\Bigg]\left(\sum_{j=1}^{m}\frac{\partial\mathcal{L}}{\partial\left(\frac{\partial u_{j}}{\partial x_{0}}\right)}\bar{\psi}_{j}^{(k)}+\mathcal{L}_{\mathcal{C}_{0}^{(k)}}\right)d x_{1}d x_{2}d x_{3}}&{{}\quad(k=1,...,r)}\end{array}
$$  

are independent of time. The $r$ quantities ( 1 25) are the required field invari­ ants, whose existence is implied by the invariance of the action functional under the $r$ -parameter family of transformations ( 1 2 1 ) .  

Remark. Of course, all the functions in ( 1 25) are supposed to be evaluated on an extremal surface of the action functional, corresponding to a solution $u(x)$ of the field equations ( 1 1 8) .  

38.3. Conservation of energy and momentum. The action functional of any physical field is invariant u nder parallel displacements, i.e., under the family of transformations  

$$
\begin{array}{l l}{{x_{i}^{*}=x_{i}+\varepsilon_{i}\quad}}&{{(i=0,1,2,3),}}\\ {{u_{j}^{*}=u_{j}\quad}}&{{(j=1,...,m),}}\end{array}
$$  

where the $\Xi_{\boldsymbol{i}}$ are arbitrary. In this case, we have  

$$
\updelta x_{i}=\upepsilon_{i},\qquad\updelta u_{j}=0,
$$  

which implies  

$$
\varphi_{i}^{(k)}=\S_{i k},\bar{\Psi}_{j}^{(k)}=-\sum_{i=1}^{n}\frac{\partial u_{j}}{\partial x_{i}}\S_{i k}=-\frac{\partial u_{j}}{\partial x_{k}},
$$  

where $\S_{i k}$ is the Kronecker delta. According to ( 1 25), the corresponding field invariants are  

$$
\int\Biggl(\sum_{j=1}^{m}\frac{\partial\mathcal{L}}{\partial\Bigl(\frac{\partial u_{j}}{\partial x_{0}}\Bigr)}\frac{\partial u_{j}}{\partial x_{k}}-\mathcal{L}\mathfrak{d}_{0k}\Biggr)d x_{1}d x_{2}d x_{3}\qquad(k=0,1,2,3).
$$  

It is convenient to introduce the second-rank tensor  

$$
T_{i k}=\sum_{j=1}^{m}\frac{\partial\mathcal{L}}{\partial\Big(\frac{\partial u_{j}}{\partial x_{i}}\Big)}\frac{\partial u_{j}}{\partial x_{k}}-\mathcal{L}\updelta_{i k},
$$  

called the energy-momentum tensor. In terms of $T_{i k}$ ' the field invariants are  

$$
P_{k}=\int T_{0k}d x_{1}d x_{2}d x_{3}(k=0,1,2,3).
$$  

The vector  

$$
P=(P_{0},P_{1},P_{2},P_{3})
$$  

is called the energy-momentum vector, and in fact, it can be shown that $P_{0}$ is the energy and $P_{1},P_{2},P_{3}$ the momentum components of the field. Thus, since $P$ is a field invariant, we have j ust proved that the energy and momen­ tum of the field are conserved.  

38.4. Conservation of angular momentum. According to the special theory of relativity, the action functional of any physical field is invariant under orthochronous Lorentz transformations, i.e., under transformations of four-dimensional space-time which leave the quadratic form  

$$
-x_{0}^{2}+x_{1}^{2}+x_{2}^{2}+x_{3}^{2}
$$  

invariant and preserve the time direction. 25 For simplicity, we consider the case where $u(x)$ is a scalar field $(m=1)$ . Then the action functional must be invariant under the family of (infinitesimal) transformations  

$$
\begin{array}{l}{{\displaystyle x_{i}^{*}\sim x_{i}+\sum_{l\neq i}g_{l l}\varepsilon_{i l}x_{l},\hfill}}\\ {{\displaystyle u^{*}=u,}}\end{array}
$$  

where  

$$
g_{00}=-1,\qquadg_{11}=g_{22}=g_{33}=1
$$  

and  

$$
\mathsf{\pmb{\upvarepsilon}}_{k l}=-\mathsf{\pmb{\upvarepsilon}}_{l k}\qquad(k\neq l)
$$  

are the parameters determining the given transformation. 26 Since the twelve parameters $\mathfrak{s}_{k l}$ $(k\neq l)$ are connected by the relations ( 1 29), only six of them are independent, and we choose the independent parameters to be those for which $k<l.$  

Corresponding to the transformations ( 1 28), we have  

$$
\begin{array}{r l}{\lefteqn{\begin{array}{l}{\displaystyle\8x_{i}=\sum_{l\neq i}g_{l l}\varepsilon_{i l}x_{l}=\sum_{l\neq k}\sum_{k=0}^{3}g_{l l}\varepsilon_{k l}\delta_{i k}x_{l}}\end{array}}}\\ &{\quad=\sum_{l<k}\sum_{k=0}^{3}\xi_{l l}\varepsilon_{k l}\delta_{i k}x_{l}+\sum_{k>l}\sum_{k=0}^{3}g_{l l}\varepsilon_{k l}\delta_{i k}x_{l}}\\ &{\quad=\sum_{l<k}\sum_{k=0}^{3}\varepsilon_{k l}\bigl(g_{l l}\delta_{i k}x_{l}-g_{k k}\delta_{i l}x_{k}\bigr),}\end{array}}\end{array}
$$  

where $\updelta_{i k}$ i s the Kronecker delta, and  

$$
{\overline{{\delta u}}}=-\sum_{i=0}^{3}{\frac{\partial u}{\partial x_{i}}}\ \delta x_{i}.
$$  

It follows that  

$$
\begin{array}{l}{\displaystyle\varphi_{i}^{(k,l)}={{g}_{l l}}\ {{\delta}_{i k}}{{x}_{l}}\ -\ {{g}_{k k}}\ {{\delta}_{i l}}{{x}_{k}},}\\ {\displaystyle\bar{\Psi}^{(k,l)}=\sum_{i=0}^{3}\frac{\partial u}{\partial{{x}_{i}}}\left({{g}_{k k}}\ {{\delta}_{i l}}{{x}_{k}}-{{g}_{l l}}\ {{\delta}_{i k}}{{x}_{l}}\right)=\frac{\partial u}{\partial{{x}_{l}}}{{g}_{k k}}{{x}_{k}}-\frac{\partial u}{\partial{{x}_{k}}}{{g}_{l l}}{{x}_{l}},}\end{array}
$$  

where the pair of indices $k$ , I plays the same role as the single index $k$ in ( 1 2 1 ) and ranges over the six combinations  

$$
0,1;0,2;0,3;1,2;1,3;2,3.
$$  

According t o ( 1 25), the corresponding field invariants are  

$$
\begin{array}{r l r}{\lefteqn{\int_{\O}\left(\frac{\partial\mathcal{L}}{\partial{\Big(\frac{\partial u}{\partial x_{i}}\Big)}}\left[\frac{\partial u}{\partial x_{l}}g_{k k}x_{k}-\frac{\partial u}{\partial x_{k}}g_{l l}x_{l}\right]\right.}}\\ &{}&\\ &{}&{+\left.\mathcal{L}[g_{l l}\vartheta_{i k}x_{l}-g_{k k}\vartheta_{i l}x_{k}]\right)d x_{1}d x_{2}d x_{3}(k<l).}\end{array}
$$  

It is convenient to introduce the third-rank tensor  

$$
\begin{array}{l}{{M_{i k}=\displaystyle\frac{\partial\mathcal{L}}{\partial\left(\frac{\partial u}{\partial x_{i}}\right)}\left[\frac{\partial u}{\partial x_{l}}g_{k k}x_{k}-\frac{\partial u}{\partial x_{k}}g_{l l}x_{l}\right]+\mathcal{L}[g_{l l}\mathbb{\delta}_{i k}x_{l}-g_{k k}\mathbb{\delta}_{1l}x_{k}]\quad(k<l)}}\\ {{M_{i k l}=\displaystyle-\ M_{i l k}\qquad(k>l),\qquad(13)}}\end{array}
$$  

called the angular momentum tensor. By definition, $M_{i k l}$ is antisymmetric in the indices $k$ and $l.$ . Using the expression ( 1 27) for the energy-momentum tensor (specialized to the case of scalar fields), we can write ( 1 3 1 ) as  

$$
M_{i k l}=g_{k k}x_{k}T_{i l}-g_{l l}x_{l}T_{i k}.
$$  

In terms of $M_{i k l}$ > the field invariants are  

$$
\int M_{0k l}d x_{1}d x_{2}d x_{3}\qquad(k<l),
$$  

a fact summarized by saying that the angular momentum of the field is conserred.  

Example. Using the quantities ${{g}_{\mathrm{*i}}}$ , we can write the Lagrangian density ( 1 20) corresponding to the Klein-Gordon equation in the form  

$$
\mathcal{L}=-\frac{1}{2}\sum_{i=0}^{3}g_{i i}\bigg(\frac{\partial u}{\partial x_{i}}\bigg)^{2}-\frac{1}{2}M^{2}u^{2}.
$$  

This leads to the energy-momentum tensor  

$$
T_{i k}=-g_{i i}\frac{\partial u}{\partial x_{i}}\frac{\partial u}{\partial x_{k}}-\mathcal{L}\updelta_{i k}
$$  

and the angular momentum tensor  

$$
M_{i k l}=g_{i l}\frac{\partial u}{\partial x_{i}}\left(g_{l l}x_{l}\frac{\partial u}{\partial x_{k}}-g_{k k}x_{k}\frac{\partial u}{\partial x_{l}}\right)+\mathcal{L}(g_{l l}x_{l}\S_{i k}-g_{k k}x_{k}\S_{i l}).
$$  

The energy density corresponding to ( 1 32) is  

$$
T_{00}=\frac{1}{2}\sum_{i=0}^{3}\left(\frac{\partial u}{\partial x_{i}}\right)^{2}+\frac{1}{2}M^{2}u^{2},
$$  

while the momentum density has the components  

$$
T_{0k}={\frac{\partial u}{\partial x_{0}}}{\frac{\partial u}{\partial x_{k}}}\quad\quad(k=1,2,3).
$$  

38.5. The electromagnetic field. To illustrate the methods developed above, we now derive the equations of the electromagnetic field from a suitable Lagrangian density. The electromagnetic field is described by two three-dimensional vectors, the electric field vector $\boldsymbol{E}=(E_{1},E_{2},E_{3})$ and the magnetic field vector $H=(H_{1},H_{2},H_{3})$ ' In the absence of electric charges, $E$ and $H$ are related by the familiar Maxwell equations  

$$
\begin{array}{r l}&{\operatorname{curl}\ E=-\frac{\partial H}{\partial x_{0}},\qquad\operatorname{curl}H=\frac{\partial E}{\partial x_{0}},}\\ &{\operatorname{div}H=0,\qquad\operatorname{div}E=0,}\end{array}
$$  

where  

$$
\begin{array}{r l}&{\mathrm{div}\ E=\frac{\partial E_{1}}{\partial x_{1}}+\frac{\partial E_{2}}{\partial x_{2}}+\frac{\partial E_{3}}{\partial x_{3}},}\\ &{\mathrm{curl}\ E=\Big(\frac{\partial E_{3}}{\partial x_{2}}-\frac{\partial E_{2}}{\partial x_{3}},\frac{\partial E_{1}}{\partial x_{3}}-\frac{\partial E_{3}}{\partial x_{1}},\frac{\partial E_{2}}{\partial x_{1}}-\frac{\partial E_{1}}{\partial x_{2}}\Big),}\end{array}
$$  

and similarly for div $H$ , curl $H_{\cdot}$ . It is convenient to express $E$ and $H$ in terms of a four-dimensional electromagneticpotential $\{A_{j}\}=(A_{0},A_{1},A_{2},A_{3}),^{27}$ by setting  

$$
E={\mathrm{grad~}}A_{0}-{\frac{\partial A}{\partial x_{0}}},\qquadH={\mathrm{curl~}}A,
$$  

where  

$$
\boldsymbol{A}=(A_{1},A_{2},A_{3})
$$  

and  

$$
\operatorname{grad}A_{0}=\Big(\frac{\partial A_{0}}{\partial x_{1}},\frac{\partial A_{0}}{\partial x_{2}},\frac{\partial A_{0}}{\partial x_{3}}\Big)\cdot
$$  

The potential $\left\{A_{j}\right\}$ is not uniquely determined by the vectors $E$ and $H.$ . In fact, $E$ and $H$ do not change if we make a gauge transformation, i.e., if we replace $\left\{A_{j}\right\}$ by a new potential $\left\{A_{j}^{\prime}\right\}$ with components  

$$
A_{j}^{\prime}(x)=A_{j}(x)+{\frac{\partial f(x)}{\partial x_{j}}}\qquad(j=0,1,2,3),
$$  

where $\boldsymbol{x}=(x_{0},x_{1},x_{2},x_{3})$ and $f(x)$ is an arbitrary function . T o avoid this lack of uniqueness, an extra condition can be imposed on $\left\{A_{j}\right\}$ . The condition usually chosen is  

$$
-\frac{\partial A_{0}}{\partial x_{0}}+\mathrm{div}A=\sum_{j=0}^{3}g_{j j}\frac{\partial A_{j}}{\partial x_{j}}=0,
$$  

and is known as the Lorentz condition.  

Next, we prove that the Maxwell equations ( 1 33) reduce to a single equa­ tion determining the electromagnetic potential $\left\{A_{j}\right\}$ . First, we introduce the antisymmetric tensor $H_{i j},$ whose matrix  

$$
\begin{array}{r}{\left\Vert\begin{array}{c c c c}{0}&{-E_{1}}&{-E_{2}}&{-E_{3}}\\ {E_{1}}&{0}&{H_{3}}&{-H_{2}}\\ {E_{2}}&{-H_{3}}&{0}&{H_{1}}\\ {E_{3}}&{H_{2}}&{-H_{1}}&{0}\end{array}\right\Vert}\end{array}
$$  

is formed from the components of $E$ and $H$ . It is easily verified that the formula relating $H_{i j}$ to the potential $\{A,\}$ is  

$$
H_{i j}=\frac{\partial A_{i}}{\partial x_{i}}-\frac{\partial A_{i}}{\partial x_{j}}.
$$  

In terms of the tensor $H_{i j}$ , we can write the Maxwell equations ( 1 33) in the form  

$$
\sum_{i=0}^{3}g_{i i}{\frac{\partial H_{j}}{\partial x_{i}}}=0\qquad(j=0,1,2,3),
$$  

$$
\frac{\partial{H_{i j}}}{\partial{x_{k}}}+\frac{\partial{H_{k i}}}{\partial{x_{j}}}+\frac{\partial{H_{j k}}}{\partial{x_{i}}}=0,
$$  

where in ( 1 38),  

$$
\begin{array}{r}{i,j,k=\left\{\begin{array}{l l}{0,1,2,}\\ {1,2,3,}\\ {2,3,0,}\\ {3,0,1.}\end{array}\right.}\end{array}
$$  

Substituting ( 1 36) into ( 1 37) and ( 1 38), and using the Lorentz cond ition ( 1 35), we find that ( 1 38) is an identity, while ( 1 3 7) reduces to  

$$
\begin{array}{r}{\bigsqcup A_{j}=0(j=0,1,2,3),}\end{array}
$$  

where $\sqsubseteq$ is the D' Alembertian  

$$
\bigtriangledown=-\frac{{\partial}^{2}}{{\partial}x_{0}^{2}}+\frac{{\partial}^{2}}{{\partial}x_{1}^{2}}+\frac{{\partial}^{2}}{{\partial}x_{2}^{2}}+\frac{{\partial}^{2}}{{\partial}x_{3}^{2}}\mathrm{.}
$$  

Finally, we show that ( 1 39) is a consequence of the principle of stationary action,28 if we choose the Lagrangian density of the electromagnetic field to be  

$$
\mathcal{L}=\frac{1}{8\pi}(E^{2}-H^{2}).
$$  

Replacing $E$ and $H$ in ( 1 40) by their expressions ( 1 34) in term s of the electro­ magnetic potential $\{A_{j}\}$ , we obtain  

$$
\mathcal{L}=\frac{1}{8\pi}\left[\left(\mathrm{grad}~A_{0}-\frac{\partial A}{\partial x_{0}}\right)^{2}-(\mathrm{curl}~A)^{2}\right].
$$  

We shall only verify that the Euler equations  

$$
{\frac{\partial{\mathcal{L}}}{\partial A_{j}}}-\sum_{i=0}^{3}{\frac{\partial{\mathcal{L}}}{\partial\left({\frac{\partial A_{j}}{\partial x_{i}}}\right)}}=0\qquad(j=0,1,2,3)
$$  

corresponding to ( 1 4 1 ) can be reduced to the form ( 1 39) for the component $\scriptstyle A_{0}$ , since the calculations for $A_{1},A_{2},A_{3}$ are completely analogous. It follows fro m ( 1 4 1 ) that  

$$
\begin{array}{r l}&{\quad\frac{\partial\mathcal{L}}{\partial A_{0}}=\frac{\partial\mathcal{L}}{\partial u}=0,}\\ &{\quad\frac{\partial\mathcal{L}}{\partial\left(\frac{\partial A_{0}}{\partial x_{0}}\right)}=\frac{1}{4\pi}\left(\frac{\partial A_{0}}{\partial x_{1}}-\frac{\partial A_{1}}{\partial x_{0}}\right),}\\ &{\quad\frac{\partial\tilde{\mathcal{L}}}{\partial\left(\frac{\partial A_{0}}{\partial x_{1}}\right)}=\frac{1}{4\pi}\left(\frac{\partial A_{0}}{\partial x_{1}}-\frac{\partial A_{2}}{\partial x_{0}}\right),}\\ &{\quad\frac{\partial\tilde{\mathcal{L}}}{\partial\left(\frac{\partial A_{0}}{\partial x_{2}}\right)}=\frac{1}{4\pi}\left(\frac{\partial A_{0}}{\partial x_{2}}-\frac{\partial A_{2}}{\partial x_{0}}\right),}\\ &{\quad\frac{\partial\mathcal{L}}{\partial\left(\frac{\partial\mathcal{L}}{\partial x_{3}}\right)}=\frac{1}{4\pi}\left(\frac{\partial A_{0}}{\partial x_{3}}-\frac{\partial A_{3}}{\partial A_{0}}\right).}\end{array}
$$  

Thus, for $j=0$ ,(142) becomes  

$$
\begin{array}{r l}{\lefteqn{\frac{\partial\mathcal{L}}{\partial A_{0}}-\sum_{i=0}^{3}\frac{\partial\mathcal{L}}{\partial\left(\frac{\partial A_{0}}{\partial x_{i}}\right)}}\quad}&{}\\ &{=\ -\ \frac{1}{4\pi}\left[\frac{\partial^{2}A_{0}}{\partial x_{1}^{2}}+\frac{\partial^{2}A_{0}}{\partial x_{2}^{2}}+\frac{\partial^{2}A_{0}}{\partial x_{3}^{2}}-\frac{\hat{\mathcal{O}}}{\partial x_{0}}\Big(\frac{\partial A_{1}}{\partial x_{1}}+\frac{\partial A_{2}}{\partial x_{2}}+\frac{\partial A_{3}}{\partial x_{3}}\Big)\right]=0.}\end{array}
$$  

According to the Lorentz condition ( 1 35),  

$$
\frac{\partial A_{1}}{\partial x_{1}}+\frac{\partial A_{2}}{\partial x_{2}}+\frac{\partial A_{3}}{\partial x_{3}}=\frac{\partial A_{0}}{\partial x_{0}},
$$  

and hence ( 1 43) reduces to  

$$
-\frac{\partial^{2}{A}_{0}}{\partial x_{0}^{2}}+\frac{\partial^{2}{A}_{0}}{\partial x_{1}^{2}}+\frac{\partial^{2}{A}_{0}}{\partial x_{2}^{2}}+\frac{\partial^{2}{A}_{0}}{\partial x_{3}^{2}}=\bigtriangledown A_{0}=0,
$$  

which is just ( 1 39), for $j=0$ .  

Remark $^{I}$ .  In deriving ( 1 39) from ( 1 4 1 ), we made use of the Lorentz condition ( 1 35). Instead, we could have introduced an additional term into the Lagrangian density by writing  

$$
\mathcal{L}=\frac{1}{8\pi}\Bigg\{\bigg(\mathrm{grad}~A_{0}-\frac{\partial A}{\partial x_{0}}\bigg)^{2}-(\mathrm{curl}~A)^{2}-\bigg(\mathrm{div}~A-\frac{\partial A_{0}}{\partial x_{0}}\bigg)^{2}\Bigg\},
$$  

which reduces to ( 1 4 1 ) if the Lorentz condition is satisfied. The Euler equations corresponding to ( 1 44) reduce to ( 1 39) for arbitrary $\left\{A_{j}\right\}$ .  

Remark 2. The Lagrangian density of the electromagnetic field, and hence its action functional, is invariant under parallel displacements, Lorentz transformations and gauge transformations. According to Sec. 38.3, the invariance under parallel displacements implies conservation of energy and momentum of the field, while, according to Sec. 38.4, the invariance under Lorentz transformations implies conservation of angular m omentum of the field. Moreover, according to Remark 4, p. 1 79, the invariance under gauge transformations (which depend on one arbitrary function) implies the exis­ tence of a relation between the left-hand sides of the corresponding Euler equations ( 1 39). Therefore, these equations do not uniquely determine the electromagnetic potential $\left\{A_{j}\right\}$ . In fact, to determ ine $\left\{A_{j}\right\}$ uniquely, we need an extra eq uation, which is usually chosen to be the Lorentz condition ( 1 35). 29  

# PROBLEMS  

1. Find the Euler equation of the functional  

$$
J[u]=\int\cdot\cdot\cdot\int_{R}\sum_{i=1}^{n}u_{x_{i}}^{2}d x_{1}\dots d x_{n}.
$$  

2. Find the Euler equation of the functional  

$$
J[u]=\int\int\int_{R}\sqrt{1+u_{\tau}^{2}+u_{y}^{2}+u_{z}^{2}}d x d y d z.
$$  

3. Write the appropriate generalization of the Euler equation for the functional  

$$
J[u]=\int\int_{R}F(x,y,u,u_{x},u_{y},u_{z x},u_{x y},u_{y y})d x d y.
$$  

4. Starting from Green's theorem  

$$
\int\int_{R}\left({\frac{\partial Q}{\partial x}}-{\frac{\partial P}{\partial y}}\right)d x d y=\int_{\Gamma}\left(P d x+Q d y\right),
$$  

prove that  

$$
\begin{array}{r l}&{\displaystyle\int\displaystyle\int_{R}\varphi\frac{\partial^{2}\psi}{\partial x^{2}}d x d y=\displaystyle\int\int_{R}\Psi\frac{\partial^{2}\varphi}{\partial x^{2}}d x d y+\displaystyle\int_{\Gamma}\left(\varphi\frac{\partial\psi}{\partial x}-\mathrm{\LARGE\Psi}\frac{\partial\displaystyle\varphi}{\partial x}\right)d y,}\\ &{\displaystyle\int\displaystyle\int_{R}\varphi\frac{\partial^{2}\psi}{\partial y^{2}}d x d y=\displaystyle\int\int_{R}\Psi\frac{\partial^{2}\varphi}{\partial y^{2}}d x d y-\displaystyle\int_{\Gamma}\left(\varphi\frac{\partial\psi}{\partial y}-\mathrm{\LARGE\Psi}\frac{\partial\displaystyle\varphi}{\partial y}\right)d x,}\\ &{\displaystyle\int\displaystyle\int_{R}\varphi\frac{\partial^{2}\psi}{\partial x\partial y}d x d y=\displaystyle\int\int_{R}\Psi\frac{\partial^{2}\displaystyle\varphi}{\partial x\partial y}d x d y-\displaystyle\frac{1}{2}\int_{\Gamma}\left(\varphi\frac{\partial\Psi}{\partial x}-\mathrm{\LARGE\displaystyle\Psi}\frac{\partial\displaystyle\varphi}{\partial x}\right)d x}\\ &{\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad+\displaystyle\frac{1}{2}\int_{\Gamma}\left(\varphi\frac{\partial\Psi}{\partial y}-\mathrm{\LARGE\displaystyle\Psi}\frac{\partial\displaystyle\varphi}{\partial y}\right)d y.}\end{array}
$$  

5. Let $J[u]$ be the functional  

$$
\frac{1}{2}\int_{t_{0}}^{t_{1}}\int\int_{R}{[-(u_{x x}+u_{y y})^{2}+2(1-\mu)(u_{x x}u_{y y}-u_{x y}^{2})]d x d y d t}.
$$  

Using the result of the preceding problem, prove that if we go from $\pmb{u}$ to $u+\varepsilon\psi$ jl , then  

$$
\delta{\cal J}=\varepsilon\int_{t_{0}}^{t_{1}}\int\int_{R}\left(-\nabla^{4}u\right)\psi d x d y d t+\varepsilon\int_{t_{0}}^{t_{1}}\int_{\Gamma}\left[P(u)\psi+\left.M(u)\frac{\partial\psi}{\partial u}\right]d s d t,
$$  

where $\pmb{M}(\pmb{u})$ and $P(u)$ are given by formulas (6 1 ) and (62).  

Hint. Express ${\partial\Psi}/{\partial x},\ {\partial\Psi}/{\partial y}$ in terms of ${\partial\Psi}/{\partial n},\ \partial\Psi/\partial s$ , and use integration by parts to get rid of ${\partial\Phi}/{\partial s}$ .  

6. Show that when $\pmb{n}=1$ ,  formula ( 1 05) of Sec. 37.4 reduces to formula (7 ) of Sec. 1 3 .  

7. Given the functional  

$$
J[\sigma]=\int\int_{R}\frac{\partial u}{\partial x}d x d y,
$$  

compute ${\cal J}[\sigma^{*}]$ if $\pmb{\sigma}^{\star}$ is obtained from $\pmb{\sigma}$ by the transformation ( l 08).  

8. Derive the Euler equations corresponding to the Lagrangian density  

$$
\mathcal{L}=\sum_{i=0}^{3}\varepsilon_{i}\left(\frac{\partial u}{\partial x_{i}}-e A_{i}\right)^{2}+M^{2}u^{2}+\sum_{i=0}^{3}\sum_{j=0}^{3}\varepsilon_{i}\varepsilon_{j}\left(\frac{\partial A_{i}}{\partial x_{j}}\right)^{2}+M\sum_{i=0}^{3}\varepsilon_{i}A_{i}^{2},
$$  

where the field variables are $u,\ A_{0},\ A_{1},\ A_{2},\ A_{3},$ and the factor $\Xi_{i}$ equals if $i=0$ and $^{-1}$ if $i=1,2,3$ .  

9. Show that the Lagrangian density $\mathcal{L}$ of the preceding problem is Lorentz­ invariant if $\pmb{u}$ transforms like a scalar and if $A_{0},A_{1},A_{2},A_{3}$ transform like the components of a vector under Lorentz transformations. Use this fact to derive various conservation laws for the field described by $\mathcal{L}$ .  

8  

DIRE CT METHODS IN THE CAL CULUS OF V ARIATIONS  

So far, the basic approach used t o solve a given variational problem (and indeed, to prove the existence of a solution) has been to reduce the prob­ lem to one involving a differential equation (or perhaps a system of differen­ tial equations). However, this approach is not always effective, and is greatly complicated by the fact that what is needed to solve a given varia­ tional problem is not a solution of the corresponding differential equation in a small neighborhood of some point (as is usually the case in the theory of differential equations), but rather a solution in some fixed region $R$ , which satisfies prescribed boundary conditions on the boundary of $R$ . The difficulties inherent in this approach (especially when several independent variables are involved, so that the differential equation is a partial difefrential equation) have led to a search for variational methods of a different kind, known as direct methods, which do not entail the reduction of variational problems to problems involving differential equations.  

Once they have been developed , direct-variational methods can be used to solve differential equations, and this technique, the inverse of the one we have used u ntil now, plays an important role in the modern theory of the subject. The basic idea is the following : Suppose it can be shown that a given differential equation is the Euler equation of some functional, and suppose it has been proved somehow that this functional has an extremum for a sufficiently smooth ad missible function. Then, this very fact proves that the differential equation has a solution satisfying the boundary con­ ditions corresponding to the given variational problem. Moreover, as we shall show below (Sec. 4 1 ), variational methods can be used not only to prove the existence of a solution of the original differential equation, but also to calculate a solution to any desired accuracy.  

# 39. M i n i m izi ng Seq u e n ces  

There are many different techniques lumped together under the heading of " direct methods." However, the direct methods considered here are all based on the same general idea, which goes as follows :  

Consider the problem of finding the minimum of a functional $J[y]$ defined on a space $\mathcal{M}$ of admissible functions $y$ . For the problem to make sense, it must be assumed that there are functions in $\mathcal{M}$ for which $J[y]<+\infty$ , and moreover thatl  

$$
\operatorname*{inf}_{y}J[y]=\mu>-\infty,
$$  

where the greatest lower bound is taken over all admissible $y.$ Then, by the definition of $\mu_{i}$ , there exists an infinite sequence of functions $\{y_{n}\}=$ $y_{1},y_{2},\ldots$ , called a minimizing sequence, such that  

$$
\operatorname*{lim}_{n\to\infty}\ J[y_{n}]=\upmu.
$$  

If the sequence $\{y_{n}\}$ has a limit function $\hat{y}$ , and if it is legitimate to write  

$$
J[{\hat{y}}]=\operatorname*{lim}_{n\to\infty}J[y_{n}],
$$  

i . e . ,  

$$
J[\operatorname*{lim}_{n\rightarrow\infty}y_{n}]=\operatorname*{lim}_{n\rightarrow\infty}J[y_{n}],
$$  

then  

$$
J[{\hat{y}}]=\mu,
$$  

and $\hat{y}$ is the solution of the variational problem. Moreover, the functions of the minimizing sequence $\{y_{n}\}$ can be regarded as approximate solutions of our problem.  

Thus, to solve a given variational problem by the direct method, we must  

1. Construct a minimizing sequence $\{y_{n}\}$ ;   
2. Prove that $\{y_{n}\}$ has a limit function $\hat{y}$ ;   
3. Prove the legitimacy of taking the limit (2) .  

Remark 1 .  Two direct methods, the Ritz method and the method offinite difefrences, each involving the construction of a minimizing sequence, will be discussed in the next section. We reiterate that a minimizing sequence can always be constructed if ( I ) holds.  

Remark 2. Even if a minimizing sequence $\{y_{n}\}$ exists for a given varia­ tional problem, it may not have a limit function $\hat{y}$ . For example, consider the functional  

$$
J[y]=\int_{-1}^{1}x^{2}y^{\prime2}d x,
$$  

where  

$$
y(-1)=-1,\qquady(1)=1.
$$  

Obviously, $J[y]$ takes only positive values and  

$$
\operatorname*{inf}_{\pmb{y}}J[y]=0.
$$  

We can choose  

$$
y_{n}(x)={\frac{\tan^{-1}n x}{\tan^{-1}n}}\qquad(n=1,2,\ldots)
$$  

as the minimizing sequence, since  

$$
\int_{-1}^{1}\frac{n^{2}x^{2}d x}{(\tan^{-1}n)^{2}(1+n^{2}x^{2})^{2}}<\frac{1}{(\tan^{-1}n)^{2}}\int_{-1}^{1}\frac{d x}{1+n^{2}x^{2}}=\frac{2}{n\tan^{-1}n},
$$  

and hence $J[y_{n}]\to0$ as $n\to\infty$ .  But a s $.n\rightarrow\infty$ 0 ,  the sequence (4) has no limit in the class of continuous functions satisfying the boundary conditions (3).  

Even if the minimizing sequence $\{y_{n}\}$ has a limit $\hat{y}$ in the sense of the $\mathscr{C}$ -norm (i. e . , $y_{n}\to\hat{y}$ as $n\to\infty$ , without any assumptions about the convergence of the derivatives of $y_{n,\cdot}$ ), it is still no trivial m atter to j ustify taking the limit (2), since in general, the functionals considered in the calculus of variations are not continuous in the $\mathscr{C}$ -norm. However, (2) still holds if continuity of $J[y]$ is replaced by a weaker condition :  

THEOREM. $\mathcal{H}\{y_{n}\}$ is a minimizing sequence of the functional $J[y]$ , with limitfunction $\hat{y}$ , and i $\cdot_{J[y]}$ is lower semicontinuous at $\hat{y},^{2}$ then  

$$
J[{\hat{y}}]=\operatorname*{lim}_{n\to\infty}J[y_{n}].
$$  

Proof. On the one hand,  

$$
J[\hat{y}]\geqslant\operatorname*{lim}_{n\rightarrow\infty}J[y_{n}]=\operatorname*{inf}J[y],
$$  

while, on the other hand, given any $\mathfrak{s}>0$ ,  

$$
J[y_{n}]-J[{\hat{y}}]>-\varepsilon,
$$  

if $n$ is sufficiently large. Letting $n\to\infty$ in (6), we obtain  

$$
J[\widehat{y}]\leqslant\operatorname*{lim}_{n\rightarrow\infty}J[y_{n}]+\varepsilon,
$$  

or  

$$
J[{\hat{y}}]\leqslant\operatorname*{lim}_{n\rightarrow\infty}J[y_{n}],
$$  

since E is arbitrary. Comparing (5) and (7), we find that  

$$
J[{\hat{y}}]=\operatorname*{lim}_{n\to\infty}J[y_{n}],
$$  

as asserted.  

# 40. The Ritz M et hod and the M ethod of F i n ite Differences3  

40.1. First, we describe the Ritz method, one of the most widely used direct variational methods. Suppose we are looking for the minimum of a func­ tional $J[y]$ defined on some space $\mathcal{M}$ { of admissible functions, which for simplicity we take to be a normed linear space. Let  

$$
\varphi_{1},\quad\varphi_{2},\ldots
$$  

be an infinite sequence of functions in $\mathcal{M}$ {, and let $\mathcal{M}_{n}$ be the $\pmb{n}$ -dimensional linear subspace of $\mathcal{M}$ { spanned by the first $\pmb{n}$ of the functions (8), i.e., the set of all linear combinations of the form  

$$
\alpha_{1}\varphi_{1}+\ldots+\alpha_{n}\varphi_{n},
$$  

where $\alpha_{1},...,\alpha_{n}$ are arbitrary real numbers. Then, on each subspace $\mathcal{M}_{n},$ the functional $J[y]$ leads to a function  

$$
J[\alpha_{1}\varphi_{1}+\ldots+\alpha_{n}\varphi_{n}]
$$  

of the $n$ variables $\alpha_{1},...,\alpha_{n}$ .  

Next, we choose $\alpha_{1},...,\alpha_{n}$ in such a way as to minimize ( 1 0), denoting the minimum by $\mu_{n}$ and the element of $\mathcal{M}_{n}$ which yields the minimum by $y_{n}$ . (In principle, this is a much simpler problem than finding the minimum of the functional $J[y]$ itself.) ClearlY, $\mu_{n}$ cannot increase with $\pmb{n}$ , i . e . ,  

$$
\mu_{1}\geqslant\mu_{2}\geqslant\cdots,
$$  

since any linear combination of $\varphi_{1},...,\varphi_{n}$ is automatically a linear combi­ nation $\varphi_{1},...,\varphi_{n},\varphi_{n+1}$ . Correspondingly, each subspace of the sequence  

$$
\mathcal{M}_{1},\quad\mathcal{M}_{2},\ldots
$$  

is contained in the next. We now give conditions which guarantee that the sequence $\{y_{n}\}$ is a minimizing sequence.  

DEFINITION. The sequence (8) is said to be complete $(i n\textbf{\mathcal{M}})$ if given any $y\in\mathcal{M}$ {and any $\mathfrak{s}>0$ , there is a linear combination $\eta_{n}$ of the form (9) such that $\|\gamma_{n}-y\|<\varepsilon$ (where $\pmb{n}$ depends on E).  

THEOREM. lf thefunctional $J[y]$ is continuous,4 and if the sequence (8) is complete, then  

$$
\operatorname*{lim}_{n\to\infty}\upmu_{n}=\upmu,
$$  

where  

$$
{\mu}=\operatorname*{inf}_{y}J[y].
$$  

Proof Given any $\mathfrak{s}>0$ , let $y^{\star}$ be such that  

$$
J[y^{\ast}]<\mu+\varepsilon.
$$  

(Such a $y^{*}$ exists for any $\mathfrak{s}>0$ , by the definition of $\mu$ .) Since $J[y]$ is continuous,  

$$
|J[y]-J[y^{*}]|<\varepsilon,
$$  

provided that $\|y-y^{*}\|<\delta=\delta(\mathfrak{e})$ . Let $\eta_{n}$ be a linear combination of the form (9) such that $\|\gamma_{1n}-y^{*}\|<8$ . (Such an $\eta_{n}$ exists for suffi­ ciently large $n$ , since $\{\varphi_{n}\}$ is complete.) Moreover, let $y_{n}$ be the linear combination of the form (9) for which ( 1 0) achieves its minimum. Then, using ( 1 1 ), we find that  

$$
\mu\leqslant J[y_{n}]\leqslant J[\eta_{n}]<\mu+2\varepsilon.
$$  

Since e is arbitrary, it follows that  

$$
\operatorname*{lim}_{n\to\infty}J[y_{n}]=\operatorname*{lim}_{n\to\infty}\mu_{n}=\mu,
$$  

as asserted.  

Remark 1. The geometric idea of the proof is the following : If $\{\varphi_{n}\}$ is complete, then any element in the infinite-dimensional space $\mathcal{M}$ { can be approximated arbitrarily closely by an element in the finite-dimensional space $\mathcal{M}_{n}$ (for large enough $n$ ). We can summarize this fact by writing  

$$
\operatorname*{lim}_{n\rightarrow\infty}\mathcal{M}_{n}=\mathcal{M}.
$$  

Let $\hat{y}$ be the element in $\mathcal{M}$ { for which $J[\widehat{y}]=\mu,$ and let $\hat{y}_{n}\in\mathcal{M}_{n}$ be a sequence of functions converging to $\hat{y}$ . Then $\{\hat{y}_{n}\}$ is a minimizing sequence, since $J[y]$ is continuous. Although this minimizing sequence cannot be con­ structed without prior knowledge of $\hat{y}$ , we can show that our explicitly constructed sequence $\{y_{n}\}$ takes values $J[y_{n}]$ arbitrarily close to $J[\hat{y}_{n}]$ . and hence is itself a minimizing sequence.  

Remark 2. The speed of convergence of the Ritz method for a given variational problem obviously depends both on the problem itself and on the choice of the functions $\varphi_{n}$ . However, it should be pointed out that in many cases, linear combinations involving only a very small number of functions $\varphi_{n}$ are enough to give a quite satisfactory approximation to the exact solution.  

Remark 3. More generally, the spaces $\mathcal{M}$ { and $\mathcal{M}_{n}$ need not be normed linear spaces themselves, but only suitable sets of admissible functions belonging to an underlying normed linear space $\mathcal{R}$ (see Remark 3 , p . 8). For example, the admissible functions may satisfy boundary conditions like  

$$
y(a)=A,\qquady(b)=B
$$  

(see Sec. 40.2), or a subsidiary condition like  

$$
\int_{a}^{b}y^{2}(x)d x=1
$$  

(see Sec. 4 1 ). This case can be handled by appropriate modifications of the present method.  

40.2. We now describe another method involving a sequence of finite­ dimensional approximations to the space $\mathcal{M}$ ,({. This is the method of finite difefrences, which has already been encountered in Sec. 7. There, in con­ nection with the derivation of Euler's equation, we noted that the problem of finding an extremum of the functional5  

$$
J[y]=\int_{a}^{b}F(x,y,y^{\prime})d x,\qquady(a)=A,\quad y(b)=B,
$$  

can be approximated by the problem of finding an extremum of a function of $\pmb{n}$ variables, obtained as follows : We divide the interval $[a,b]$ into $n+1$ equal subintervals by introducing the points  

$$
x_{0}=a,\quad x_{1},\ldots,x_{n},\quad x_{n+1}=b,\qquadx_{i+1}-x_{i}=\Delta x,
$$  

and we replace the function $y(x)$ by the polygonal line with vertices  

$$
(x_{0},y_{0}),(x_{1},y_{1}),\dotsc,(x_{n},y_{n}),(x_{n+1},y_{n+1}),
$$  

where now $y_{i}=y(x_{i})$ . Then ( 1 2) can be approximated by the sum  

$$
J(y_{1},...,y_{n})=\sum_{i=0}^{n}F\left[x_{i},y_{i},{\frac{y_{i+1}-y_{i}}{\Delta x}}\right]\Delta x,
$$  

which is a function of $n$ variables. ( Recall that $y_{0}=A$ and $y_{n+1}=B$ are fixed.) If for each $n$ , we find the polygonal line minimizing ( 1 3), we obtain a sequence of approximate solutions to the original variational problem .  

# 4 1 .  T h e St u r m - l i o u v i l l e  P ro b l e m  

In this section, w e illustrate the application o f direct variational methods to differential equations (cf. the remarks on p. 1 92), by studying the follow­ ing boundary value problem, known as the Sturm-Liouville problem : Let $P=P(x)>0$ and $Q=Q(x)$ be two given functions, where $\ensuremath{\boldsymbol{Q}}$ is continuous and $P$ is continuously differentiable, and consider the differential equation  

$$
-(P y^{\prime})^{\prime}+Q y=\lambda y
$$  

(known as the Sturm-Liouville equation), subject to the boundary conditions  

$$
y(a)=0,\qquady(b)=0.
$$  

It is required to find the eigenfunctions and eigenvalues of the given boundary value problem, i.e., the nontrivial solutions6 of ( 1 4), ( 1 5) and the correspond­ ing values of the parameter $\lambda$ .  

THEOREM. The Sturm-Liouville problem ( 1 4), ( 1 5) has an infinite sequence of eigenvalues A(1), A(2), . . , and to each eigenvalue $\lambda^{(n)}$ there corresponds an eigenfunction $y^{(n)}$ which is unique to within $\pmb{a}$ constant factor.  

The proof of this theorem will be carried out in stages, and at the same time we shall derive a method for approximating the eigenvalues $\lambda^{(n)}$ and eigenfunctions $y^{(n)}$ .  

41. 1 . We begin by observing that ( 1 4) is the Euler equation corresponding to the problem of finding an extremum of the quadratic functional  

$$
J[y]=\int_{a}^{b}\left(P y^{\prime2}+Q y^{2}\right)d x,
$$  

subject to the boundary conditions ( 1 5) and the subsidiary condition7  

$$
\int_{a}^{b}y^{2}d x=1.
$$  

Thus, if $y(x)$ is a solution of this variational problem, it is also a solution of the differential equation ( 1 4), satisfying the boundary conditions ( 1 5). Moreover, $y(x)$ is not identically zero, because of the condition ( 1 7).  

Next, we apply the Ritz method (see Sec. 40. 1 )  to the functional ( 1 6), first  

verifying that it is bounded from below, as required [cf. formula ( I )]. Since $P(x)>0$ , this fact follows from the inequality  

$$
\int_{a}^{b}{(P y^{\prime2}+Q y^{2})d x}>\int_{a}^{b}{Q y^{2}d x}\geqslant M\int_{a}^{b}{y^{2}d x}=M,
$$  

where  

$$
M=\operatorname*{min}_{a\leqslant z\leqslant b}Q(x).
$$  

For simplicity, we assume that $a=0,b=\pi$ , and we choose $\{\sin n x\}$ as the complete sequence of functions $\{\varphi_{n}(x)\}$ used in the Ritz method. This sequence also has the desirable feature of being orthogonal, i.e. ,  

$$
\int_{0}^{\pi}\sin k x\sin l x d x=0\qquad(k\neq l).
$$  

If a linear combination  

$$
\sum_{k=1}^{n}\alpha_{k}\sin{k x}
$$  

is to be admissible, it m ust satisfy the conditions ( 1 5) and ( 1 7). The condition ( 1 5) is automatically satisfied by our choice of the functions sin $n x$ , but ( 1 7) leads to the requirement  

$$
\int_{0}^{\pi}\Bigl(\sum_{k=1}^{n}\alpha_{k}\sin k x\Bigr)^{2}d x=\frac{\pi}{2}\sum_{k=1}^{n}\alpha_{k}^{2}=1.
$$  

Moreover, for a linear combination ( I 8), the functional $J[y]$ reduces to  

$$
J_{n}(\alpha_{1},\ldots,\alpha_{n})=\int_{0}^{\pi}\Big[P(x)\Big(\sum_{k=1}^{n}\alpha_{k}\sin k x\Big)^{\prime2}+Q(x)\Big(\sum_{k=1}^{n}\alpha_{k}\sin k x\Big)^{2}\Big]d x,
$$  

which is a function of the $\pmb{n}$ variables $\alpha_{1},\ldots,\alpha_{n}$ (in fact, a quadratic form in these variables.  

Thus, in terms of the variables $\alpha_{1},\ldots,\alpha_{n}$ , our problem is to minimize $J_{n}(\alpha_{1},...,\alpha_{n})$ on the surface ${\pmb{\sigma}}_{\pmb{n}}$ of the $\pmb{n}$ -dimensional sphere with eq uation ( 1 9). Since $\upsigma_{n}$ is a compact set and $J_{n}(\alpha_{1},...,\alpha_{n})$ is continuous on $\sigma_{n},J_{n}(\alpha_{1},\ldots,\alpha_{n})$ has a minimum $\lambda_{n}^{(1)}$ at some point $\alpha_{1}^{(1)},...,\alpha_{n}^{(1)}$ of ${\pmb{\sigma}}_{\pmb{n}}$ • 8 Let  

$$
y_{n}^{(1)}(x)=\sum_{k\mathop{=}1}^{n}\alpha_{k}^{(1)}\sin k x
$$  

be the linear combination ( 1 8) achieving the minimum $\lambda_{n}^{(1)}$ . If this procedure is carried out for $n=1,2,\ldots$ , we obtain a sequence of numbers  

$$
\lambda_{1}^{(1)},\lambda_{2}^{(1)},...,
$$  

and a corresponding sequence of functions  

$$
y_{1}^{(1)}(x),y_{2}^{(1)}(x),...
$$  

Noting that ${\pmb{\sigma}}_{\pmb{n}}$ is the subset of $\upsigma_{n+1}$ obtained by setting $\alpha_{n+1}=0$ , while  

$$
J_{n}(\alpha_{1},...,\alpha_{n})=J_{n+1}(\alpha_{1},...,\alpha_{n},0),
$$  

we see that  

$$
\begin{array}{r}{\lambda_{n+1}^{(1)}\leqslant\lambda_{n}^{(1)},}\end{array}
$$  

since increasing the domain of definition of a function can only decrease its minimum. It follows from (23) and the fact that $J[y]$ is bounded from below that the limit  

$$
\lambda^{(1)}=\operatorname*{lim}_{n\rightarrow\infty}\ \lambda_{n}^{(1)}
$$  

exists.  

41.2. Now that we have proved the convergence of the sequence of numbers (2 1 ), representing the minima of the functional  

$$
\int_{0}^{\pi}(P y^{\prime}{}^{2}+Q y^{2})d x
$$  

on the sets of functions of the form  

$$
\sum_{k=1}^{n}\alpha_{k}\sin{k x}
$$  

satisfying the condition ( 1 9), it is natural to try to prove the convergence of the sequence of functions (22) for which these minima are achieved. We first prove a weaker result :  

LEMMA l . The sequence $\{y_{n}^{(1)}(x)\}$ contains a uniformly convergent subsequence.  

Proof For simplicity, we temporarily write $y_{n}(x)$ instead of $y_{n}^{(1)}(x)$ . The sequence  

$$
\lambda_{n}^{(1)}=\int_{0}^{\pi}\left(P y_{n}^{\prime2}+Q y_{n}^{2}\right)d x
$$  

is convergent and hence bounded, i.e.,  

$$
\int_{0}^{\pi}\left(P y_{n}^{\prime2}+Q y_{n}^{2}\right)d x\leqslant M
$$  

for all $n$ , where $M$ is some constant. Therefore  

$$
\int_{0}^{\pi}P y_{n}^{\prime2}d x\leqslant M+\left|\int_{0}^{\pi}Q y_{n}^{2}d x\right|\leqslant M+\operatorname*{max}_{a\leqslant x\leqslant b}\left|Q(x)\right|=M_{1},
$$  

and since $P(x)>0$ ,  

$$
\int_{0}^{\pi}y_{n}^{\prime2}(x)d x\leqslant\frac{M_{1}}{\underset{a\leqslant x\leqslant b}{\operatorname*{min}}P(x)}=M_{2}.
$$  

Using (25), the condition  

$$
y_{n}(0)=0,
$$  

and Schwarz's inequality, we findOthat  

$$
|y_{n}(x)|^{2}={\bigg|}\int_{0}^{x}y_{n}^{\prime}(\xi)d\xi{\bigg|}^{2}\leqslant\int_{0}^{x}y_{n}^{\prime2}(\xi)d\xi\int_{0}^{x}d\xi\leqslant M_{2}\pi,
$$  

SO that $\{y_{n}(x)\}$ is uniformly bounded. 9 Moreover, again using Schwarz's inequality, we have  

$$
|y_{n}(x_{2})-y_{n}(x_{1})|^{2}=\bigg|\int_{z_{1}}^{z_{2}}y_{n}^{\prime}(x)d x\bigg|^{2}\leqslant\int_{z_{1}}^{z_{2}}y_{n}^{\prime2}d x\cdot\bigg|\int_{x_{1}}^{z_{2}}d x\bigg|\leqslant M_{2}|x_{2}-x_{1}|,
$$  

so that $\{y_{n}(x)\}$ s equicontinuous. 1 o Thus, according to Arzela's theorem, l 1 we can select a uniformly convergent subsequence $\{y_{n_{m}}(x)\}$ from the sequence $\{y_{n}(x)\}$ and Lemma I is proved.  

We now set  

$$
y^{(1)}(x)=\operatorname*{lim}_{m\rightarrow\infty}y_{n_{m}}(x).
$$  

Our object is to show that $y^{(1)}(x)$ satisfies the Sturm-Liouville equation ( 1 4) with $\lambda=\lambda^{(1)}$ . However, we are still not in a position to take the limit as $m\to\infty$ of the integral  

$$
\int_{0}^{\pi}(P y_{n_{m}}^{\prime2}+Q y_{n_{m}}^{2})d x,
$$  

since as yet we know nothing about the convergence of the derivatives $y_{n_{m}}^{\prime}$ . Therefore, the fact that for each $m_{i}$ , the function $y_{n_{m}}$ minimizes the functional $J[y]$ for $y$ in the ${\boldsymbol{n}}_{m}$ -dimensional space spanned by the linear combinations  

$$
\sum_{k=1}^{n_{m}}\alpha_{k}\sin{k x}
$$  

[subject t o  the condition ( 1 9) with $n=n_{m}]$ still does not imply that the limit function $y^{(1)}(x)$ minimizes $J[y]$ for $y$ in the full space of admissible functions. To avoid this difficulty, we argue as follows :  

LEMMA 2. Let $y(x)$ be continuous in $[0,\pi]$ , and let  

$$
\int_{0}^{\pi}{\left[-(P h^{\prime})^{\prime}+Q_{1}h\right]_{\textstyle3}d x}=0
$$  

9 A family of functions $\Psi$ defined on $[a,b]$ is said to be uniformly bounded if there is a constant $M$ such that  

$$
|\Psi(x)|\leqslant M
$$  

for all $\boldsymbol{\Psi}\in\boldsymbol{\Psi}$ a n d all $a\leqslant x\leqslant b$ .  

$^{10}\mathbf{A}$ family of functions $\Psi$ defined on $[a,b]$ is said to be equ;continuous if given any $\varepsilon>0$ , there i s a $\delta>0$ such that  

$$
|\uppsi(x_{2})-\uppsi(x_{1})|<\upvarepsilon
$$  

for all $\boldsymbol{\Psi}\in\boldsymbol{\Psi}$ Y, provided that $|x_{2}-x_{1}|<\delta.$  

1 1 Arzelil's theorem states that every uniformly bounded and equicontinuous sequence of functions contains a uniformly convergent subsequence (converging to a continuous l i m i t function). See e . g . , R . Courant and D . H i l bert, op. cit . , vol. 1 , p . 59.  

for every function $h(x)\in{\mathcal{D}}_{2}(0,\pi),$ 12 satisfying the boundary conditions  

$$
h(0)=h(\pi)=0,\qquadh^{\prime}(0)=h^{\prime}(\pi)=0.
$$  

Then $y(x)$ also belongs to $\mathcal{D}_{2}(0,\pi)$ , and  

$$
-(P y^{\prime})^{\prime}+Q_{1}y=0.
$$  

Proof If we integrate (27) by parts and use (28), we find that  

$$
\begin{array}{r l r}{\lefteqn{\int_{0}^{\pi}\left[-(P h^{\prime})^{\prime}+Q_{1}h\right]y d x=-\int_{0}^{\pi}P h^{\prime}y d x-\int_{0}^{\pi}P^{\prime}h^{\prime}y d x+\int_{0}^{\pi}Q_{1}h y d x}}\\ &{}&{=-\int_{0}^{\pi}\left[-P y+\int_{0}^{x}P^{\prime}y d\xi+\int_{0}^{z}\left(\int_{0}^{\xi}Q_{1}y d t\right)d\xi\right]d x=0.}\end{array}
$$  

It follows from Lemma 3, p. 10 that  

$$
-P y+\int_{0}^{\tau}P^{\prime}y d\xi+\int_{0}^{\tau}\left(\int_{0}^{\xi}Q_{1}y d t\right)d\xi=c_{0}+c_{1}x,
$$  

where $c_{0}$ and $c_{1}$ are constants. Since the right-hand side and the second and third terms in the left-hand side of (29) are obviously differentiable, $(P y)^{\prime}$ exists, and in fact, differentiati ng (29) term by term, we find that  

$$
-(P y)^{\prime}+P^{\prime}y+\int_{0}^{x}Q_{1}y d\xi=c_{1}.
$$  

Since the function $P$ is continuously differentiable and does not vanish, $y^{\prime}$ exists and is continuous. Thus, (30) reduces to  

$$
-P y^{\prime}+\int_{0}^{x}Q_{1}y d\xi=c_{1}.
$$  

Since the right-hand side and the second term in the left-hand side of (3 1) are differentiable, it follows that $(P y^{\prime})^{\prime}$ exists, a n d in fact  

$$
-(P y^{\prime})^{\prime}+Q_{1}y=0,
$$  

as asserted. Moreover, by the same argument as before, $y^{\prime\prime}$ exists and is continuous.  

41.3. We can now show that the function $y^{(1)}(x)$ defined by (26), whose existence follows from Lemma 1 , satisfies the Sturm-Liouville equation  

$$
-(P y^{(1)\prime})^{\prime}+Q y^{(1)}=\uplambda^{(1)}y^{(1)},
$$  

where $\lambda^{(1)}$ is the limit (24). According to the theory of Lagrange mul tipliers (cf. footnote 7, p. 43), at the point $\big(\pmb{\alpha}_{1}^{(1)},\dots..,\pmb{\alpha}_{n}^{(1)}\big)$ where the quadratic form (20) achieves its minimum subject to the subsidiary condition ( 1 9), we have  

$$
\frac{\partial}{\partial\alpha_{r}}\left\{J_{n}(\alpha_{1},...,\alpha_{n})-\mathrm{\Large~\wedge}_{n}^{(1)}\int_{0}^{\pi}\left(\sum_{k=1}^{n}\alpha_{k}\mathrm{\Large~sin~}k x\right)^{2}\right\}d x=0\qquad(r=1,...,n),
$$  

This leads to the $\pmb{n}$ equations  

$$
\begin{array}{l}{{\displaystyle\int_{0}^{\pi}\biggl\{P(x)\biggl[\sum_{k=1}^{n}\alpha_{k}^{(1)}(\sin k x)^{\prime}\biggr](\sin r x)^{\prime}}}\\ {{+\left[Q(x)-\uplambda_{n}^{(1)}\right]\biggl[\sum_{k=1}^{n}\alpha_{k}^{(1)}\sin k x\biggr]\sin r x\biggr\}d x=0\qquad(r=1,...,n).}}\end{array}
$$  

Multiplying each of the equations (33) by an arbitrary constant ${C}_{r}^{\left(n\right)}$ and summing over $r$ from 1 to $\pmb{n}$ , we obtain  

$$
\int_{0}^{\pi}\left[P y_{n}^{\prime}h_{n}^{\prime}+(Q-\lambda_{n}^{\scriptscriptstyle(1)})y_{n}h_{n}\right]d x=0,
$$  

where  

$$
h_{\mathfrak{n}}(x)=\sum_{r=1}^{\mathfrak{n}}C_{r}^{(n)}\sin r x.
$$  

An integration by parts transforms (34) into  

$$
\int_{0}^{\pi}{\bigl[}-(P h_{n}^{\prime})^{\prime}+(Q-\lambda_{n}^{\scriptscriptstyle(1)})h_{n}\bigr]y_{n}d x=0.
$$  

If $h(x)$ is an arbitrary function in $\mathcal{D}_{2}(0,\pi)$ satisfying the boundary conditions (28), we can choose the coefficients $C_{r}^{(n)}$ in such a way that  

$$
h_{n}\Rightarrow h,\quad h_{n}^{\prime}\Rightarrow h^{\prime},\quad h_{n}^{\prime\prime}\Rightarrow h^{\prime\prime}
$$  

(see Prob. 8). Here, the symbol $\mid\Rightarrow$ denotes convergence in the mean, i.e., $\displaystyle h_{n}\Rightarrow h$ stands for  

$$
\operatorname*{lim}_{n\to\infty}\int_{0}^{\pi}|h_{n}(x)-h(x)|^{2}d x=0
$$  

Since $y_{n}^{(1)}\to y^{(1)}$ uniformly in $[0,\pi],^{13}$ it follows from (36) that  

$$
\begin{array}{c}{{\displaystyle\operatorname*{lim}_{m\to\infty}\int_{0}^{\pi}{[{-(P h_{n_{m}}^{\prime})^{\prime}+(Q-\lambda_{n_{m}}^{\scriptscriptstyle(1)})h_{n_{m}}}]y_{n_{m}}^{\scriptscriptstyle(1)}d x}}}\\ {{{}}}\\ {{{}=\displaystyle\int_{0}^{\pi}{[{-(P h^{\prime})^{\prime}+(Q-\lambda^{\scriptscriptstyle(1)})h}]y^{\scriptscriptstyle(1)}d x}=0}}\end{array}
$$  

(see Prob. 9). The fact that $y^{(1)}$ is an element of $\mathcal{D}_{2}(0,\pi)$ and satisfies the Sturm-Liouville equation (32) is now an immediate consequence of Lemma 2, with $Q_{1}=Q-\lambda^{(1)}$ .  

So far, the function $y^{(1)}(x)$ has been defined as the limit of a subsequence $\{y_{n_{m}}^{(1)}(x)\}$ of the original sequence $\{y_{n}^{(1)}(x)\}$ . We now show that the sequence  

$\{y_{n}^{(1)}(x)\}$ itself converges to $y^{(1)}(x)$ . To prove this, we use the fact that for a given $\lambda$ , the solution of the Sturm-Liouville equation  

$$
-(P y^{\prime})^{\prime}+Q y=\lambda y
$$  

satisfying the boundary conditions  

$$
y(0)=0,~y(\pi)=0
$$  

and the normalization condition  

$$
\int_{0}^{\pi}y^{2}(x)d x=1
$$  

is unique except for sign. Let $y^{(1)}(x)$ be a solution of (37) corresponding to $\lambda=\lambda^{(1)}$ , and suppose $y^{(1)}(x_{0})\neq0$ at some point $x_{0}$ in $[0,\pi]$ . Then choose the sign so that $y^{(1)}(x_{0})>0$ . Simi larly, let $y_{n}^{(1)}(x)$ be a solution of (37) corresponding to $\lambda=\lambda_{n}^{(1)}$ , and choose the signs so that $y_{n}^{(1)}(x_{0})\geqslant0$ for all $n$ If $y_{n}^{(1)}(x)$ does not converge to $y^{(1)}(x)$ , we can select another subsequence from $\{y_{n}^{(1)}(x)\}$ converging to another solution $\bar{y}^{(1)}(x)$ of (37), where again $\lambda=\lambda^{(1)}$ . Because of the uniqueness (except for sign) of solutions of (37), subject to (38) and (39), this means that  

$$
\bar{y}^{(1)}(x)=-y^{(1)}(x),
$$  

and hence $\bar{y}^{(1)}\bigl(x_{0}\bigr)<0$ , which is impossible, since $y_{n}^{(1)}\bigl(x_{0}\bigr)\geqslant0$ fo r all $n$ . Therefore, $y_{n}^{(1)}(x)\to y^{(1)}(x)$ [in fact, uniformly], provided we choose each $y_{n}^{(1)}(x)$ with the proper sign.  

41.4. We have just proved that the Sturm-Liouville problem has the eigen­ function $y^{(1)}(x)$ corresponding to the eigenvalue $\lambda^{(1)}$ . The " next " eigen­ function $y^{(2)}(x)$ and the corresponding eigenvalue $\lambda^{(2)}$ can be found by minimizing the quadratic functional  

$$
J[y]=\int_{0}^{\pi}\left(P y^{\prime2}+Q y^{2}\right)d x
$$  

subject to the same conditions (38) and (39) as before, plus an extra orthog­ onality condition  

$$
\int_{0}^{\pi}y^{(1)}(x)y(x)d x=0.
$$  

In fact, substituting  

$$
y(x)=\sum_{k=1}^{n}\alpha_{k}\sin{k x}
$$  

into (40), we again obtain the quadratic form $J_{n}(\alpha_{1},...,\alpha_{n})$ given by (20), but this time we study $J_{n}(\alpha_{1},\ldots,\alpha_{n})$ on the set of functions of the form (42) which not only lie on the $\pmb{n}$ -dimensional sphere $\upsigma_{n}$ with equation ( 1 9) , thereby satisfying the normalization condition (39), but are also orthogonal to the function  

$$
y_{n}^{(1)}(x)=\sum_{k=1}^{n}\alpha_{k}^{(1)}\sin k x,
$$  

i.e. , satisfy the condition  

$$
\sum_{k=1}^{n}\alpha_{k}\int_{0}^{\pi}\sin k x\bigg(\sum_{l=1}^{n}\alpha_{l}^{(1)}\sin l x\bigg)d x=\frac{\pi}{2}\sum_{k=1}^{n}\alpha_{k}\alpha_{k}^{(1)}=0.
$$  

This is the equation of an $(n\mathrm{~-~}1)$ -dimensional hyperplane, passing through the origin of coordinates in $n$ dimensions. Its intersection with the sphere ( I 9) is an $(n\mathrm{~-~}1)$ -dimensional sphere $\hat{\sigma}_{n-1}$ . By the same argument as before (cf. footnote 8), $J_{n}(\alpha_{1},...,\alpha_{n})$ has a minimum $\lambda_{n}^{(2)}$ on $\hat{\sigma}_{n-1}$ . It is not hard to see that  

$$
\lambda_{n+1}^{(2)}\leqslant\lambda_{n}^{(2)}
$$  

[cf. (23)], and hence the limit  

$$
\lambda^{(2)}=\operatorname*{lim}_{n\rightarrow\infty}\ \lambda_{n}^{(2)}
$$  

exists, since $J[y]$ is bounded from below. Moreover, it is obvious that  

$$
\lambda^{(1)}\leqslant\lambda^{(2)}.
$$  

Now let  

$$
y_{n}^{(2)}=\sum_{k=1}^{n}\alpha_{k}^{(2)}\sin k x
$$  

be the linear combination (42) achieving the minimum $\lambda_{n}^{(2)}$ , where, of course, the point $\big(\mathsf{\alpha}_{1}^{(2)},....,\mathsf{\alpha}_{n}^{(2)}\big)$ lies on the sphere $\hat{\sigma}_{n-1}$ • As before, we can show that the sequence $\{y_{n}^{(2)}(x)\}$ converges uniformly to a limit function $y^{(2)}(x)$ which satisfies the Sturm-Liouville equation (37) [with $\lambda=\lambda^{(2)}]$ , the boun­ dary conditions (38), the normalization condition (39), and the orthogonality condition (4 1 ). In other words, $y^{(2)}(x)$ is the eigenfunction of the Sturm­ Liouville problem corresponding to the eigenvalue $\lambda^{(2)}$ . Since orthogonal functions cannot be linearly dependent, and since only one eigenfunction corresponds to each eigenvalue (except for a constant factor), we have the strict inequality  

$$
\lambda^{(1)}<\lambda^{(2)},
$$  

instead of (44). Finally, we note that by repeating the above argument, with obvious modifications, we can obtain further eigenvalues ${\lambda^{(3)},\lambda^{(4)},\dots,}$ and corresponding eigenfunctions $y^{(3)}(x),\ y^{(4)}(x),\ldots...$  

For further material on the use of direct methods in the calculus of varia­ tions, we refer the reader to the abundant literature on the subject. 1 4  

# PROBLEMS  

1. Let the functional $J[y]$ be such that $J[y]>{}-\infty$ for some admissible function, and let  

$$
\mathsf{s u p}J[y]=\mu<+\infty,
$$  

where sup denotes the least upper bound or supremum. By analogy with the treatment given in Sec. 39, define a maximizing sequence, and then state and prove the corresponding version of the theorem on p. 1 94.  

2. Use the Ritz method to find an approximate solution of the problem of minimizing the functional  

$$
J[y]=\int_{0}^{1}\left(y^{\prime2}-y^{2}-2x y\right)d x,\qquady(0)=y(1)=0,
$$  

and compare the answer with the exact solution.  

Hint. Choose the sequence $\{\varphi_{n}(x)\}$ (see p. 1 95) to be  

$$
x(1\ -\ x),x^{2}(1\ -\ x),x^{3}(1\ -\ x),\ .\ .\ .
$$  

3. Use the Ritz method to find an approximate solution of the extremum problem associated with the functional  

$$
J[y]=\int_{0}^{1}\left(x^{3}y^{\prime\prime2}+100x y^{2}-20x y\right)d x,\qquady(1)=y^{\prime}(1)=0.
$$  

Hint. Choose the sequence $\{\varphi_{n}(x)\}$ to be  

$$
(x\ -\ 1)^{2},\quad x(x\ -\ 1)^{2},\quad x^{2}(x\ -\ 1)^{2},\ldots
$$  

4. Use the Ritz method to find an approximate solution of the problem of minimizing the functional  

$$
J[y]=\int_{0}^{2}\left(y^{\prime2}+y^{2}+2x y\right)d x,\qquady(0)=y(2)=0,
$$  

and compare the answer with the exact solution.  

5. Use the Ritz method to find an approximate solution of the equation  

$$
{\frac{\partial^{2}u}{\partial x^{2}}}+{\frac{\partial^{2}u}{\partial y^{2}}}=-1
$$  

inside the square  

$$
\begin{array}{r}{R:\qquad-a\leqslant x\leqslant a,\qquad-a\leqslant y\leqslant a,}\end{array}
$$  

where $\pmb{u}$ vanishes on the boundary of $R$ .  

Hint. Study the functional  

$$
J[u]=\int\int_{R}\left[\left(\frac{\partial u}{\partial x}\right)^{2}+\left(\frac{\partial u}{\partial y}\right)^{2}-2u\right]d x d y,
$$  

and choose the two-dimensional generalization of the sequence $\{\varphi_{n}(x)\}$ to be  

$$
(x^{2}-a^{2})(y^{2}-b^{2}),\quad(x^{2}+y^{2})(x^{2}-a^{2})(y^{2}-b^{2}),\cdot\cdot\cdot\cdot
$$  

6. Write the Sturm-Liouville equation associated with the quadratic functional  

$$
J[y]=\int_{a}^{b}\left(c_{1}y^{\prime2}+c y^{2}\right)d x,
$$  

where $\boldsymbol{\mathscr{c}}$ and $c_{1}>0$ are constants, subject to the boundary conditions  

$$
y(a)=0,\qquady(b)=0.
$$  

Find the corresponding eigenvalues and eigenfunctions.  

7. Formulate a variational problem leading to the Sturm-Liouville equation (14) subject to the boundary conditions  

$$
y^{\prime}(a)=0,\qquady^{\prime}(b)=0,
$$  

instead of the boundary conditions ( 1 5).  

Hint. Recall the natural boundary conditions (29) of Sec. 6.  

8. Prove that any function $h(x)\in\mathcal{D}_{2}(0,\pi)$ satisfying the boundary conditions (28) can be approximated in the mean by a linear combination  

$$
h_{n}(x)=\sum_{r=1}^{n}C_{r}^{(n)}\sin{r x},
$$  

where a t  the same time $h_{n}^{\prime}(x)$ approximates $h^{\prime}(x)$ and $\pmb{h}_{n}^{\prime\prime}(\pmb{x})$ approximates $h^{\prime\prime}(x)$ [in the mean]. Show that the coefficients $C_{r}^{(n)}$ need not depend on $\pmb{n}$ and can be written simply as $C_{r}$ .  

Hint. Form the Fourier sine series of $h^{\prime\prime}(x)$ and integrate it twice term by term.  

9. Show that if $f_{n}(x)\rightarrow f(x)$ in the mean and $g_{n}(x)\to g(x)$ uniformly i n some interval $[a,b],$ , then  

$$
\int_{a}^{b}f_{n}(x)g_{n}(x)d x-\int_{a}^{b}f(x)g(x)d x.
$$  

Hint. Use Schwarz's inequality.  

# Appendix I  

# PROPA GATION OF DISTURBAN CES AND THE CANONICAL EQUA TIONS  

In this appendix, w e consider the propagation o f " disturbances " i n a medium which is regarded as being both inhomogeneous and anisotropic. Thus, in general, the velocity of propagation of a disturbance at a given point of the medium will depend both on the position of the point and on the direction of propagation of the disturbance. We also make the following two assumptions about the process under consideration :  

I .  Each point can be in only one of two states, excitation or rest, i.e. , no concept of the intensity of the disturbance is introduced.   
2. If a disturbance arrives at the point $P$ at the time $t$ , then starting from the time $t,$ , the point $P$ itself serves as a s o u rce of fu rther distu rbances propagating in the medium.  

In the analysis given here, our aim is to show that a study of processes of excitation of the kind described , together with purely geometric considera­ tions, can be used to derive such basic concepts of the calculus of variations as the canonical equations, the H amiltonian function, the H amilton-Jacobi equation, etc. The treatment given here does not rely upon the derivations of these concepts given in the main body of the book (see Secs. 1 6, 23), and in fact can be used to replace the previous derivations. The reader acquainted with optics will recognize that we are essentially constructing a mathe­ matical model of the familiar Huygens ' principle.2  

1. Statement of the problem. Let the medium in which the disturbance propagates fill a space $\mathcal{X}$ !l', which for simplicity we take to be $n$ -dimensional Euclidean space. Thus, every point $\boldsymbol{x}\in\mathcal{X}$ is specified by a set of $\pmb{n}$ real numbers $x^{1},...,x^{n}$ . Choosing a fixed point $\boldsymbol{x}_{0}\in\mathcal{X}$ !l', we consider the set of all smooth curves  

$$
x=x(s)
$$  

passing through $x_{0}$ . The set o f vectors tangent t o the curve ( 1 ) a t the point $x_{0}$ , i.e. , the set of vectors  

$$
x^{\prime}={\frac{d x}{d s}},
$$  

forms an $\pmb{n}$ -dimensional linear space, which we call the tangent space to $\mathcal{X}$ at $x_{0}$ and denote by $\mathcal{T}(x_{0})$ . Note that the end points of the vectors in any tangent space $\mathcal{T}(x)$ are points of $\mathcal{X}$ itself. 3  

Since the medium is inhomogeneous and anisotropic, the velocity of propagation of disturbances in $\mathcal{X}$ depends on position and direction, i.e. , on $x$ and $x^{\prime}$ . Let $f(x,x^{\prime})$ denote the reciprocal of this velocity. Then, if $x(s)$ and $x(s+d s)$ are two neighboring points lying on some curve $x=x(s)$ , the time $d t$ which it takes the disturbance to go from the point $x(s)$ to the point $x(s+d s)$ can be written in the form  

$$
d t=f{\bigg(}x,{\frac{d x}{d s}}{\bigg)}d s,
$$  

and the time it takes the disturbance to propagate along some infinite path joining the points $x_{0}=x(s_{0})$ and $x_{1}=x(s_{1})$ equals  

$$
\int_{s_{0}}^{s_{1}}f\bigg(x,\frac{d x}{d s}\bigg)\ d s.
$$  

Suppose the point $x_{0}$ is " excited , " and consider all possible paths joining $x_{0}$ and $x_{1}$ ' Then, because of the " off or on " character of the excitation, the only path which plays any role in the propagation process is the one along which the disturbance propagates in the smallest time, say T. (Disturbances arriving at $x_{1}$ via some other path which is traversed in a time $>\tau$ will arrive at $x_{1}$ " too late " to have any further effect on the propagation process, since $x_{1}$ will already be found in a state of excitation.) In other words,  

$$
\tau=\displaystyle\operatorname*{min}\int_{s_{0}}^{s_{1}}f\left(x,\frac{d x}{d s}\right)d s,
$$  

where the minimum is taken with respect to all curves $x=x(s)$ joining the points $x_{0}$ and $x_{1}$ ' Thus, the propagation of disturbances in the medium obeys the familiar Fermat principle (p. 34), i.e., among all paths joining $\scriptstyle x_{0}$ and $x_{1{\mathrm{:}}}$ , the disturbance always propagates along the path which it traverses in the least time. We shall refer to such paths as the trajectories of the disturbance.  

Next, we state a physically plausible set of properties for the function $f(x,x^{\prime})$ :  

1 .  The propagation time along any curve is positive, and hence  

$$
f(x,x^{\prime})>0\quad{\mathrm{if}}\quad x^{\prime}\neq0.
$$  

2. The propagation time along any curve $\upgamma$ joining $x_{0}$ and $x_{1}$ > given by the integral (2), depends only on $\upgamma$ and not on how $\upgamma$ is parameterized. It follows by the argument given in Chap. 2, Sec. 10 that $f(x,x^{\prime})$ is positive-homogeneous of degree 1 in $x^{\prime}$ :  

$$
f(x,\lambda x^{\prime})=\lambda f(x,x^{\prime})\quad\mathrm{for~every}\quad\lambda>0.
$$  

In particular, (4) implies that  

$$
f(x,x^{\prime}+\bar{x}^{\prime})=f(x,x^{\prime})+f(x,\bar{x}^{\prime}),
$$  

if $\bar{x}^{\prime}=\lambda x^{\prime}$ , where $\lambda>0$ .  

3 . The time it takes a disturbance to traverse a curve $\upgamma$ connecting $x_{0}$ to $x_{1}$ is the same as the time it takes a disturbance to traverse $\upgamma$ in the opposite direction from $x_{1}$ to $x_{0}$ , and hence  

$$
f(x,-x^{\prime})=f(x,x^{\prime}).
$$  

4. If the medium is homogeneous, so that $f$ is a function of direction only, then the disturbance propagates in straight lines (see Prob. 1 ) . In particular, no disturbance emanating from a given point $x_{0}$ can arrive at another point $x_{1}$ more quickly by taking a path consisting of two straight line segments than by going along the straight line segment joining $x_{0}$ and $x_{1}$ ' This implies the convexity condition  

$$
f(x^{\prime}+\bar{x}^{\prime})\leqslant f(x^{\prime})+f(\bar{x}^{\prime})
$$  

(see Prob . 2). If $f$ depends on $x$ in a sufficiently smooth way (e.g. , if the derivatives $\partial f/\partial x^{1},...,\partial f/\partial x^{n}$ exist), the same argument sh ows that the convexity condition  

$$
f(x,x^{\prime}+\bar{x}^{\prime})\leqslant f(x,x^{\prime})+f(x,\bar{x}^{\prime})
$$  

holds for sufficiently small $x^{\prime},\bar{x}^{\prime}$ , but then (7) holds for all $x^{\prime},\bar{x}^{\prime}$ because of the homogeneity property (4).  

5. Actually, we strengthen the condition (7) somewhat, by requiring that $f$ satisfy the strict convexity condition, consisting of (7) plus the stipula­ tion that (5) holds only if $\bar{x}^{\prime}=\lambda x^{\prime}$ , where $\lambda>0$ .  

Now suppose we have a disturbance which at time $t=0$ occupies some region of excitation $R$ in $\mathcal{X}$ , and propagates further as time evolves. The boundary of $R$ will be called the wave front. Let  

$$
S(x,t)=0
$$  

be the equation of the wave front at the time $t.$ . Then our problem can be stated as follows : Find the equation satisfied by the function $\boldsymbol{S}(\boldsymbol{x},\ t)$ describing the wave front, and find the equations of the trajectories of the disturbance.  

2. Introduction of a norm in $\mathcal{T}(x)$ . Our next step is to use the function $f(x,x^{\prime})$ to introduce a norm in the $\pmb{n}$ -dimensional tangent space $\mathcal{T}(x)$ . This can be done by defining the norm of the vector $x^{\prime}=0$ to be zero and setting  

$$
\|{\boldsymbol{x}}^{\prime}\|=f({\boldsymbol{x}},{\boldsymbol{x}}^{\prime})
$$  

for all vectors $x^{\prime}\neq0$ in $\mathcal{T}(x)$ . The fact that $\|{\boldsymbol{x}}^{\prime}\|$ actually meets all the require­ ments for a norm (see p. 6) is an immediate consequence of (3), (4), (6) and (7). The set of all vectors in $\mathcal{T}(x)$ such that  

$$
f(x,x^{\prime})=\|x^{\prime}\|=\alpha
$$  

is called a sphere of radius $\alpha$ in $\mathcal{T}(x)$ , with center at the point $x$ . The sphere (9) is just the boundary of the closed region of $\mathcal{T}(x)$ [and hence of $\mathcal{X}]$ which is excited during the time $\alpha$ by a disturbance originally concentrated at the point $x$ . In this language, our problem can be rephrased as follows : Suppose a tangent space $\mathcal{T}(x)$ , equipped with the norm (8) satisfying the strict convexity condition, is defined at each point $x$ of an n-dimensional space $\mathcal{X}$ !C . Find the equations describing the propagation of disturbances in $\mathcal{X}$ !C, if during the time dt the disturbance originally at $x$ " spreads out and fills " the sphere  

$$
f(x,d x)=d t.
$$  

3. The conjugate space $\tilde{\mathcal{T}}(x)$ . Let $\varphi[{\boldsymbol{x}}^{\prime}]$ be a linear functional (see p. 8), defined on the tangent space $\mathcal{T}(x)$ . Then there is a unique vector  

$$
p=(p_{1},...,p_{n}),
$$  

such that  

$$
\varphi[x^{\prime}]=(p,x^{\prime})
$$  

for all $x^{\prime}\in\mathcal{T}(x)$ , where by $(p,x^{\prime})$ is meant the scalar product  

$$
\sum_{i=1}^{n}p_{i}x^{1\prime}+\cdots+p_{n}x^{n\prime}
$$  

(see Prob. 3).4 Conversely, any scalar product $(p,x^{\prime})$ obviously defines a linear functional on ${\mathcal{T}}(x).$ . The set of all linear functionals on ${\mathcal{T}}(x).$ , or equivalently the set of all vectors $p$ , is itself an $\pmb{n}$ -dimensional linear space, called the conjugate space of $\mathcal{T}(x)$ and denoted by $\tilde{\mathcal{T}}(x)$ . We define the norm of a vector $\pmb{p}\in\tilde{\mathcal{T}}(x)$ by the formulas  

$$
\|p\|=\operatorname*{sup}_{x^{\prime}}{\frac{(p,x^{\prime})}{\|x^{\prime}\|}},
$$  

where the least upper bound is taken over all vectors $x^{\prime}\neq0$ in $\mathcal{T}(x)$ [see Prob. 4]. In the present context, we write $H(x,p)$ instead of $\|p\|$ , i . e . ,  

$$
H(x,p)=\operatorname*{sup}_{x^{\prime}}{\frac{(p,x^{\prime})}{\|x^{\prime}\|}}.
$$  

It can be shown that the transition from the function $f(x,x^{\prime})$ to the function $H(x,p)$ defined by ( 1 1 ) is just the parametric form of the Legendre transfor­ mation discussed in Sec. 1 8.  

4. The propagation process. Suppose the wave front at the time $t$ is the surface ${\pmb{\sigma}}_{t}$ , with equation  

$$
S(x,t)=0.
$$  

We now examine in more detail the mechanism governing the evolution of ${\pmb{\sigma}}_{t}$ in time. By hypothesis, each point of ${\pmb{\sigma}}_{t}$ serves as a source of new distur­ bances, which during the time $d t$ excite the region bounded by the sphere  

$$
f(x,d x)=d t.
$$  

Since the function $f(x,x^{\prime})$ determining the propagation process is assumed to be differentiable and strictly convex (in the sense explained above), there is a unique hyperplane tangent to each point of the sphere ( 1 3), and this hyper­ plane has only one point in common with the sphere, i.e., its point of tangency. If we construct a family of spheres ( 1 3), one for each point $\boldsymbol{x}\in\sigma_{t}$ , then the wave front ${\pmb{\sigma}}_{t+d t}$ at the time $t+d t$ , with "equation  

$$
S(x,t+d t)=0,
$$  

is j ust the envelope $E$ of this family of spheres. I n fact, $E$ is the " interface " separating the points of $\mathcal{X}$ which can be reached from ${\upsigma}_{t}$ in times $\leqslant d t$ from the points which can only be reached from ${\upsigma}_{t}$ in times $>d t$ . This construction has two important implications :  

1 .  G iven a point $x\in\pmb{\sigma}_{t}$ . there is a unique point $x+d x\in\sigma_{t+d t}$ which is excited after the time $d t$ by a disturbance initially at $x$ . In fact, $x+d x$ is the point of ${\sigma}_{t+d t}$ lying on the (unique) hyperplane tangent to both ( 1 3) and ${\pmb{\sigma}}_{t+d t}$ . To see this, we observe that it takes a time $>d t$ for a disturbance starting from $x$ to reach any other point of $\upsigma_{t+d t}$ . 6 Thus, there is a unique direction of propagation defined at each point $\boldsymbol{x}\in\sigma_{t}$ > and it is clear that a disturbance leaving $x$ in this direction will arrive at the surface ${\pmb{\sigma}}_{t+d t}$ more quickly than a disturbance leaving $x$ in any other direction, as required by Fermat's principle.  

2. Conversely, given a point $x+d x\in\sigma_{t+d t}$ , there is a unique point $\boldsymbol{x}\in\sigma_{t}$ , which at the time $t$ was the source of the disturbance reaching $x+d x$ at the time $t+d t$ . I n fact, $x$ is just the center of the (unique) sphere of radius dt which shares a tangent hyperplane with ${\pmb{\sigma}}_{t+d t}$ .  

5. The Hamilton-Jacobi equation. As was j ust shown, every hyperplane tangent to the surface ${\upsigma}_{t+d t}$ with equation ( 1 4) must also be tangent to some sphere of radius $d t$ whose center lies on the surface ${\upsigma}_{t}$ with eq uation ( 1 2) . This fact can b e used t o derive a differential equation satisfied b y the function $\boldsymbol{S}(\boldsymbol{x},t)$ . First, we observe that every hyperplane in the tangent space $\mathcal{T}(\boldsymbol{x})$ can be written in the form  

$$
\sum_{i=1}^{n}p_{i}x^{i\prime}=\mathrm{const},
$$  

where $p=(p_{1},...,p_{n})$ is a vector in the conjugate space $\tilde{\mathcal{T}}(x)$ . Let $x+d x$ be an arbitrary point of $\sigma_{t+d t}$ whose " source " is the point $x\in\upsigma_{t}$ . Then the hyperplane in $\mathcal{T}(x)$ tangent to $\sigma_{t+d t}$ at $x+d x$ has the equation  

$$
\sum_{i=1}^{n}{\frac{\partial S}{\partial x^{i}}}d x^{i}=c,
$$  

where $c$ is a constant. If the hyperplane ( \ 5) is also tangent to the sphere ( 1 3) , as required, then $c$ equals the norm of the vector  

$$
\nabla S={\bigg(}{\frac{\partial S}{\partial x^{1}}},\ldots,{\frac{\partial S}{\partial x^{n}}}{\bigg)},
$$  

multiplied by the radius of the sphere, i . e . ,  

$$
c=H(x,\nabla S)d t.
$$  

Therefore, ( 1 5) becomes  

$$
\sum_{i=1}^{n}{\frac{\partial S}{\partial x^{i}}}d x^{i}=H(x,\nabla S)d t.
$$  

But  

$$
\sum_{i=1}^{n}{\frac{\partial S}{\partial x^{i}}}d x^{4}+{\frac{\partial S}{\partial t}}d t=0,
$$  

because of the meaning of $x$ and $x+d x$ . Comparing ( 1 6) and ( 1 7), we finally obtain  

$$
\frac{\partial S}{\partial t}+H(x,\nabla S)=0.
$$  

This equation describes the way the wave front evolves in time, and is just the familiar Hamilton-Jacobi equation, already considered in Sec. 23.  

We now show the relation between the trajectories of the disturbance and the general solution of ( 1 8). It will be recalled that as a wave front evolves in time, each of its points goes into a succession of uniquely defined points lying on neighboring wave fronts, thereby " sweeping out " a trajectory $\upgamma$ which automatically minimizes the functional (2). Thus, if we specify a one-parameter family of wave fronts  

$$
S(x,t)=0,
$$  

where the parameter is the time $t_{i}$ , every point $x_{0}$ on some " initial " surface $S(x,t_{0})$ generates a trajectory. Choosing the point $\scriptstyle x_{0}$ arbitrarily, we find that the one-parameter family of surfaces ( 1 9) determines an $(n\mathrm{~-~}1)\cdot$ parameter family of trajectories, such that one and only one trajectory of the family passes through each point $\boldsymbol{x}\in\mathcal{X}$ . More generally, let  

$$
S(x,t,\alpha_{1},...,\alpha_{n})
$$  

be a complete integral of the Hamilton-Jacobi equation depending on $\pmb{n}$ parameters $\alpha_{1},...,\alpha_{n}$ . This complete integral determines an $(n+1)$ ­ parameter family of surfaces7  

$$
S(x,t,\alpha_{1},...,\alpha_{n})=0,
$$  

which in turn determines a $(2n-1)$ -parameter family of trajectories. Then the fact that the trajectories of the disturbances are the extremals of the functional (2) leads to a geometric interpretation of Jacobi's theorem (p. 9 1 ), concerning the construction of a general solution of the system of Euler equations of a functional from a complete integral of the corresponding Hamilton-Jacobi equation.8  

6. The canonical equations. To derive the differential equations satisfied by the trajectories of the disturbance, we might use Fermat's principle, minimizing the functional (2) and solving the corresponding Euler equations. However, we prefer to use our geometric model of the propagation process. If we introduce the time $t$ as the parameter along each trajectory, it follows from  

$$
f(x,d x)=d t
$$  

and the homogeneity of $f(x,d x)$ in the argument $d x$ that  

$$
f{\biggl(}x,{\frac{d x}{d t}}{\biggr)}=1,
$$  

i.e., the norm of the vector $d x/d t$ is identically equal to 1 .  Using ( 1 6) , we find that at each point $x_{i}$ , the vector $d x/d t$ (tangent to the trajectory along which the disturbance propagates) is related to the covariant vector $p$ (determining the hyperplane tangent to the wave front) by the formula  

$$
\sum_{i=1}^{n}p_{i}{\frac{d x^{i}}{d t}}=H(x,p).
$$  

According to (2 1 ) and the definition ( 1 1 ) of the norm of vectors in $\tilde{\mathcal{T}}(x)$ , we see that  

$$
\sum_{i=1}^{n}\frac{d x^{i}}{d t}\leqslant H(x,p)\ 
$$  

if $p$ is any other vector in $\tilde{\mathcal{T}}(x)$ . Thus, the expression  

$$
\sum_{i=1}^{n}{\frac{d x^{i}}{d t}}-H(x,p),
$$  

regarded as a function of $p_{:}$ , achieves its maximum when $p$ is the vector determining the hyperplane tangent to the wave front. Therefore, along the trajectories, the conditions  

$$
\frac{\partial}{\partial p_{\mathrm{i}}}\left[\sum_{i=1}^{n}p_{i}\frac{d x^{i}}{d t}-H(x,p)\right]=0\qquad(i=1,...,n)
$$  

must hold , i . e . ,  

$$
\frac{d x^{i}}{d t}=\frac{\partial H(x,p)}{\partial p_{i}}\qquad(i=1,...,n).
$$  

We have just obtained a system of $n$ ordinary differential equations of the first order satisfied by the trajectories. Since these equations involve $2n$ unknown functions $x^{1},\ldots,x^{n}$ and $p_{1},...,p_{n}.$ , we still need $n$ m ore equations to completely describe the trajectories. To find the missing equations, we use the fact that the surfaces representing the wave fronts at different times are not arbitrary, but satisfy the Hamilton-Jacobi equation ( 1 8), while the values $p_{i}$ at each point of a trajectory are the components $\partial S/\partial x^{i}$ determining the hyperplane tangent to the wave front. In other words,  

$$
p_{\imath}=p_{\imath}(t)=\frac{\partial}{\partial x^{i}}S[x^{1}(t),...,x^{n}(t),t]
$$  

along each trajectory, and hence  

$$
{\frac{d p_{i}}{d t}}={\frac{d}{d t}}{\frac{\partial S}{\partial x^{i}}}={\frac{\partial}{\partial t}}{\frac{\partial S}{\partial x^{i}}}+\sum_{k=1}^{n}{\frac{\partial^{2}S}{\partial x^{k}\partial x^{i}}}{\frac{d x^{k}}{d t}}.
$$  

We now introduce the following notation : If the function $H(x,p)$ , where $p_{\mathrm{{i}}}=\partial S/\partial x_{\mathrm{{i}}},$ > is regarded as a function of $x^{1},...,x^{n}$ and $t$ , we indicate its partial derivative with respect to $x^{i}$ by  

$$
\left.\frac{\partial H}{\partial x^{i}}\right|_{t=\mathrm{const}},
$$  

whereas if $H(x,p)$ is regarded as a function of the $2n$ variables $x^{1},...,x^{n}$ and $p_{1},...,p_{n},$ , we indicate its partial derivative with respect to $x^{i}$ by  

$$
\left.{\frac{\partial H}{\partial x^{i}}}\right|_{p=\mathrm{const}}.
$$  

Then, using the Hamilton-Jacobi equation ( 1 8), we can write (23) in the form  

$$
{\frac{d p_{i}}{d t}}=\left.-{\frac{\partial H}{\partial x^{i}}}\right|_{t=\mathrm{const}}+\sum_{k=1}^{n}{\frac{\partial^{2}S}{\partial x^{k}\ \partial x^{i}}}{\frac{d x^{k}}{d t}}.
$$  

Along the trajectories, we have  

$$
\left.{\frac{\partial H}{\partial x^{i}}}\right|_{t=\mathrm{const}}=\left.{\frac{\partial H}{\partial x^{i}}}\right|_{p=\mathrm{const}}+\sum_{k=1}^{n}{\frac{\partial H}{\partial p_{k}}}\right|_{x=\mathrm{const}}{\frac{\partial p_{k}}{\partial x^{i}}},
$$  

and  

$$
p_{k}={\frac{\partial S}{\partial x^{k}}},\qquad{\frac{d x^{k}}{d t}}={\frac{\partial H}{\partial p_{k}}}.
$$  

Substituting (25) and (26) into (24) , we obtain $\pmb{n}$ differential equations  

$$
\frac{d p_{i}}{d t}=\left.-\frac{\partial H}{\partial x^{i}}\right|_{p=\mathrm{const}}\qquad(i=1,...,n).
$$  

Combining these equations with (22), we obtain a system of $2n$ differential equations  

$$
\begin{array}{l}{\displaystyle\frac{d x^{i}}{d t}=\frac{\partial H(x,p)}{\partial p_{i}},}\\ {\displaystyle\frac{d p_{i}}{d t}=-\frac{\partial H(x,p)}{\partial x^{i}},}\end{array}
$$  

where $i=1,\ldots,n.$ . The integral curves of (27) are the trajectories along which the disturbance propagates, i.e., the extremals of the functional (2).  

The system (27) is of course the canonical system of Euler equations for the variational problem associated with (2) [cf. Sec. 1 6] , and represents the so­ called characteristic system associated with the Hamilton-Jacobi equation ( 1 8) [cf. p. 90].  

# PROBLEMS  

1 .  Prove that i f $f(x,x^{\prime})$ depends o n direction only, then the disturbance propagates through the medium along straight lines.  

2. Prove that if $f(x,x^{\prime})\equiv f(x^{\prime})$ is independent of $x$ , then $f(x^{\prime})$ is precisely the time required to traverse the vector $x^{\prime}$ .  

3. Prove that every linear functional $\varphi[x]$ defined on an $_n$ -dimensional Euclidean space of points $x=(x^{1},...,x^{n})$ is of the form  

$$
\varphi[x]=p_{1}x^{1}+\cdot\cdot\cdot+p_{n}x^{n},
$$  

where $p=(p_{1},....,p_{n})$ is uniquely determined by $\varphi$ o  

4. Verify that formula ( 1 0) actually defines a norm for the elements $p$ of the conjugate space $\tilde{\mathcal{T}}(x)$ .  

5. Why is the strict convexity condition (p. 2 1 1 )  needed in constructing wave fronts for the disturba nce ?  

# Appendix II  

In this appendix, w e sketch some results obtained by L . S. Pontryagin and his students, in their i nvestigations of the theory of optimal control processes.  The connection between this subject and classical variational theory wiII also be discussed .  

1 . Statement of the problem. I n many cases, finding the optimal " operating regime " for a physical system (with a suitable optimality criterion) leads to the following mathematical problem : Suppose the state of the physical system is characterized by $\pmb{n}$ real n u mbers $x^{1},\ldots,x^{n}$ , form ing a vector $x=(x^{1},\ldots,x^{n})$ in the $n$ -dimensional " phase space " $\mathcal{X}$ of the system , and suppose the state varies with time i n the way described by the system of differential equations  

$$
\frac{d x^{i}}{d t}=f^{i}(x^{1},...,x^{n},u^{1},...,u^{k})\qquad(i=1,...,n).
$$  

H ere, the $k$ real numbers $u^{1},\ldots,u^{k}$ form a vector $\pmb{u}=(u^{1},\ldots..,u^{k})$ belonging to some fixed " control region " $\Omega$ , which we take to be a subset of  

$k$ -dimensional Euclidean space, and the $f^{i}(x,u)$ are $n$ continuous functions defined for all $\boldsymbol{x}\in\mathcal{X}$ and all $\pmb{u}\in\Omega$ .  

Now suppose we specify a vector function $u(t)$ , $t_{0}\leqslant t\leqslant t_{1}$ , called the control function, with values in $\Omega$ . Then, substituting $u=u(t)$ in ( I ), we obtain the system of differential equations  

$$
\frac{d x^{i}}{d t}=f^{i}[x^{1},...,x^{n},u^{1}(t),...,u^{k}(t)]\qquad(i=1,...,n).
$$  

For every initial value $x_{0}=x(t_{0})$ , this system has a definite solution, called a trajectory. The aggregate  

$$
U=\{u(t),t_{0},t_{1},x_{0}\},
$$  

consisting of a control function $u(t)$ , an interval $[t_{0},t_{1}]$ and an i nitial value $x_{0}=x(t_{0})$ , will be called a control process. Thus, to every control process, there corresponds a trajectory, i . e . , a solution of (2).  

Next, let  

$$
f^{0}(x^{1},...,x^{n},u^{1},...,u^{k})
$$  

be a function which is defined, together with its partial derivatives  

$$
\frac{\partial f^{0}}{\partial x^{i}}\qquad(i=1,...,n),
$$  

for all $x\in\mathcal{X}$ and $u\in\Omega$ . To every control process $U$ , we assign the number  

$$
J[U]=\int_{t_{0}}^{t_{1}}f^{0}(x,u)d t,
$$  

i . e . , $J[U]$ is a functional defined on the set of control processes. Then , the control process (3) is said to be optimal if the inequality  

$$
J[U]\leqslant J[U^{*}]
$$  

holds for any other control process $U^{*}$ carrying the given point $x_{0}$ into the point $x_{1}$ , i.e., such that the corresponding trajectory $x^{*}(t)$ satisfies the con­ dition $x^{*}(t_{1}^{*})=x_{1}$ . By the optimal trajectory, we mean the trajectory corresponding to the optimal control process. Our aim is to find necessary conditions characterizing optimal control processes and optimal trajectories.  

It should be pointed out that in call ing a control process optimal, it is assumed that some class of admissible control processes has been specified in advance. Here, we assume that the components $u^{1}(t),...,u^{k}(t)$ of any adm issible control process take values in $\Omega$ , and are bounded and piecewise continuous (with left-hand and right-hand limits at every point of dis­ continuity).  

An important special case of the problem of optimal control is the situation where the functional (4) reduces to the integral  

$$
\int_{t_{0}}^{t_{1}}d t,
$$  

representing the time it takes to go from the point $x_{0}$ to the point $x_{1}$ ' In this case, optimality means taking the least time to go from $x_{0}$ to $x_{1}$ '  

2. Relation to the calculus of variations. The problem of optimal control is intimately related to certain traditional problems of the calculus of variations. In fact, the integral  

$$
\int_{t_{0}}^{t_{1}}f^{0}(x,u)d t
$$  

can be regarded as a functional depending on $n+k$ functions $x^{1},...,x^{n}$ , $u^{1},...,u^{k}$ , i.e., as a functional defined on some class of curves in $n+k+1$ dimensions. Since the functions $x^{1},\ldots,x^{n},u^{1},\ldots,u^{k}$ are connected by the equations ( I ), we are dealing with the problem of finding a minimum subject to nonholonomic constraints (see p. 48). Since the boundary conditions are equivalent to the req uirement that the desired opti mal trajectory $x(t)$ begin at the point $x_{0}$ and end at the point $x_{1}$ the end points of the admissible curves in our $(n+k+1)$ -dimensional space have to lie on two $(k+1)$ -dimensional hyperplanes, determined by giving the coordinates $x^{1},\ldots,x^{n}$ the fixed values $x_{0}^{1},...,x_{0}^{n}$ and $x_{1}^{1},...,x_{1}^{n}$ ·  

Thus, we see that the problem of optimal control is a variant of the problem of finding a minimum subject to subsidiary conditions. The problem of optimal control has the special feature that we specify in advance a definite class of admissible control processes, where the functions $u^{1}(t),\ldots,u^{k}(t)$ are required to take values in a given fixed region n, but in general are not required to be continuous.  

We can easily show that the simplest $n$ -dimensional variational problem, where the integrand does not depend on $t$ explicitly, 2 is a special case of the problem of optimal control. To this end, suppose that among the curves passing through two fixed points  

$$
(x_{0}^{1},...,x_{0}^{n}),\qquad(x_{1}^{1}....,x_{1}^{n}),
$$  

it is required to find the curve for which the functional  

$$
\int_{t_{0}}^{t_{1}}f^{0}\bigg(x^{1},...,x^{n},\frac{d x^{1}}{d t},...,\frac{d x^{n}}{d t}\bigg)d t
$$  

has a minImum. To paraphrase this problem as a problem of optimal control, we need only write (5) in the form  

$$
\int_{t_{0}}^{t_{1}}f^{0}(x^{1},\ldots,x^{n},u^{1},\ldots,u^{k})d t,
$$  

and take the system ( 1 )  to be simply  

$$
\frac{d x^{i}}{d t}=u^{i}\qquad(i=1,...,n).
$$  

3. Necessary conditions for optimality. To find necessary conditions for a given control process and the corresponding trajectory to be optimal, we supplement the system of equations  

$$
{\frac{d x^{i}}{d t}}=f^{i}(x,u)\qquad(i=1,...,n)
$$  

with the extra equation  

$$
\frac{d x^{0}}{d t}=f^{0}(x,u),
$$  

where $f^{\circ}(x,u)$ is the integrand of the functional (4) which is to be minimized. At the same time, we supplement the initial conditions  

$$
x^{i}(t_{0})=x_{0}^{i}\qquad(i=1,...,n)
$$  

with the extra condition  

$$
x^{0}(t_{0})=0.
$$  

For convenience, we introd uce the $(n+1)$ -dimensional vector function  

$$
\mathbf{x}(t)=(x^{0}(t),x(t))=(x^{0}(t),x^{1}(t),...,x^{n}(t)).
$$  

It is clear that i f $U$ is an admissible co ntrol process and if ${\mathbf x}={\mathbf x}(t)$ is the solution of the system 3  

$$
\frac{d x^{\mathrm{i}}}{d t}=f^{i}(x,u)\qquad(i=0,1,...,n),
$$  

corresponding to $U$ and the initial conditions (6) and (7), then  

$$
J[U]=\int_{t_{0}}^{t_{1}}f^{0}(x,u)d t=x^{0}(t_{1}).
$$  

Thus, the problem of optimal control can be stated as follows : Find the admissible control process $U$ for which the solution ${\bf x}(t)$ of the system (8), sati sfying the initial conditions (6) and (7), h a s the smallest possible value of $x^{0}(t_{1})$ '  

Next, in addition to the variables $x^{0},x^{1},\ldots,x^{n}$ , we introduce new variables $\psi_{0},\updownarrow_{1},....,\uppsi_{n}$ satisfying the following system of differential equations, known as the conjugate4 of the system (8) :  

$$
{\frac{d\Psi_{i}}{d t}}=\mathrm{~-~}\sum_{\alpha=0}^{n}{\frac{\partial f^{\alpha}(x,u)}{\partial x^{i}}}\Psi_{\alpha}(i=0,1,...,n).
$$  

$$
\sum_{\alpha=0}^{n}\Psi_{\alpha}^{0}x_{\alpha}=c=\mathrm{const}
$$  

Let  

$$
\Psi(t)=(\Psi_{0}(t),\Psi_{1}(t),\ldots,\Psi_{n}(t)),
$$  

and consider the following function of the variables $x^{1},...,x^{n},\psi_{0},\psi_{1},...,\psi_{n},$ $u_{1},...,u_{k}$ :  

$$
\Pi(\Psi,x,u)=\sum_{\alpha=0}^{n}\Psi_{\alpha}f^{\alpha}(x,u).
$$  

I n terms o f $\Pi$ , we can write the equations (8) and (9) i n the form  

$$
\begin{array}{l}{\displaystyle\frac{d x^{i}}{d t}=\frac{\partial\Pi}{\partial{\dot{\psi}}_{i}},}\\ {\displaystyle\frac{d\Psi_{i}}{d t}=-\frac{\partial\Pi}{\partial{x^{i}}},}\end{array}
$$  

where $i=0,1,...,n.$ The equations ( 1 1 )  remind us of the canonical system of Euler equations [see formula ( 1 1 ), p. 70] . However, they have a different meaning, since the canonical equations form a closed system, in which the number of equations equals the number of unknown functions, whereas ( 1 1 ) involves not only $\mathbf{x}$ and $\boldsymbol{\Psi}$ but also the unknown function $\pmb{u}$ , and hence ( 1 0) beӟomes a closed system only. when $\pmb{u}$ is specified . In fact, in order to write equations for the optimal control problem resembling the canonical equations, we would have to use the function  

$$
{\mathcal{H}}(\Psi,x)=\operatorname*{sup}_{u\in\Omega}\Pi(\Psi,x,u),
$$  

instead of the function $\Pi(\Psi,x,u)$ . 5  

4. The maximum principle. We can now state the following theorem, whose proof can be found in the references cited on p. 2 1 8 :  

THEOREM (The maximum principle). Let $U=\{u(t),t_{0},t_{1},x_{0}\}$ be an admissible control process, and let ${\bf x}(t)$ be the corresponding integral curve of the system (8) passing through the point $(0,x_{0}^{1},...,x_{0}^{n})$ for $t=0$ , and satisfying the conditions  

$$
x^{1}(t_{1})=x_{1}^{1},...,x^{n}(t_{1})=x_{1}^{n}
$$  

for $t=t_{1}$ . Then if the control process $U$ is optimal, there exists a con­ tinuous vector function $\Psi(t)=(\Psi_{0}(t),\Psi_{1}(t),\ldots,\Psi_{n}(t))$ such that  

1 .  The function $\boldsymbol{\Psi}(t)$ satisfies the system (9) for $x=x(t)$ , $u=u(t)$ ;  

2. For all $t$ in $[t_{0},t_{1}]$ , the function ( t o) achieves its maximum for $u=u(t)$ , i. e . ,  

$$
\Pi[\Psi(t),x(t),u(t)]=\mathcal{H}[\Psi(t),x(t)],
$$  

where the function $\mathcal{H}$ is defined by ( 1 2) ;  

# 3. The relations  

$$
\begin{array}{r}{\Psi_{0}(t_{1})\leqslant0,\mathcal{H}[\Psi(t_{1}),u(t_{1})]=0}\end{array}
$$  

hold at the time $t_{1}$ . A ctually, $i f\Psi(t),\mathbf{x}(t)$ and $u(t)$ satisfy the system (8), (9) and the condition ( 1 3), the functions $\psi_{0}(t)$ and $\mathcal{H}[\Psi(t),x(t)]$ turn out to be constants, and hence $i n$ ( 1 4) we can replace $t_{1}$ by any value of $t$ in $[t_{0},t_{1}]$ '  

Remark 1 .  The maximum principle can often be used as a prescription for constructing the optimal trajectory, in the following way : For every fixed $\boldsymbol{\Psi}$ and $x$ , we find the value of $\pmb{u}$ for which the expression  

$$
\sum_{\alpha=0}^{n}\psi_{\alpha}f^{\alpha}(x,u)
$$  

takes its maximum. If this determines $\pmb{u}$ as a single-valued function  

$$
u=u(\Psi,x)
$$  

of $\boldsymbol{\Psi}$ and $x$ , then, substituting ( 1 5) into the equations (8) and (9), we obtain a closed system of $2(n+1)$ equations involving $2(n+1)$ unknown functions. These are j ust the equations which have to be satisfied by the optimal trajectory.  

Remark 2. For the simple $\pmb{n}$ -dimensional variational problem discussed on p . 220, the system (8), (9) , or the equivalent system ( I I ), together with the maximum principle, reduces to the usual system of Euler equations. To see this, consider the functional  

$$
\int_{t_{0}}^{t_{1}}f^{0}(x^{1},...,x^{n},u^{1},...,u^{n})d t
$$  

[cf. (5)], where  

$$
u^{i}=\frac{d x^{i}}{d t}\qquad(i=1,...,n).
$$  

In this case, the function ( 1 0) is  

$$
\Pi(\Psi,x,u)=\Psi_{0}f^{0}(x,u)+\sum_{\alpha=1}^{n}\Psi_{\alpha}u^{\alpha},
$$  

and the system ( 1 1 ) becomes  

$$
\begin{array}{l l}{{\displaystyle{\frac{d x^{0}}{d t}}=f^{0}(x,u),\quad}}&{{\displaystyle{\frac{d x^{i}}{d t}}=u^{i},}}\\ {{\displaystyle{\frac{d\psi_{0}}{d t}}=0,\quad}}&{{\displaystyle{\frac{d\psi_{i}}{d t}}=\mathrm{-}\psi_{0}\displaystyle{\frac{\partial f^{0}(x,u)}{\partial x^{i}}},}}\end{array}
$$  

where $i=1,...,n$ . Maximizing $\Pi(\Psi,x,u)$ , we find that  

$$
\frac{\partial\Pi}{\partial u^{i}}=\Psi_{0}\frac{\partial f^{0}(x,u)}{\partial u^{i}}+\Psi_{i}=0,
$$  

i . e . ,  

$$
\begin{array}{l}{\displaystyle{\Psi_{i}=-\psi_{0}\frac{\partial f^{0}(x,u)}{\partial u^{i}}}\quad}\end{array}\quad(i=1,...,n).
$$  

Since $d\Psi_{0}/d t=0$ , we have $\uppsi_{0}=$ const, and hence  

$$
\begin{array}{c}{{{\displaystyle{\frac{d}{d t}\left[\frac{\partial f^{0}(x,u)}{\partial u^{i}}\right]=\frac{\partial f^{0}(x,u)}{\partial x^{i}}},}}}\\ {{{\displaystyle{\frac{d x^{i}}{d t}=u^{i}}.}}}\end{array}
$$  

This is just the system of Euler equations corresponding to the functional ( 1 6), reduced to a system of fi rst-order differential eq uations by introducing the derivatives $d x^{i}/d t=u^{i}$ as new functions (cf. p. 68).  

Remark 3. I n Appendix I, we have already encountered the fact that every propagation process can be described in two ways, either in terms of the trajectories along which the disturbance propagates (the " rays " in optics), or in terms of the motion of the wave front. The first approach leads to the canonical Euler eq uations (or, as in the example j ust considered, to the usual form of the Euler eq uations), i.e., a system of ordinary differential equations. The second approach leads to the Hamilton-Jacobi equation, i.e., a partial differential eq uation. Our maxim u m principle involves the study of trajectories, and in this sense is analogous to the method of canonical equations. The " wave front approach " to problems of optimal control has been developed by R. Bellman . 6  

5 . Relation t o Weierstrass' necessary condition. W e again consider the simple fu nctional ( 1 6), ( 1 7), where the fu nction $\Pi(\Psi,x,u)$ is given by ( 1 8). U sing ( 1 7), we can also write the functional ( 1 6) i n the form  

$$
\int_{t_{0}}^{t_{1}}f^{0}(x^{1},...,x^{n},x^{1\prime},...,x^{n\prime})d t.
$$  

The Weierstrass $E$ -function for such a functional is7  

$$
E(x,x^{\prime},z)=f^{0}(x,z)-f^{0}(x,x^{\prime})-\sum_{i=1}^{n}{(z-x_{i}^{\prime})}f_{x^{\prime}}^{0}(x,x^{\prime}).
$$  

Using ( 1 8) and (20), we find that  

$$
\begin{array}{l}{{\Pi(\Psi,x,z)-\Pi(\Psi,x,x^{\prime})-\displaystyle\sum_{i=1}^{n}\left(z_{i}-x^{i\prime}\right)\frac\partial{\partial u^{i}}\Pi(\Psi,x,x^{\prime})}}\\ {{\mathrm{}=\displaystyle\Psi_{0}f^{0}(x,z)-\Psi_{0}f^{0}(x,x^{\prime})+\displaystyle\sum_{i=1}^{n}\Psi_{i}(z_{i}-x^{i\prime})-\displaystyle\sum_{i=1}^{n}\left(z_{i}-x^{i\prime}\right)(\Psi_{0}f_{x^{\prime}}^{0}+\Psi_{0}f^{0}(x^{\prime}))}}\\ {{\mathrm{}=\displaystyle\Psi_{0}f^{0}(x,z)-\Psi_{0}f^{0}(x,x^{\prime})-\displaystyle\sum_{i=1}^{n}\left(z_{i}-x^{i\prime}\right)\Psi_{0}f_{x^{\prime}}^{0}=\displaystyle\Psi_{0}E(x,x^{\prime},z).\quad(2)}}\end{array}
$$  

I f the function $\Pi$ achieves its maximum for values of $u=x^{\prime}$ which are interior points of the region $\Omega,$ , then  

$$
{\frac{\partial\Pi}{\partial u^{i}}}=0
$$  

at these points. Then, since $\Psi_{0}\leqslant0$ , it fol l ows from (2 1 )  that the condition ( 1 3) is eq uivale nt to the condition  

$$
E(x,x^{\prime},z)\geqslant0.
$$  

This is Weierstrass' necessary condition, with which we are already familiar (see p. 1 49). Thus, the maximum principle leads to another, independent derivation of (22). It can be shown that the formula  

$$
\Psi_{0}E=\Pi(\Psi,x,z)-\Pi(\Psi,x,x^{\prime})-\sum_{i=1}^{n}\left(z_{i}-x^{i\prime}\right)\frac{\partial}{\partial u^{i}}\Pi(\Psi,x,x^{\prime})
$$  

remains true for variational problems subject to constraints, i . e . , for more general problems of optimal control.  

We have just proved the equivalence of the maxim um principle and Weierstrass' necessary condition (22) in the case where the set $\Omega$ of admissible values of the control function $u(t)$ is open, i.e., where every point of $\Omega$ is a n interior point. I n the case where the opti mal control process involves values of $u(t)$ lying on the boundary of the region $\Omega$ , the condition (22) is in general no longer valid. H owever, it can be shown that in such cases, the maximum principle continues to apply.  

# PROBLEMS  

1 . State the maximum principle ( p . 222) for the problem o f "fastest motion" or "time optimal problem," where the functional (4) reduces to simply  

$$
J[U]=\int_{t_{0}}^{t_{1}}d t.
$$  

A ns. I n this case, we write  

$$
P(\Psi,x,u)=\sum_{\alpha=1}^{n}\Psi_{\alpha}f^{\alpha}(x,u)
$$  

i nstead of ( 1 0) , a n d i n  the system ( I I ) , $i$ need only range from 1 to $\pmb{n}$ .  The function $\mathcal{H}$ in the maximum principle is now replaced by  

$$
H(\Psi,x)=\operatorname*{sup}_{u\in\Omega}P(\Psi,x,u)=\mathcal{H}(\Psi,x)-\Psi_{0}.
$$  

Finally, the relations ( 1 4) are replaced by  

$$
H[\uppsi(t_{1}),x(t_{1})]=-\uppsi_{0}\geqslant0,
$$  

which actually holds for any $t$ i n $[t_{0},t_{1}]$ .  

2. Consider the differential equation  

$$
{\frac{d^{2}x}{d t^{2}}}=u,
$$  

where the control function $\pmb{u}$ obeys the condition $|u|\leqslant1$ .  Introducing the "phase coordinates " $x^{1}$ and $x^{2}$ , we can write (a) as a system  

$$
{\frac{d x^{1}}{d t}}=x^{2},\qquad{\frac{d x^{2}}{d t}}=u.
$$  

What trajectory corresponds to the fastest motion from a given i n itial point $\scriptstyle x_{0}$ to the final point $\pmb{x}_{1}=(\mathbf{0},\mathbf{0})\}$  

Hint. The auxiliary variables $\uppsi_{1}$ and $\phi_{2}$ obey the equations  

$$
\frac{d\Psi_{1}}{d t}=0,\frac{d\Psi_{2}}{d t}=-\Psi_{1}.
$$  

By the maximum principle (modified in accordance with Prob. 1 ),  

$$
u(t)=\mathsf{s g n}\ \Psi_{2}(t)=\mathsf{s g n}\ (c_{2}\mathrm{~-~}c_{1}t),
$$  

where $\pmb{c}_{1}$ and $c_{2}$ are constants, sgn $x\equiv x/|x|$ and $u(t)$ can only change sign once. Integrate the system (b) for $u=\pm1$ ,  and draw the corresponding fa mil ies of parabolas i n the $(x^{1},x^{2})$ plane, analyzing the various possibilities (corresponding to different in itial positions $\scriptstyle x_{0}$ ) .  

3. Study the same "time-optimal problem " for the equation  

$$
{\frac{d^{2}x}{d t^{2}}}+x=u,\qquad|u|\leqslant1.
$$  

Hint. The appropriate system is now  

$$
\frac{d x^{1}}{d t}=x^{2},\frac{d x^{2}}{d t}=-x^{1}+u.
$$  

4. Study the same "ti me-optimal problem " for the system  

$$
\frac{d x^{1}}{d t}=x^{2}+u^{1},\frac{d x^{2}}{d t}=-x^{1}+u^{2},
$$  

where there are two control functions $u^{1},u^{2}$ obeying the conditions $\left|u^{1}\right|\leqslant1$ , $\left|u^{2}\right|\leqslant1$ .  

Comment. For a detailed discuss ion of Probs. 2 -4, see Chap. 1 ,  Sec 5 of the book cited on $\mathsf{p}.\ 218$ .  

5. Verify the relations ( 1 4) for the si mple variational problem ( 1 6) discussed i n Remark 2, p. 223.  

Hint. Use Euler's theorem on positive-homogeneous functions (Chap. 2, Prob. 6).  

Akhiezer, N. I . , The Calculus of Variations, translated by A. H. Frink, Blaisdell Publishing Co., New York ( 1 962).   
Bellman, R., Dynamic Programming, Princeton University Press, Princeton, N. J . ( 1 957).   
Bellman, R., Adaptive Control Processes: A Guided Tour, Princeton University Press, Princeton, N. J. ( 1 96 1 ) .   
Bellman, R. and S. E. Dreyfus, Applied Dynamic Programming, Princeton University Press, Princeton, N. J. ( 1 962).   
Bliss, G. A., Calculus of Variations, Open Court Publishing Co. , Chicago ( 1 925).   
Bliss, G . A., Lectures on the Calculus 0/ Variations, University of Chicago Press, Chicago (1 946).   
Bolza, 0., Lectures on the Calculus 0/ Variations, reprinted by G. E. Stechert and Co. , New York ( 1 9 3 1 ).   
Courant, R. and D. Hilbert, Methods ofMathematical Physics, Vol. I, Interscience Publishers, Inc. , New York ( 1 95 3), Chaps. 4 and 6.   
Elsgolc, L. E., Calculus of Variations, translated from the Russian, Addison­ Wesley Publishing Co., Reading, Mass. (1 962).   
Forsyth, A. R., Calculus of Variations, reprinted by Dover Publications, Inc., New York ( 1 960).   
Fox, c., An Introduction to the Calculus of Variations, Oxford University Press, New York (1 950).   
Gould, S. H., Variational Methods for Eigenvalue Problems, University of Toronto Press, Toronto ( 1 957).   
Lanczos, c., The Variational Principles of Mechanics, University of Toronto Press, Toronto ( 1 949).   
Morrey, C. B. Jr., Multiple Integral Problems in the Calculus of Variations and Related Topics, University of California Press, Berkeley and Los Angeles ( 1 943).   
Morse, M., The Calculus of Variations in the Large, American Mathematical Society, Providence, R. I. ( 1 934).   
Murnaghan, F. D., The Calculus of Variations, Spartan Books, Washington, D.C. ( 1 962).   
Pars, L. A., Calculus of Variations, John Wiley and Sons, Inc., New York ( 1 963).   
Weinstock, R., Calculus of Variations, with Applications to Physics and Engi­ neering, McGraw-Hili Book Co., Inc., New York ( 1 952).  

# A  

Action ( functional ) ,  84, 1 5 4   
for physical fields, 1 80   
Admissible curves, 8   
Admissible functions, 8   
Angular momentum, 87   
Angular momentum tensor, 1 85 , 1 86   
Apostol, T. M . , 1 3 9 , 1 9 9   
Approximation in the mean, 207   
Arc length , 7, 8, 1 9 , 39   
Arzeill's theorem, 20 1  

# B  

Backward sweep, 1 3 6   
Baker, B. B., 209   
Bellman, R., 224   
Benster, C . D., 205   
Berezin, I. S., 1 3 6   
BernouJli, J ames, 3   
Bernoulli, John, 3   
Bernstein, S. N . , 1 6   
Bernstein's theorem, 1 6, 3 3   
Bessel-Hagen, E . ,  1 8 9   
Bilinear form, 9 8   
Boltyanski, V. G . , 2 1 8   
Brachistochrone, 3 ,  1 4, 1 6 , 2 6   
Broken extremal, 21, 62  

Cartesian product, 1 64   
Castigli ano's principle, 1 68   
Catenary, 2 1   
Catenoid, 2 1   
Cauchy sequence, 3 1   
Cauchy's problem, 1 5   
Coddi ngton, E .  A . , 1 06, 1 3 2   
Complete sequence, 1 95   
Conj ugate points, 1 06 ff. various definitions of, 1 06 , 1 1 2 , 1 1 4, 1 20, 1 2 3 , 1 24   
Conjugate system of differential equa­ tions, 22 1   
Conservation of angular momentum, 87, 1 8 5 , 1 8 9   
Conservation of energy, 86, 1 84, 1 89   
Conservation laws, 85-88 for phys ical fields, 1 8 1 - 1 86   
Conservation of momentum, 86, 1 84, 1 89   
Consistent boundary conditions, 1 3 2, 1 3 9- 1 45   
Constraints ( see Subsidiary 1:onditions ) : holonomic, 48 nonholonomoic, 48   
Contravariant vectors, 2 1 2   
Control function, 2 1 9   
Control process, 2 1 9 admissible, 2 1 9 optimal, 2 1 8 , 2 1 9   
Control region, 2 1 8   
Convergence i n  the mean, 203, 207   
Convex set, 3 1   
Convexity condition, 2 1 0 strict, 2 1 1 ,  2 1 7   
Copson, E . T . ,  209   
Coupled oscillators, 1 60   
Courant, R . , 90, 1 6 8, 20 1   
Covariant vectors, 2 1 2   
Cycloid, 3 , 26  

# c  

Canonical Euler equations, 70 ff. first integrals of, 7 0-7 1 relation to propagation o f disturbances, 2 1 5-2 1 7   
Canonical transformation, 77-79, 94 generating function of, 78, 94   
Canonical variables, 58, 63, 67, 68  

# D  

D'Alembertian ( operator ) ,  1 8 1 ,  1 8 8   
Descending principal minors, 1 26   
Direct variational methods, 1 92-207  

# E  

El astic moduli, 1 5 6 Electric field vector, 1 86 Electromagnetic field, 1 86- 1 89 Lagrangian density of, 1 8 8, 1 89 Electromagnetic potential, 1 86 Energy-momentum tensor, 1 84, 1 85, 1 86 Energy-momentum vector, 1 84 Equations of motion : of conti nuous mechanical systems,   
1 65 - 1 6 8 o f a system o f particles, 85 Equicontinuous family of functions, 201 Euclidean space, $\pmb{n}$ -dimensional, 4, 8 ,   
209 E u l e r , L., 2 , 3 , 4 Eul er's equation ( s ) ,  1 5  ff. canonical (see Canonical Euler equa­ tions ) first integrals of, 70, 80, 8 2 , 8 3 , 94 for functionals involving higher-order derivatives, 42 for functionals involving m u ltiple integrals, 25, 1 54 in n unknown functions, 3 5 in tegral curves of, 1 5 i nvariance of, 29-3 1 ,  77 Weierstrass' form o f , 5 1 Euler's theorem , 5 1 ,  226 Extremals, 15 ff. imbedding of, in a field, 1 44 piecewise smooth, 1 8, 62 smooth, 1 8  

# F  

Fastest motion, problem of, 225   
Fermat's principle, 34, 3 6-3 7, 66, 89,   
2 1 0, 2 1 3   
Field functions, 1 80   
Field invariants, 1 8 2- 1 85  

Field (of directions ) ,  1 f central, 1 43-144 definition of, 1 3 2 of a functional, 1 3 7- 1 45 relation to H amilton-Jacobi system , 1 3 3 traj ectories of, 1 3 3 ,  1 40   
Field theory, 1 80- 1 89   
Finite differences, m ethod of, 4, 2 7 , 3 1 , 1 9 3 , 1 9 7   
Forward sweep, 1 3 6   
Function o f  infinitely many variables, 4   
Function of $\pmb{n}$ variables, 4 maximum of, 1 2 m i n i m u m of, 1 2 ( relative ) extremum of, 1 2 unconstrained extremum of, 50   
Function spaces, $\scriptstyle4-8\ \{\mathfrak{F}}$ . $\mathcal{C}(a,b)$ ,  6 $\overline{{\mathcal{C}}}(a,b),31$ $\mathcal{D}_{1}(a,b)$ ,  6 $\mathcal{D}_{n}(a,b)$ , 7   
Functional derivative (see Variational de­ rivative )   
Functionals involving multiple integrals, 1 5 2- 1 9 1 variation of : on a fixed region, 2 3 , 1 52- 1 54 on a variable region, 1 68-1 79   
Functional ( s )  : bilinear, 98 calculus of, 2 continuous,7 examples of, 8-9 d i fferentiable, 1 1 , 99 equivalent, 3 6 fields of, 1 3 7- 1 4 5 general variation of, 54-66 increment of, I I principal linear part of, 1 1 - 1 2 invariant under transformations, 80-83 , 1 7 7 involving functions of several variables (see Functionals i nvolving m ulti­ ple integrals ) involving higher-order derivatives, 40-42 involving $\pmb{n}$ unknown functions, 34-3 8 linear, 8   
Functional ( s ) ( Cont. ) lower semicontinuous, 7, 1 94 nonlocal, 3 quadratic, 98 ff. analysis of, 1 05-1 1 1 nonnegative, 98 positive definite, 98 strongly positive, 1 00 ( relative ) extremum of, 1 2 necessary condition for, 1 3 second variation of, 97, 1 0 1 - 1 02, 1 1 8 strong extremum of, 1 3 ,  1 5 sufficient conditions for, 1 3 1 - 1 5 1 twice differentiable, 99 upper semicontinuous, 7 variation ( d ifferential ) of, 8, 1 1 - 1 2, 9 9 uniqueness of, 12 weak extremum of, 1 3 , 1 5 sufficient conditions for, 97- 1 30   
Fundamental quadratic form e s ) ,  24, 3 7   
Fundamental sequence (see Cauchy se quence )  

# I  

# G  

Gamkrelidze, R. V., 2 1 8   
Gauge transformation ( s ) ,  1 79, 1 87, 1 89   
Geodesics, 34, 3 7-3 8, 3 9   
Geodetic distance, 88   
Green's theorem : four-dimensional, 1 82 $\pmb{n}$ -dimensional, 1 5 3 ,  1 7 4 two-dimensional, 2 3 , 1 6 3 , 1 90  

# H  

Indicatrix, 63   
Involution, 72   
Isoperimetric problem, 3, 39, 42-46, 48  

# J  

J acobi form, 1 26   
J acobi m atrix, 1 26   
J acobi system, 1 2 3 , 1 24   
J acobi's equation, 1 1 2- 1 1 4 , 1 2 8 , 1 3 0 as variational equation of Euler's equa­ tion, 1 1 3   
J acobi's ( necessary ) condition, 1 1 2, 1 1 6, 1 24 relation to theory of quadratic forms, 1 25- 1 2 9 strengthened, 1 1 6, 1 25, 1 3 0   
J acobi's theorem, 9 1 -93 , 2 1 4   
Ham iltonian ( function ) ,  56, 68, 208   
Hamilton-Jacobi equation, 67, 90-93 ff. characteristic system of, 90, 2 1 7 complete integral of, 9 1 ,  2 1 4 relation to propagation o f disturbances, 2 1 3-2 1 7   
Hamilton-J acobi system , 1 3 3 , 1 3 4, 1 3 6, 1 40, 1 4 3 relation t o Hamilton-Jacobi equation, 1 4 3   
H ilbert's invariant integral, 1 45- 1 46, 1 48, 1 5 1   
Hilbert, D . , 90, 1 6 8, 2 0 1   
Huygens' principle, 209  

# K  

Kantorovich, L. V., 205   
Klein-Gordon equation, 1 8 1 ,  1 86   
Kreysig, E., 24   
Kronecker delta, 1 72, 1 8 3 , 1 85   
Krylov, N., 205   
Krylov, V. I., 205  

# L  

Lagrangian density, 1 8 1   
Lagrangian ( function ) ,  84, 1 8 1   
Lagrange multipliers, 43, 45-46, 49, 202   
Laplacian (operator) , 1 64   
Least action, principle of, 83-85, 1 54   
Least action vs. stationary action, 1 59-   
1 6 2   
Legendre transformation, 72, 2 1 2, 222   
Legendre's condition, 1 03 , 1 1 9, 129   
s t rengthened, 1 04, 1 1 6, l S I   
L ' H ospital, G . F . A . , 3   
Linear space, S   
normed, 5, 6   
Liouville surface, 95-96   
Localization property, 3   
Lorentz condition, 1 8 7, 1 8 8, 1 89  

Lorentz transformations, 1 84, 1 89, 1 9 1 orthochronous, 1 84 proper, 1 84  

# M  

Magnetic field vector, 1 86   
Maximizing sequence, 206   
Maximum principle, 222-224   
Maxwell equations, 1 86, 1 87, 1 89   
Mean curvature, 24   
M i k h l i n , S. G . , 205   
Minimal surfaces, 24, 3 3   
Minimizing sequence, 1 93-1 96   
Minimum potential energy, principle of,   
1 6 8   
Mishchenko, E. F., 2 1 8   
Momenta, 86, 1 3 8  

#  

Natural boundary conditions, 26   
Natural frequencies, 1 60   
Neustadt, L. W., 2 1 8   
Newton, I., 3   
Niemeyer, H . , 1 1 9 , 1 20   
Noether's theorem, 79-83 If.   
in several dimensions, 1 77- 1 79   
Nonnegative definite matrix, 1 1 9   
Norm, 5, 6   
Normal coordinates, 1 60   
Normed linear space, 5, 6  

# o  

Optimal control, problems of, 2 1 8-226   
relation to calculus of variations, 220  

# p  

Phase space, 2 1 8   
Piecewise smooth curves, 6 1   
Poisson bracket ( s ) ,  7 1 ,  94   
Poisson's ratio, 1 65   
Pontryagin, L. S . , 2 1 8   
Positive definite matrix, 74, 1 1 9   
Positive-homogeneous function, 39, 5 1   
Propagation of disturbances, 208-2 1 7,   
224   
Propagation time, properties of, 2 1 0  

# Q  

# Quadratic form, 98  

# R  

Rectifiable curve, I length of, I   
Riccati equation, 1 08 , 1 3 4, 1 3 6 m atrix version of, 1 20, 1 3 5   
Ritz method, 1 9 3 , 1 9 5 , 1 9 6, 1 9 8 , 1 9 9 , 206  

# s  

Scalar potential, 1 8 6   
Scalar product, 1 1 8 , 2 1 1   
Self-adjoint boundary conditions, 1 3 8- 1 42, 1 44 , 1 45   
Shilov, G. E . , 5, 3 1 , 9 8 , 1 2 7 , 1 6 0, 1 6 5 , 2 1 2   
Side conditions (see Subsidiary conditions )   
S i l verman, R. A . , 5, 1 6 1 ,  1 84   
Simple harmonic oscillator, 94, 1 5 9   
Smirnov, V . I . , 1 84   
Smooth function, 1 8   
Stationary action, principle of, 1 62   
Sturm-Liouville equation, 1 9 8 If.   
Sturm-Liouville problem, 1 9 8-205 eigenfunctions and eigenvalues of, 1 98, 204, 205   
Subsidiary conditions, 43 finite, 46   
Surface of revolution of minimum area, 20-2 1   
Sweep method, 1 3 5   
Sylvester criterion, 1 27   
System of particles : conservation laws for, 85-88 kinetic energy of, 83 Lagrangian (function ) of, 84 Newton's equations for, 85 potential energy of, 84 total angular momentum of, 84 total energy of, 8 6 total momentum of, 87  

# T  

Tangent space, 209 conjugate space of, 2 1 2, 2 1 7 n o r m i n , 2 1 2 , 2 1 7 i n troduction of norm in, 2 1 1   
Tangential coordinate, 72   
Time optimal problem, 225, 226   
Tolsto v , G . P . , 1 6 1   
Trajectories : of a disturbance, 2 1 0 equations of, 2 1 1 of a field, 1 3 3 , 1 40 of a system of differential equations, 2 1 9 optim a l , 2 1 9   
Transversal, 60   
Transversality con d itions, 60, 6 1 ,  64, 65   
Tr i rogoff, K . N . , 2 1 8   
TsetIyn, M . L . , 2 0 8   
Vector potential, 1 86   
Vibrating membrane, 1 62- 1 64 action functional for, 1 63 equation of, 1 64 kinetic energy of, 1 62 Lagrangian density of, 1 8 1 potential energy of, 1 62   
V i brating plate, 1 65- 1 6 8 action functional for, 1 66 clamped, 1 67 equation for forced vibrations of, 1 67 equation for free vibrations of, 1 67 k inetic energy of, 1 65 potential energy of, 1 65- 1 66 supported, 1 67   
Vibrating string, 1 5 5- 1 59 action functional for, 1 5 7 equation of, 1 5 8 kinetic energy of, 1 5 5 Lagrangian density of, 1 8 1 potential energy of, 1 56  

# u  

Uniformly bounded family of functions, 2 0 1  

# v  

Variable end point problems, 25-27, 5 9-6 1 m ixed case, 26   
Variational derivative, 27-29   
Variational equation, 1 1 3   
Variational princ iples, 3 , 67   
Var iational p roblem s : examples of, 2-3 in parametric form, 3 8-40 invariant, 80, 1 76 involving h igher-order derivatives, 40-42 involving multiple integrals, 22-24, 1 5 2- 1 9 1 involving $\pmb{n}$ unknown functions, 34-3 8 simplest, 8, 1 4-22 defi n i tion, 1 4 with subsidiary conditions, 42-50  

# w  

Wave front ( s ) ,  2 1 1 , 2 1 2, 2 1 4, 2 1 5 , 2 1 6, 224   
Weierstrass $E$ -fu nction, 1 46- 1 49 , 1 5 1 , 224   
Weierstrass-Erdmann (corner ) condi­ tions, 6 3 , 65, 69   
Weierstrass' necessary condition, 1 49, 1 5 1 , 224, 225   
Widder, D. V . , 2 3 , 24, 3 7 , 4 3 , 1 1 0, 1 3 9, 1 45  

# y  

# Young's inequality, 75  

# z  

Zero element, 5   
Z h i d k o v , N. P . , 1 3 6  