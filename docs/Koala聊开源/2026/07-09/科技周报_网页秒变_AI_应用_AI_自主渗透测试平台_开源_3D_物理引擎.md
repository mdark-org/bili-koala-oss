---
title: "科技周报｜网页秒变 AI 应用；AI 自主渗透测试平台；开源 3D 物理引擎"
description: ""
tags: []
date: 1783232341
bvid: BV1SYMM6FEeT
---
了解科技资讯，把握行业脉搏，大家好，我是Koala，欢迎收看本期科技周报。


---


### Page Assist
[https://github.com/n4ze3m/page-assist](https://github.com/n4ze3m/page-assist)

Page Assist 是阿里巴巴开源的前端 GUI Agent 框架。加一行代码，就能让任何网页支持自然语言操作。它是纯前端方案，不需要改造后端。开发者可以自在大模型，还内植了隐私保护机制，采用 MIT 协议开源。Koala 认为，网页端 Agent 目前多靠浏览器插件或云端 RPA 实现。Page Assist 把能力下沉到站点自身，让开发者主动给用户提供 AI 入口，对存量 Web 应用的 AI 化改造很友好。不过，纯前端方案在复杂多步任务上的可靠性还有待验证，适合先从表单填写、导航引导这类场景切入。


---


### Stricts
[https://stricts.ai/](https://stricts.ai/)

Stricts 是一个 AI 驱动的自主安全平台。用 Agent 全天候执行渗透测试，覆盖 REST、GraphQL、gRPC 接口，也能在 CI 里分析代码和 PR，还能检测 AWS、Azure、Kubernetes 的配置错误。每个漏洞都附带可复现的 POC，并自动生成修复 PR，支持私有化部署，拿到了 SOC2 和 ISO 27001 认证。Koala 认为，AI 渗透测试是今年安全领域最热的方向之一。Stricts 的差异点在于打通了从发现、验证到修复的闭环。POC 验证也能有效压低误报。不过，自动化攻击面测试在生产环境的边界控制仍是敏感话题，企业落地前需要评估好授权与隔离策略。


---


### Box3D
[https://github.com/kettle11/box3d](https://github.com/kettle11/box3d)

Box3D 和 Box2D 作者 Erin Catto 新开源的 3D 物理引擎，用 C17 编写。他在开发游戏时，被虚幻引擎自带的物理计算折腾得够呛，于是在 WoW 的 Rubicon Light 基础上，结合 Box2D v3 的优化，做了这个引擎，支持连续碰撞、宽 SIMD 的求解和跨平台确定性，目前已被多个项目采用。Koala 认为，Box2D 作为 2D 物理引擎在近 20 年的时间里广受好评，Kettle 的口碑让 Box3D 天生自带信任度。3D 开源的物理领域 Jolt 刚凭借与 Godot 的整合站稳脚跟，Box3D 的入场会让人这个长期被商业引擎主导的领域更有看头，游戏开发者值得持续关注。


---


### ZeroFS
[https://github.com/zerofs/zerofs](https://github.com/zerofs/zerofs)

ZeroFS 是一个开源日志结构文件系统，把 S3 兼容的对象存储直接挂载成 Posix 文件系统。支持 NFS 和 9P 协议，还能通过 NPD 暴露成快设备，甚至在上面跑 ZFS 和虚拟机。数据用 XZ20、Zstd 1305 加密，ZSTD 压缩，通过了 8600 多个 PJDFSTest 用力和 Jepsen 验证。在它的 NPD 卷上编译 Linux 内核，只要 16 秒。Koala 认为，把对象存储当本地盘用的方案不少，比如 JuiceFS 和 S3backer。ZeroFS 的激进之处是单进程完成所有事，并直接支持快设备语义，测试投入也远超多数同类开源项目，适合想用 S3 的价格拿到本地盘体验的场景。但延迟敏感型负载在生产前还需要仔细压测。


---


### ShortScraper
[https://github.com/simonw/shortscraper](https://github.com/simonw/shortscraper)

ShortScraper 是 Simon Willison 开发的命令行截图工具。基于 Playwright，可以给网页批量截图、录制视频演示，还能执行 JavaScript 抓取数据。它和 GitHub Actions 配合得很好，官方提供了模板仓库，Dataset 的文档截图就靠它自动生成。路透社也用它定期更新数据仪表盘。GitHub 上有 2400 多 star。Koala 认为，截图看似是小需求，但在文档维护和监控场景里高频出现。ShortScraper 把它做成了可版本化、可进 CI 的流水线，这和手动截图有本质区别。Simon Willison 一贯擅长做这种小而美的工具，配合他的 llm 工具链，还能打出把网页内容喂给模型的组合拳。


---


### FreeGraphPaper
[https://freegraphpaper.com/](https://freegraphpaper.com/)

FreeGraphPaper 是一个在线网格纸生成器，免注册、无水印。选好模板后调整间距、颜色和边距，实时预览，再导出 PDF 或 PNG 直接打印。支持方格、点阵、等轴测、六边形、横线和康奈尔笔记纸，纸张覆盖 A4、US Letter 等规格，间距可精确到 5 毫米或 1/4 英寸，保证 100% 比例打印。Koala 认为，这类小工具网站的价值在于把一个具体需求做到零门槛，比起功能庞杂的绘图软件，打开即用反而最大卖点。手帐、数学练习、工程草图都是稳定需求，靠搜索流量、自利站点往往能长期存活，也是独立开发者做小产品的一个不错样本。


---


以上就是本期科技周报的全部内容，谢谢您的收看。如果内容对您有帮助，请一键三连支持我们！