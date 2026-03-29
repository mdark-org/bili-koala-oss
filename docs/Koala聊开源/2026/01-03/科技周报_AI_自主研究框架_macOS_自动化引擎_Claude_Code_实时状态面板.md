---
title: "科技周报｜AI 自主研究框架；macOS 自动化引擎；Claude Code 实时状态面板"
description: ""
tags: []
date: 1774755422
bvid: BV1WbXUBGEJr
---
了解科技资讯，把握行业脉搏，大家好，我是Koala。欢迎收看科技周报。

### AutoResearch | AI 自主研究框架
AutoResearch 是 Capacity 开源的自主 AI 研究框架，让 Claude 等 AI Agent 在夜间自动进行机器学习实验。它给 Agent 一个小型 LLM 训练环境，每次实验固定五分钟训练预算。Agent 只能修改 `train.py` 这一个文件，用 `validation based per byte` 作为统一指标评估效果。

研究者通过编写 `program.md` 来定义 Agent 的实验策略。在 H100 上大约每小时能跑 12 轮实验，一晚上可以迭代约 100 次。Koala 认为，Capacity 的项目总能精准把握 AI 社区的脉搏。这次想验证的是 AI Agent 在受限环境下能否做出有意义的研究迭代。

五分钟预算和单文件约束的设计非常克制，既控制了风险，又保证了可复现性。这可能是 AI 辅助研究从工具走向自动研究者的早期信号，但目前仍需人类定义实验方向，离真正的自主研究还有距离。

---

### Hammerspoon | macOS 自动化引擎
Hammerspoon 是一个 macOS 自动化工具，充当操作系统和 Lua 脚本引擎之间的桥梁。你可以用 Lua 脚本控制窗口管理、键盘快捷键、Wi-Fi 事件、电池监控、剪贴板操作等几乎所有系统功能。

它开箱即用时什么都不做，完全由用户在 `Hammerspoon init.lua` 中定义行为，还支持通过 Spoons 插件扩展功能。Koala 认为，Hammerspoon 是 macOS 自动化领域的老牌项目。选择 Lua 作为脚本语言，让它在性能和易用性之间找到了不错的平衡点。

与 Shortcuts、BetterTouchTool 等图形化方案相比，它的上限更高，但学习曲线也更陡，适合喜欢用代码掌控一切的 Power User，不适合追求开箱即用的普通用户。

---

### Claude HUD | Claude Code 实时状态面板
Claude HUD 是一个 Code Code 插件，能在终端底部显示一个持久状态栏，实时展示上下文窗口使用量、Token 消耗、活跃工具、Agent 的运行状态和 Todo 进度。

它基于 Cloud Code 的 Status Line API 构建，支持三种预设布局和 30 多项自定义配置，包括颜色方案和显示元素排列。

---

### Email.md | Markdown 写邮件
Email.md 让你用 Markdown 语法写出响应式邮件，彻底告别 HTML 邮件模板的复杂性。它提供 NPM 包和命令行工具，内置多重邮件模板、可视化编辑器和实时预览，支持主题切换和组件系统。

整个开源项目由 NMT 团队维护。Koala 认为，HTML 邮件开发一直是前端领域的老大难问题。各邮件客户端对 CSS 的支持参差不齐，开发体验停留在 10 年前。Email.md 用 Markdown 抽象掉了底层兼容性细节，对 Agent 也更加友好。

---

### TUI Studio | 终端 UI 可视化编辑器
TUI Studio 是一个类似 Figma 的可视化编辑器，专门用来设计终端界面应用。你可以拖拽 21 种以上的内置组件到画布上，实时预览 ANSI 渲染效果，支持 Absolute、Flexbox 和 Grid 三种布局模式。

内置 Dracula、Node 等八种配色主题。项目保存为可版本控制的 JSON 文件，计划支持导出到 Ink、Bubble Tea、Textual 等六个主流 TUI 框架。Koala 认为，终端 UI 开发一直是纯代码驱动的领域。TUI Studio 试图用可视化编辑来降低门槛，想法很有吸引力，并且现在越来越多的 TUI 项目也需要设计。

---

### Portless | 本地服务对外暴露方案
Portless 是 Vercel 推出的 CLI 工具，把开发环境中的 localhost 3000 替换成 `https://my-app.localhost` 这样的命名 URL。它自动生成并信任 HTTPS 证书，支持子域名组织多服务，自动检测 Git 工作区并按分支分配域名，还能为 Vite、Astro 等主流框架自动注入兼容参数。

跨平台支持 macOS、Linux 和 Windows。默认运行在 1355 端口。Koala 认为，同类产品很多，Vercel 更多还是将它们在开发体验方面的深度积累，融入到默认配置中，减少用户踩坑的概率。

---

以上就是本期科技周报的全部内容，谢谢你的收看。如果内容对您有帮助，请一键三连支持我们。

---

**相关链接：**
搜索查询已发布项目的图文，大家可以访问「Koala 聊开源」官网 https://koala-oss.app 的「科技周报」数据库。
本期 Hacker Newsletter 地址：https://www.daemonology.net/hn-daily/

