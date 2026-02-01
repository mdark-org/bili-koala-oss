---
title: "科技周报｜ 把 Mermaid 图直接变好看；GPUI 加持的 Redis 客户端；LLM API 追踪工具"
description: ""
tags: []
date: 1769916728
bvid: BV1Ny6xBSEpb
---
了解科技资讯，把握行业脉搏，大家好，我是Koala。欢迎收看科技周报。

### Beautiful Mermaid | 把 Mermaid 图直接变好看
Craft 团队开源了一个 Mermaid 图表渲染库，叫 Beautiful Mermaid。它提供了15种精心设计的主题，支持 SVG 和 ASCII 双输出格式，覆盖流程图、时序图、类图、ER 图等几乎所有 Mermaid 支持的图表类型。官方演示页面做的相当用心，每种图表都有实际渲染效果的对比。

---

### Zedis | GPUI 加持的 Redis 客户端
这是一个用 Rust 和 GPUI 构件的 Redis 图形客户端。GPUI 就是 Zed 编辑器用的那套 GPU 渲染引擎，性能上有保障。功能亮点包括自动解压 Gzip 和 Zstandard 数据，MessagePack 反序列化，图片预览，16进制查看等。还能自动识别 Redis 的 standalone, cluster, sentinel 拓扑模式。Koala 认为，Redis GUI 工具市场并不缺选手，但贴心的功能设计和 GPUI 的技术选型，适合对性能有追求的重度 Redis GUI 用户。

---

### Sherlock | LLM API 追踪工具
Sherlock 是一个拦截 Agent 调用 LLM API 流量的工具。通过 Man-in-the-Middle Proxy 代理 HTTPS 请求，实时显示 Token 消耗量和成本估算。支持终端仪表盘展示，还会自动保存每次请求的 Prompt 为 Markdown 和 JSON 格式。目前主要支持 Claude Codec, CodeX 和 Gemini CLI。Koala 认为，开源项目中所描述的定位是成本核算，但这个项目更大的潜力还是用于逆向研究 Agent 的行为。

---

### QMD | 本地知识库搜索新选择
QMD 是 Shopify CEO Tobi Lütke 做的一个本地 Markdown 搜索引擎。技术上结合了 BM25 全文检索、向量语义搜索和 LLM 重排序。全程通过 Ollama 本地运行，支持 MCPI 协议，可以直接集成到 Claude Desktop 或 Claude Code 里。Koala 认为，这个项目的亮点在于，融合搜索策略设计的比较精细，包括查询扩展、RRF 融合、位置感知全重混合等。CEO 还能保持精力写代码，也让 Tobi 在技术圈中始终拥有不错的口碑。

---

### Convex | 实时同步的全栈后端
近期 Convex 与 Supabase 在社交平台上产生对立，竞争之势愈演愈烈，引发关注。Convex 是一个全栈后端平台，主打实时数据同步和 TypeScript 端到端类型安全。用纯 TypeScript 定义数据库 schema, query 和 API。前端通过 React Hooks 自动订阅数据变化，不需要手动处理缓存失效或 WebSocket。支持 Cron 任务、AI 工作流集成，还有一套组件生态。Koala 认为，定位上像是 Firebase 该有的样子。开发者体验确实很丝滑，但作为托管服务，长期成本和数据迁移成本需要提前考虑。

---

### Flameshot | 截图界的瑞士军刀
Flameshot 是一款跨平台的开源截图软件，支持 Linux, macOS 和 Windows。功能包括截图编辑、自定义外观、Debug 接口、多种图床上传等。Koala 认为，如果你在 Linux 上找一款好用的截图工具，Flameshot 仍然是第一选择。在 macOS 和 Windows 上也能用，但可能不如原生工具顺手。

以上就是本期科技周报的全部内容，谢谢你的收看。如果内容对您有帮助，请一键三连支持我们。

