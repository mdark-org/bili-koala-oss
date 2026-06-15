---
title: "科技周报｜语义级代码 Diff；数据库内的持久化工作流； Mac 原生 Linux 容器"
description: ""
tags: []
date: 1781413563
bvid: BV1CWJF6xE1d
---
欢迎收看本期 Hacker News 周报。了解行业资讯，把握行业脉搏，大家好，我是 Koala。


---


### Same
Same 是一个命令行工具，它不在按行对比代码改动，而是从函数、类这种语义实体的层面，理解一次提交到底改了什么。它提供 same diff 命令，做语义式差异识别；Same blame 把改动归因到具体开发者；Same impact 分析跨文件依赖影响。所有都消弭原生 git 操作，增加了易用性。像用 rust 写的，支持 26 种语言，一次 diff 通常只要 8 毫秒，零配置即可接入 git。作者称把 Same 的输入喂给 AI agent，准确率比原声行 diff 高 2.3 倍。Koala 认为，传统行 diff 是给人看的，但在 AI 写代码的时代，agent 需要的是结构化、语义化的变更信息。Same 通过代码静态分析，希望提供这种对 agent 更友好的新格式。


---


### pg_durables
pg_durables 是微软推出的 PostgreSQL 扩展，让长时间运行、可容错的工作流，直接在数据库里，用 SQL 定义和执行。你把工作流写成一连串 SQL 步骤，pg_durables 自动给每一步打检查点。数据库崩溃或工作流失败后，能从最近的检查点恢复，而不用手动重建状态。它用 Rust 和 pgx 开发，无需 Redis、Temporal 这类外部编排服务，还自带后台 worker 执行，并用行级安全做多用户隔离。适合向量嵌入、流水线、批量摄取、定时任务等场景。Koala 认为，持久化执行这两年很火，Temporal、Resonate 等专门的编排系统是主流方案。微软反其道而行，把这套能力塞进数据库，对于本就将状态存在 PostgreSQL 的团队，能省掉一整套 worker 和队列基础设置，运维心智负担显著降低。代价是工作流和数据库强耦合，跨语言、跨服务的复杂编排未必合适。


---


### Apple Container
Apple Container 是苹果官方推出的命令行工具，让 Mac 用户能在 Apple 芯片上，以轻量虚拟机的方式运行 Linux 容器。它完全用 Swift 编写，底层基于 containerization 这个 Swift 包来做容器、镜像和进程管理。支持 OCI 标准镜像和现有的容器生态兼容，运行需要 Apple 芯片的 Mac 以及 macOS 2.6 及以上版本。Koala 认为，长期以来，Mac 上跑容器主要靠 Docker Desktop，背后是一个统一的大虚拟机。苹果这次的思路是给每个容器分配独立的轻量虚拟机，隔离性更好，启动也更快，并且深度绑定 Apple 芯片做了优化。


---


### Metamorphosis
Metamorphosis 是 Slickt 的开源自托管替代里最成熟的一个。它提供实时聊天、工作流自动化、语音通话、屏幕共享以及 AI 集成等能力，后端用 Go，前端用 React，以单个 Linux 二进制文件运行，数据存在 PostgreSQL。采用 MIT 许可证，支持 Docker、Kubernetes、Helm 等多种部署方式，应用市场有超过 700 个集成。主打 DevesecOps、事后响应和 IT 服务台等场景。Koala 认为，Metamorphosis 没有正面去拼 Slack 的消费级体验，而是聚焦研发和安全运营场景，把自己欠进 DevesecOps 工具链。这个差异化定位，让它在企业市场站稳了脚跟。


---


### Extend UI
Extend UI 是 Extend AI 推出的开源 React 组件库，专注于文档和文档处理这一垂直场景。首个公开版本规划了 15 个组件，覆盖 PDF 查看器、Docs 查看与编辑、Excel 查看编辑、CSV 查看等文档编辑器。Koala 认为，通用 UI 组件库已经红海一片，Extend UI 聪明的选了文档处理这个细分赛道。这类组件做起来又重又琐碎，PDF 渲染、表格编辑、签名都是硬骨头，市面上现成的高质量开源方案不多。Extend AI 组营文档智能处理，把内部打磨过的能力开源出来，既是技术品牌建设，也是给开发者获客的入口，这是当下 AI 公司常见的打法。对于要做文档类、合同类、数据提取类应用的团队，这是个值得关注的现成轮子。


---


### Fable Pool
Fable Pool 是一个有趣的创意，将 prompt 以众筹的形式发布。它让一群人凑钱去资助一个有野心的软件项目，然后由 AI agent 透明的把活干完。平台用积分制运作，项目发起方设定众筹目标，达标后，AI agent 分阶段按里程碑推近。所有花费记在公开账本上。目前平台上已有 70 多个项目，方向五花八门。Koala 认为，这是一个相当有趣的实验，把 agent 当成更加平等的生产力，也让众筹所得的用途非常透明。


---


以上就是本期科技周报的全部内容，谢谢你的收看。如果内容对您有帮助，请一键三连，支持我们。