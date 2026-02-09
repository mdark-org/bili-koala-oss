---
title: "科技周报｜轻量化 AI 助手；全自动漏洞发现探索；语音识别新模型"
description: ""
tags: []
date: 1770610468
bvid: BV1MgcTzXEjH
---
了解科技资讯，把握行业脉搏，大家好，我是Koala。欢迎收看科技周报。

### NanoClaw | 轻量化 AI 助手
最近一个名为 NanoClaw 的开源项目吸引了不少关注。它是一款个人用的 AI 助手实现，核心代码约 500 行，并在 macOS 的 Apple 容器或 Docker 中进行每个对话的隔离实例。这个设计强调可读性和可定制性，方便用户直接修改源代码实现自定义功能，包含 WhatsApp 接入、任务调度等基本功能。

Koala 认为，这类项目展示了开发者对透明性和可控性的追求，是学习和定制化实验的好材料。但作为生产工具，还需要更成熟的生态支持和社区协作。

---

### Shannon | 全自动漏洞发现探索
Shannon 是一款可以发现 Web 应用漏洞的自动化工具。它不仅扫描已知漏洞，还真的尝试利用漏洞进行 SQL 注入、认证绕过，进行攻击链验证。目前在 Expo 基础测试上做到 96% 的成功率，在 OWASP Juice Shop 里找出 20 多个高危漏洞。

Koala 认为，这是目前最接近 AI 红队想象的开源实现。误利用不报告的原则也解决了安全扫描的误报痛点。但 AGPL 协议和仅支持白盒测试的限制需要注意。且每次扫描消耗 3 到 5 美元 API 费用，对于大型代码库成本不低。更重要的是，它真的会实时攻击，千万别在生产环境跑。

---

### Voxtral Transcribe 2 | 语音识别新模型
Mistral 发布了 VoxTranscribe 2 系列，包含批量处理的 Mini 和实时转写的 Real-time 两个版本。Real-time 模型做到了 200 毫秒以内的延迟，且基于 Apache 2.0 开源。从公布的基准测试结果看，在意大利语、西班牙语等语种上，错误率已经压低到 3% 以下，中文表现相对弱一些。定价上则比 Eleven Labs 的 Scribe V2 便宜五倍。

Koala 认为，开源权重加亚毫秒级延迟的组合确实有竞争力，对需要本地部署的隐私敏感场景是好消息。但注意本次开源只针对 Real-time，Mini 版仍只有 API 服务。

---

### Excalidraw MCP | 让 Claude 学会手绘图
Excalidraw MCP 通过 MCP 协议，让 Claude 等 Agent 能在对话里直接画 Excalidraw 风格的手绘图。支持流畅的视口控制和全屏编辑，支持部署在 Vercel 上，也可以本地运行。相比让 AI 生成 Mermaid 或 PlantUML，手绘风格的适用空间更广泛。

---

### ZeroBrew | 把 Homebrew 提速 20 倍
ZeroBrew 是用 Rust 重写的 Homebrew 替代品。核心思路是把 Homebrew 的重构故事搬到 macOS 包环境。官方测试中，冷启动比 Homebrew 快两倍，热更新快 7.6 倍。它直接复用 Homebrew 的 CDN 和包定义，所以理论上你可以无缝替换 Brew 命令。

Koala 认为，这个项目的速度提升来自存储层优化而非协议更新，保持了很好的兼容性。但 Homebrew 的生态粘性不只是速度，那些复杂的编译依赖和 Cargo 包的处理才是硬仗。

---

### rust-ui | Rust UI 组件生态积累
Rust UI 是 Rust UI 框架 LapTools 的组件集合，主打和 ShadCN 一样的复制粘贴即用。基于 Tailwind CSS 定义样式，目前提供了表格、对话框、聊天界面等常见组件，风格偏现代简洁。

Koala 认为，Rust 的前端生态正在快速演进，但相比 React Vue 丰富的成熟组件库，LapTools 的周边仍然薄弱。作者也希望通过这个项目降低使用 Rust 开发 UI 的门槛。

---

以上就是本期科技周报的全部内容，谢谢您的收看。如果内容对您有帮助，请一键三连支持我们。

