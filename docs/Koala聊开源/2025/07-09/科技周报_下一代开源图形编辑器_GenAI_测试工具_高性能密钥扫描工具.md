---
title: "科技周报｜下一代开源图形编辑器；GenAI 测试工具；高性能密钥扫描工具"
description: "了解科技资讯、把握行业脉搏。每周快速浏览 Hacker News 精选。本期 Hacker Newsletter 地址：https://www.daemonology.net/hn-daily/"
tags: []
date: 1751770487
bvid: BV1eo3fzBEgV
---
### 下一代开源图形编辑器
https://github.com/GraphiteEditor/Graphite

Graphite 是一款基于 Rust 编写的开源 2D 图形编辑器。它的目标是成为一个全能 2D 内容创作工具，支持平面设计、数字艺术和实时动态图形。它最大的亮点是基于节点的程序化编辑。你可以通过链接不同的节点来创建复杂的图形效果，而且所有操作都是非破坏性的，随时可以回溯修改。

Koala 认为，尽管界面看上去有点像 Photoshop，但 Graphite 有着更大的野心，想做一个通用的图形工具箱，像游戏引擎一样强大。如果您是图形开发者或是 Rust 的爱好者，这是一个值得关注和参与的项目。

---

### GenAI 测试工具
https://www.evalite.dev/

Evalite 是一个专为生成式 AI 应用设计的测试工具，用 TypeScript 编写。使用方式和体验与您熟悉的单元测试没有差别。它提供了一个美观的交互式 UI，可以方便在本地查看输出、追踪和日志。

Evalite 基于 Vites 构建，因此可以无缝集成到你的现有技术栈中，使用 mocks 或 fixtures 等功能来模拟真实场景。它不依赖任何云平台或 API 密钥，所有数据都保存在你的本地机器上，无需担心数据安全和隐私问题。Koala 认为，对于使用 TypeScript 开发 GenAI 应用的开发者来说，Evalite 提供了一个简单、高效且安全的测试解决方案。

---

### 高性能密钥扫描工具
https://github.com/mongodb/kingfisher

Kingfisher 是 MongoDB 开源的一款高性能密钥扫描和验证工具。它结合了 Intel 的 Hyperscan 正则引擎和 Tree-sitter 的语言感知解析，内置了数百条规则，能在密钥泄露到生产环境之前就检测、验证和分类。

Kingfisher 不仅速度快，还能通过云服务 API 实时验证密钥的有效性，减少误报。无论是扫描本地代码仓库，还是 GitHub 和 GitLab 上的代码，Kingfisher 都能胜任。如果需要自行实现和 GitHub 类似的密钥检测功能，Kingfisher 是个不错的选择。

---

### 玻璃质感 CSS 生成器
https://glass3d.dev/

在苹果发布了新的视觉设计之后，半透明玻璃效果也变得流行。想给你的网页元素加上同样的视觉风格吗？Glass3D generator 就能帮你生成对应的 CSS。

它提供了一个可视化界面，你可以调整模糊度、亮度、饱和度、颜色等各种参数，实时预览效果。调整好之后，直接复制生成的 CSS 代码，就能应用到你的项目中了。

---

### 开源 CapCut 替代品
https://github.com/OpenCut-app/OpenCut

OpenCut 是一款开源的视频编辑器，目标是成为 CapCut 的替代品。它支持网页、桌面和移动平台，注重隐私保护。您的视频都保存在本地设备上。

OpenCut 提供时间线编辑、多轨道支持和实时预览等功能，没有水印和订阅限制。如果您正在寻找一款免费易用的轻量级视频编辑工具，不妨试试 OpenCut。项目本身使用 Next.js 构建，代码结构清晰，方便开发者参与贡献。

---

### 高性能 tokenizer 实现
https://github.com/M4THYOU/TokenDagger

TokenDagger 是 OpenAI 的 tiktoken 的一个高性能替代，专为大规模文本处理而设计。按照它的文档介绍，在部分基准测试中，吞吐量是 tiktoken 的两倍，在代码 token 化的场景中，速度快四倍。如果在你的文本处理流水线中有大规模的 token 化需求，且 tiktoken 等已有实现已经成为瓶颈，那么可以考虑用 TokenDagger 进行替换。

