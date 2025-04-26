---
title: "[Hacker News 周报] Python 开发者的完美终端工具；、Systemd 示例教程；你的云上数据库安全吗？"
description: "了解科技资讯、把握行业脉搏。每周快速浏览 Hacker News 精选。Hacker Newsletter 和 Hacker News Daily 地址：https://mailchi.mp/hackernewsletter/589；https://www.daemonology.net/hn-daily/"
tags: []
date: 1644106890
bvid: BV1nL4y1s7q1
---
了解科技资讯，把握行业脉搏，大家好，我是Koala。
欢迎收看第589期Hacker News周报。

---
### Hibiki

https://www.hibikihtml.com/

Hibiki 自称是一个新的强大前端框架，可开发现代化的动态前端应用，而不必使用JavaScript。
与之前周报中曾介绍过的一些类似方案一样，大家都在考虑减少JavaScript的使用。
在我们做的调研中，很多同学通过弹幕投票也表达过前端开发工具过于复杂。
这些新的框架是否已生产可用，还不得而知，不过前端开发正在寻求新的方向，看来已是事实。

---
### Systemd by example

https://seb.jambor.dev/posts/systemd-by-example-part-1-minimization/

Systemd是一个常用的系统服务，在日常使用中，大家可能不一定了解它的使用细节。

这篇博客的作者介绍了他开发的一个Systemd使用的cheat sheet，以及他开发的初衷，通过修改配置文件，你可以观察Systemd的工作方式是否符合你的预期，进一步掌握它的使用技巧。

---
### Malloy | SQL 方言
https://github.com/malloydata/malloy

Malloy是一个实验性语言，用来描述数据的关联关系和变化方式，与上一期介绍的PRQL一样，它们都是SQL的一种方言，也会转译为SQL。
虽然这种新兴工具的使用性还有待观察，但可由此看出业界对查询语言的研究方向。

---

### Rich CLI

Rich-cli是用Python编写的命令行工具，是基于一个使用非常广泛的命令行库Rich开发的。
Rich可以帮助你在终端上打印各种格式丰富的内容，而Rich-cli就是对Rich功能的进一步简化。
如果你是命令行的重度使用者，可以了解一下这个工具，看是否合用。

---

### 博客文章 ｜ 我在AWS上发现数了以千计的开放数据库

https://infosecwriteups.com/how-i-discovered-thousands-of-open-databases-on-aws-764729aa7f32

最后是一篇博客，博客作者介绍了他是如何在AWS上发现数以千计的开放数据库的。
在作者的hack经历中，他首先对IP段进行了扫描，再对IP特定端口的返回结果进行记录后，他就获得了几十万条结果。
这些结果中很多使用了Kibana，Elastic这些典型的服务端口。
虽然使用Elastic Search Rest API很方便，但对于那些没有进行保护的数据库，只要知道它的端口，以作者的经历，他就可以进一步获得更多的数据。
总之，博客介绍了数据库挖掘的过程，并揭示了对数据安全的危害性，作者希望以此提醒，在云服务越来越方便的今天，一定要特别重视数据安全，在使用公有云服务时，务必去了解这些安全配置，否则会面临数据安全的风险。

---

以上就是本期Hacker News周报的摘要，谢谢您的收看，喜欢的话请一键三连，我们下期见。

