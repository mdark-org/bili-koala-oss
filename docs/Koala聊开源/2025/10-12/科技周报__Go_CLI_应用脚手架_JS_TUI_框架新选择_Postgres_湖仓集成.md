---
title: "科技周报｜ Go CLI 应用脚手架；JS TUI 框架新选择；Postgres 湖仓集成"
description: ""
tags: []
date: 1762659345
bvid: BV1rXkSBEEvC
---
了解科技资讯，把握行业脉搏，大家好，我是Koala。欢迎收看科技周报。

---

### Fang | Go CLI 应用脚手架
Charm 团队推出了 Fang，这是一个面向 Cobra CLI 应用的实验性脚手架库。它将常见功能直接打包进来，包括美化过的帮助页面、自动版本管理、man page 生成和 shell 补全等特性。开发者只需调用一个函数，就能获得这些能力。

Koala 认为，Charm 在终端工具美学上一直很有追求。Fang 延续了这个传统，让 CLI 新手开发者也能做出健壮应用的命令行程序。

---

### OpenTUI | JS TUI 框架新选择
SST 团队正在开发 OpenTUI，一个用 JS 和 TS 构件终端界面的框架。它提供了 React 和 SolidJS 的 reconciler，让前端开发者可以用熟悉的声明式写法来构建 TUI 应用。这个项目将成为 OpenCode AI 和 Terminal Shop 的基础设施。

Koala 认为，用前端框架思维做终端应用是个有趣的方向。之前该方向的 Ink 项目，也支撑了许多 TUI 形态 AI Agent 的开发。但 Ink 的维护不算活跃。OpenTUI 在功能与 UI 组件丰富度以及性能上，都有着更大的野心，且有生产级项目基于它开发，是值得关注的新项目。

---

### pg_lake | Postgres 湖仓集成
Snowflake 开源了 PG Lake，这是一套让 PostgreSQL 能直接操作 Iceberg 表的扩展。开发者可以在 PostgreSQL 里用标准 SQL 查询和管理基于 Iceberg 的数据湖中的表。打通了数型数据库和 Lakehouse 之间的壁垒。这个项目源自 Snowflake 今年收购的 Crunch Data。

Koala 认为，对于重度依赖 PostgreSQL 的团队来说是个实用工具，不需要额外的 ETL 就能接入数据湖。不过 Snowflake 开源这个项目的动机也很明显，就是为自家的 Lakehouse 生态进一步铺路，也是收购 Crunch Data 之后成功推出的产品功能。

---

### TOON | LLM 专属数据格式
TOON 是一个专为 LLM 设计的数据序列化格式。目标是在保持可读性的同时，大幅减少 token 消耗。对于表格型数据，它能比 JSON 节省 30% 到 60% 的 token。格式本身借鉴了 YAML 的缩进结构和 CSV 的表格思路，并针对 LLM 的解析特点做了优化。适合用于序列化 AI Agent 的工具调用返回结果。

Koala 认为，这个工具在 token 成本敏感的场景下确实有价值。但额外的抽象，也意味着学习与维护成本较高。考虑到对 YAML 的实现并不复杂，且自定义需求多，自行维护一个更加可定制的版本也许也是一个好的选择。

---

### Skyvern | AI 浏览器自动化
Skyvern 是一个基于 AI 的浏览器自动化平台，能用自然语言指令完成网页操作。它支持 Captcha 识别、2FA 认证、代理网络等高级功能。典型场景包括批量填表、发票下载、自动采购等重复性工作。

Koala 认为，和其它 AI 浏览器工具相比，Skyvern 的定位更偏企业级集成。Browserless 等开源框架，虽然灵活，但需要自己搭建基础设施。Stage Hand 在 Playwright 上加了 AI 层，允许开发者混合编写代码和自然语言指令。Skyvern 走的则是 API First 的路线，专注少量更具体的企业办公场景，牺牲一点通用性，但保证开箱即用。

---

### slime | LLM RL 训练框架
智谱 AI 开源了 SLIME，这是支撑 GLM 4.5 和 GLM 4.6 的强化学习训练框架。它通过连接 Megatron 和 SG Long 实现高性能训练，并提供灵活的数据生成接口。除了智谱自家模型，也支持千问、DeepSeek、Llama 系列。

Koala 认为，大模型训练框架的开源对行业是好事，能降低后训练的技术门槛。不过这类框架的使用门槛仍然不低，更适合有 GPU 集群和训练经验的专业模型团队。

---

以上就是本期科技周报的全部内容，谢谢你的收看。如果内容对您有帮助，请一键三连支持我们。

