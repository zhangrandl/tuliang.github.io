---
layout: post
title: 麻省理工《计算机科学及编程导论》第十二课
category: open
---
##调试、背包问题、动态规划简介

大体上说，最优化问题（optimization problem）都差不多。包括两部分，一些你想获得最大或最小值的函数，还必须符合一些约束条件。典型的最优化问题，其中一个最著名的是最短路径问题。另一类的最优化问题是旅行商问题（traveling salesman problem）。装箱问题（bin packing），用大小不同形状不同的东西填装容器。 序列比问题（sequence alignment），例如DNA序列，RNA序列。还有一个最优化问题，背包问题（knapsack problem）。

背包问题具体来说是，你有一堆东西，东西比较多背包放不下，你需要选择带什么，留下什么。你需要在背包能带东西有限的情况下，最大化你所带东西的价值。

在贪婪算法中，需要在每一步最大化你的值。不用提前计划，做好当前的事情就好。就像是有些人吃东西时先吃甜点，这样能够保证在吃饱前吃到最好的东西。

局部的最优化并不能保证全局的最优化。所以，你不能重复的进行局部优化，期望得到全局的最优。

动态规划（dynamic programming），不要在这个名字上花费精力。这个方法由数学家贝尔曼发明，国防部曾经让他帮忙做一些工作，他不想让他们知道他在做什么，所以他编造了一个与此毫不相关的名字。不幸的是，我们一直沿用至今。所以不要认为，它特指任何动态的东西。它能解决很多表面上是指数增长的问题，关键有两点，一是找到重叠子问题，二是所谓最优子结构。