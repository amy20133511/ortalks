---
title: "[Tech Talk #39] 开源FinRL和FinGPT"
#subtitle: ""
date: 2023-05-12T21:30:00+08:00
lastmod: 2023-05-12T21:30:00+08:00
draft: false
author: "刘小洋"
authorLink: ""
license: ""
tags: ["LLM", "强化学习", "FinGPT", "FinRL", "金融数据处理"]
categories: ["金融 Finance"]
#series: "Tech Talk"
featuredImage: ""
featuredImagePreview: ""
summary: "本次分享中，刘小洋博士将介绍FinGPT——金融领域的大模型架构，并重点分享金融强化学习中由于金融数据的高度动态性而呈现出独特的挑战及其解决方案。"
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
深度学习革命始于卷积神经网络AlexNet在ImageNet 2012挑战赛中的获胜，而开源框架PyTorch进一步促进了模型创新，推动了该领域的进一步发展。最近，数据在人工智能中变得越来越重要，导致数据中心的人工智能的出现。在这次演讲中，我将分享我使用ImageNet-21K数据集的经验，该数据集是静态ImageNet-1K数据集的一个更大版本，以及我如何利用机器学习、信号处理和计算之间的相互作用来实现进一步的进展。

作为开源项目FinRL、ElegantRL和FinGPT的创建者，我将讨论我使用这些工具应对金融市场这一具有挑战性的领域的经验。金融强化学习由于金融数据的高度动态性而呈现出独特的挑战。FinRL和FinGPT建立在深度学习的成功基础上，我将主要关注一个自动数据筛选管道，该管道解决了处理金融数据所面临的挑战。

## 嘉宾介绍
{{< figure src="/tech_images/tech_39/speaker.png" title="刘小洋" width="200">}}

**刘小洋**，哥伦比亚大学电子工程系博士，开源项目FinRL，ElegantRL和FinGPT的主创。研究方向为量子张量网络和深度学习，AI领域活跃学者（专注于算法设计和开源库开发）。

小雅 ElegantRL是一个基于PyTorch的轻量-高效-稳定的深度强化学习框架；FinRL是一个解决量化交易的开放源代码库，可为从业人员提供流水线式的策略开发的统一框架；FinGPT是金融领域的开源大语言模型框架。

## 观众提问
大量关于 **RL/LLM/金融数据处理** 的应用讨论（“**坑**”）请移步B站录播视频，自行食用。

## 直播回放
{{< bilibili BV1dT411x7eC >}}

## 相关资料及延伸阅读

- Github: 

  https://github.com/AI4Finance-Foundation

  https://ai4finance-foundation.github.io/FinNLP/

  论文：

  [1] Xiao-Yang, Liu, Xiaodong Wang, et al. Spectral Tensor Layers for Communication-free Distributed Deep Learning. (Major revision) IEEE Transactions on Neural Networks and Learning Systems. 

  [2] Xiao-Yang, Liu, et al. "Dynamic Datasets and Market Environments for Financial Reinforcement Learning." arXiv preprint arXiv:2304.13174 (2023). 

  [3] Xiao-Yang, Liu, et al. "FinRL-Meta: Market Environments and Benchmarks for Data-Driven Financial Reinforcement Learning." Advances in Neural Information Processing Systems 35 (2022): 1835-1849. 

  [4] Xiao-Yang Liu, et al. FinRL: Deep reinforcement learning framework to automate trading in quantitative finance. ACM International Conference on AI in Finance, 2021. 

  [5] Xiao-Yang Liu, Michael I. Jordan, et al. "ElegantRL-Podracer: Scalable and elastic library for cloud-native deep reinforcement learning." Deep reinforcement learning workshop, NeurIPS, 2021.

## 往期直播及相关推文

- [直播回顾｜哥大 刘小洋：开源FinRL助力数字经济 「TechTalk 36」](http://mp.weixin.qq.com/s?__biz=Mzk0ODMwMjMwMA==&mid=2247590027&idx=2&sn=d25eef0c58cae39a624a35c3a712bfed&chksm=c36a9838f41d112e689e70adc14c03dd44a2aab490eefd0a2413034e7efb69d44d9e713d07dc&scene=21#wechat_redirect)

- [AI4Finance: 从AlphaGo到FinRL｜ 行业InTalk 第三季金融科技专场No.3](http://mp.weixin.qq.com/s?__biz=Mzk0ODMwMjMwMA==&mid=2247527755&idx=1&sn=6cdc66989d04af64c8273094396a5029&chksm=c36b95f8f41c1ceea6f41db8a5342df81f5b2992b667f01170b365f7ec1e467f48125c7e9f23&scene=21#wechat_redirect)

  [OM | ElegantRL: 基于PyTorch的轻量-高效-稳定的深度强化学习框架](http://mp.weixin.qq.com/s?__biz=Mzk0ODMwMjMwMA==&mid=2247527831&idx=1&sn=c92cddc9eb9699dace14842b8d6e1ef3&chksm=c36b9524f41c1c32f667334918c38fef80776ec7633c48aa989e3f0308b7614d155a66f99b56&scene=21#wechat_redirect)