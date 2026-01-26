---
title: Be sceptical of your own work
date: 2007-05-06T18:57:36+00:00
source_url: https://terrytao.wordpress.com/career-advice/be-sceptical-of-your-own-work/
fetched_at: 2025-10-11T08:51:03.899933Z
status: 200
categories:
  - mathematics
  - research
  - problem-solving
tags:
  - skepticism
  - proof-validation
  - error-detection
  - mathematical-reasoning
  - research-methodology
toc: true
show_title: false
---

[中文版本](../zh/be-sceptical-of-your-own-work.zh.md)
[原博客链接](https://terrytao.wordpress.com/career-advice/be-sceptical-of-your-own-work/)


# Be sceptical of your own work

> An expert is a man who has made all the mistakes, which can be made, in a very narrow field.
> — Niels Bohr

If you unexpectedly find a problem solving itself almost effortlessly, and you can't quite see why, you should try to analyse your solution more sceptically.

In particular, the method may also be able to prove much stronger statements which are known to be false, which would imply that there is a flaw in the method.

In a related spirit, if you are trying to prove some ambitious claim, you might try to first look for a counterexample; either you find one, which saves you a lot of time and may well be publishable in its own right, or else you encounter some obstruction, which should give some clue as to what one has to do in order to establish the claim positively (in particular, it can "identify the enemy" that has to be neutralised in order to conclude the proof).

Actually, it's not a bad idea to apply this type of scepticism to other mathematician's claims also; if nothing else, they can give you a sense of why that claim is true and how powerful it is.

A sceptical attitude towards your own work should be **especially** enforced when dealing with a problem which is known to be difficult (and this includes most "famous problems"), or one which is outside your usual area of expertise. In particular, if your solution to that problem resembled this process:

1. Transform the difficult problem to another difficult problem.
2. Transform the problem again to yet another difficult problem.
3. ...
4. Transform the problem again to yet another difficult problem.
5. Transform the problem again. Suddenly the problem becomes much simpler!
6. Transform the simple problem to another simple problem.
7. ...
8. Transform the simple problem again to another simple problem.
9. Solve the last simple problem. Done!

then there is almost certainly a major error in your argument in Step 5. (This is especially true if the difficulty of the transformed problem had been steadily **increasing** through steps 1-4.) At a bare minimum, this suspicious step should be thoroughly checked and rechecked, any hand-waving arguments near this step should be written out in full, and some analysis should be undertaken as to understanding what exactly was the decisive step in the argument that dramatically simplified the problem, and how that step could be so powerful as to achieve such a simplification.

Here is another common type of suspicious argument:

1. To prove Famous Conjecture X, use reductio ad absurdum, and assume for sake of contradiction that X is false.
2. Do some random computations of tangential relevance to X.
3. Do some more random computations of this type.
4. ...
5. Do another random computation, but this time unwittingly make a sign error, division by zero, or similar mistake.
6. Do yet more random computations.
7. ...
8. Notice that two of your computations are inconsistent with each other.
9. Congratulations – you've obtained the desired contradiction. Declare victory!

A good way to stress-test this sort of false argument is to try to run the same argument **without** the initial assumption that X is false. If one can easily modify the argument to again lead to a contradiction, it shows the problem wasn't with X – it was with the argument. A classic example here would be a "proof" that the existence of non-trivial natural number solutions to the equation `a^n + b^n = c^n` leads to a contradiction, which mysteriously fails to use in any significant way the hypothesis that `n > 2` and would in fact would also work (perhaps after some small modification) for `n = 2` also. Another good practice is to take an argument that you first found using reductio ad absurdum, and try to untangle it to create a more direct proof that avoids reductio ad absurdum. If the argument is fairly "linear" in nature, this should end up with a simpler and more streamlined argument (which is **part of the rewriting process** in any event), and can often also catch errors of the type in Step 5 above.

Another warning sign is if the computations lead you further and further away from the mathematical topics and connections that X is supposed to be addressing (e.g. a proposed proof of the Riemann hypothesis that proceeds almost entirely using the theory of meromorphic functions, with almost no reference to integers, primes, or other basic number-theoretic concepts; or, conversely, an argument that proceeds entirely by working with the integers, with barely any reference to the zeta function).

A final type of warning sign is if your approach is based on adapting a method that has been used frequently in the past by many experts in the field, but with an additional twist of your own that all the previous experts somehow "missed". In such situations, there is a high probability that this twist contains a serious technical flaw that the previous experts were aware of and avoided, and a particularly high level of scepticism is warranted in such situations.

For comparison, actual solutions to a major problem tend to be arrived at by a process more like the following (often involving several mathematicians over a period of years or decades, with many of the intermediate steps described here being significant publishable papers in their own right):

1. Isolate a toy model case x of major problem X.
2. Solve model case x using method A.
3. Try using method A to solve the full problem X.
4. This does not succeed, but method A can be extended to handle a few more model cases of X, such as x' and x".
5. Eventually, it is realised that method A relies crucially on a property P being true; this property is known for x, x', and x", thus explaining the current progress so far.
6. Conjecture that P is true for all instances of problem X.
7. Discover a family of counterexamples y, y', y", … to this conjecture. This shows that either method A has to be adapted to avoid reliance on P, or that a new method is needed.
8. Take the simplest counterexample y in this family, and try to prove X for this special case. Meanwhile, try to see whether method A can work in the absence of P.
9. Discover several counterexamples in which method A fails, in which the cause of failure can be definitively traced back to P. Abandon efforts to modify method A.
10. Realise that special case y is related to (or at least analogous to) a problem z in another field of mathematics. Look up the literature on z, and ask experts in that field for the latest perspectives on that problem.
11. Learn that z has been successfully attacked in that field by use of method B. Attempt to adapt method B to solve y.
12. After much effort, an adapted method B' is developed to solve y.
13. Repeat the above steps 1-12 with A replaced by B' (the outcome will of course probably be a little different from the sample storyline presented above). Continue doing this for a few years, until all model special cases can be solved by one method or another.
14. Eventually, one possesses an array of methods that can give partial results on X, each of having their strengths and weaknesses. Considerable intuition is gained as to the circumstances in which a given method is likely to yield something non-trivial or not.
15. Begin combining the methods together, simplifying the execution of these methods, locating new model problems, and/or finding a unified and clarifying framework in which many previous methods, insights, results, etc. become special cases.
16. Eventually, one realises that there is a family of methods A^* (of which A was the first to be discovered) which, roughly speaking, can handle all cases in which property P^* (a modern generalisation of property P) occurs. There is also a rather different family of methods B^* which can handle all cases in which Q^* occurs.
17. From all the prior work on this problem, all known model examples are known to obey either P^* or Q^*. Formulate Conjecture C: all cases of problem X obey either P^* or Q^*.
18. Verify that Conjecture C in fact implies the problem. This is a major reduction!
19. Repeat steps 1-18, but with problem X replaced by Conjecture C. (Again, the storyline may be different from that presented above.) This procedure itself may iterate a few times.
20. Finally, the problem has been boiled down to its most purified essence: a key conjecture K which (morally, at least) provides the decisive input into the known methods A^*, B^*, etc. which will settle conjecture C and hence problem X.
21. A breakthrough: a new method Z is introduced to solve an important special case of K.
22. The endgame: method Z is rapidly developed and extended, using the full power of all the intuition, experience, and past results, to fully settle K, then C, and then at last X.
23. The technology developed to solve major problem X is adapted to solve other related problems in the field. But now a natural successor question X' to X arises, which lies just outside of the reach of the newly developed tools… and we go back to Step 1.

See also "[Learn the limitations of your tools](Learn the limitations of your tools)", "[Ask yourself dumb questions](Ask yourself dumb questions)", "[Think ahead](Think ahead)", and "[Use the wastebasket](Use the wastebasket)".
