---
title: "科技周报｜Google Workspace 统一命令行工具；LLM 的测试驱动开发；Go 终端库全面升级"
description: ""
tags: []
date: 1772943299
bvid: BV1txNKztENM
---
了解科技资讯，把握行业脉搏，大家好，我是Koala。欢迎收看科技周报。

### Google Workspace 统一命令行工具 (gws)

Google 推出 GWS，用统一命令行控制 Drive、Gmail、Calendar 等全部 Workspace 服务。它选择在运行时读取 Google 的 Discovery Service，动态生成命令。API 一旦更新，客户端自动同步。

它内置了 40 多个 AI Agent 技能，并且原生支持 Gemini CLI 扩展。Koala 认为，CLI 现在是帮助 SaaS 服务融入 Agent 生态的重要手段。Google Workspace 服务有着大量的用户，办公场景又是 Agent 服务的重点领域。本次 Google 推出 GWS，预计会解锁更多 Agent 办公场景。

GWS 的动态服务发现机制也体现了设计上的深思熟虑，比已有的不少第三方 MCP 形态集成方案，更加易于维护。

---

### Promptfoo | LLM 的测试驱动开发

Promptfoo 是一个开源的 LLM 测试框架，支持用 YAML 定义测试用力，自动对比多个模型输出，还能检查 Prompt 注入等安全风险。它强调测试驱动的 LLM 开发，而不是反复试错。支持接入 CI/CD，也提供合规报告，映射到 OWASP、NIST 等标准。

Koala 认为，LLM 应用进入生产环境后，可观测性和测试覆盖是两大痛点。Promptfoo 把传统软件测试的方法论引入 AI 领域，这种思路比单纯依赖人工评估更可持续。

前段时间 Anthropic 发布博客中提到，他们内部也在使用这个工具，做 Agent 的质量评估，也是让 Promptfoo 获得了更多的关注。

---

### Charm v2 | Go 终端库全面升级

Charm 团队发布了 Bubbletea 等库的第二版，这是六年来首次重大更新。新版渲染性能提升十倍以上，API 从命令式转向声明式，并且已经在他们的 AI 编头助手 Fossil 里，从实践验证了数月。GitHub、AWS、Nvidia 都在用这套方案做终端工具。

Koala 认为，终端不再是复古玩具，而是 AI 时代人机交互的重要界面。V2 的声明式 API 设计让状态管理更清晰，性能优化则直接降低 SSH 场景下的带宽成本。25000 个依赖项目的迁移压力不小，但 Charm 提供了详尽的升级指南，甚至给 LLM 准备了专用提示词。

---

### Oxfmt Beta | 30 倍速的 Rust 版 Prettier 来了

前端工具链 Oxformat 进入 Beta。这个用 Rust 写的格式化工具，比 Prettier 快 30 倍，同时保持完全兼容。Vue、Vercel、Sentry 这些大项目已经在用。它不只是快，还内置了 Import 排序和 Tailwind 的支持等实用功能。迁移命令一行搞定。

Koala 认为，JavaScript 工具链的 Rust 化已成定局。Oxformat 没试图重新定义格式标准，而是选择完全兼容 Prettier。这种务实让社区可以无痛迁移。随着 Agent 领域 Harness 工程的流程，所有自动化工具链的性能，都需要有更高的追求。

---

### Dependency Cruiser | 代码架构的守门员

JS 项目长期缺乏有效的模块边界控制。Dependency Cruiser 填补了这个空白。它通过配置文件定义规则，比如禁止客户端代码引用服务端模块，在 CI 中自动检查依赖违规，还能生成可视化的依赖图，帮助理解代码结构。

Koala 认为，架构防腐在 AI 参与开发的项目中越来越重要。这个工具把原本靠 Code Review 人工把关的事情自动化了。配置即代码的方式适合纳入现有工作流，但规则设计需要团队对架构有清晰共识，否则容易流于形式。

---

### Jido 2.0 | Elixir 的 Agent 框架

Jido 是用 Elixir 写的多 Agent 协作架构。2.0 版本改进了通信机制和错误处理。它采用纯函数式的 Agent 设计，状态变更通过指令描述，副作用由 OTP 运行时执行。内置的 Supervisor 树能自动恢复崩溃的 Agent，支持热更新。

Koala 认为，当 Python 和 JS 几乎垄断 AI 开发时，Jido 提供了另一种思路。Elixir 的并发模型和容错机制确实适合构建高可靠的 Agent 系统，但生态成熟度仍有差距。适合对性能和稳定性有极致要求，且团队愿意接受函数式编程思维的场景。不过 Jido 2.0 的代码设计，对想要深入 Agent 实现的小伙伴很有参考价值。

---

以上就是本期科技周报的全部内容，谢谢您的收看。

如果内容对您有帮助，请一键三连支持我们。

