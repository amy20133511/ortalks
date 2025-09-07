---
title: "ORTalk 33: Texas Tech 曾文耀 新一代列–约束生成方法" # 在此添加talk的题目
date: 2025-06-15T00:00:00-00:00
draft: false
# 编辑完成后把 `draft` 改成 false (不要双引号)
tags: ["两阶段鲁棒优化","列约束生成"]
categories: [""]
series: "OR Talk"
summary: "提出了针对两阶段鲁棒优化问题的非精确列约束生成方法i-C&CG和混合原式对偶列约束生成方法hC&CG，为不确定性环境下的复杂决策问题提供更强大、更可靠的计算工具" # 在此添加talk总结
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
两阶段鲁棒优化（RO）是处理不确定性决策问题的关键技术，但其求解过程通常计算成本高昂且充满挑战。本报告聚焦于经典的**列-约束生成（C&CG）**算法框架，旨在提升其求解效率。C&CG方法通过在主问题（Master Problem）和子问题（Subproblem）之间迭代，逐步构建并求解问题的精确形式。
在此基础上，本报告提出两种创新的改进算法：
第一种是非精确C&CG（i-C&CG）。该方法针对大规模问题中主问题求解困难的痛点，允许其解在迭代过程中存在不精确性，并通过引入智能的回溯机制来确保算法最终收敛，从而显著提升求解的灵活性与效率。
第二种是混合原始-对偶C&CG（hC&CG）。该方法巧妙地利用第二阶段问题的原始与对偶结构信息，以生成比传统方法更强大、更有效的约束（cuts），从而大幅减少迭代次数，加速算法的整体收-敛速度。
这两种新算法均具备严格的有限收敛性理论保证。最后的数值实验结果也充分证明，我们提出的i-C&CG与hC&CG方法相较于当前最优的C&CG算法，在计算性能上具有显著的优越性。

## 分享提纲
1. 介绍经典的列-约束生成（C&CG）方法及其在求解两阶段鲁棒优化（RO）模型时所面临的局限性。
2. 探讨对经典C&CG方法进行泛化与扩展的非精确C&CG（i-C&CG）方法和混合原始对偶C&CG（hC&CG）方法。
3. 检验这些新型C&CG算法及其变体的收敛性。
4. 展示数值实验结果，以证明我们所提出的C&CG方法具备的计算优势。



## 嘉宾介绍
{{< figure src="/or_images/or_33/speaker_tim.png" title="Man Yiu Tseng(Tim)" width="200">}}
曾文耀（Tim）博士将于2025年秋季在德克萨斯理工大学（Texas Tech University）工业、制造与系统工程系担任助理教授。他目前是理海大学（Lehigh University）工业与系统工程系的博士候选人，导师为Karmel S. Shehadeh教授。他于香港中文大学获得风险管理科学学士及硕士学位。

他的方法论研究兴趣与专长主要集中在数据驱动的随机优化领域，具体包括提出并分析不同的不确定性建模范式，以及设计高计算效率的算法来求解大规模随机优化模型。他的主要应用领域为金融风险管理、医疗健康运筹学和交通运输系统。

他的研究成果已获得Van Hoesen家族最佳论文奖（获奖者）以及青年教师兴趣小组论文奖（与其导师Karmel S. Shehadeh共同入围决赛）。



## 直播回放
{{< bilibili BV1gSNnzME57 >}}


## 相关资料及延伸阅读
- Tsang, M. Y., Shehadeh, K. S., & Curtis, F. E. (2023). An inexact column-and-constraint generation method to solve two-stage robust optimization problems. Operations Research Letters, 51(1), 92-98. 

## 招生广告
Texas Tech工业工程系（IMSE）的曾文耀教授现正招收博士研究生，欢迎具备优化、数学或统计背景的同学申请，具有随机优化研究经验者将优先考虑。如有兴趣加入其研究团队，请将个人简历发送至 mytimtsang@gmail.com。曾教授同时也欢迎在随机优化各方向开展科研合作。发送邮件时请在主题处注明OR Talks。

---

<!-- ### 往期直播及相关推文
- 像这样列举相关的推文。注意符号都是英文符号。
- [推文名称](推文链接)
- [专访｜华人运筹学新星、MIT博士生 彭天翼：协助全球最大啤酒生产集团进行销售决策](https://mp.weixin.qq.com/s/GSfAatYmLMcVna1Q12exHA)
--- -->