---
title: "科技周报｜Firebase/Supabase 替代方案；基于 Markdown 的看板；手机里的 Ollama"
description: "了解科技资讯、把握行业脉搏。每周快速浏览 Hacker News 精选。本期 Hacker Newsletter 地址：https://buttondown.com/hacker-newsletter/archive/hacker-newsletter-753/"
tags: []
date: 1752374586
bvid: BV1PYMfz5ENn
---
了解科技资讯，把握行业脉搏，大家好，我是 Koala。欢迎收看科技周报。

---

### bknd | Firebase/Supabase 替代方案
https://github.com/bknd-io/bknd

BKND 是一个轻量级的后端框架，可以作为 Firebase 和 Supabase 的替代品。它基于 TypeScript 开发，但可以与各种运行时以及数据库搭配使用。

它可以在 Node.js、Bun、Deno 和浏览器中运行，也可以部署到 Cloudflare Workers、Vercel 和 AWS Lambda 中。数据库层面也支持 SQLite 和 PostgreSQL，以及它们的各种商业化版本。

对象存储只要是 S3 兼容的，也都可以使用。这些设计让它的适用场景更为丰富。

除了后端服务，它也提供了客户端封装，以及各种客户端框架的对接。Koala 认为，总的来说，BKND 和 Go 生态中的 PocketBase 有些相似，但在数据库选择和部署方面更加灵活。

---

### Backlog.md | 基于 Markdown 的看板
https://github.com/MrLesk/Backlog.md

Backlog MD 是一个用 Markdown 文件来管理项目任务的看板工具，并且设计之初就考虑到要和 AI 无缝协作。

你可以用它来管理项目和任务，同时支持命令行和外围 UI 两种方式进行各种操作。由于所有的数据都以易读的方式保存在 Markdown 文件中，所以 Backlog MD 和各种终端 AI Agent 配合良好。

只需要引导 Agent 阅读它提供的使用手册，Agent 就能接管任务，并在复杂需求中自行拆解和管理任务。Koala 认为，Backlog MD 本身并不复杂，但其设计体现了设计对 AI Agent 友好的新一代软件的一些思路。

---

### Cactus | 手机里的 Ollama
https://github.com/cactus-compute/cactus

Cactus 让你可以在手机上本地部署 LLM、VLLM 和 TTS 模型。它可以作为库被 Flutter 和 React Native 应用加载使用，方便开发者开发出跨平台应用。

它目前支持运行各种基于 UFF 模型，比如千问、Gemma、Llama、DeepSeek 等等。Cactus 还能根据设备性能调整模型量化级别，从 FP32 到两比特都能支持，尽可能保证效率和设备流畅。

它也同时支持云端模型 API 调用。应用开发者可以选择本地优先、云端优先和严格本地等多种运行策略，进一步提升 API 调用的成功率。

---

### BrowserOS | 开源 Agentic 浏览器
https://www.browseros.com/

BrowserOS 是一款基于 Chromium 的开源浏览器，主打 AI 自动化功能。它最大的亮点是内置了本地 AI Agents，可以直接在浏览器里执行各种任务。

比如自动填写表单、安排会议等等，所有数据都保存在本地，不用担心隐私问题。BrowserOS 还支持 Ollama，未来还会推出基于 LLM 的广告拦截器。

感觉 Chrome 拦截 UBlock Origin 之后，这类工具会越来越受到欢迎。Koala 认为，BrowserOS 相当于把 AI Agent 直接集成到了浏览器里，让浏览器的自动化能力更强，也是一种有趣的实践。

---

### Meilisearch | 开源搜索引擎
https://www.meilisearch.com/

Meilisearch 是一款开源的高性能搜索引擎，它可以无缝集成到你的应用和工作流程中，为用户提供闪电般的搜索体验。

它具有强大的全文搜索功能，新版本中已整合了语义搜索，形成混合搜索能力，以此进一步提升搜索相关性。Meilisearch 易于集成，API 设计简洁明了，还提供了各种 SDK，对开发者友好。

Koala 认为，在 RAG 场景中，当简单的语义搜索无法提供足够好的结果时，大家又把目光转向了传统搜索引擎。Meilisearch 凭借出色的性能和开源的属性，也有机会从中获益。

---

### 思源笔记 | 开源个人知识管理软件
https://github.com/siyuan-note/siyuan

最后推荐的是思源笔记，这是一款非常棒的个人知识管理软件，主打隐私保护和知识的自由掌控。

它完全开源，基于 TypeScript 和 Golang 开发，性能和安全性上都下了功夫。思源笔记除了基础的 Markdown 编辑，还有快引用、双向链接和 AI 写作等进阶功能。

它提供了美观的安卓、iOS 客户端以及 Docker 部署方案，让你随时随地都能访问和管理你的知识库。

---

以上就是本期科技周报的全部内容，谢谢你的收看。如果内容对您有帮助，请一键三连支持我们。

