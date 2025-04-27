---
title: "科技周报｜AI 生成代码库指南；百行代码的 Agent 框架；多合一安全扫描神器"
description: "了解科技资讯、把握行业脉搏。每周快速浏览 Hacker News 精选。本期 Hacker Newsletter 地址：https://buttondown.com/hacker-newsletter/archive/hacker-newsletter-743/"
tags: []
date: 1745727605
bvid: BV1pijczvE8K
---
了解科技资讯，把握行业脉搏。

大家好，我是Koala。

欢迎收看科技周报。

### DeepWiki：AI 生成代码库指南
https://deepwiki.com/

想快速理解 GitHub 上的代码库吗？DeepWiki 可以帮你搞定。

这是 Daemon 团队推出的一个超酷平台。只要把 GitHub 链接里的 GitHub 换成 DeepWiki，就能获得 AI 自动生成的文稿、交互式图表，还能和 AI 助手聊天提问。

DeepWiki 已经索引了超过 3 万个代码库，分析了 40 亿行代码，确实是开发者和开源爱好者的福音。

它能深入代码，生成详细易懂的解释，还能生成交互式图表，让你直观了解代码结构。

最棒的是，你可以直接提问，AI 会根据上下文代码给出清晰的答案。有了 DeepWiki，探索代码库就像逛自家后花园一样轻松。

Koala 认为，对代码库的理解也是 AI 编程工具的核心竞争力。Daemon 团队开发此项目，也证明了他们的 AI 开发工具具备领先水平。

---

### PocketFlow：百行代码的 Agent 框架
https://github.com/The-Pocket/PocketFlow

接下来给大家推荐一个超轻量级的 LLM 框架 PocketFlow。

它只有 100 行代码，没有臃肿的功能，没有依赖，更没有厂商锁定。你可以用它轻松构建各种 Agent，实现 Workflow、RAG 等复杂应用。

它甚至内置了 Agent Encoding 理念，让 AI Agent 自己构建 Agent，大幅提升开发效率。

如果你觉得 LangChain 等方案太重，不妨试试 PocketFlow。社区还提供了 Python、TypeScript、Java、C++ 和 Go 等多个版本。

Koala 认为，PocketFlow 的推广策略十分值得学习。在仓库内，它简洁明了地给出了多种常见应用在 PocketFlow 中的实现方式，同时还开发了类似 DeepWiki 的代码库解读项目 Tutorial Codebase Knowledge，让用户可以快速感受 PocketFlow 开发 Agent 应用的潜力。

---

### Trivy：多合一安全扫描神器
https://github.com/aquasecurity/trivy

Trivy 是一款非常强大的安全扫描工具。它可以帮你找出容器、Kubernetes 集群、代码仓库以及云环境中的各种安全问题，像漏洞、错误配置、敏感信息泄露等等，它都能发现。

Trivy 支持多种目标扫描，包括容器镜像、文件系统、Git 仓库等，还能扫描操作系统包、软件依赖、Infrastructure as Code package 等。

最棒的是，Trivy 使用起来非常简单，一条命令就能搞定扫描。而且它还支持集成到 GitHub Actions、Kubernetes Operator 和 VS Code 插件中，在代码开发、CI/CD 等环节持续扫描。

Koala 认为，对于企业级应用，如果希望保证自身代码和上游供应链安全，那么 Trivy 是一个可靠的选择。

---

### Atuin Desktop | 让 Runbook 运行起来
https://blog.atuin.sh/atuin-desktop-runbooks-that-run/

还在为那些散落在各处的命令脚本发愁吗？脚本管理工具 Atuin 推出了 Desktop 版本。

它既像一个文稿那样易于阅读，又能像你的终端一样运行。你可以把脚本、内嵌终端、数据库客户端、Prometheus 图表都整合在一起。再也不用在 Slack 上翻记录，或者从 Notion 复制粘贴了。

Atuin Desktop 让你轻松创建可重复使用、易于分享且可靠的工作流。它支持 Jinja 风格的模板，可以从你的 Shell 历史记录中自动补全。而且它是本地优先的，支持 CRDT，可以同步和分享到 Atuin Hub。

目前 Atuin 团队已经用它来发布 CLI、迁移基础设施、启动环境和管理数据库查询了。感兴趣的话，可以申请 Early Access 体验一下。

---

### ActorCore：有状态 Serverless 框架
https://actorcore.org/

Action Code 是一个用于构建有状态 Serverless 应用的框架。它让开发者可以轻松构建 AI Agent、协作应用或本地优先的应用。

它由 Replit 团队开发，但不仅可以将它部署到 Replit，也可以部署到 Cloudflare、Bun、Node.js 等更通用的运行时中。

Action Code 的核心在于它的有状态计算。每个计算单元就像一个微型服务器，可以在请求之间记住数据，无须每次都重新加载，非常适合构建实时性要求高的应用。

它还支持自动化持久代码状态，无须连接外部数据库或 ORM，直接使用 JavaScript 对象或 SQLite 即可。是一个十分有趣的 Serverless 应用开发方案。

---

### spm: macOS 包管理器
https://github.com/alexykn/spm

spm 是一个用 Rust 编写的 macOS 包管理器，它的目标是替代 Homebrew。

spm 支持安装和管理命令行工具、库、语言以及桌面应用，也支持并行下载和安装，可以自动解决依赖问题。

如果你想自己编译也很简单，克隆仓库后用 Rust 工具链就能搞定。

如果你对 Rust 和 macOS 开发感兴趣，或者想体验一下新的包管理器，可以关注这个项目。不过要提醒大家，目前它还处于 Alpha 阶段，所以尝鲜需谨慎。

---

以上就是本期科技周报的全部内容，谢谢您的收看。

如果内容对您有帮助，请一键三连支持我们。

