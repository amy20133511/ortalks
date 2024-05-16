{{/*- The following var extracts Talk #s -*/}}
{{- $talkNo := substr .Name 9 -3 -}}
---
title: "Tech Talk {{ $talkNo }}: " # 在此添加talk的题目
date: {{ .Date }}
draft: true
# 编辑完成后把 `draft` 改成 false (不要双引号)
tags: [""]
categories: [""]
summary: "" # 在此添加talk总结
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
在此加入talk的内容摘要。


## 嘉宾介绍
在此添加嘉宾照片。步骤：
1. 在static/tech_images下添加一个文件夹，文件夹名为“tech_XX”（替换XX为当前talk编号）；
2. 上传照片到static/tech_images/tech_XX，并把图片文件名修改为“speaker.jpg”；
3. 把下面这行指令中的“41”修改为当前talk编号XX，并把嘉宾名字改为当前talk的嘉宾名字；
4. 删掉这段文字。
{{< figure src="/tech_images/tech_41/speaker.png" title="彭天翼" width="200">}}

在此添加嘉宾简介。

 
## 观众提问
提问写在这里。
: 回答写在这里。下面是一个示范例子。


A/A测试中的两个A是指不同版本间的比较吗？
: 不是，A/A测试是对于同一个算法的分流测试。在这种情况下，真实的treatment effect是0。它一般用于检查estimator的鲁棒性或者估计estimator的方差。A/A测试可以对用户分成两组测试，有时也会分成两个时间段测试。


---

## 直播回放
{{< bilibili BV11G411R7hR >}}
把上面的BV号改成当前talk对应的bv号即可。


## 相关资料及延伸阅读
- 像这样列举相关的文章。
- Farias, Vivek, Andrew Li, Tianyi Peng, and Andrew Zheng. "Markovian interference in experiments." *Advances in Neural Information Processing Systems* 35 (2022): 535-549.

---

### 往期直播及相关推文
- 像这样列举相关的推文。注意符号都是英文符号。
- [推文名称](推文链接)
- [专访｜华人运筹学新星、MIT博士生 彭天翼：协助全球最大啤酒生产集团进行销售决策](https://mp.weixin.qq.com/s/GSfAatYmLMcVna1Q12exHA)
---