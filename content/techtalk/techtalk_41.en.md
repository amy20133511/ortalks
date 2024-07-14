---
title: "[TechTalk No. 41] Columbia DRO Tianyi Peng: When A/B Testing Platforms Meet Reinforcement Learning"
#subtitle: ""
date: 2023-09-03T10:00:00
draft: false
author: ""
authorLink: ""
license: ""
tags: ["A/B testing", "experiment design", "interference", "off-policy evaluation", "reinforcement learning"]
categories: ["Applied Statistics"]
#series: "Tech Talk"
summary: "A novel \"Difference-in-Q\" (DQ) estimator, based on reinforcement learning, is proposed to address the Interference problem in A/B testing. DQ outperforms traditional estimators in bias-variance trade-off, reducing bias and exponentially decreasing variance. Collaborating with ByteDance, DQ achieved a 99% reduction in mean squared error in large-scale commercial scenarios."
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


## Talk Abstract
In the current internet era, A/B testing has become the gold standard for evaluating algorithm performance. However, the issue of interference (the phenomenon where different experimental units affect each other) has consistently posed a significant challenge in A/B testing. This problem undermines the reliability of test results from experimental platforms, despite substantial investments from the industry. To address the interference issue, we propose an innovative solution based on a reinforcement learning framework to reassess A/B testing. This solution estimates the treatment effect by solving for the difference in Q-values in reinforcement learning, hence we name it the "Difference-in-Q" (DQ) estimator. Theoretically, we found that DQ performs exceptionally well in terms of the bias-variance trade-off: it significantly reduces the bias of traditional estimators while achieving exponential reductions in variance compared to any unbiased estimator. In collaboration with Douyin, we applied DQ to large-scale commercial scenarios, where preliminary tests showed a reduction in mean squared error by over 99%. Additionally, DQ demonstrated outstanding performance in a commercial-grade car-sharing simulator. In this presentation, I will introduce the theory and practice of DQ, and discuss the design and prospects of the next generation of intelligent experimental platforms.


## About the Speaker
{{< figure src="/tech_images/tech_41/speaker.png" title="Tianyi Peng" width="200">}}

Assistant Professor (appointed) in the Decision, Risk, and Operations Division at Columbia Business School. He earned his Ph.D. from the Massachusetts Institute of Technology in 2023 and graduated from the Yao Class at Tsinghua University in 2017. Currently, he serves as the Chief AI Researcher at Cimulate.AI. His research interests focus on generative artificial intelligence, reinforcement learning, and causal inference. He enjoys exploring the application of cutting-edge theoretical problems to real-world issues and has collaborated with companies such as ByteDance, Anheuser-Busch, and the Broad Institute. He has received several awards, including the INFORMS Daniel H. Wagner Prize for Excellence in Operations Research Practice, the Applied Probability Society Best Student Prize, the RMP Jeff McGill Student Paper Award, and was a finalist for the MSOM Best Student Prize.

 
## Q&A
Can A/B testing be extended to scenarios with multiple groups like A/B/C/D?
: Yes, it can. The methodology is highly scalable, but it requires modifications to the corresponding mathematical descriptions.


In A/A testing, does the two A’s refer to comparisons between different versions?
: No, A/A testing refers to split testing of the same algorithm. In this case, the true treatment effect is 0. It is generally used to check the robustness of the estimator or to estimate the variance of the estimator. A/A testing can divide users into two groups for testing, and sometimes it is also conducted across two different time periods.


What is the inspiration/intuition behind the DQ method?
: From the perspective of reinforcement learning (RL), interference mainly arises because the current action affects future rewards. Therefore, our method to eliminate interference uses the sum of future rewards (i.e., Q-value) instead of the current reward to calculate the difference between the two experimental groups. We provided two examples in the Douyin scenario to further explain this, and for more details, you are welcome to watch the video or read the paper.

---

## Livestream Video
{{< bilibili BV11G411R7hR >}}


## Relevant Papers & Recommended Reading
- Farias, Vivek, Andrew Li, Tianyi Peng, and Andrew Zheng. "Markovian interference in experiments." *Advances in Neural Information Processing Systems* 35 (2022): 535-549.
- Farias, Vivek F., Hao Li, Tianyi Peng, Xinyuyang Ren, Huawei Zhang, and Andrew Zheng. "Correcting for Interference in Experiments: A Case Study at Douyin." *Accepted by RecSys 2023.
---


### Past Talks & Related Articles
- [Interview｜Rising Star in Operations Research and MIT PhD Student Peng Tianyi: Assisting the World's Largest Beer Production Group in Sales Decisions](https://mp.weixin.qq.com/s/GSfAatYmLMcVna1Q12exHA)
- [OM | Meituan's A/B Evaluation System Construction and Practice](https://mp.weixin.qq.com/s/9TjC9NWeA492lpydyrDr2A)
- [Introduction to Didi's Trading Strategies Part One: Trading Market](https://mp.weixin.qq.com/s/qPPycUikDrHZFoGij3I-pg)

---