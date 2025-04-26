---
title: "[Hacker News 周报] 高性能 JS 运行时 Bun；Electron 轻量级替代品；自动探测 Web 应用内存泄漏"
description: "了解科技资讯、把握行业脉搏。每周快速浏览 Hacker News 精选。本期 Hacker Newsletter 地址：https://mailchi.mp/hackernewsletter/611"
tags: []
date: 1657413000
bvid: BV1Wg411f7VV
---
了解科技资讯，把握行业脉搏，大家好，我是 Koala，欢迎收看第611期 Hacker News 周报。

### Bun｜高性能 JS 运行时
https://bun.sh/

首先是一个叫做 Bun 的 JavaScript 运行时，与已有的 Node.js 和 Deno 相比，Bun 主打的是有极快的性能，并将很多常用功能集成在自己内部。特别的是 Bun 是用一种比较新的小众语言 Zig 开发的。作者表示 Zig 可以帮助更好的管理内存和性能，这使得 Bun 具有极快的性能。不过虽然 Bun 还处在早期的测试阶段，还有很多待完善的工作，但已经发布已经受到了很多的关注。

---
### TAURI｜Electron 轻量级替代品
https://tauri.app/

Tauri 是一个基于 Web 前端技术开发桌面端应用工具，与常规的方案 Electron 相比，Tauri 会使用你本地已有的浏览器，而不是像其中再打包一个浏览器，这样会使得桌面应用的大小远小于基于 Electron 开发的软件。目前 Tauri 方案变得流行，它最近也发布了1.0版本。

---
### Felt｜在线地图编辑网站
https://felt.com/

想让自己的写好和需要创建一个地图吗？Felt 是一个网站，可以帮助你在线编辑地图。你可以在世界地图的基础上，去勾画特定的区域，特定的路线，或是做一些标注，还可以把你做好的地图在线分享出去。

---
### PocketBase｜ 开源实时后端方案
https://pocketbase.io/

PocketBase 是一个开源软件，它基于 SQLite 构建了一个实时后端，它主打轻量化，既在一个文件中提供包括前端和后端等所有功能。例如实时数据库，权限校验，文件存储和后台管理界面等。它的功能还是比较齐全的，如果你需要做一些轻量级的应用，可以考虑用它来作为后端服务。

---
### fuite｜自动探测 Web 应用内存泄漏
https://github.com/nolanlawson/fuite

下面是一个叫做 Fuite 的工具，它可以帮助你找到 Web 应用中可能存在的内存泄漏问题。它的工作方式是，当你启动浏览器，在里面持续运行一些测试脚本，并且观测这个过程中是否产生了一些没有被回收的内存对象，从而判定是否产生了内存泄漏。

---
### 一篇关于 rsync 工作原理的文章
https://michael.stapelberg.ch/posts/2022-07-02-rsync-how-does-it-work

最后是一篇系列文章，在他的第三部分详细介绍了大家常用的命令行工具 Rsync 的工作原理。Rsync 是以效率好和易用著称的，了解它的内部工作原理，也可以对数据传输和复制这些类型的工具有一个更好的理解。

---

以上就是本期 Hacker News 周报摘要，谢谢您的收看。

