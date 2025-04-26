---
title: "[Hacker News 周报] Redis 替代方案；开源 Stripe 替代品；Databricks 开源基础大模型"
description: "了解科技资讯，把握行业脉搏。每周快速浏览 Hacker News 精选。本期 Hacker Newsletter 地址：https://mailchi.mp/hackernewsletter/694"
tags: []
date: 1711862567
bvid: BV1DH4y1H7f4
---
了解科技资讯，把握行业脉搏。大家好，我是 Koala。欢迎收看第694期 Hacker News 周报。

---

### KeyDB｜Redis 替代方案
https://keydb.dev/

KeyDB 是一个开源的 Redis 替代品。最初的定位是在 Redis 基础上增加多线程能力。随着多年的开发，KeyDB 已经成为一个在性能、功能和可用性上更强大的 KV 数据库。除了与原生 Redis 功能保持一致，KeyDB 还提供非阻塞 MVCC 架构、跨 Region 多主节点、Multijs 功能扩展等独特功能。Koala 认为，随着 Redis 开源 license 变更事件的发酵，越来越多的 Redis 替代方案受到关注。KeyDB 团队在这一时间点加入社交软件 Snapchat，并将所有代码正式开源，无疑成为了 Redis 社区迁移方案中的有力竞争者。

---

### Lago｜开源 Stripe 替代品
https://www.getlago.com/

随着 SaaS 软件的兴起，计费与支付功能也成为许多商业软件的重要组成部分。由于此类功能对可靠性的要求极高，采用 Stripe 等支付功能是较为常见的选择。Lago 是一个开源的计费与支付解决方案，提供基于计算资源、存储用量、用户席位、API 调用次数等多种维度的计费能力，以及多种支付方式的对接。用户可以通过自部署开源版本降低成本。Koala 认为，Stripe 等支付方式通常需要对每笔订单加收超过 1% 的费用，是一项不低的成本，但开发支付软件的难度也让开发者不会轻易尝试自行开发。Lago 这类项目切入了这一痛点，以开源的形式获取用户，同时也可以提供成本更低的托管或自部署方案。

---

### GritQL｜ 用于搜索和修改代码的查询语言
https://github.com/getgrit/gritql

GritQL 是一个用于搜索修改代码的查询语言。当对一个大型代码仓库进行重构或代码迁移时，简单的搜索替换通常不能满足需求，而基于 AST 匹配和修改又有较高的开发门槛且性能不易优化。GritQL 是一个对 AST 修改方案的封装，通过 Tree Sitter 解析代码并进行修改，为用户提供一套类似正则但更易于编写的专属语言，从而快速稳定的实现对大批量代码的重构。Koala 认为，在 GritQL 之前也有 Code Mode 等代码批量重构迁移工具。与它们相比，GritQL 在性能上更为突出，希望通过全新设计的查询语言得以降低使用门槛，但该语言的学习门槛则成为项目能否成功的关键。为此，该项目提供了较为完整的文档和交互式实例。

---

### PrimeVue｜ 一组 Vue 组件库
https://primevue.org/

PrimeVue 是一组美观、功能丰富的 Vue 组件库。除了组件之外，该项目也有不错的组题定制能力以及 TailWind CSS 集成，并且提供超过400个示例区快，复制粘贴即可进行二次开发。Koala 认为，尽管 Vue 的社区越来越繁荣，但作为主流前端框架之一，Vue 的组件库选择相对较少，不少组件库在 Vue2/3 时代已经不再更新。PrimeVue 则在功能完整性，美观程度上脱颖而出，除了基础组件之外，还提供自动补全、验证码输入框、日期选择器等复杂组件，是一个值得一试的方案。

---

### Dropflow｜基于 CSS 标准实现的布局引擎
https://github.com/chearon/dropflow

Dropflow 是一个基于 CSS 标准实现的布局引擎。它的渲染结果可以基于 Node Canvas 在 Nodejs 中输出为图片或 PDF，也可以在浏览器中渲染至 Canvas 画布中。目前 Dropflow 已经支持超过 30 种 CSS 属性，也支持渲染所有 Open Type 或 True Type 格式的字体。Koala 认为，随着 Web 的蓬勃发展，CSS 已经成为最流行的布局方案，但主流的 CSS 布局引擎都是在浏览器内部实现，无法直接应用于图片、PDF 等无浏览器中。Dropflow 这类方案则可以进一步扩展 CSS 的适用性，例如基于 Web Dom 设计一个海报，再将所有布局效果渲染到图片上，形成最终的图片版海报。

---

### DBRX｜Databricks 开源基础大模型
https://www.databricks.com/blog/introducing-dbrx-new-state-art-open-llm

本周 Databricks 发布了他们新的开源大语言模型 DBRX，并表示性能已经达到了开源模型领域的领先水平。根据 Databricks 的测试，该模型在性能上超越 GPT3.5，与 Gemini 1.0 Pro 版本接近。作为一个通用模型，在代码生成的特定任务上也超越了 Code Llama 等专用模型。Koala 认为，DBRX 的定位是基础模型，与 Llama、Mistral、Grook 相同。根据发布说明，DBRX 基于 3072 张 H100 GPU 训练而来，也体现了基础模型所需要的算力之大。值得注意的是 Databricks 着重强调了训练 DBRX 的过程，运用了 Databricks 的一系列工具，以及 Databricks 本身的数据平台，并且这些工具已开放给 Databricks 用户的是同一版本。DBRX 本身固然有价值，但也或许 Databricks 更想向他们的客户展示，在自家产品上训练大语言模型的独特优势。

---

以上就是本期 Hacker News 周报摘要，谢谢您的收看。


