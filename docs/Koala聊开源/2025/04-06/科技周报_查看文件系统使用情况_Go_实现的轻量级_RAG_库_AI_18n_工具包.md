---
title: "科技周报｜查看文件系统使用情况；Go 实现的轻量级 RAG 库；AI 18n 工具包"
description: "了解科技资讯、把握行业脉搏。每周快速浏览 Hacker News 精选。本期 Hacker Newsletter 地址：https://www.daemonology.net/hn-daily/"
tags: []
date: 1750561293
bvid: BV1bcNDzpERC
---
了解科技资讯，把握行业脉搏，大家好，我是 Koala。欢迎收看科技周报。

---

### NoxDir | 查看文件系统使用情况
https://github.com/crumbyte/noxdir

NoxDir 是一个命令行工具，它通过检测磁盘和分区，然后用一个交互式的终端界面，展示磁盘的使用情况，比如已用空间、可用空间和总容量。

你可以用键盘操作，快速找到占用空间大的文件和目录，方便清理。

NoxDir 支持 Windows、macOS 和 Linux，而且因为它适配了多种系统指令，整体执行速度很快。NoxDir 完全本地运行，不会收集你的任何数据。如果你觉得你的磁盘空间不够用，或者想快速找到占用空间的文件，就可以用它扫描一次，看看结果。

---

### Raggo | Go 实现的轻量级 RAG 库
https://github.com/teilomillet/raggo

Raggo 是一个用 Go 编写的 RAG 库。虽然 Python 和 JS 生态中的 AI 框架和库层出不穷，但 Go 开发者目前的选择还不是很多。如果你想用 Go 语言快速搭建 RAG 系统，可以从 Raggo 开始尝试。

它将 RAG 的核心组件进行了抽象，你可以组合内置或自身实现的各个组件，例如文档提取器、切分器、向量数据库等，构建最终的 RAG 系统。Raggo 还提供了多种 RAG 策略，包括 Simple RAG、Contextual RAG 和 Memory Context，满足不同的应用场景。

无论是实际使用还是学习，都很值得一看。

---

### Lingo.dev | AI 18n 工具包
https://github.com/lingodotdev/lingo.dev

Lingo.dev 是一个开源的 AI i18n 工具包。它通过与 AI 集成，可以帮助开发者快速实现应用的本地化。你可以选择使用 Lingo.dev 提供的 AI 后端，或者集成你自己的 LLM 模型。

Lingo.dev 提供的 CLI、CI/CD 工具和 SDK，方便你在不同阶段进行本地化工作。它还支持多种格式，包括 JSON、YAML 和 Markdown。对于开发者来说，配置之后，就可以让 Lingo 像文档工程师一样参与到项目的开发过程中，完成翻译工作。

---

### Prefect | Python 数据管道框架
https://github.com/PrefectHQ/prefect

Prefect 是一个工作流编排框架，可以帮助你用 Python 构建更健壮的数据管道。简单来说，它能让你把普通的 Python 脚本变成可以在生产环境中稳定运行的工作流。

Prefect 提供了调度、缓存、重试和基于事件的自动化等功能，让你的数据流程更加可靠。你可以使用自部署的 Prefect Server，也可以选择它云端服务的 Prefect Cloud。

Koala 认为，编写脚本处理数据并不复杂，但要过渡到大量数据的场景，仍然保持健壮和高效，就不那么简单了。Prefect 通过框架封装了这一场景的复杂性，让普通开发者也可以构建出灵活强大的数据管道。

---

### Liveblocks | 为产品加入 AI 协同助手
https://liveblocks.io/

Liveblocks 作为一个在线协同服务，能够快速为应用添加各种协同功能，比如多人编辑、评论、通知等。但现在它更进一步，集成了 AI 功能。

Liveblocks 把这个功能集成为了 AI Copilots。在文档编辑、评论、问答等场景中，使用它提供的预置 UI，就能快速为产品加入内容续写、总结、翻译和问答等典型的 AI 功能。同时，Liveblocks 的设计也保持灵活，例如用户可以自定义 AI 结构化的输出，渲染为丰富的 UI 样式，而不只是文本，增强了可读性和交互性。

---

### Canine | K8s 的强大，Heroku 的简洁
https://github.com/czhu12/canine

Canine 是一款简化 K8s 上部署应用流程的工具。目标是提供像 Heroku 一样流畅的体验。如果你觉得直接操作 K8s 太复杂，但又需要它强大的功能，Canine 就能派上用场。

它支持 GitHub 集成和一键部署，简化日常流程，也能自动管理 SSL 证书，避免安全问题，还有实时的监控功能，以及弹性伸缩，带来更好的可控性。

---

以上就是本期科技周报的全部内容，谢谢你的收看。如果内容对您有帮助，请一键三连支持我们。

