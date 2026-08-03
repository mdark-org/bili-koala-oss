---
title: "科技周报｜DeepSeek 正式版 V4-Flash；2G 内存跑 26B 模型；自托管的迷你 Heroku"
description: ""
tags: []
date: 1785644540
bvid: BV1Fz3X62ETW
---
了解科技资讯，把握行业脉搏，大家好，我是Koala，欢迎收看本期科技周报。


### DeepSeek V4 Flash
https://github.com/deepseek-ai/DeepSeek-V4
DeepSeek 正式版 V4 Flash 上线 Hugging Face，304B 参数的 MoE 架构，搭配 DeepSeek 投机解码模块，来加速推理。它提供低、高、最高三档推理强度。最大亮点是官方给出的数据里，经过后训练的它，在多个 Agent 基准测试上，超过了体量更大的 V4 Pro 预览版。Koala 认为，本次发布的 V4 Flash 正式版，将私有化部署的模型能力边界，提升到了新的高度，也让大家对 V4 Pro 的正式版有了更高的期待。与此同时，DeepSeek 在发布说明中也透露了，本次基准测试均使用即将发布的 DeepSeek Harness 完成。


---


### TurboFieldFire
https://github.com/turbo-field-fire/tff
TurboFieldFire 是个专为 Apple Silicon 写的推理引擎，能让 Llama 3 的 26B ASB 模型，只占约 2GB 内存跑起来，8GB 的 Mac 也能用。原理是：不把 14.3GB 的模型塞进整个内存，只让 1.35GB 的共享核心常驻，其余专家权证，从 SSD 按需流式读取。项目用 Swift 6.2 和 Metal 3 写成，带原生 Mac 应用，命令行工具，和一个兼容 OpenAI 接口的本地服务。Koala 认为，这个项目真正的价值在于，它最大化发挥了 MoE 架构模型的特点，降低资源需求。这一思路的前提是 SSD 够快，苹果的统一内存和高速 NVMe 恰好是最适合的土壤，换到普通 PC 上，收益可能会明显缩水。


---


### Dooku
https://github.com/dooku-io/dooku
Dooku 自称是你见过的最小的 Pass 实现。一条 Bootstrap 脚本完成，之后 git push 就能部署。它底层用 Docker 做应用隔离，用 Buildpack 来编译应用。整个平台本身就是一堆插件拼起来的，核心功能也是插件。你想扩展的话，用任何语言写都行。目前版本是 0.38.25，这个项目已经维护了十多年，社区仍然活跃。Koala 认为，Dooku 的定位很清晰，花几十元租一台 VPS，就能得到 Heroku 这类 Pass 平台八成的体验。和 Fly.io 这类托管平台比，Dooku 走的是完全相反的路线，用户自己管运维、备份和监控，换来的是零锁定和成本可控。它适合个人项目、内部工具和小团队，在 Agent 大量生成应用、部署需求变得零碎的当下，这种一台机器跑几十个小应用的模式，反而比几年前更有生命力。


---


### GitHub Pull Request 堆叠模式
https://github.blog/2024-05-15-stack-pull-requests-on-github/
GitHub 正式推出堆叠式 PR Request，你可以把一个大改动拆成一串互相依赖的小 PR，每个独立评审，独立合并。它通过 GH CLI 的 stack 扩展来实现，支持一次合并、单个合并或者跳一段连续的、一起合并。改了底层某个 PR 之后，上面的分支会跟着 rebase。它还接了 GitHub Actions，工作流里能拿到整个堆叠的原数据，避免依赖链上的 PR 反复跑重复的 CI。Koala 认为，堆叠式 PR 这个实践，在 Meta 和 Google 内部用了很多年。GitHub 现在提供原生解决方案，时机也很微妙。Agent 生成代码的量在暴涨，几分钟产出上千行 diff 已经很常见，评审成为新的瓶颈，把大改动切成可消化的小块正好对症。


---


### SuperPool
https://github.com/superpool-io/superpool
SuperPool 解决的是多个 Agent 并行开发时，都需要独立数据库的问题。它基于命令行，为每次开发临时开一个隔离的 Superbase 实例。包含真实的 PostgreSQL、Auth 和 S3 兼容存储，默认租约 30 分钟，执行期间每 5 分钟自动续期。启动前会自动跑完 Superbase Migration 目录下的所有 SQL 迁移，然后把标准 Superbase 环境变量、Postgres 连接串别名和各框架的前缀变量，一并注入进去。Koala 认为，这也是典型的被 Agent 催生出来的基准设施。相比 Superbase 官方的数据库分支功能，SuperPool 主打的是快和便宜，用完即抛，而不是长期维护一套分支。


---


### Blog 开源 Bus
https://github.com/blog-bus/bus
Blog 开源的 Bus 是个自托管写座平台，特别之处在于它跑在 Nostr 协议上。每个社区就是一个 Relay，所有动作都是一条加密签名的事件，消息、表情回应、代码评审、工作流步骤，全都进同一份事件日志。功能上有频道、话题、私信、画板，以及带审批能力的 YAML 工作流，还能接入各类 Webhook 事件。后端是 Rust 的加 Ocsal 和 PostgreSQL，桌面用 Tauri，移动端用 Flutter。Koala 认为，选 Nostr 是个大胆的决策，好处是天生去中心化和可验证，代价是生态工作链远不如成熟 IM 协议。另外，自托管意味着运维人员也要对相关的概念有所了解。


以上就是本期科技周报的全部内容，谢谢您的收看。如果内容对您有帮助，请一键三连，支持我们。