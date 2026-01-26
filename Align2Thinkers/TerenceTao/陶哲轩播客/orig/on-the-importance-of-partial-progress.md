---
title: On the importance of partial progress
date: 2019-09-22T16:44:26+00:00
source_url: https://terrytao.wordpress.com/career-advice/on-the-importance-of-partial-progress/
fetched_at: 2025-10-11T08:50:35.181678Z
status: 200
categories:
  - mathematics
  - problem-solving
  - education
tags:
  - partial-progress
  - mathematical-thinking
  - problem-solving-techniques
  - integration
  - graduate-student
  - mathematical-mindset
toc: true
show_title: false
---

[中文版本](../zh/on-the-importance-of-partial-progress.zh.md)
[原博客链接](https://terrytao.wordpress.com/career-advice/on-the-importance-of-partial-progress/)


# On the importance of partial progress

*[Initially posted on Google+ on July 17, 2012. -T]*

One of the secrets to mathematical problem solving is that one needs to place a high value on partial progress, as being a crucial stepping stone to fully solving the problem. This can be a rather different mindset than what one commonly sees in more "real world" situations such as business, sports, engineering, or politics, where actual success or failure often matters much more than what one can salvage from a partial success. I think the basic reason for this is that in the purely theoretical world of mathematics, there is basically a zero cost in taking an argument that partially solves a problem, and then combining it with other ideas to make a complete solution; but in the real world, it can be difficult, costly, or socially unacceptable to reuse or recycle anything that is (or is perceived to be) even a partial failure. Software engineering is one of the few exceptions to this general rule, as it is almost as easy to reuse software code as it is to reuse a mathematical argument.

For beginning maths students, who have not yet adopted the partial progress mindset, it is common to try a technique to solve a problem, find out that it "fails", and conclude that one needs to try a completely different technique (or to give up on the problem altogether). But in practice, what often happens is that one's first solution attempt is able to solve some portion of the problem, and one needs to then look to combine that argument with techniques that can solve complementary portions of the problem in order to reach the final solution.

For instance, recently a graduate student came to me with an integral on the real line he was trying to estimate. He had tried integration by parts, and found that the resulting terms from that integration behaved well on one side of the real line, but diverged on the other. A beginner might have given up on this method at this point; but having already had some mathematical experience, he realised that this was a partial success, and split the real line into two pieces, using integration by parts to control the integral on one piece, and a different technique (Taylor expansion of the integrand) to control the other integral. Unfortunately, when he added up the estimates, he found that no matter how where he divided the real line into two, the total estimate still fell short of what he wanted, at which point he came to me for help. But actually, this failure was in fact further partial progress; he had discovered one method (integration by parts) that handled the integral for large positive values of the integration parameter, and another (Taylor expansion) that handled large negative values, and all that remained was to add a third technique (which, in this case, was crude estimation by replacing everything by its absolute value) to treat the intermediate values which were not well handled by the previous two techniques. Thus the first two "failures" were in fact crucial advances that were needed to solve the full problem, by resolving at least some of the difficulties present of the problem, and in focusing attention on the remaining issues that needed resolution.

One corollary of the partial progress mindset is that it can often be profitable to try a technique on a problem even if you know in advance that it cannot possibly solve the problem completely. (For instance, the technique may be unable to distinguish between the actual problem $P$, and a similar-looking problem $P'$ for which the answer is already known to be negative. Or the technique may already be known to many experts who have tried for many years to solve $P$, which gives strong empirical evidence that this technique is insufficient for the problem. Or, the technique has no chance to solve the full problem $P$, but can only hope to solve "toy" or "model" instances $P_0$ of the problem in which some (but crucially, not all) of the difficulties have been removed.) The point is that even if the technique is doomed to fail, the precise point in the argument at which it fails can be very instructive, as it can delineate what portion of the problem can be handled (in principle, at least) by such arguments, and it highlights the key component of the problem which needs a further tool to resolve, and to which one can then focus attention on.
