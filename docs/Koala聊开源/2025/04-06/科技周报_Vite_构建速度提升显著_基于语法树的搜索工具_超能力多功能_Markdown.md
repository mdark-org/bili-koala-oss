---
title: "科技周报｜Vite 构建速度提升显著；基于语法树的搜索工具；超能力多功能 Markdown"
description: "了解科技资讯、把握行业脉搏。每周快速浏览 Hacker News 精选。本期 Hacker Newsletter 地址：https://buttondown.com/hacker-newsletter/archive/hacker-newsletter-749/"
tags: []
date: 1749352553
bvid: BV1drTUzPEuD
---
了解科技资讯，把握行业脉搏。

大家好，我是Koala。欢迎收看科技周报。

### Rolldown-Vite | Vite 构建速度提升显著
https://voidzero.dev/posts/announcing-rolldown-vite

Vite 团队正式推出 Rolldown-Vite，这是一个基于 Rust 的下一代打包工具，目标是成为 Vite 默认的打包器。简单来说，你可以通过替换 Vite 包为 Rolldown-Vite 来体验它。

已经有早期用户反馈，构建速度提升了 3 到 16 倍，内存占用也大大降低。如果你想让你的 Vite 项目速度起飞，不妨试试 Rolldown-Vite。

切换后，ESBuild 也变成了可选依赖，进一步提升安装体验。已经体验的小伙伴，Vite 团队也鼓励大家到 GitHub 上反馈你的使用感受。

---

### ast-grep | 基于语法树的搜索工具
https://ast-grep.github.io/

AST-grep 是一个支持多语言的代码搜索与重构工具，基于抽象语法树进行结构化搜索。它允许开发者使用模式精准定位源码，支持 CLI、编辑器插件和程序 API，适合代码审查、重构和自定义 Lint 规则等场景。

此项目由 Herrington Darkholme 推荐，感谢你的投稿。

---

### Quarkdown | 超能力多功能 Markdown
https://github.com/iamgio/quarkdown

Quarkdown 是一款基于 Markdown 的现代排版系统，核心概念是多功能性。通过内置的扩展语法和配套的编译器，它可以将 Quarkdown 文档编译成可直接用于印刷的书籍或交互式演示文稿。

它不仅可以用于做复杂的排版布局，还支持自定义函数和变量实现各种动态视图，让你的 Quarkdown 文件更加强大。总的来说，Quarkdown 扩展了 Markdown 的功能，让它不仅仅是简单的文本标记语言，更像是一个轻量级的排版工具。

---

### Workers OAuth Provider | 为 CloudFlare Workers 添加 OAuth 认证
https://github.com/cloudflare/workers-oauth-provider

想给你的 CloudFlare Workers 应用加上 OAuth 认证，但又觉得自己从头开始实现太琐碎吗？CloudFlare 发布了 Workers Olds Provider 帮你搞定。它实现了 Olds 2.1 协议，你只需要像平常一样写你的 API handler，就能拿到已经认证的用户信息，不用自己做任何检查。

这个库不关心你如何管理用户，也不限制你使用什么 UI 框架。而且，它只存储 token 的哈希值，保证安全性。

另外一个有趣的细节是，该仓库的 README 中作者提到该项目极大程度上是和 Clo AI 共同编写的，并在早期的 commit 中带上了 prompt 信息。作者表示，作为延迟程度很高的认证功能，项目代码经过专家的严格审查。审核者都认为 Clo AI 在项目中的表现非常不错。

---

### go-binsize-treemap | Go binary 体积可视化工具
https://github.com/nikolaydubina/go-binsize-treemap

Go by size tree map 这个工具可以帮你分析 Go 语言编译出的二进制文件，然后生成一个 SVG 格式的 tree map，让你清晰的看到二进制文件中各个部分的大小占比。

这工具有啥用呢？如果你想研究编译器的工作原理，或者想看看你的项目里都包含了哪些第三方依赖，再或者你想优化你的 Go 代码，减少最终生成的可执行文件的大小，那么这个工具决定能帮得上你。使用起来也很简单，一条命令就能搞定。

---

### Go 官方 | 不再改进错误处理语法
https://go.dev/blog/error-syntax

Go 语言团队宣布，短期内将不再寻求通过语法层面修改来改进错误处理。长期以来，Go 的错误处理方式因冗长而备受诟病。大量的 if error 不为 nil 代码块让代码可读性降低。

官方曾尝试试过 check handle、try 以及问号等方案，但都没能获得社区的广泛支持。官方认为，Go 已经有了一套完善的错误处理机制，即使它看起来有些繁琐。而且，强行推行新的语法可能会导致用户群体分裂。

虽然不排除未来重新考虑，但目前团队将专注于其他 Go 语言的改进。

---

以上就是本期科技周报的全部内容，谢谢你的收看。

如果内容对您有帮助，请一件三连支持我们。

