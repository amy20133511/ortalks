---
title: "Tech Talk 38: 精确算法，精准决策：用“交互式优化”解决学校上下学时间问题"
#subtitle: ""
date: 2023-03-11T09:00:00+08:00
lastmod: 2023-05-12T09:00:00+08:00
draft: false
author: "连真"
authorLink: ""
license: ""
tags: ["Optimization","Interactive", "Decision support", "Public policy","School Schedules"]
categories: ["智能决策 Smart Decision"]
#series: "Tech Talk"
featuredImage: ""
featuredImagePreview: ""
summary: "本次分享中，连真博士将介绍使用交互式优化算法在美国首次实现学校时间更改的实践经验。"
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
基于与旧金山联合校区 (San Francisco Unified School District, SFUSD) 的合作，本文为复杂的公共政策问题定制了一个系统性解决方案（“交互式优化”框架）。这些公共政策问题常常存在着“先有鸡还是先有蛋”的困境：政策制定者了解目标和约束，但缺乏解决问题的能力（“优化问题”），而研究人员具备必要的算法，但缺乏对政策背景的必要洞察力（“政策问题”）。我们的框架通过结合三个关键要素来应对这一挑战：（1）一个高效的优化算法，可以在已知政策目标的情况下解决问题，（2）一种生成大量多样化、接近最优解的方法，以及（3）一个辅助政策制定者探索解决方案的交互式工具。我们在旧金山联合学区针对其上下学时间表问题应用了这套方案；截止2021年8月， 我们为该学区节省了超过500万美元的经费。据我们所知，这是美国首次成功实现基于优化算法的学校时间更改。

## 嘉宾介绍
{{< figure src="/tech_images/tech_38/speaker.png" title="连真" width="200">}}

**连真**，is a postdoctoral fellow at Lyft Rideshare Labs. At the intersection of operations and economics, her research focuses on (1) the implications of marketplaces such as ride-hailing, and (2) transportation and public policy. Prior to Lyft, Zhen obtained her PhD from Cornell university. In Summer 2023, Zhen will join Yale School of Management as an assistant professor.

## 观众提问
**Q:** 你们关于旧金山学区的研究是否具有普适性，即是否可以应用到其他学区？亦或是具有一定的特殊性，只适用于旧金山学区？

**A:** 每个学区都有很独特的地方，跟城市有很大的关系。我们的成功一定程度上依赖于旧金山学区的open-minded的culture，很愿意接受scientific的approach。还得益于疫情期间学生及家长在家待了很长一段时间，回到学校后更容易接受政策的改变。但我们的framework从formulation来说还是比较general的，很多其他学区的人也有问我们的软件是否open-source，可能也可以用到他们的学区。

 

大量关于 **优化/公共政策** 的应用讨论请移步B站录播视频，自行食用。

## 直播回放
{{< bilibili BV1oM411p7iG >}}

## 相关资料及延伸阅读



## 往期直播及相关推文

- [直播回顾 | MIT/SMU/CMU 王海：共享交通及相关研究问题 OR Talk](https://mp.weixin.qq.com/s/7fXPMR8oMV3UYFla3vwjGA)
- [人物|公共运筹学研究：Richard Larson的个人旅程](https://mp.weixin.qq.com/s/HgUhszXBvIVriPamDnKaPQ)