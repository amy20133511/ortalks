---
title: "[OR Talk #22] 一种城市无人机空运航线网络规划方法"
#subtitle: ""
date: 2023-04-29T20:00:00
draft: false
tags: []
categories: []
summary: "对于城市空中运输中，有效管理大量无人机在复杂城市环境中的交通是扩展空运服务的关键。我们提出一种通过优先级排序和解耦NP-hard问题的方法，以快速规划复杂城市环境中的航线网络，并引入空间成本函数以设计密集对齐的航线网络。测试结果显示，该方法生成的航线网络接近最优且节省计算时间。"
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
当前高科技巨头和初创企业都在积极投资无人机技术以提供城市空中运输服务。然而，如果无法在复杂的城市环境中对大量无人机进行有效的交通管理，空运服务将无法扩大。目前基于管道形式的运营管控概念所设计的航线网络已在全球部分地区用于无人机快递业务，未来有望继续服务于密集复杂空域下的场景。针对管道形式的运营管控概念，该报告将介绍一种航线网络规划方法以设计复杂城市环境中的航线网络。该方法通过对机场OD对进行优先级排序并依次规划，以考虑商业需求。它将 NP-hard 的网络规划问题解耦为一系列单路径规划问题以进行快速规划。我们还引入了一种空间成本函数，以支持设计密集且对齐的航线网络。所提出的方法在各种场景中进行了测试，并与其他方法进行比较。结果表明，我们的方法可以生成接近最优的航线网络，并且可以显著节省计算时间。


## 分享提纲
1. 无人机交通管理的背景及文献综述
2. 介绍无人机物流网络规划问题表述
3. 介绍一个基于优先级的启发式规划算法
4. 讨论未来可能相关研究的方向 


## 嘉宾介绍
{{< figure src="/or_images/or_22/speaker1.png" title="李立帅" width="200">}}
香港城市大学数据科学学院的副教授。于复旦大学飞行器设计与工程专业获得本科学位，并于麻省理工学院航空航天系获得硕士和博士学位。她是世界经济论坛 (World Economic Forum)的全球未来理事会的成员并在2022年被斯坦福-爱思唯尔指标 (单年)评为全球前2%的被引用最多的学者之一。其研究着眼于智能交通系统和数据科学的跨学科领域。包括利用大规模运营数据开发各类数据分析方法，用于传统航空航空安全管理和运营改进、空中交通管理和预测，和列车系统的健康监测。其正在研究无人机送货服务和城市空中交通的交通管理问题和基础设施挑战。 


{{< figure src="/or_images/or_22/speaker2.png" title="何鑫宇" width="200">}}
香港城市大学数据科学学院在读博士生。研究方向为城市空中交通航路网络设计，无人机系统交通管理，相关研究成果发表于 Transportation Research Part E 等高水平期刊。


## 直播回放
{{< bilibili BV1Ka4y1G75P >}}

## 相关资料及延伸阅读
- 论文链接：[A route network planning method for urban air delivery](https://doi.org/10.1016/j.tre.2022.102872)

---