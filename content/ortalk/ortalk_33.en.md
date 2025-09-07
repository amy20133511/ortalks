---
title: "[ORTalk #33]: Texas Tech Man Yiu Tseng (Tim) Next-Generation Column-and-Constraint Generation Methods" # 在此添加talk的题目
date: 2025-06-15T00:00:00-00:00
draft: false
# 编辑完成后把 `draft` 改成 false (不要双引号)
tags: ["Two-stage robust optimization","column-and-constraint generation"]
categories: [""]
series: "OR Talk"
summary: "Robust optimization (RO) is a useful methodology for formulating optimization problems in which some parameters are uncertain, but belong to a given uncertainty set. Two-stage RO models have received substantial attention in various application domains because of their ability to provide robust, reliable, and adaptable solutions. However, they are often challenging to solve. In this talk, I will introduce innovative and computationally efficient column-and-constraint generation (C&CG) algorithms for solving two-stage RO problems. C&CG algorithms operate within a master-subproblem framework. ."
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
Robust optimization (RO) is a useful methodology for formulating optimization problems in which some parameters are uncertain, but belong to a given uncertainty set. Two-stage RO models have received substantial attention in various application domains because of their ability to provide robust, reliable, and adaptable solutions. However, they are often challenging to solve. In this talk, I will introduce innovative and computationally efficient column-and-constraint generation (C&CG) algorithms for solving two-stage RO problems. C&CG algorithms operate within a master-subproblem framework. In the C&CG, the solution process alternates between a master problem and a subproblem. The master problem is first solved using a lower-bound approximation of the original objective, constructed by incorporating second-stage variables and constraints. Then, a subproblem is solved to enhance the quality of this approximation. First, I will present a new inexact C&CG (i-C&CG) that allows solutions to the master problems to be inexact, which is desirable when solving large-scale, challenging problems. We equip i-C&CG with a backtracking routine that controls the trade-off between bound improvement and inexactness, allowing us to establish theoretical guarantees for finite convergence. Next, I will introduce a new hybrid primal-dual C&CG (hC&CG) method that leverages the structural properties of the second stage’s primal and dual formulations to generate stronger cuts than those produced by classical C&CG methods. We derive theoretical guarantees on the finite convergence of i-C&CG and hC&CG. Finally, I will present numerical experiments demonstrating the superior computational performance of our i-C&CG and hC&CG over state-of-the-art C&CG.


## Talk Outline
1.  Introduce the classical column-and-constraint generation (C&CG) method and its limitations for solving two-stage RO models
2.  Discuss an inexact C&CG (i-C&CG) method and a hybrid C&CG (hC&CG) method that generalize and extend the classical C&CG method
3.  Examine the convergence of these new C&CG-based algorithms and their variants
4.  Present numerical results demonstrating the computational advantages of our proposed C&CG methods



## About the Speakers
{{< figure src="/or_images/or_33/speaker_tim.png" title="Man Yiu Tseng(Tim)" width="200">}}
Man Yiu (Tim) Tsang is an incoming assistant professor in the Department of Industrial, Manufacturing, and Systems Engineering at Texas Tech University starting Fall 2025. He is currently a Ph.D. candidate in Industrial and Systems Engineering at Lehigh University under the supervision of Prof. Karmel S. Shehadeh. He obtained his BSc and MPhil in Risk Management Science from the Chinese University of Hong Kong. His methodological research interests and expertise center around data-driven stochastic optimization, which includes proposing and analyzing different uncertainty modeling paradigms and designing computationally efficient algorithms to solve large-scale stochastic optimization models. His primary application areas are financial risk management, healthcare operations research, and transportation systems. His research has been recognized with the Van Hoesen Family Best Publication Award (winner) and Junior Faculty Interest Group Paper Prize (finalist with advisor Karmel S. Shehadeh). 



## Livestream Video
{{< bilibili BV1gSNnzME57 >}}


## Relevant Papers & Recommended Reading
- Tsang, M. Y., Shehadeh, K. S., & Curtis, F. E. (2023). An inexact column-and-constraint generation method to solve two-stage robust optimization problems. Operations Research Letters, 51(1), 92-98. 

## Recruitment Advertisement
I am actively looking for PhD students to join my research group in Texas Tech IMSE with strong optimization, mathematics, and/or statistics background. Prior experience in stochastic optimization is preferred. If you are interested, please send your CV to the email address mytimtsang@gmail.com for consideration. I am also open to collaborations in all areas of stochastic optimization.

---

<!-- ### 往期直播及相关推文
- 像这样列举相关的推文。注意符号都是英文符号。
- [推文名称](推文链接)
- [专访｜华人运筹学新星、MIT博士生 彭天翼：协助全球最大啤酒生产集团进行销售决策](https://mp.weixin.qq.com/s/GSfAatYmLMcVna1Q12exHA)
--- -->