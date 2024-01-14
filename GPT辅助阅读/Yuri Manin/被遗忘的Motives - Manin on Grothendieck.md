FORGOTTEN MOTIVES: THE VARIETIES OF SCIENTIFIC EXPERIENCE （被遗忘的动机：科学经验的多样性）
---


Yuri I. Manin 
尤里·曼宁

*Max–Planck–Institut f ̈ ur Mathematik, Bonn, Germany* 

*德国波恩马克斯·普朗克数学研究所*

```
 Le gros public: A poˆele, Descartes! `a poˆele! (R. Queneau, Les Oeuvres compl`etes de Sally Mara)

 对于一般大众：笛卡尔，去烤火吧！（R·奎诺，《莎莉·玛拉的完整作品》）
 ```

---


When I arrived in Bures–sur–Yvette in May 1967, the famous seminar SGA 1966–67, dedicated to the Riemann–Roch theorem, was already drawing to an end. Mlle Rolland, then L ́eon Motchane’s secretary at the IH ́ ES, found for me a nice small apartment in Orsay. Each early morning, awoken to the loud chorus of singing birds, I walked to Bures, anticipating the new session of private tutoring on the then brand–new project of motives, by the Grand Maı ˆtre himself, Alexandre Grothendieck. Several pages, written by his hand then, survive in my archive; in particular, the one dedicated to the “Standard Conjectures”. These conjectures remain unproved after half a century of vain efforts. Grothendieck himself saw them as the cornerstone of the whole project. In the letter to me dated March 20, 1969, he wrote: Je dois avouer `a ma honte que je ne sais plus distinguer `a premi`ere vue ce qui est d ́emontrable (voire plus ou moins trivial) sans les conjectures standard, et ce qui ne l’est pas. C’est  ́evidemment honteux qu’on n’ait pas d ́emontr ́ees les conjectures standard!

当我在1967年5月抵达Bures-sur-Yvette时，著名的SGA 1966-67研讨会，专门讨论黎曼-罗赫定理，已经接近尾声。当时在IHES（高等研究应用学院）担任Léon Motchane秘书的Rolland小姐为我找到了一个漂亮的小公寓在Orsay。每天清晨，被鸟儿的大合唱惊醒后，我走路去Bures，期待着由大师Alexandre Grothendieck亲自授课关于当时崭新的动机项目的新一期私人辅导。他亲手写下的几页笔记现在保存在我的档案中，其中包括一张专门讨论“标准猜想”的页面。经过半个世纪的努力，这些猜想仍未被证明。Grothendieck本人认为它们是整个项目的基石。在1969年3月20日写给我的信中，他写道：“我必须承认我已经不再一眼区分什么是基于标准猜想证明的（甚至更或多少是微不足道的），什么不是。当然，标准猜想未被证明是可耻的！”

Still, during the decades that have passed since then the vast realm of motives kept rewarding the humility of many researchers prepared to be happy with what they could do using the tools they could elaborate. 

Several times Grothendieck invited me to his house at rue de Moulon. He allowed me to browse through his bookshelves; I borrowed a few books to read at home. When I last visited him a day or two before my departure, I asked him to sign a book or paper for me. To my amazement, he opened “Les Œuvres compl`etes de Sally Mara” by Raymond Queneau and scribbled on the first page:

> Hommage affectueux R. Queneau

然而，自那时以来的几十年里，广阔的动机领域一直在回报着许多研究人员的谦卑，他们愿意接受他们能够使用和发展的工具所能做的事情。

Grothendieck几次邀请我去他在Moulon街的家。他让我翻阅他的书架；我借了一些书回家看。在我离开前的一两天最后一次拜访他时，我问他能否为我签名一本书或论文。令我惊讶的是，他打开了雷蒙德·凯诺的《莎莉·玛拉的全部作品》，在第一页上匆匆写下了几行：

> 亲切致敬，R·昆诺。

# Early history of motives （关于动机的早期历史）

Having returned to Moscow in June 1967, after five or six weeks of intense training with Grothendieck, I spent several months writing down his main definitions related to motives and studying necessary background material in the literature. I was very pleased when it turned out that I could answer one of his questions and calculate the motive of a blow–up without using standard conjectures. My paper [Ma68] containing this exercise was submitted next summer and published in Russian. It became the first ever publication on motives, and Grothendieck recommended it to David Mumford (in his letter of April 14, 1969) as “a nice foundational paper” on motives. 

Grothendieck wrote a letter in Russian to me about this paper (05/02/1969). This seems to be the only document showing that he had some Russian, probably, learned from his father.


1967年6月，我在与Grothendieck进行了五六周的密集培训后回到了莫斯科，并花费了几个月的时间写下了他与动机相关的主要定义，并学习了必要的背景知识。当我能够回答他的一个问题并计算出一个吹气的动机时，我非常高兴，而没有使用标准猜想。我的论文[Ma68]包含了这个练习，于次年夏天提交并发表在俄语上。这成为动机的第一篇出版物，Grothendieck在1969年4月14日给David Mumford的信中将其推荐为“一个很好的关于动机的基础性论文”。

Grothendieck也给我写了一封关于这篇论文的俄文信（1969年5月2日）。这似乎是唯一一份显示他会一些俄文的文件，很可能是从他的父亲那里学来的。


The first step in the definition of a category of (pure) motives is this.
We keep objects of a given algebraic--geometric category, say of  smooth projective varieties over a fixed field $Var_k$,  
but replace its morphisms
 by *correspondences*.
This passage implies that morphisms $X\to Y$ now form an *additive group,*
or even a $K$--module rather than simply a set, where $K$ is an appropriate coefficient ring.
Moreover, correspondences themselves are not just cycles on $X\times Y$ but
 *classes* of such cycles modulo an ``adequate'' equivalence relation. The coarsest such relation 
is that of numerical equivalence, when two equidimensional  cycles are equivalent if  their intersection indices
with each cycle of complementary dimension coincide. The finest one is the rational  (Chow) equivalence,
when equivalent cycles are deformations over a base which is a chain of rational curves.
Direct product of varieties induces tensor product structure on the category.

纯动机范畴的定义的第一步如下：我们保留给定代数几何范畴中的对象，比如固定域 $Var_k$上的光滑射影簇，但是将其态射替换为对应。这意味着，现在$X → Y$的态射形成一个加性群，甚至是一个$K-$模，而不仅仅是一个集合，其中K是一个适当的系数环。此外，对应本身不仅仅是 $X × Y$上的环，而是适当等价关系下的这些环的类。最粗糙的等价关系是数值等价，即如果两个等维数的环与补充维数的每个环的交点指数相等，则它们是等价的。最好的等价关系是有理（Chow）等价，当等价环在一个由有理曲线构成的链上的变形时。簇的直积在范畴上引入张量积结构。

The second step in the definition of the relevant category of pure motives consists in a formal construction of new objects (and relevant morphisms) that are “pieces” of varieties: kernels and images of projectors, i. e. correspondences p : X → X with p2 = p. This produces a pseudo–abelian, or Karoubian completion of the category. In this new category, the projective line P1 becomes the direct sum of the (motive of) a point and the Lefschetz motive L (intuitively corresponding to the affine line). 

The third, and last step of the construction, is one more formal enhancement of the class of objects: they now include all integer tensor powers L⊗n, not just non–negative ones, and tensor products of these with other motives.

定义纯动机的相关范畴的第二步是形式地构造新的对象（和相关的态射），它们是“曲面”的“部分”：投影算子的核和像，即具有p2=p的对应p：X→X。这样就产生了类假可除或Karoubian完备的范畴。在这个新的范畴中，射影直线P1成为一个点的动机和Lefschetz动机L（直观地对应于仿射直线）的直和。

构造的第三步也是最后一步，它是对象类的又一种形式增强：现在它们包括所有的整数张量幂L ⊗n，而不仅仅是非负的，以及这些动机与其他动机的张量积。

Various strands of intuition are interwoven in this fundamental pattern discovered by Grothendieck, and I will now try to make them (more) explicit. 

The basic intuition that guided Grothendieck himself, was the image of the category of pure Chow motives M otk as the receptacle of the “universal cohomology theory” Vk → M otk: V 7→ h(V ). The universal theory was needed in order to unite various cohomological constructions, such as Betti, de Rham–Hodge, and  ́etale cohomology. 

What looked paradoxical in this image was the following observation about transcendental cycles on an algebraic variety X. One could get hold of these cycles for k = C by appealing to algebraic topology, or else to complicated constructions of homological algebra involving all finite covers of X.

Grothendieck 发现了这个基本模式，其中融合了各种直觉，我现在会尝试使它们更明确。

Grothendieck自己的基本直觉是，纯Chow代数学范畴Motk是“通用上同调理论”Vk → Motk: V 7→ h(V )的容器。需要这个通用理论是为了统一各种上同调结构，比如Betti、de Rham-Hodge和étale上同调。

在这个形象中看起来很矛盾的是，关于代数簇X上的超越周期的以下观察：通过代数拓扑或者涉及X所有有限覆盖的复杂同调代数构造，我们可以通过k = C来获取这些周期。

But in the category of pure motives, from the start one dealt only with algebraic cycles, represented by correspondences, and it was intuitively not at all clear how on earth they could convey information about transcendental cycles. Indeed, the main function of the “Standard Conjectures” was to serve as a convenient bridge from algebraic to transcendental. Everything that one could prove without them was indeed “plus ou moins trivial” – until people started treating correspondences themselves using sophisticated homological algebra (partly generated by the development of  ́etale cohomology and Grothendieck–Verdier’s introduction of derived and triangulated categories). 

However, the passage from the set of morphisms to the K–module of correspondences involves one more intuitive idea, and it can be most succinctly invoked by referring to physics, namely the great leap from the classical mode of description of nature to the quantum one. This leap defined the science of the XXth century. Its basic and universal step consists in the introduction of a linear span of everything that in classical physics was only a set: points of a phase space, field configurations over a domain of space–time etc. Such quantum superpositions then form linear spaces on which Hilbert–like scalar products are defined, that in turn allow one to speak about probability amplitudes, quantum observations etc.

但在纯动机范畴中，从一开始就只处理由对应关系表示的代数周期，并且从直觉上来看，这些周期如何能传递关于超越周期的信息根本不清楚。事实上，“标准猜想”的主要作用是作为从代数到超越的方便桥梁。一切可以在没有它们的情况下证明的东西确实是“差不多平凡的”-直到人们开始使用复杂的同调代数来处理对应关系本身（部分是由于 étale 同调的发展和 Grothendieck-Verdier 引入衍生和三角范畴）。

然而，从态射集合到对应关系的 K-模的过渡涉及到更多的直觉思想，并且可以通过引用物理学来最简洁地调用，即从经典自然描述模式到量子描述模式的巨大飞跃。这个飞跃定义了20世纪的科学。它的基本和普遍的步骤在于引入一切在经典物理学中只是一个集合的东西的线性跨度：相空间中的点，空间 - 时间域上的场配置等。这些量子叠加形成线性空间，在其上定义了 Hilbert 样的标量积，进而允许讨论概率幅，量子观测等。

I have no evidence that Grothendieck himself thought then about quantum physics in relation to his algebraic geometry project. We do know that concerns about weapons of mass destruction and collaborationist behaviour of scientists towards their governments and military–industrial complexes inspired in him deep disturbance and aversion. The most direct source of his inspiration might have been algebraic topology which, after the 1940s, laid more stress on chains and cochains than on simplices and the ways they are glued together. 

However, in my personal development as a mathematician in the 1970’s–80’s and later, the study of quantum field theory played a great role, and feedback from theoretical physics – that was ahead – to algebraic geometry became a great source of inspiration for me. I was and remain possessed by a Cartesian dream, poetic rationalism, whatever history has yet to say about Der Untergang des Abendlandes. 

Below I will sketch a map of two branches of the development of Grothendieck ideas about motives that approximately followed two intuitions invoked above: from homological algebra and from physics respectively. The references at the end of this essay constitute the bare minimum of the relevant research, but the reader will be able to find much additional bibliographical material in the survey collection [Mo91] and in [A04], [VoSuFr00], [Ta11].

我没有证据表明 Grothendieck 自己曾经考虑过量子物理与他的代数几何项目之间的关系。我们知道，对大规模杀伤性武器和科学家向政府和军工复合体的合作行为的担忧，在他心中引起了深刻的不安和厌恶。他灵感最直接的来源可能是代数拓扑，在20世纪40年代之后，代数拓扑更加强调链和余链，而不是单纯形和它们的粘合方式。

然而，在我作为数学家在20世纪70年代和80年代以及之后的个人发展中，量子场论的研究发挥了重要作用，理论物理的反馈 - 这是领先的 - 对代数几何成为了我灵感的重要源泉。我一直被笛卡尔的梦想、诗意的理性主义所支配，不管历史对《西方的没落》有何评价。

在下面，我将勾勒出 Grothendieck 对动机的想法发展的两个分支的大致图景：从同调代数和从物理学分别考虑。本文末尾的参考文献是相关研究的最低限度，但读者可以在综述文集[Mo91]和[Ta11]中找到更多的参考资料。

# Motives and homological algebra (动机与同调代数)

The most common linear objects are modules over rings in algebra and sheaves of modules in algebraic geometry. Free modules/locally free sheaves are the closest to classical linear spaces. 

General algebraic variety X, or a scheme, is a highly non–linear object. 

In classical algebraic geometry over, say, the complex numbers, the variety X used to be identified with the topological space X(C) of its C–points, and could be studied by topological methods involving triangulations or cell decompositions. In the geometry over, say, finite fields, this did not work, and when in 1949 Andr ́e Weil stated his famous suggestion that point counting over finite fields should be done using trace of the Frobenius endomorphism acting upon appropriately defined (co)homology groups of X, it generated a flow of research. 

The first product of this research was the creation of the cohomology theory of coherent sheaves of modules F on varieties X or more general schemes. Now, in a constructive definition of H∗(X, F ), one could either stress combinatorics of covers of X by open sets in the Zariski topology ( ˇ Cech cohomology) or, alternatively, “projective/injective resolutions” of F , that is special exact complexes of sheaves · · · → F2 → F1 → F0 := F → 0 or similarly with arrows inverted. This passage from the dependence of H∗(X, F ) on the non–linear argument X to the dependence on the linear argument F was very characteristic for the early algebraic geometry of 1950’s and 1960’s. “Homological Algebra” by H. Cartan and S. Eilenberg, the famous FAC, “Faisceaux Alg ́ebriques Coh ́erents” by J.-P. Serre, became the standard handbooks for every aspiring young algebraic geometer.



在代数中，最常见的线性对象是环上的模，而在代数几何中是模层。自由模/局部自由层最接近于经典线性空间。

一般代数簇X，或者一个方案，是一个高度非线性的对象。

在经典代数几何中，比如在复数域上，簇X被认为是其C点的拓扑空间X（C），并且可以通过涉及三角剖分或细胞分解的拓扑方法进行研究。但在有限域上的几何中，这种方法行不通。1949年，安德烈·韦伊尔提出了他著名的建议，即在适当定义的（余）同调群上，通过Frobenius自同构的迹来计算有限域上的点的数量，这激发了一波研究热潮。

这项研究的第一个成果是创造了同调理论的一般化，即变量为代数簇X或更一般的方案上的一致层F的同调理论。在构造H∗（X，F）的定义中，人们可以强调Zariski拓扑下的开集覆盖的组合（cech上同调），或者是F的“投射/内射分辨”，即特殊的精确层复合物，例如：...→ F2→ F1→ F0：= F→ 0，或类似地，箭头倒转。这种从H∗（X，F）对于非线性变量X的依赖到对于线性变量F的依赖的转变非常符合20世纪50年代和60年代早期的代数几何的特点。H. Cartan和S. Eilenberg的“同调代数”（H. Cartan and S. Eilenberg）以及J.-P. Serre的“可数理想层”（Faisceaux Alg ́ebriques Coh ́erents）成为每个有抱负的年轻代数几何学家的标准手册。


David Mumford and I started our training as algebraic geometers at the same time, about 1956, he at Harvard, I at Moscow University. David reminisces that his teacher Zariski “was motivated by the need to make the work of the Italian school rigorous by using the new methods of commutative algebra”. My teacher Shafarevich also suggested to us to study glorious Italian algebraic geometry, approaching it armed with modern insights and techniques developed by Serre, Grothendieck and their school. 

I had no time nor use for a course in “Instant Italian”, so I tried to read two books simultaneously, “Le Superficie Algebriche” by Federigo Enriques (Zanichelli, 1949) and “La Divina Commedia”, and each time that I opened Enriques (or for that matter, SGA), I recited mournfully: lasciate ogni speranza voi ch’entrate ...

Nevertheless, it worked. When I brought xeroxed papers by Gino Fano back from Bures in 1967, Vassya Iskovskikh and I could read them without bothering much in which language they have been written, and then produce the first examples of birationally rigid varieties, and unirational but not rational threefolds using Fano methods.


David Mumford和我大约在1956年同时开始成为代数几何学家，他在哈佛大学，我在莫斯科大学。David回忆说他的导师Zariski“出于使用交换代数的新方法使意大利学派的工作变得严谨的需要而受到激励”。我的导师Shafarevich也建议我们学习辉煌的意大利代数几何，运用Serre、Grothendieck及其学派的现代见解和技巧来接近它。

我没有时间也用不着上“Instant Italian”课程，所以我尝试同时阅读两本书，“Le Superficie Algebriche”（Federigo Enriques著，Zanichelli，1949年出版）和“La Divina Commedia”，每次我打开Enriques（或者说，SGA）的书，我都会忧郁地吟唱：“lasciate ogni speranza voi ch’entrate...”。

尽管如此，它还是奏效了。当我在1967年从Bures带回Gino Fano的复印论文时，Vassya Iskovskikh和我可以不太在意它们是用哪种语言写的，然后使用Fano方法产生出第一个具有有理同构刚性的代数簇和不可逆但不是有理的三次曲面的例子。


Homological algebra proved more resistant, and here I learned most of what I understand now from the next generation of eager young Moscow students, who by now have been mature researchers themselves for a long time. 

We first learned, of course, about the basic Grothendieck–Verdier presentation of homological algebra as the theory of derived, and more generally, triangulated categories. Passage from the Bourbaki language of structures to the now domineering language of categories (and then polycategories) involved several radical changes of intuition, and as is now clear, led into the garden of forking paths. The passage from one crossroad to another one always involved a decision about what should be disregarded, and later it could happen – and always did happen – that one was bound to turn back again and recollect some forgotten ideas.

 The story of derived categories started with categories, whose objects were complexes (of abelian groups/sheaves/objects of an abelian category) considered modulo homotopy.

 同调代数则表现出更强的抵抗力，而我现在所理解的大部分内容，是从下一代充满热情的莫斯科学生那里学到的，他们现在早已成为成熟的研究人员。

当然，我们首先学习了基本的 Grothendieck-Verdier 理论，将同调代数表达为导出范畴和更一般的三角范畴理论。从结构的 Bourbaki 语言到现在主导的范畴语言（然后是多范畴）的转变，涉及到几个激进的直觉变化，并且现在清楚的是，它引导了我们进入了分叉道路的花园。从一个十字路口到另一个十字路口，总是涉及到关于什么应该被忽略的决定，然后后来可能会发生-并且总是会发生-人们不得不再次转回去，回忆起一些被遗忘的想法。

导出范畴的故事始于范畴，其对象是复合物（群的/层的/Abel 范畴中的对象的），这些复合物被视为模同伦下的等价。

In the framework of Grothendieck–Verdier triangulated categories, one forgot about initial objects–complexes and focused on an abstract additive category, endowed with a translation functor and a class of diagrams, called distinguished triangles. But the problem of non–functoriality of cones led back to the complexes of abelian groups, this time upgraded to the level of morphisms rather than objects. 

This was, of course, a special case of enriched categories, which in the simplest incarnation postulate Bourbaki–structured morphism sets Hom (X, Y ), but with an upgrading: this time one clearly had to deal with the case of categorified morphism sets. However, when one allows morphisms to be objects of a category, then morphisms of this second floor category might form a category as well . . . and we find ourselves ascending the Tower of Babel that could cause despair even in Grothendieck himself. 

For the limited purposes of this note, I will disregard subtleties and various versions of the notion of triangulated/dg–categories, and will only sketch several basic discoveries of the last decades relating such categories with motives. 

Roughly speaking, starting with a category of varieties (or schemes) X, one may consider either the replacement of each X by a triangulated category D(X) of complexes of (quasi)–coherent sheaves on X, or else return to the initial Grothendieck insight, but replace correspondences by complexes of correspondences.

在 Grothendieck-Verdier 三角范畴的框架内，人们忘记了初始物——复形，而是关注一个抽象的加性范畴，它配备了一个平移函子和一类被称为特殊三角形的图表。但是，锥不具备函子性的问题又将人们带回到了阿贝尔群复形的范畴，这一次将其升级到了映射的级别而不是对象。

这当然是富有结构的 Hom 集合的富有结构范畴的一个特殊情况，最简单的形式是保证 Hom(X,Y)，但是这一次需要升级：这一次需要明确处理范畴化的映射集合的情况。但是，当我们允许映射是一个范畴的对象时，这个二层范畴的映射可能会形成一个范畴……我们发现自己正在攀登巴别塔，这甚至会让 Grothendieck 自己都感到绝望。

对于本笔记的有限目的，我将忽略三角/差分范畴的细微差别和各种版本，并仅概述过去几十年来涉及动机的一些基本发现。粗略地说，从一个代数簇（或概型）的范畴X开始，可以考虑将每个X替换为在X上（准）连续层的复形范畴D(X)，或者返回最初的Grothendieck见解，但用对应复形替换对应。

The latter approach led to the Voevodsky’s motives ([VoSuFr00]). I will focus on some achievements of the first one. 

One of the first great surprises was Alexander Beilinson’s discovery ([Be83]) that a derived category of a projective space can be described as a triangulated category made out of modules over a Grassmann algebra. In particular, a projective space became “affine” in some kind of non–commutative geometry! The development of Beilinson’s technique led to a general machinery describing triangulated categories in terms of exceptional systems and extending the realm of candidates to the role of non–commutative motives. 

D. Orlov ([Or05]) proved a general theorem to the effect that if X, Y are smooth projective k–varieties and if there is a fully faithful functor F : Db(X) → Db(Y ), then the Chow motive h(X) is a direct summand of h(Y ) “up to translations and twists by Lefschetz/Tate motives”. 

M. Kontsevich formalised the properties of dg–categories, expressing properness and smoothness in case of the derived categories of varieties, and defined the respective class of categories (modulo homotopy) as “spaces” in non–commutative algebraic geometry. He then defined the respective class of Chow motives and has shown that there exists a natural fully faithful functor embedding Grothendieck’s Chow motives (modulo twists) into non–commutative motives. These ideas were further developed by Tabuada, Marcolli, Cisinski et al., cf. the recent survey [Ta11] and references therein.

后一种方法导致了Voevodsky的动机([VoSuFr00])。我将着重介绍第一种方法的一些成果。

其中一个最大的惊喜是Alexander Beilinson的发现([Be83])，即一个投影空间的导出范畴可以被描述为由Grassmann代数上的模组成的三角范畴。特别地，一个投影空间在某种非交换几何中变成了“仿射的”！Beilinson技术的发展导致了一个描述基于例外系统的三角范畴的一般机制，并将候选者的范围扩展到非交换动机的角色。

D. Orlov([Or05])证明了一个一般定理，即如果X，Y是光滑的投影k-变量，并且存在一个完全忠诚的函子F: Db(X) → Db(Y)，则Chow动机h(X)是h(Y)“在Lefschetz / Tate动机的平移和扭曲下的直和分量”。

M. Kontsevich将变量的导出范畴的适当性和光滑性形式化，并定义了相应类别（模同伦下）作为非交换代数几何中的“空间”。他随后定义了相应的Chow动机类别，并证明了存在一个自然完全忠诚的函子，将Grothendieck的Chow动机（模扭曲）嵌入非交换动机中。这些思想由Tabuada，Marcolli，Cisinski等人进一步发展，参见最近的调查[Ta11]及其中的参考文献。

# Motives and physics （动机与物理学）

In the mid–1970’s and later, algebraic geometry interacted with physics more intensely that ever before: self–dual gauge fields (instantons), completely integrable systems (Korteweg–de Vries equations), emergence of supergeometry (based upon formal rules of Fermi statistics), the Mumford form and the Polyakov measure on moduli spaces of curves (quantum strings) have been discussed at joint seminars and local and international conferences of physicists and mathematicians. 

Motives did not yet appear in this picture. However, in 1991 something new and unexpected happened. 

B. Greene in his book “The Elegant Universe. Superstrings, Hidden Dimensions and the Quest for the Ultimate Theory” tells the following story: 

```
“At a meeting of physicists and mathematicians in Berkeley in 1991, Candelas announced the result reached by his group using string theory and mirror symmetry: 317 206 375. Ellingsrood and Strømme announced the result of their very difficult mathematical computation: 2 682 549 425. For days, mathematicians and physicists debated: Who was right? [ . . . ] 

About a month later, an e–mail message was widely circulated among participants in the Berkeley meeting with the subject heading: Physics Wins! Ellingsrood and Strømme had found an error in their computer code that, when corrected, confirmed Candelas’s result.”

```


在1970年代中期及以后的时间里，代数几何与物理学的交互比以往任何时候都更加紧密：自对偶规范场（瞬子）、完全可积系统（KdV方程）、超几何的出现（基于费米统计的形式规则）、Mumford形式和Polyakov测度在曲线的模空间（量子弦理论）上进行了物理学家和数学家的联合研讨会和国内外会议上的讨论。

动机在这张画卷中尚未出现。然而，1991年发生了一些新的、出乎意料的事情。

B.格林在他的书《优雅的宇宙：超弦、隐藏的维度和终极理论的探索》中讲述了以下故事：
```
“1991年在伯克利的一次物理学家和数学家的会议上，Candelas宣布了他的小组利用弦理论和镜像对称得出的结果：317206375。Ellingsrood和Strømme宣布了他们非常困难的数学计算结果：2682549425。数学家和物理学家争论了数天：谁是正确的？[......]

大约一个月后，在伯克利会议的参与者之间广泛传播了一封电子邮件，主题是：物理学胜利了！Ellingsrood和Strømme发现了他们计算机代码中的一个错误，纠正后确认了Candelas的结果。”
```

The problem about which Greene speaks is this. Consider a smooth hypersurface V of degree 5 in P4. Denote by n(d) the (appropriately defined) number of rational curves of degree d on V . Calculating n(d) looks like perfectly classical problem of enumerative algebra geometry, and in fact the numbers n(1) = 2875 and n(2) = 609250 were long known. The physicists Ph. Candelas, X. C. de la Ossa, P. S. Green, and L. Parkes using machinery and heuristics of quantum string theory, calculated not just n(3), but gave an analytic expression for a total generating function for these numbers, using the so called Mirror Conjecture. The mathematicians G. Ellingsrood and S. A. Strømme produced a computer code calculating n(3). 

Omitting a lot of exciting developments of this rich story, I will briefly explain only the part that refers to the new and highly universal motivic structur that emerged in algebraic geometry. I will speak about varieties, although in fact Deligne–Mumford stacks form the minimal habitat for this structure, and the respective extension of the construction of pure motives for them is needed; this was done by B. To ̈en.

Greene所提到的问题是这样的：考虑P4中一个5次平滑超曲面V。用n(d)来表示V上的次数为d的有理曲线的数量（适当地定义）。计算n(d)看起来像是一个纯粹的代数几何计数问题，实际上n(1)=2875和n(2)=609250这些数字早已为人所知。物理学家Ph.Candelas、X.C.de la Ossa、P.S.Green和L.Parkes使用量子弦论的机制和启发式，不仅计算了n(3)，而且还利用所谓的镜像猜想给出了这些数字的总生成函数的解析表达式。数学家G.Ellingsrood和S.A.Strømme编写了一个计算n(3)的计算机代码。

在省略了这个丰富故事中许多令人兴奋的发展后，我将简要解释只涉及新出现的高度通用的动机结构的那部分代数几何。我将谈论多样性，尽管事实上Deligne-Mumford堆栈形成了这种结构的最小栖息地，并且需要为它们提供相应的纯动机构造的扩展。这项工作由B.Toën完成。

Roughly speaking, we now treat the general problem, inherited from classical enumerative geometry: given a projective variety V , (define and) calculate the number of algebraic curves of genus g on V , satisfying additional incidence conditions that make this number finite, as in the Euclidean archetype: ”one line passes through two different points of plane”. After considerable efforts, one can define for all stable values of (g, n) a Chow class Ig,n on V n × M g,n with coefficients in the completed semi–group ring, say Q[[qβ]] where β runs over integral classes in the Mori cone of V . This class expresses the virtual incidence relation, described above, by reducing it to the positions of the respective points in V n on the one hand, and to the position of the respective curve in the Deligne–Mumford stack of curves of genus g with n marked points. 

When this is done, a list of universal properties of the classes Ig,n treated as motivic morphisms, defines essentially the (co)action of the modular (co)operad with components h(M g,n) in the category of motives upon each total motive h(V ) (I use the word total in order to stress that we are not allowed to pass to pieces here, although twisting and translations are in fact present, cf. [BehM96]). 

The sophistication of both theoretical (and imaginative) physics and abstract mathematics that cooperated to discover this picture is really amazing, and I would like to draw attention to the fact that our traditional (mis)representation of mathematics as a language and technical tool needed to make physical intuition precise, was reversed here: physical intuition helped discover mathematical structures that were not known before. One remarkable result of this was Deligne’s generalisation of the Tannakian Galois formalism ([De02]): it turned out that motivic Galois groups are actually supergroups, so that the Fermi statistics now firmly resides in algebraic geometry as well, which up to then was “purely bosonian”.

简而言之，我们现在处理从经典枚举几何学继承而来的一般问题：给定一个射影簇V，（定义并）计算在V上满足使这个数有限的额外关系的g维代数曲线的数量，就像欧几里得原型中的“一条直线穿过平面上的两个不同点”。经过相当大的努力，可以为所有稳定的(g，n)值在Vn×Mg，n上定义一个Chow类Ig，n，其系数为完成的半群环Q[[qβ]]，其中β在V的Mori锥中运行。这个类通过在一方面减少到Vn上相应点的位置，另一方面减少到带有n个标记点的g种类曲线的Deligne-Mumford堆中相应曲线的位置，表达了虚拟的关系。

当这样做时，将Ig，n作为激励态射处理的一系列通用属性，在范畴中定义了模态（共）操作的（共）作用，其组件为h(Mg，n)。模态和每个总模态h(V)的相互作用（共）作用（我使用单词总来强调我们在这里不被允许分成碎片，尽管在事实上扭曲和翻译是存在的，参见[BehM96]）。

理论（和想象力）物理学和抽象数学的复杂性合作发现这个画面真的很惊人，我想引起注意的是，我们传统的（误）将数学表示为需要精确物理直觉的语言和技术工具，反转了这里：物理直觉帮助发现以前不知道的数学结构。这其中一个显著的结果是Deligne对Tannakian Galois形式主义的概括（[De02]）：结果表明，激励Galios群实际上是超群，因此Fermi统计现在也牢固地驻留在代数几何中，而这直到那时都是“纯玻色子的”。

Of course, such reversals have happened many times in history, but here the contemporary status of both theory of motives and quantum strings adds a strong romantic touch to the story. The beautiful two–volume cooperative project of the two communities trying to enlighten each other, [QFS99], is branded by two epigraphs. The epigraph to the first volume is a quotation from Grothendieck’s “R ́ecoltes et Semailles”:

```
Passer de la m ́ecanique quantique de Newton `a celle d’Einstein doit ˆetre un peu, pour le math ́ematicien, comme de passer du bon vieux dialecte proven ̧cal `a l’argot parisien dernier cri. Par contre, passer `a la m ́ecanique quantique, j’imagine, c’est passer du fran ̧ cais au chinois. 
```

(In the pre–post–modern times one would have said: “It’s all Greek to me!”). 

The second volume starts with epigraph, written in Chinese logograms, from Confucius’ “Analects”, 17:2. Here I give its translation: 
```
The Master said: “Men are close to one another by nature. They drift apart through behavior that is constantly repeated”. 
```

This is the collective riposte of the two communities, arguing their closeness, but in the language that is foreign for both.

当然，这样的颠倒在历史上已经发生过很多次，但是当今动机理论和量子弦理论的现代状态为这个故事增添了浓厚的浪漫色彩。两个社区合作的美丽的两卷本项目 [QFS99] 印有两个引文。第一卷的引语摘自格罗滕迪克的《收获和播种》：

```
“对于数学家来说，从牛顿量子力学到爱因斯坦量子力学的转变，有点像从古老的普罗旺斯方言到最新的巴黎俚语的转变。然而，我想，从经典物理到量子力学的转变，就像从法语到汉语的转变一样。”
```

（在前现代时代，人们会说：“这对我来说就像希腊语一样！”）

第二卷以中国汉字写的引语开头，摘自《论语》第17章第2节。这里我给出它的翻译：

```
“子曰：“人之生也直，罔之生也幸而免。””
```

这是两个社区的集体回应，证明他们的亲近，但使用了对双方都陌生的语言。

---
In his letter to me from Les Aumettes dated March 8, 1988, the last letter that I have, Grothendieck has written:

 . . . thanks for your letter of birthday congratulations, and please excuse my being late in replying to this letter, as well as the previous one and thanking for the reprint with dedication of november last year. Your letter struck me as somewhat formal and kind of ill at ease, and surely my silence has contributed to it. What I had to say about the spirits in mathematics today I said in the volumes I sent you and a number of other former friends. I am confident that before the year 2000 is reached, mathematicians (and even non–mathematicians) will read it with care and be amazed about times strange at last left behind . . . 
 
 I met Grothendieck almost half a century ago. Thinking back on his imprint on me then, I realise that it was his generosity and his uncanny sense of humour that struck me most, the carnivalistic streak in his nature, which I later learned to discern in other anarchists and revolutionaries. 
 
 On the front cover of the issue no 14 of “Survivre . . . et Vivre” (Octobrenovembre 1972) that miraculously reached me by post in Moscow, I read: 
 
 ```
 2 FRANCS
 Canada 50 c 
 Communaut ́es:
 1 fromage de ch`evre.
 ```

 在他1988年3月8日从Les Aumettes写给我的信中，也是我拥有的最后一封信中，Grothendieck写道：

```
“……感谢你的生日祝福信，对于回信的迟延以及之前的信件和去年11月的书赠请原谅。你的信给我留下了一种有些正式、有些不自在的印象，而我的沉默也肯定加重了这种印象。我在我给你和其他一些老朋友寄的书中已经说了我对当今数学精神的看法。我相信在2000年之前，数学家（甚至非数学家）会认真阅读这些书，并为最后摆脱的奇怪时代而惊叹不已……”
```

我与Grothendieck相识已有近半个世纪。回想起当时他对我产生的影响，我意识到最深刻的是他的慷慨和他那种异乎寻常的幽默感，他个性中的狂欢主义倾向，我后来发现这种特点也存在于其他无政府主义者和革命者中。

在“Survivre . . . et Vivre”第14期（1972年10月至11月）的封面上，我读到：
```
2法郎
加拿大50分
社区：
1块山羊奶酪。
```

# References 

[Gr 69] A. Grothendieck. Standard conjectures on algebraic cycles. In: Algebraic Geometry, Bombay Colloquium, 1968, Oxford UP, 1969, pp. 193–199.

 [Ma68] Yu. Manin. Correspondences, motives and monoidal transformations. Math. USSR–Sb., 6 (1968), pp.439–470.
 
  [Ja92] U. Janssen. Motives, numerical equivalence, and semi–simplicity. Invent. Math. 107 (1992), 447–452. 
  
  [Mo91] Motives. Proc. Summer Research Conference, 1991. Eds. U. Janssen, S. Kleiman, J.–P. Serre. Proc. Symp. in Pure Math., vols. 55.1, 55.2, AMS 1994. 
  
  [VoSuFr00] V. Voevodsky, A. Suslin, E. Friedlander. Cycles, transfers, and motivic homology theories. Ann. Math. studies, Princeton UP, 2000. 
  
  [A04] Y. Andr ́e. Une Introduction aux Motifs (motifs purs, motifs mixtes, p ́eriodes). Panoramas et Synth ́eses, Nr. 17, Soc. Math. de France, 2004. 
  
  [Or05] D. Orlov. Derived categories of coherent sheaves and motives. arXiv:math/0512620 
  
  [Be83] A. Beilinson. The derived category of coherent sheaves on Pn. Selecta Math. Soviet. 3, 1983, pp. 233–237. 
  
  [Ta11] G. Tabuada. A guided Tour through the Garden of Noncommutative Motives. arXiv:1108.3787
  
   [QFS99] Quantum Fields and Strings: A Course for Mathematicians. Vols. 1, 2. Ed. by P. Deligne, Ed Witten, et al., AMS, 1999. 
   
   [De02] P. Deligne. Cat ́egories tensorielles. (Dedicated to Yuri I. Manin on the occasion of his 65th birthday.) Mosc. Math. J. 2 (2002), no. 2, 227–248. 
   
   [BehM96] K. Behrend, Yu. Manin. Stacks of stable maps and Gromov–Witten invariants. Duke Math. J., 85, no.1, 1996, pp. 1–60.