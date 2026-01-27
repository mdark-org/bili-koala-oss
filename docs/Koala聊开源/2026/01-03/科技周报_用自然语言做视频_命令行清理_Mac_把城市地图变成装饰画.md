---
title: "科技周报｜用自然语言做视频；命令行清理 Mac；把城市地图变成装饰画"
description: ""
tags: []
date: 1769345813
bvid: BV1NozxBmEe3
---
了解科技资讯，把握行业脉搏，大家好，我是 Koala。欢迎收看科技周报。

---

### 用自然语言做视频

Remotion 一直是用 React 组件做视频的标杆。这一次，他们发布了专为 AI Agent 优化的 Skills 工具包。开发者可以让 Cloud Code 等 Agent 用自然语言生成动画代码，不用手写 TypeScript。它还支持 MCP 协议集成，方便嵌入各类 AI 工作流。

Koala 认为，本频道一直认为程序化视频是重要的更新，也使用 Remotion 制作了多期视频动画，并发布教程。把视频制作门槛从会 React 降到会说话，对产品演示视频和动态内容创作者是重大利好。Skills 也降低了使用者学习 Remotion 的负担。

---

### 命令行清理 Mac

Mot 是一个 Shell 脚本加 Go 写成的 Mac 清理工具。功能覆盖缓存清理、残留卸载、磁盘分析和系统状态监控。基本是 CleanMyMac 的命令行平替。支持 Touch ID 授权 sudo，还能对接 Raycast 快速调用。

Koala 认为，免费开源且单文件部署是核心卖点。7000 加 Star 证明开发者对付费清理软件的不满是真实的。Mot 的清理足够自动且全面，但系统清理类工具始终有风险。建议先用 Dry Run 预览，重要数据做好备份。

---

### 把城市地图变成装饰画

Map to Poster 是一个 Python 脚本，输入城市名则会输出一张极简风格的城市地图海报。数据来自 OpenStreetMap，内置 17 种配色主题，从赛博朋克到日式水墨都有。代码结构简单，自定义主题只需编辑一个 JSON 文件。

Koala 认为，该项目技术复杂度不高，但实用性强，适合做快手礼物或装饰品。6900 多 Star 也说明这类小而美的工具依然有市场。如果你做地理相关产品，该项目使用的 OSMnx 库也值得学习研究。

---

### Playwright CLI

Playwright 封装成一套 CLI 命令，专门为 AI Agent 设计。用 Snapshot 命令获取页面元素引用，再用 Click、Fill 等命令操作。整个流程无需写测试代码，还能作为 Skills 安装至不同 Agent 中。

Playwright CLI 的思路并非首创，几天之前，Vercel 的工程师就推出了 Agent Bowzer 项目。定位为 API 设计，基本与后出现的 Playwright CLI 一致。但 Vercel 选择了 Rust 加 Node.js 混合架构。核心卖点是 Snapshot 命令输出的无障碍树。AI 可以用元素引用直接操作，不用纠结 CSS 选择器。还支持 Session 隔离、流式视频预览和 CDP 协议连接。

Koala 认为，目前 AI 操作浏览器的方案还远不如 AI 编程成熟，各方都在推出更好的方案，抢夺这块市场。

---

### ChatGPU

浏览器端的数据可视化一直受限于 Canvas 和 SVG 的绘制性能瓶颈，在大规模数据可视化中表现一般。ChatGPU 选择了一条不同的道路，充分使用 WebGPU 渲染图表，将更多计算任务放入 WebGPU 中进行。在功能层面，它支持折线图、柱状图、K 线图等常见类型。内置交互手势和缩放滑块。项目用 TypeScript 编写，配套的 React 绑定也已就绪。

Koala 认为，WebGPU 用于图表是个有趣的技术选型。但目前 WebGPU 的浏览器兼容性较弱，生产环境还不推荐使用。对 WebGPU API 有兴趣的小伙伴，可以通过该项目学习其中细节。

---

### Agentation

Agentation 是一个轻量的 React 组件，让用户可以在 React 应用中选择指定区域并标记信息。主要使用场景是使用 AI Agent 编程时，可以从开发的 UI 界面中快速反馈，让 Agent 进行修改。除了基本的点击之外，还支持多选、区域框选，甚至暂停 CSS 动画来捕捉特定状态。

Koala 认为，Agentation 是一款非常垂直的工具，解决的是 AI Coding 工作流中沟通效率问题。与其用文字描述右边那个蓝色按钮，不如直接给一个 `sidebar button primary`。特别对于没有代码知识的 Web Coding 用户来说，值得一试。

---

以上就是本期科技周报的全部内容，谢谢你的收看。如果内容对您有帮助，请一键三连支持我们。

