---
title: "科技周报｜Vitess 作者主导的 Postgres 扩展方案；高效优化 LLM 应用；更友好的 netstat 替代品"
description: "了解科技资讯、把握行业脉搏。每周快速浏览 Hacker News 精选。本期 Hacker Newsletter 地址：https://buttondown.com/hacker-newsletter/archive/hacker-newsletter-750/"
tags: []
date: 1749960000
bvid: BV1f6Msz6EV7
---
了解科技资讯，把握行业脉搏。大家好，我是Koala。欢迎收看科技周报。

---

### Multigres | Vitess 作者主导的 Postgres 扩展方案
https://supabase.com/blog/multigres-vitess-for-postgres

Superbase 团队宣布启动 Multigres 项目，目标是为 Postgres 构建类似 Vitess 的数据库集群系统。Vitess 擅长扩展 MySQL，提供分片、连接池、查询路由、故障恢复和原生编排等功能。Multigres 的目标是将这些优势带给 Postgres 生态，解决 Postgres 在扩展性上遇到的瓶颈。

初期，Multigres 将提供简单的连接池，逐步发展到高可用，最终实现 PB 级别的数据分片。Koala 认为最重要的是，该项目由 Vitess 的联合创始人 Sugu 领导。Sugu 离开 Vitess 的商业化公司 PlanetScale 之后，与多家公司探讨了在 Postgres 上开发类似系统的愿望，最终认为 Superbase 是最适合完成这一目标的公司，最终选择加入。这也体现了 Postgres 社区的超高热度。

---

### TensorZero | 高效优化 LLM 应用
https://github.com/tensorzero/tensorzero

如果你正在开发 LLM 应用，那么可以试试使用开源项目 TensorZero。

它可以为你的 LLM 应用创建一个反馈回路，通过生成数据不断优化模型，让它们变得更智能、更快速、更便宜。TensorZero 统一了 LLM 网关、可观测性、优化、评估和实验，形成了一个数据和学习的飞轮。你可以用它的网关来做 AB 测试和流量路由，一方面让它选择最划算的模型完成任务，另一方面收集数据用于后续微调。

TensorZero 使用 Rust 编写，性能强悍，避免在 API 中引入过多延迟。Koala 认为，随着 LLM 应用从 Demo 走向生产，这类观测与优化工具还有更大的潜力等待挖掘。

---

### Somo | 更友好的 netstat 替代品
https://github.com/theopfr/somo

如果你经常使用 netstat 或者需要监控网络状态，那就试试 Somo 吧。

它是一个用 Rust 编写的命令行工具，可以方便地监控 Linux 上的端口和网络连接，同时它能以更友好的表格形式展示信息，而且支持过滤。你可以根据端口、IP、进程名等条件来查找。Somo 以 TUI 的形式提供交互，在排查问题时保持高效。

特别对于不熟悉 netstat 工具的用户来说，一个像 Somo 这样更加直观易用的工具，可以避免在网络异常时，还因为工具不顺手而变得更加焦虑。

---

### Taskmaster | AI agent 专用项目经理
https://www.task-master.dev/

Taskmaster 是一个专门为 AI agent 设计的项目管理工具。你可以用它来组织、协调和追踪 AI 代理的任务，就像管理一个真实的团队一样。

Taskmaster 提供了看板、任务分配、进度跟踪等功能，帮助你更好地掌握 AI agent 的工作流程。Koala 认为，如果你正在构建复杂的 agent 系统，Taskmaster 是一个不错的工具。它能通过事前规划和进度追踪的方式提升 AI agent 的效率，确保项目按计划进行，也避免 AI 因为上下文有限记不住已经完成和未完成的任务。

---

### s3mini | 超轻量级 S3 客户端
https://github.com/good-lly/s3mini

s3mini 是一个超轻量级的 S3 客户端，使用 TypeScript 编写。它非常小巧，压缩后只有大约 14KB，而且性能也不错。

最重要的是，它没有任何依赖，完美支持以 Cloudflare Worker 为代表的各类边缘计算平台，也兼容 MinIO、Backblaze B2 等 S3 存储服务。如果你需要在边缘环境处理对象存储，又不想引入 AWS SDK 这种太重的库，s3mini 就值得一试。它只提供了最核心的 S3 API，比如 list、put、get、delete 等，非常适合轻量级应用。

---

### Spark | THREE.js 的高效渲染器
https://github.com/sparkjsdev/spark

Spark 是一个为 Three.js 设计的 3D Gaussian Splatting 渲染器。Splatting 实际上是一种高效渲染方案，可以实现逼真的光照和透明度效果，同时兼顾性能和真实感。

Spark 将 Splat 完美融入 Three.js 渲染管线，原生支持多种文件格式，基于 GPU Shader Graph 实现动态编辑，并在 WebGL2 环境下保持高兼容性和流畅度，为开发者提供灵活的交互和混合渲染能力。

---

以上就是本期科技周报的全部内容，谢谢你的收看。如果内容对您有帮助，请一键三连支持我们。

