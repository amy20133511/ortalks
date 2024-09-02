---
title: "Tech Talk 40: 针对双边约束的在线资源分配问题的接近最优算法"
#subtitle: ""
date: 2023-05-27T20:00:00+08:00
lastmod: 2023-05-27T20:00:00+08:00
draft: false
author: "陈再毅"
authorLink: ""
license: ""
tags: ["在线资源分配", "双边约束", "分布式", "供应链", "物流"]
categories: ["供应链 Supply Chain"]
#series: "Tech Talk"
featuredImage: ""
featuredImagePreview: ""
summary: "本次分享中，陈再毅博士将介绍在线资源分配问题中的接近最优算法，特别是在存在双边约束的情况下。他将讨论算法的设计思路、理论分析以及在供应链和物流领域的应用实践。"
hiddenFromHomePage: false
hiddenFromSearch: false
toc:
  enable: true
  auto: true
mapbox:
share:
  enable: true
comment:
  enable: true
---



## 分享摘要
在线资源分配问题是计算机科学和运筹优化领域中的一个重要问题。在供应链和物流领域，我们发现实时流量调控也可以被建模为在线资源分配问题，但资源大都同时具有上下界双边约束。最大化目标函数的分配问题中，下界约束在管理学中被定义为公平性(fairness)约束，这类约束具备实际的合理性并在市场中广泛存在。然而在有限样本的情况下，已有在线算法无法保障约束的满足。为解决该问题，我们定义了“可行性”测度(measure of feasibility)ξ” 来衡量有解时问题的难度。在在线场景下，我们基于集中不等式(concentration inequality)构造出算法框架，并按阶段使用已分配的历史样本对算法参数进行逐渐精确的估计。通过理论分析，我们证明算法在该场景下有接近最优的竞争比，相关结果已发表ICML’2023。另外，我们通过高效的分布式实现取得了良好的实际表现。

## 嘉宾介绍
{{< figure src="/tech_images/tech_40/speaker.png" title="陈再毅" width="200">}}

**陈再毅**，2019年于中国科学技术大学获得计算机博士学位，期间主要从事一阶优化算法相关的研究，发表数篇ICML、ICLR等机器学习领域顶会论文。目前在菜鸟网络担任高级算法专家，专注于物流、供应链领域的组合问题近似算法、在线决策算法和相关的实际应用。

## 观众提问
Q: 在什么情况下引入统计学的相关知识可能会得到比较好的优化效果？和优化问题的规模有关吗？
A: 当优化问题存在随机性的时候可以考虑引入统计学。和优化问题的规模有关。

Q: 样本收集的规模需要达到什么水平才能达到一个比较准确的概率估计？
A: 从物流的实践来看，能收集到多少有效的样本取决于业务场景，我们的经验大概是有几百的样本量水平就可以达到百分位误差的估计。

Q: 请问下考虑非平稳有作用吗？
A: 有作用。但面向实践使用的算法上考虑非平稳目前还没有很好的解决方案。

**详细解答以及大量关于随机优化/强化学习/启发式算法的应用讨论（“坑”）请移步B站录播视频，自行食用。**

## 直播回放
{{< bilibili BV1eo4y1K7Sh >}}

## 相关资料及延伸阅读

- Shipra Agrawal, Zizhuo Wang, and Yinyu Ye. "A dynamic near-optimal algorithm for online linear programming." *Operations Research*, 62(4):876–890, 2014.
- Nikhil R Devanur, Kamal Jain, Balasubramanian Sivan, and Christopher A Wilkens. "Near optimal online algorithms and fast approximation algorithms for resource allocation problems." *Journal of the ACM (JACM)*, 66(1):7, 2019.

## 往期直播及相关推文

- [直播回顾 | 阿里 吴悠：阿里达摩院MindOpt优化求解器最新进展 「TechTalk 37」](http://mp.weixin.qq.com/s?__biz=Mzk0ODMwMjMwMA==&mid=2247601082&idx=2&sn=73d94c55a226fa9321c3c5b38a48a532&chksm=c36ab309f41d3a1f32ec89fd57af9b95f3a38fb8567b25e3138d3a699debf610ba7af084eac9&scene=21#wechat_redirect)
- [优化 | 如何建模多类用户、多类资源的在线分配问题？](https://mp.weixin.qq.com/s?__biz=Mzk0ODMwMjMwMA==&mid=2247594203&idx=1&sn=72603766c5071ae29922b7f54a2ad391&chksm=c36a8868f41d017e5ff23f0f4fd64cc15038de301e7210e82762ccbea4883ce9fe3cb6d40dec&scene=21#wechat_redirect)
- [OM | 突传染病的资源分配：贪婪、近似和动态策略](http://mp.weixin.qq.com/s?__biz=Mzk0ODMwMjMwMA==&mid=2247527450&idx=1&sn=5c071b7b09279598afc4a29c4f15d0f9&chksm=c36b94a9f41c1dbf3ac19a1e0981cce93c8376be609727183b4684012f9e4795085d190f4135&scene=21#wechat_redirect)