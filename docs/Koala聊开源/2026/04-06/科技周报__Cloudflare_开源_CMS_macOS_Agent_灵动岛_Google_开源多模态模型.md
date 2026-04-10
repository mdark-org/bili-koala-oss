---
title: "科技周报｜ Cloudflare 开源 CMS；macOS Agent 灵动岛；Google 开源多模态模型"
description: ""
tags: []
date: 1775364347
bvid: BV1rLD5BKEtE
---
了解科技资讯，把握行业脉搏，大家好，我是Koala。欢迎收看科技周报。

---

### EmDash | Cloudflare 开源 CMS
搜索查询已发布项目的图文，大家可以访问「Koala 聊开源」官网 https://koala-oss.app 的「科技周报」数据库。

Cloudflare 推出开源 CMS EmDash，定位为 WordPress 的精神续作。实际就是一种 Cloudflare Native 的替代品。该项目基于 TypeScript 加 Astro 6.0，跑在 Workers 上。用插件沙箱机制，运行解决 WordPress 的顽疾。内置 MCP Server，让 AI Agent 直接管理内容和部署。

Koala 认为，技术选型现代，但 WordPress 有 43% 的市场份额和 6 万插件生态护城河，并不是 EmDash 可以快速撬动的。但我们认为更重要的是，Cloudflare 展现出了全新的战略思路，通过搭建 Cloudflare Native SaaS，为自家基础设施带货，最终加大市场占有率。相信 EmDash 只是一个开始，未来他们还会有更多同类项目推出。

---

### Vibe Island | macOS Agent 灵动岛
搜索查询已发布项目的图文，大家可以访问「Koala 聊开源」官网 https://koala-oss.app 的「科技周报」数据库。

Vibe Island 把 MacBook 灵动岛变成 AI 编程 Agent 的控制面板。支持 Cloud Code、Code CLI、Gemini CLI 等六种工具。启动自动配置，权限审批在灵动岛完成，不用切窗口。Swift 原生，内存低于 50MB。不过目前是收费工具。

Koala 认为，多 Agent 并行时，频繁切窗口确实烦。灵动岛监控这个创意执行的不错。局限在于用户群受限新款 MacBook，外接屏退化为悬浮条。

---

### Gemma 4 | Google 开源多模态模型
搜索查询已发布项目的图文，大家可以访问「Koala 聊开源」官网 https://koala-oss.app 的「科技周报」数据库。

Google DeepMind 发布 Gemma 4 开源模型，含 1.2B、1.4B、2B、3B、4B 四档。3B 数学测试 89.2%，编程 80%。全系列支持音视频多模态和函数调用，覆盖 140 种语言。1.2B、1.4B 可在手机和树莓派上离线运行。

Koala 认为，本次 Gemma 号称在 Gemini 3.0 的研究成果之上训练而成，有望打破 Google 内部两派模型水平差异过大的问题。但 Gemma 作为开源中小模型，聚焦的仍然是本地，甚至端侧部署的场景。目前竞中对手也主要是千问和 Mistral 的同规格模型。

---

### nono | AI Agent 运行时沙箱
搜索查询已发布项目的图文，大家可以访问「Koala 聊开源」官网 https://koala-oss.app 的「科技周报」数据库。

nono 是开源 AI Agent 的运行时安全框架，Six Store 创始人出品。提供五层防御，包含内核隔离、文件快照回滚、Marko 树审计、供应链签名验证、动态权限审批。提供 Python、TypeScript、Rust 和 C 多语言 SDK。

Koala 认为，这个项目的技术深度远超简单沙箱，但 Agent 的生态尚早，开发者安全投入意愿有限。能否在安全和便捷间取得平衡，以及支持大规模云化部署是一个关键问题。

---

### Semiotic | React 流式数据可视化框架
搜索查询已发布项目的图文，大家可以访问「Koala 聊开源」官网 https://koala-oss.app 的「科技周报」数据库。

Semiotic 是一个支持流式数据的 React 可视化库，包含 40 多种图表类型，架构分三层，从开箱即用到颗粒度定制都支持。流式引擎双画布架构，支持 60FPS 流畅渲染不断涌入的数据。内置预测和异常检测等统计功能，还提供 MCP Server，供 LLM 生成图表。

Koala 认为，项目的 API 设计在 D3 和 Recharts 之间找到平衡。流式渲染和 MCP 集成是差异化所在，适合结合 LLM 的流式输出做可视化渲染。

---

### Cult UI | Shadcn 扩展组件库
搜索查询已发布项目的图文，大家可以访问「Koala 聊开源」官网 https://koala-oss.app 的「科技周报」数据库。

Cult UI 基于 Shadcn UI 的开源动效组件库开发。67 个以上动画组件可直接复制使用。技术栈包括 React、Tailwind、TypeScript。还收录了 100 多种 AI Agent 的交互模式预览，包括最近流行的终端动画效果、粒子花布效果等等。如果想快速构建出一个有品位，又美观的 AI 产品落地页，不妨在 Cult UI 上找找灵感和现成的组件。

---

以上就是本期科技周报的全部内容，谢谢您的收看。如果内容对您有帮助，请一键三连支持我们。

本期 Hacker Newsletter 地址：https://www.daemonology.net/hn-daily/

