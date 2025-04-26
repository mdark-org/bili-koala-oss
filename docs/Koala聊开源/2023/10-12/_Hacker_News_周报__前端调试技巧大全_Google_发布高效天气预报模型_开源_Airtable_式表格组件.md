---
title: "[Hacker News 周报] 前端调试技巧大全；Google 发布高效天气预报模型；开源 Airtable 式表格组件"
description: "了解科技资讯，把握行业脉搏。每周快速浏览 Hacker News 精选。本期 Hacker Newsletter 地址：https://mailchi.mp/hackernewsletter/677"
tags: []
date: 1700353800
bvid: BV1Fv411c781
---
了解科技资讯，把握行业脉搏，大家好，我是 Koala，欢迎收看第 677 期 Hacker News 周报。

### React Datasheet Grid｜ 开源 Airtable 式表格组件

https://react-datasheet-grid.netlify.app/

在 Airtable、 Notion 等效率工具中，最重要的组件之一就是功能强大的表格。React Datasheet Grid 则是这类强大表格的开源实现。它对快捷键操作、拖拽选择、从 Excel 中复制粘贴数据等高级功能实现的十分完备，每个单元格也都可以自定义渲染，从而轻松定制符合产品需求的表格呈现形式。在性能方面，使用 virtualized 技术，也使其在数十万行数据量级下保持流畅。

---
### flyscrape｜基于 Go 的数据抓取工具

https://github.com/philippta/flyscrape

Flyscript 是一个独特的数据抓取工具，基于 Go 编写，使其具有高效的性能，但同时支持用户使用 Javascript 编写脚本，提取网页中的数据，又保持了灵活性，降低使用者的学习成本。在开发体验方面，Flyscript 也做了许多努力，例如提供开发者模式，用于实时查看提取的结果，加速脚本开发。

---

### Loro｜ CRDT 工具库

https://www.loro.dev/

使用 CRDT 等方案开发本地优先的协同工具是近年来颇为活跃的研发方向。Loro Apps 这一领域新出现的创业公司，其开源项目 Loro 是一个 CRDT 工具库，不仅支持基础数据类型，还支持为富文本编辑设计的 Paratext 算法，以及树状数据结构 Umbo Tree 等。Loro 本身基于 Rust 开发，也支持通过 WebAssembly 的方式在 JS 状态中使用。

---
### GraphCast｜Deepmind 发布高效天气预报模型

https://deepmind.google/discover/blog/graphcast-ai-model-for-faster-and-more-accurate-global-weather-forecasting/

最近 DeepMind 发表了一篇论文，介绍了其基于机器学习和图神经网络的天气预测系统 GraphCast。GraphCast 可以在不到一分钟的时间内进行十天的中期天气预测，其准确度明显超过业内的传统数值天气预报系统。它还可以提前预测极端天气事件，包括识别洪水风险等，对防灾减灾很有帮助。GraphCast 展现了 AI 在天气预测领域的巨大潜力，它不仅预测准确，运算效率也远远高于传统方法。DeepMind 开源了 GraphCast 的模型代码，使全球科学家都可以基于该技术进行研究与应用。

---

### Tiny LLMs｜在浏览器中本地运行的大语言模型

https://tinyllms.vercel.app/

大语言模型需要有多大？Tiny LLMs 的答案是越小越好。该项目是一组可以在浏览器中本地运行的 AI 模型，适用于语音识别、语音生成、图片处理、图片识别等多种任务。该项目的目标是探索一种对用户友好且隐私安全的大语言模型使用方式。

---
### perfect freehand｜手绘功能代码仓库

https://github.com/steveruizok/perfect-freehand

TL Draw 白板工具的作者将该项目中最出色的手绘功能维护成了一个单独的代码仓库，名为 Perfect Freehand。该项目的特点是其支持模拟手写笔的压力，还可以通过参数调整线条的粗细、平滑度等。绘制结果可以导出为 SVG 路径数据，使其非常适合在 Web 上渲染手绘线条。无论是白板工具还是电子签名的场景，都可以使用这个仓库加速开发。

---

### 一篇介绍 67 种浏览器中调试技巧的文章

https://alan.norbauer.com/articles/browser-debugging-tricks

接下来是一篇介绍浏览器调试技巧的文章。在文章中，作者总结了 67 种浏览器中的调试技巧，涵盖调试断点、性能分析、 DOM 检查等方面。这些技巧大多基于浏览器开发者工具，但运用巧妙，对于中高级前端开发者，这些技巧可以提高调试效率，例如快速分析界面异常，追踪不明错误来源等。

---
### 一篇介绍消息队列 pgmq 的技术原理的文章

https://tembo.io/blog/pgmq-self-regulating-queue/

最后是来自 Tembo 团队的一篇文章，介绍了其开源的基于 Postgres 的消息队列 PGMQ 的技术原理。对于想要使用消息队列，但又不想维护额外基础组件的用户，PGMQ 提供了新的选择。基于 Postgres 数据库的 for update skip locked 的特性，以及 visibility timeout page，就能实现一个简单应用的消息队列，而无需运维其他程序。

---

以上就是本期 Hacker News 周报摘要，谢谢您的收看。