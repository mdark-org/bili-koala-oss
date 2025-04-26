---
title: "[Hacker News 周报] 面向机器学习设计的列式数据结构；开源 Jira 替代品；Nvidia 万亿市值"
description: "了解科技资讯，把握行业脉搏。每周快速浏览 Hacker News 精选。本期 Hacker Newsletter 地址:https://mailchi.mp/hackernewsletter/654"
tags: []
date: 1685877880
bvid: BV1Mk4y1p7Jg
---
### Lance｜面向机器学习设计的列式数据结构
https://github.com/lancedb/lance

Lance 是一种为机器学习场景而设计的列式数据结构，与大数据领域常用的列式数据结构 parquet 相比，Lance 可以提供更快的随机读性能、向量搜索等能力，同时也可以轻松在 parquet, pandas dataframe, duckDB 等多种数据源和数据格式之间转换，让使用者既能快速浏览数据，也可以轻易数据进行模型训练等任务。在机器学习场景下，Lance 还提供了实用的数据多版本管理能力，便于在调试、重现模型时可以切换至数据集的任何版本。

---
### Trogan｜Textualize 社区的新项目
https://github.com/Textualize/trogon

Textual 是面向 Python 的终端 UI 框架，它背后的 Textualize 社区又开发出了新的项目 Trogan。该项目可以帮助用户将基于 Click 库开发的 CLI 快速转换为一个 Textual 终端 UI，提升 CLI 程序的易用性。Trogan 从 CLI 中提取指令、选项、描述等信息，再转换为 Textual 的配置信息，最终生成美观的终端 UI。在 Trogan 的计划中，下一步将继续支持对 Click 之外的其他库或编程语言开发的 CLI 工具进行转换。

---
### Plane｜ 开源 Jira 替代品
https://github.com/makeplane/plane

软件项目管理工具是许多团队重度使用的开发工具之一，以 Jira 为代表的商业产品通常以功能强大，但使用复杂著称。Plane 是一个开源的软件项目管理工具，希望基于开源加云服务结合的模式挑战已有的商业化产品。功能上除了必备的软件项目管理能力之外，更加增强了自定义能力、快速导航以及与 GitHub 等代码管理平台集成的能力。项目以 Apache 2.0 License 发布，这是否会让你选择部署一套进行尝试呢？

---
### CSS Pro｜CSS 编辑解决方案
https://csspro.com/ 

如何可视化友好的编辑 CSS 样式是许多低代码编辑器都希望解决的问题。这款名为 CSS Pro 的开发者工具，提供了一套精心设计的解决方案，通过对不同的 CSS 属性分类并提供针对性的控件，让没有 CSS 代码知识的用户也可以完成样式编辑的工作。作为一个独立商业产品，CSS Pro 还支持页面元素采集、图片提取、及时编辑、尺寸测量等高级功能，看完这个产品的功能设计，你是否也有所启发呢？

---
### Logicboard｜ 一个在线编程工具
https://logicboard.com/demo 以及 https://logicboard.com/demo/:replay 

Logicboard 是一个在线编程工具，支持多人实时协同编辑、云端代码执行等功能，并且内置了多人的实时音视频功能，可以快速变为你的在线代码面试工具，同时每一次代码编辑的过程事后都可以进行回放，进一步对面试过程进行回溯。

---
### AI 小结


接下来是本周 AI 小结：
1. 阿联酋技术创新研究院开源的大模型 Falcon 40B，并被免版税使用。Falcon 作为 Hugging Face 排行榜中目前名列前茅的大语言模型，对其调整可能会激发更多基于 Falcon 二次训练的新项目。
https://www.tii.ae/news/uaes-falcon-40b-now-royalty-free

2. 日本政府宣布不会对 AI 训练中使用的数据实施版权保护，以此推动日本在 AI 领域的发展速度。
https://technomancers.ai/japan-goes-all-in-copyright-doesnt-apply-to-ai-training

3. Nvidia 达到万亿美元市值，其中 AI 领域爆发引起的 GPU 需求是重要的推动力。
https://www.theverge.com/2023/5/30/23742123/nvidia-stock-ai-gpu-1-trillion-market-cap-price-value

4. 老牌浏览器厂商 Opera 计划发布 AI 就绪的浏览器 One，从浏览器层面充分发挥与 AI 的交互能力。
https://www.opera.com/zh-cn/one

---

以上就是本期 Hacker News 周报摘要，谢谢您的收看。

