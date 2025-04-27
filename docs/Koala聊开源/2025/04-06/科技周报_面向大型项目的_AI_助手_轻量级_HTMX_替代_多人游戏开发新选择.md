---
title: "科技周报｜面向大型项目的 AI 助手；轻量级 HTMX 替代；多人游戏开发新选择"
description: "了解科技资讯、把握行业脉搏。每周快速浏览 Hacker News 精选。本期 Hacker Newsletter 地址：https://buttondown.com/hacker-newsletter/archive/hacker-newsletter-742/"
tags: []
date: 1745123449
bvid: BV1ij5fz2En9
---
了解科技资讯，把握行业脉搏，大家好，我是Koala，欢迎收看科技周报。

---

### Plandex | 面向大型项目的 AI 助手
https://github.com/plandex-ai/plandex

Plandex 是一款基于终端的AI开发工具，它能帮你规划和执行大型编码任务。这些任务可能涉及多个步骤和大量文件。它内置了记忆与索引功能，支持高达200万tokens的上下文，并且能索引包含200万tokens以上的目录。

Plandex 也内置了沙箱机制，将AI生成的更改与你的项目文件隔离，直到它们准备就绪。你可以控制命令的执行，方便回滚和调试。Plandex 希望在充分利用AI优势的同时，避免在项目中留下混乱。

Koala认为，与Cloud Code和OpenAI Codex类似，Plandex也是一个基于终端的AI开发工具，但其功能更为丰富，且不与任何AI厂商绑定。

---

### Datastar | 轻量级 HTMX 替代
https://data-star.dev/

Datastar 是一个服务段渲染框架，可以帮助你构建响应式的外币应用。它兼具服务段渲染的简单性，和全站SPA框架的强大功能。只需一个14.5KB的文件就可以将Datastar引入你的项目，并立即为前端UI增添响应式逻辑。

后端可以使用任何你喜欢的语言编写，可以使用官方提供的SDK，也可以直接从后端发送SSE事件。Datastar的前端JS文件体积比Alpine.js和HTMX还要小，但却提供了不逊于两者的功能，且官方提供的SDK让开发者能够获得更好的开发体验。

---

### SpacetimeDB | 多人游戏开发新选择
https://spacetimedb.com/

SpacetimeDB 是一个很有意思的开源项目，它把数据库和服务器合二为一了。你可以直接让客户端连接到数据库，并在数据库内部执行逻辑。具体的业务逻辑可以通过Rust或C#编写Spacetime Modules实现。Modules最终会被编译为WebAssembly，内置到SpacetimeDB中被调用，使得整体框架更为紧凑简洁，不再需要云上运维复杂的多服务架构。

该团队认为，使用SpacetimeDB能够让少量开发者构建出大型多人游戏，包括后端逻辑、玩家实时位置、持久化状态全部都能搞定。

---

### AutoRAG | 全托管的 RAG 方案
https://blog.cloudflare.com/introducing-autorag-on-cloudflare/

Cloudflare 推出了AutoRAG，这是一个全托管的RAG流水线。自LLM兴起以来，RAG就一直是研究与实践的热点领域。基于RAG构建企业或个人的知识库也是热门的AI应用场景。

基于Cloudflare的基础设施，AutoRAG能够帮你搞定所有复杂的配置，只需点几下鼠标就能完成数据接入、分块、向量化、存储等一系列操作。它还支持自动更新索引，保证你的AI始终掌握最新信息。这样一来，你就可以专注于构建更智能的应用，而不用在繁琐的底层维护上浪费时间。

---

### Better Auth | 身份认证方案
https://www.better-auth.com/

Better Auth 是一款身份验证解决方案，最近在开发者社区中获得了很高的评价。许多开发者都说，它用起来非常简单，而且类型安全。有人提到，与Auth.js相比，Better Auth更容易集成。例如，连接数据库时，只需直接连接到Visual ORM，并注册一个存储页面即可。

如果你的新项目正在寻找一个简单而强大的身份验证方案，Better Auth值得一试。

---

### Smartfunc | 把 Docstring 变成 LLM 函数
https://github.com/koaning/smartfunc

想快速把你的Python函数变成AI接口吗？Smartfunc这个简洁优雅的工具库，让你只需要在函数的Docstring里写好Prompt，就能自动生成对应的LLM函数。它基于Simon Willison开发的LLM库，用简洁的模板引擎解析Docstring，运行时注入变量生成Prompt，然后调用后端LLM接口。

Smartfunc简单易用，支持Pydantic模型定义返回结构，还支持Async异步调用，方便你做Microbatching。开启Debug模式后还能看到详细的Prompt和返回信息，帮你更好的调试。

---

以上就是本期科技周报的全部内容，谢谢你的收看。如果内容对您有帮助，请一键三连支持我们。

