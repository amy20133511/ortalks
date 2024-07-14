---
title: "【Tech Talk第41期】 哥大 彭天翼：当A/B实验平台遇上强化学习"
#subtitle: ""
date: 2023-09-03T10:00:00
draft: false
author: ""
authorLink: ""
license: ""
tags: ["A/B测试", "实验设计", "实验干扰", "off-policy evaluation", "强化学习"]
categories: ["应用统计"]
#series: "Tech Talk"
featuredImage: ""
featuredImagePreview: ""
summary: "A/B测试面临实验干扰问题，影响结果可靠性。我们提出基于强化学习的\"Difference-in-Q\"(DQ)估计器，通过求解Q值差分估计treatment effect。理论上，DQ在偏差-方差权衡方面表现出色，显著降低偏差，方差指数级缩减。与抖音合作应用于大规模商业场景，均方误差减少99%以上，展现卓越性能。"
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
在当今互联网时代，A/B测试已被奉为评估算法效果的黄金标准。然而，Interference问题（即不同实验单元相互影响的现象）却一直是A/B测试中的一大挑战。这一问题的存在使得业界投入巨大资金构建的实验平台的测试结果变得不再可靠。为了克服Interference问题，我们提出了一种基于强化学习框架的创新方案，用于重新审视A/B测试。该方案通过求解强化学习中的Q值的差分来估计treatment effect，因此我们将其命名为“Difference-in-Q”（简称DQ）estimator。从理论角度看，我们发现DQ在bias-variance trade-off方面表现出色：一方面，DQ显著减少了传统estimator的bias；另一方面，DQ的variance较任何unbias estimator都可以实现指数级的缩减。我们与抖音公司合作，将DQ应用于大规模商业场景，在初步测试中，其均方误差减少了超过99%。同时，在商业级共享汽车模拟器中，DQ也展现出了卓越的性能。在本次演讲中，我将介绍DQ的理论与实践，并探讨下一代智能实验平台的设计与展望。


## 嘉宾介绍
{{< figure src="/tech_images/tech_41/speaker.png" title="彭天翼" width="200">}}

哥伦比亚大学商学院决策风险与运筹系助教教授（拟入职）。他于2023年取得麻省理工学院博士学位，2017年毕业于清华大学姚班。现于Cimulate.AI担任首席人工智能研究员。他的研究兴趣聚焦于生成式人工智能，强化学习，和因果推断。他喜欢关注前沿理论问题在实际问题中的应用，并曾与字节跳动，百威啤酒，the Broad Institute等公司展开合作。他曾获得INFORMS Daniel H. Wagner实践卓越奖，Applied Probability Society Best Student Prize，RMP Jeff McGill Student Paper Award，和MSOM Best Student Prize Finalist。

 
## 观众提问
A/B测试是否可以扩展到A/B/C/D等多组场景？
: 可以。方法论上具有很强的可扩展性，但是需要修改相应的数学描述。


A/A测试中的两个A是指不同版本间的比较吗？
: 不是，A/A测试是对于同一个算法的分流测试。在这种情况下，真实的treatment effect是0。它一般用于检查estimator的鲁棒性或者估计estimator的方差。A/A测试可以对用户分成两组测试，有时也会分成两个时间段测试。

关于DQ方法的灵感/直觉来源什么？
: 从RL的角度来看，interference的产生主要是由于当下的action会影响到未来的reward。所以我们消除interference的方法就采用了未来的reward总和（也就是Q-value）来代替当下的reward去计算两组实验的差值。我们在抖音场景下举了两个例子来进一步阐释，具体内容欢迎观看video或者阅读论文。

**详细解答以及大量关于 A/B测试/强化学习/Interference 的应用讨论（“坑”）请移步B站录播视频，自行食用。**

---

## 直播回放
{{< bilibili BV11G411R7hR >}}

## 相关资料及延伸阅读
- Farias, Vivek, Andrew Li, Tianyi Peng, and Andrew Zheng. "Markovian interference in experiments." *Advances in Neural Information Processing Systems* 35 (2022): 535-549.
- Farias, Vivek F., Hao Li, Tianyi Peng, Xinyuyang Ren, Huawei Zhang, and Andrew Zheng. "Correcting for Interference in Experiments: A Case Study at Douyin." *Accepted by RecSys 2023.
---

### 往期直播及相关推文
- [专访｜华人运筹学新星、MIT博士生 彭天翼：协助全球最大啤酒生产集团进行销售决策](https://mp.weixin.qq.com/s/GSfAatYmLMcVna1Q12exHA)
- [OM | 美团配送A/B评估体系建设与实践](https://mp.weixin.qq.com/s/9TjC9NWeA492lpydyrDr2A)
- [初识滴滴交易策略之一：交易市场](https://mp.weixin.qq.com/s/qPPycUikDrHZFoGij3I-pg)

---
 