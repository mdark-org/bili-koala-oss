---
title: "科技周报｜原生堆叠式 PR；开源本地化设计编辑器；无头浏览器环"
description: ""
tags: []
date: 1776601412
bvid: BV1qmoFBzE1e
---
了解科技资讯，把握行业脉搏。大家好，我是 Koala。欢迎收看科技周报。

### GitHub Stacked PRs | 原生堆叠式 PR
GitHub 官方推出 Stacked PRs，原生支持把一个大改动拆成若干个按顺序堆叠的 PR，可以一键合并整条链。包含网页端可视化和 GH Stack 命令行工具。

CLI 会处理分支创建、及链 Rebase、推送和 PR 生成。分支保护规则作用于最终目标分支而非直接 Base。

同时提供 NPM 包，让 AI 编程 Agent 也能创建堆叠。目前处于 Private Preview。

Koala 认为，堆叠 PR 这个工作流在 Meta、Google 内部用了很多年，外部则靠第三方工具支撑。GitHub 下场做原生集成是一大进步，意味着这种工作流从小众走向主流。

我们的俱乐部视频也在近期介绍了基于 AI 精确切分 PR 的思路，感兴趣的小伙伴可以观看。

---

### OpenPencil | 开源本地化设计编辑器
OpenPencil 是一个开源设计编辑器，能原生打开 Figma 文件，并通 KV2 字节编辑码器，互相复制粘贴保持保真度。

内置约 90 个工具的对话式 AI，可作为 MCP Server 接入 Cloud Code 和 Cursor。支持通过 WebRTC 的点对点实时协作，提供无头 CLI 用于快速阅读设计稿，还能输出 Tailwind CSS 或 JSON。

Koala 认为，Figma 在 AI 时代的态度一直让人捉摸不透，在 API 开放性上更是表现得十分保守。

OpenPencil 尽管在兼容性上还存在一些问题，但是能让 Agent 方便地补写设计稿，极有可能突破 Figma 的固有市场。当然，本周发布的 Cloud Design 更是对设计 SaaS 的一大挑战。

---

### Happy DOM | 无头浏览器环境
Happy DOM 是一个用 TypeScript 实现的 Headless 浏览器环境，提供完整的 DOM API，包括 Custom Elements、Shadow DOM、Mutation Observer、Fetch 等。

它被 Vitest、Jest、Babel 等测试框架作为默认或可选的 DOM 环境。支持 React、Vue 等主流框架的测试。

Koala 认为，长期以来，JSDOM 几乎是 Node 测试 DOM 的唯一选择，但它相对笨重，维护节奏缓慢。Happy DOM 选择重写一套更轻量的实现，Vitest 的默认推荐它作为环境就是最好的背书。

在前端基础设施越来越追求速度的当下，Deno 和 Vitest 带起的这波提速浪潮里，Happy DOM 是基础设施层的关键一环。局限是 API 覆盖度仍不如 JSDOM 全面，遇到冷门 DOM 特性，偶尔需要绕路。

---

### Open Agents | Vercel 编程 Agent 参考实现
Open Agents 是 Vercel Labs 开源的后台编程 Agent 参考实现。包含 Web UI、Agent 运行时、沙箱编排和 GitHub 集成的完整栈。

架构上把 Agent 和沙箱解耦。Agent 在 VM 外运行，通过工具调用与 VM 内的文件系统、Shell、Git 交互。

支持多步持久化执行，流式输出，快照恢复，自动 Commit 推 PR，甚至集成 Eleven Labs 做语音输入。

Koala 认为，这是 Vercel 对云端 Agent 这条赛道给出的开源答案，让开发者不必从零造轮子。

Agent 和沙箱分离的设计是对的，这意味着 Agent 的逻辑可以独立演进，沙箱可以按需替换。对 Vercel 自己来说，这也是推广 Vercel Sandbox 产品的一种方式。对云端 Agent 以及沙箱感兴趣的小伙伴，也可以观看我们最近两期俱乐部视频。

---

### BrightBean Studio | 开源自托管社媒管理
BrightBean Studio 是一个开源自托管的社交媒体管理平台。目前支持几乎所有海外主流平台，对国内平台支持相对较少。

功能上覆盖内容撰写、排期、审阅、发布、统一收件箱和客户门户等完整功能流。

SaaS 社媒工具长期按账号数和席位数收费，对多客户代运营的中小机构来说成本高企。自托管方案的核心价值不只是省钱，更是掌握数据和凭证的主动权。不过项目使用 AGPL 需要注意 License 风险。

---

### Fuse.js | 轻量级模糊搜索库
Fuse.js 是一个零依赖的 JS 模糊搜索库，基于 Bitap 算法实现容错匹配。完整版只有 8KB。

支持全重字段、嵌套字段、扩展搜索语法以及逻辑表达式，可以跑在浏览器、Node.js 和 Deno 环境。

Koala 认为，Fuse.js 在前端纯客户端搜索这个场景，它几乎没有对手。在 AI 问答如火如荼的今天，很多文档站点的即时搜索仍然靠它支撑，因为许多用户需要的还是毫秒级响应。

即使与 AI 结合，Fuse.js 的查询能力也是很不错的基层工具。

以上就是本期科技周报的全部内容，谢谢你的收看。如果内容对您有帮助，请一键三连支持我们。

