---
title: "科技周报｜给 Agent 用的代码检索库；Obsidian 本地开源替代；GitHub Diff 的高性能替代"
description: ""
tags: []
date: 1779606096
bvid: BV1yYG76oESe
---
了解科技资讯，把握行业脉搏，大家好，我是Koala。欢迎收看科技周报。

---

### Semble | 给 Agent 用的代码检索库
Semble 是专为 Agent 设计的代码搜索库，号称比 grep 加 read 节省 98% 的 token。它的核心选型是用 Tree-sitter，解析代码语法树，把检索粒度精确到函数、类这种语义单元，而不是行级匹配。再叠加 BM25 词法检索和轻量嵌入做混合排序。索引一个仓库平均 250 毫秒，单次查询 1.5 毫秒。

可以作为 MCP server、CLI 或 Python 库接入。Koala 认为让 Agent 高效读代码这件事情，过去一年方案分两派：纯向量检索精度不稳，纯 grep 又烧 token。Semble 深耕 Tree-sitter 是个值得关注的选择。语法树天然对应代码的结构编辑，返回的片段更完整、更可用，比起 code embedding 猜语义要可靠得多。

---

### files.md | Obsidian 本地开源替代
files.md 是一个完全本地的 Markdown 笔记应用，数据不上云，提供 Web 版和机器人两种接口。它内置笔记、日志、待办、习惯等结构，但不强制使用。主打用聊天式输入，快速捕捉想法，再通过链接构建知识网络。

Koala 认为在 Obsidian、Notion、Logseq 这些越做越重的 PKM 工具大型其道时，files.md 的姿态相当反潮流。它的官网明确反对复杂的第二大脑系统，认为系统越完善，真正的思考反而越少。适合那些被插件、双链、模板搞得心累的用户回归本源。软件本身的交互体验也做得非常不错。

---

### DiffsHub | GitHub Diff 的高性能替代
DiffsHub 是一个 GitHub 代码差异查看器。使用方法很简单，把 URL 里的 github.com 换成 diffshub.com 就行。它的卖点是用虚拟化渲染，撑住超大规模 diff。宣称能流畅打开 Linux 内核版本间的对比，移动端浏览器也不会崩。PR、commit、compare、patch 这几个页面都能接管。

Koala 认为，最后这家公司 Peary，我们之前介绍过他们的两个底层组件：filetree 和 diff。DiffsHub 就是基于这两个组件搭出来的上层产品。可以看出他们再往 Patch Review 这个垂直方向深耕。这个时机也很合理，AI 让代码产出速度爆炸增长，Code Review 的工具体验反而成了瓶颈。GitHub 原生 Diff 在大 PR 下卡顿是公认痛点。垂直工具用更好的工程实现来抢占体验是个合理的切入角度。

---

### dotlottie-web | Web 版 Lottie 播放器
dotlottie-web 是 LottieFiles 官方推出的新一代网页动画播放器。基于 Rust WebAssembly 实现，同时支持 Canvas 2D、WebGL2 和实验性的 WebGPU 后端。它和 iOS、Android 客户端共享同一个内核，跨端表现完全一致。

新格式 dotlottie v2 原生支持状态机、运行时主题切换、嵌入音频，老的 JSON 也能兼容。官方提供了 Vanilla JS、React、Vue 等六套 SDK。Koala 认为 Lottie 生态长期被各端实现不一致拖累。同一个动画，iOS 上正常，Web 上掉帧或样式错位是常态。这次 LottieFiles 用 Rust 内核统一全平台渲染，是从根本上解决问题。dotlottie v2 加入状态机和主题切换，也把 Lottie 从播放动画推向交互组件。对设计师和前端协作流程是个升级。

---

### Polypad | 数学虚拟教具集大成者
Polypad 是教育公司 Amplify 推出的免费在线数学操作平台，免登录，跨设备可用。它把传统课堂的实物教具搬到屏幕上，形成了分数条、3D 多面体、天平、函数机、转盘、数据科学工具、逻辑门等几十种模块，覆盖从小学算术到中学逻辑、数据科学的全跨度。

Koala 认为 Polypad 内置的丰富模块，让交互式的数学教学变为可能。原本有一定上手门槛的模块搭建过程，如果能与 Agent 结合变为自然语言交互，很有可能获得更多的落地机会。

---

### Kubernetes Skill | 深度优化的 K8s Skill
分享一个给 Agent 用的 Kubernetes Skill。专门解决 LLM 生成 K8S 配置时常见的标签不对齐、端口不一致、安全默认值缺失等问题。它的方法论叫 Failure Mode First。先用六类已知故障模式预先诊断风险，再生成 YAML，减少幻觉。配套了 20 份按需加载的参考文挡，覆盖安全、网络、RBAC、健康检查、存储等。

Koala 认为作者对 Skill 机制的理解相当不错。把领域知识按需加载，激活成本压到几百 token。比起单纯让 LLM 记住 K8S 最佳实践，Failure Mode First 这种先验证再生成的工作流是更加可靠。虽然 LLM 对 K8S 的通识不错，但是结合这样的专家型 Skill 还能进一步提升可靠性。

---

以上就是本期科技周报的全部内容，谢谢您的收看。如果内容对您有帮助，请一键三连支持我们。

