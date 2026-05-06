---
title: "科技周报｜Claude Design 开源替代；Agent 千种工具集成层；全能型 HTTP 文件服务器"
description: ""
tags: []
date: 1777780363
bvid: BV1U19ZBLEcf
---
了解科技资讯，把握行业脉搏，大家好，我是Koala。欢迎收看科技周报。

### Open Design | Claude Design 开源替代
Open Design 是 Claude Design 的开源版本，主打本地优先。最大差异是不绑定 Agent，能自动检测系统里12种常见 Coding Agent。

COI 作为后端，复刻了 Design System 以及沙箱预览，自带五维评分，防止 AI 生成低质量设计。Koala 认为 Anthropic 上月发布 Claude Design 之后，AI 设计 Agent 赛道关注度迅速上升，但闭源加供应商绑定让许多团队观望。

Open Design 用极快的速度做出可插拔、多 Backend 替代，并把71个品牌级 Design System 内置。本质是把 Claude Design 的工作流封装价值提取出来，变成开放工具。当然不可忽视的是作为商业产品，Claude Design 仍然能够像 Claude Code 一样通过数据驱动，持续改进模型与产品。这是开源项目难以匹敌的。

---

### Composio | Agent 千种工具集成层
Composio 是开源的 AI Agent 工具集成 SDK，预先打包好1000多个第三方应用的连接器。Gmail、Slack、GitHub、Notion、Spotify、Hacker News 等等都即插即用，自带 OOS 和凭证管理。

框架兼容性很广，主流的 Agent 产品和框架都能兼容。提供了 TS 和 Python 的官方 SDK，还附带一个名为 Root 的 MCP 服务器，连通500多个应用。Koala 认为 Agent 落地的最大瓶颈不再是模型能力，而是接入已有系统的工程量。每个 SaaS 各自的 OOS、API 限流、错误处理，重复一遍就会劝退多数团队。

Composio 把这一层做成基础设施，本质上是在做 Agent 时代的栽培，但走的是开发者优先和开源路线。

---

### goshs | 全能型 HTTP 文件服务器
Goshs 是 Go 写 的 Simple HTTP Server 现代替代。V2 在简单文件分享之外加入了大量企业级特性，例如基于 ACL 的目录鉴权、限时加限次的分享链接配二维码、WebDAV 与 SFTP 支持、IP 白名单和 Webhook 通知等功能。

Kali、Homebrew 等安装器均已收入。Koala 认为 Python Simple HTTP Server 是流行的20年的临时文件服务器，但功能止步于最基础的 HTTP。想要 HTTPS、鉴权、配额都得自己折腾。Goshs 把这些杂事一次解决，从内网文件传输到对外有限分享都能用一个二进制搞定。

---

### DuckLake 1.0 | SQL 即元数据的 Lakehouse
DuckLake 是 DuckDB 团队4月13日发布的1.0版本 Lakehouse 格式规范。最大特点是把所有元数据放进 SQL 数据库，不再像 Iceberg、Delta Lake 那样用一堆 JSON 加 Avro 文件描述表状态，事务直接是一条 SQL。

1.0 加入了数据 Inlining、有序表、Bucket 分区、原生 Geometry 和 Variants 类型。Koala 认为 Iceberg 标准化进展是过去两年的热点，但元数据的复杂性也是它最大的门槛。小团队跑 Iceberg 等于运维一个分布式系统。

DuckLake 判断九成 Lakehouse 用户其实不需要 Iceberg 的扩展性，把元数据塞进一台 PostgreSQL 反而更简单可靠。是简化数据栈的典型操作，对中小数据规模团队会有真实吸引力。

---

### Agent Vault | AI Agent 凭证代理
Agent Vault 是 Infrascal 出品的 HTTPS 代理加凭证保险库。Agent 发出的请求经过 MITM 代理时，由 HTTPS 代理负责注入 Bearer 和 API Key 等多种认证凭证。Agent 自己永远看不到真正的密钥。

支持 WebSocket 透传，可是白名单或拒绝模式。Koala 认为当前 Agent 调用第三方 API 普遍是把密钥直接塞进环境变量或 Prompt，等于把自家门钥匙交给一个会犯错且可能被 Prompt 注入的程序。

Agent Vault 的思路是把凭证下沉到网络层。Agent 只看到一个本地代理 URL，密钥泄露面降到最小。这是 Infrascal 从企业密钥管理向 AI Agent 场景的自然延伸，方向合理。但要让 Agent 理解如何使用，仍需生态配合。

---

### Ghostty 离开 GitHub | 开源治理事件
Mitchell Hashimoto 近日宣布把 Go 的项目迁离 GitHub 引发热议。作为 HashiCorp 创始人 和多个知名开源项目的作者，HashiMoto 是 GitHub 最深度的一批用户之一。本次决定离开的理由是平台可靠性问题。他记录的故障日记几乎天天有事故，曾有基础设施故障两小时无法做 PR Review。

Koala 认为，后续 GitHub CTO 也发播客介绍了 GitHub 正在进行的基础升级，并表示在 AI Coding 强势的今天，GitHub 的负载正在以数十倍的速度增长。不可否认的是，GitHub 对绝大多数开源开发者来说还是事实标准。但 AI 时代一个去除社交属性，更加稳定、可靠、轻量级的 Git 基础设施也很可能是新的创新机会。

---

以上就是本期科技周报的全部内容，谢谢你的收看。如果内容对你有帮助，请一键三连支持我们。

