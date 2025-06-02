---
title: "科技周报｜MacOS 快捷工作流；Svelte 的工作流框架；PostgreSQL 自动分片方案"
description: "了解科技资讯、把握行业脉搏。每周快速浏览 Hacker News 精选。本期 Hacker Newsletter 地址：https://www.daemonology.net/hn-daily/"
tags: []
date: 1748835936
bvid: BV1mF7mzzEKm
---
了解科技资讯，把握行业脉搏。

大家好，我是 Koala。

欢迎收看科技周报。

### KeyboardCowboy | MacOS 快捷工作流
https://github.com/zenangst/KeyboardCowboy

KeyboardCowboy 是一个为 macOS 用户设计的生产力工具。

用户可以将重复的操作、应用启动、系统设置、文件操作等各类工作流定义为快捷键。

双手无需离开键盘就能触发各种重复性工作并快速完成，进而用户还可以根据丰富的上下文信息，定义工作流的触发条件，以及将不同的工作流分组管理。

Koala 认为，虽然 KeyboardCowboy 上手会有些难度，但一旦熟悉且完成自定义配置后，效率就能成倍地提升。

---

### Svelte Flow | Svelte 的工作流框架
https://xyflow.com/blog/svelte-flow-release

Svelte Flow 1.0 终于来了。

这次更新可是下了大功夫，整个库都基于 Svelte 5 重写，带来了脱胎换骨的改变。

新版本不仅修复了之前版本的一些问题，还增加了很多新功能，比如 Edge 重连、更强大的 Fit View、键盘导航和更好的可访问性。

如果您听说过 React Flow，那么您对 Svelte Flow 也会熟悉，因为它是由 React Flow 的团队维护的。

在 Svelte 社区，一些商业化公司，例如 Windmill，已经在使用了 Svelte Flow 构建产品。

对于构建 AI 工作流 UI 的开发者，Svelte Flow 也让 UI 框架的选择更加多变。

---

### pgdog | PostgreSQL 自动分片方案
https://github.com/pgdogdev/pgdog

pgdog 是一个 PostgreSQL 的自动分片方案。

通过管理数据库的逻辑复制以及事物池化，实现 PostgreSQL 的水平扩展。

项目使用 Rust 编写，注重性能和安全性，能够管理数百个数据库，支持数千个数据库连接。

除了上述功能，pgdog 也支持数据库查询的负载均衡，并且所有功能均提供详细的配置项。

对于过去已经使用 PgBouncer 等同类项目的用户，应该会给 pgdog 配置和使用方法感到熟悉。

---

### Cap | 开源轻量级验证码
https://capjs.js.org/

还在用那些又慢又强行收集用户数据的验证方案吗？

试试 Cap 吧。

这是一个使用 SHA-256 Proof of Work 的开源 Captcha 方案，体积很小，只有 hCaptcha 的 250 分之一。

它完全保护隐私，不需要追踪或收集用户数据。

用户也可以完全自定义前端和后端。

Cap 通过工作量证明来区分人和机器，对人类更友好，对机器人则更具挑战。

对于想要使用 Cap 的用户，只需两行代码就可以将它接入网页，为网页带来安全防护。

对验证码安全机制感兴趣的小伙伴，也可以阅读 Cap 的文稿，学习相关知识。

---

### Linkify | 文本链接识别工具
https://linkify.js.org/

Linkify 是一款 JavaScript 插件，能帮你快速把纯文本中的链接转换成 HTML 的 A 标签。

它能自动识别 URL、邮箱地址，还能高亮井号标记的话题标签、@用户等等。

用起来非常简单。

它还支持 React 和 jQuery，也能处理多语言和 Emoji。

同时它也力争保持较小的体积，压缩后只有 11KB 左右。

Koala 认为，对于博客、论坛、评论区等场景，使用 Linkify 可以节省很多解析文本链接的工作，但需要确认文本内容可信时才使用这个工具，避免用户输入恶意链接诱导点击。

---

### 科普博客 | 什么时候微调有意义
https://getkiln.ai/blog/why_fine_tune_LLM_models_and_how_to_get_started

还在好奇微调大语言模型能解决什么问题吗？

这篇文章介绍了什么时候微调才是最佳选择。

微调能解决像输出不稳定的 JSON 格式、降低提示词成本、避免提示词太复杂影响效果等问题。

文章会带你了解微调的时机好处，帮你确定哪些目标对你的项目最重要，并指导你如何开始，最终获得可衡量的结果。

简单来说，如果你想提高任务质量、降低成本、加快速度，或者让模型更好地调用工具、遵循规则，那么微调就是个不错的选择。

文章也表示，知识更新用目前的微调方法并不高效，RAG 和其他方法会更合适。

以上就是本期科技周报的全部内容。

感谢您的收看。

如果内容对您有帮助，请一键三连支持我们。

