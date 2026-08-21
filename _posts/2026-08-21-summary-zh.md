---
layout: default
title: "Horizon 日报：2026-08-21 (ZH)"
date: 2026-08-21
lang: zh
---

> 从 48 条内容中筛选出 14 条重要资讯。

---

1. [恶意 Rust crate Arrayref 在构建时执行载荷](#item-1) ⭐️ 9.0/10
2. [GitHub 8 月 17 日宕机复盘：重试风暴风险凸显](#item-2) ⭐️ 8.0/10
3. [速卖通无声 WebAudio 指纹识别干扰蓝牙多点连接](#item-3) ⭐️ 8.0/10
4. [HTML 也能做到：现代 HTML 特性取代 JavaScript](#item-4) ⭐️ 8.0/10
5. [用 125M 模型在设备上自动补全钢琴演奏](#item-5) ⭐️ 8.0/10
6. [共享哈希表能否加速 PostgreSQL 并行聚合？](#item-6) ⭐️ 8.0/10
7. [Databricks 收购 Electric，PGlite 嵌入式 PostgreSQL 的开发者](#item-7) ⭐️ 8.0/10
8. [公民构建，智能体执行，专家治理](#item-8) ⭐️ 8.0/10
9. [Bun 1.4 的 Bun.WebView 实现了 shot-scraper 风格的 JSON API](#item-9) ⭐️ 8.0/10
10. [Rider 让 AI 代理使用重构引擎，代码修改更安全](#item-10) ⭐️ 7.0/10
11. [pg_shmemviz：PostgreSQL 共享内存可视化新工具](#item-11) ⭐️ 7.0/10
12. [使用事务发件箱和 QStash 构建可重试安全的 HubSpot 同步](#item-12) ⭐️ 7.0/10
13. [join_collapse_limit：PostgreSQL 文档化的连接顺序控制](#item-13) ⭐️ 7.0/10
14. [ChatGPT 搜索在 GPT-5.6 后大规模采用 site:操作符](#item-14) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [恶意 Rust crate Arrayref 在构建时执行载荷](https://safedep.io/arrayref-proc-macro1-rust-build-time-malware/) ⭐️ 9.0/10

Rust crate 'arrayref' 的恶意版本在构建时执行恶意负载，引发了官方和社区对 crates.io 安全事件处理的回应。

hackernews · abhisek · 8月20日 13:23 · [社区讨论](https://news.ycombinator.com/item?id=49374269)

**标签**: `#supply chain`, `#Rust`, `#security`, `#malware`, `#crates.io`

---

<a id="item-2"></a>
## [GitHub 8 月 17 日宕机复盘：重试风暴风险凸显](https://github.blog/news-insights/company-news/the-august-17-outage-and-the-work-ahead/) ⭐️ 8.0/10

GitHub 发布了 8 月 17 日宕机的根因分析，将原因归于重试放大的流量以及自 4 月以来月度提交量从 14 亿增长到 29 亿的创纪录速度。VS Code 中一个潜在的重试缺陷将流量放大了约 10 倍，导致 Copilot Token Service 恢复延迟。 这次宕机凸显了大规模分布式系统在指数级增长下的脆弱性，尤其是善意的重试逻辑如何引发级联故障。这对所有依赖 GitHub 的开发者以及设计弹性系统的平台工程师都至关重要。 依赖服务中的错误触发了客户端重试循环，在恢复期间增加了流量，而单个内部端点的延迟响应则暴露了 VS Code 的重试缺陷。复盘报告强调了分布式架构中重试风暴的危险性。

hackernews · 0xedb · 8月20日 19:22 · [社区讨论](https://news.ycombinator.com/item?id=49378957)

**背景**: 重试风暴是指临时故障导致大量客户端反复重试，从而放大流量并进一步压垮系统的现象。分布式系统通常采用指数退避、熔断器和抖动来避免此类反馈循环。GitHub 在 AI 辅助开发推动下的快速增长，给其基础设施带来了更大压力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2511.23278">RetryGuard: Preventing Self-Inflicted and Attack-Driven Retry Storms in Cloud Applications</a></li>
<li><a href="https://medium.com/@kandaanusha/the-retry-storm-when-your-reliability-strategy-becomes-your-worst-enemy-cec77ddaa20c">The “Retry Storm”: When Your Reliability Strategy Becomes Your Worst Enemy | by Kandaanusha | Medium</a></li>
<li><a href="https://medium.com/@pranesh005/retry-storms-139869b956e3">Retry Storms . The Hidden Failure Mode in Distributed | Medium</a></li>

</ul>
</details>

**社区讨论**: 评论者反应强烈：cube00 批评了隐藏错误的倾向，指出用户盯着加载动画数小时；blakesterz 对月度提交量的激增感到惊叹。madrox 怀疑 GitHub 能否承受这种规模，其他人则质疑这些新代码都是什么，有人称之为“生产力恐慌”。

**标签**: `#GitHub`, `#outage`, `#reliability`, `#infrastructure`, `#DevOps`

---

<a id="item-3"></a>
## [速卖通无声 WebAudio 指纹识别干扰蓝牙多点连接](https://blog.laserphile.com/2026/08/aliexpress-webpage-keeping-multipoint.html) ⭐️ 8.0/10

一项新调查显示，速卖通（AliExpress）网页会执行无声的 WebAudio 指纹识别，这种隐藏的音频处理会意外破坏用户设备上的蓝牙多点连接（Bluetooth multipoint）。该问题由 laserphile.com 博客记录后迅速引发广泛关注。 此事意义重大，因为一家大型电商网站正在悄悄对访客进行指纹识别，同时还干扰了耳机、音箱常用的蓝牙多点连接功能。它表明指纹识别脚本可能带来真实且意想不到的副作用，也进一步促使浏览器对无声音频播放进行提示或拦截。 WebAudio 指纹识别通过渲染音频并读取依赖硬件的信号特征来实现；这条无声音频流显然会占用蓝牙链路，使多点连接将其当作活跃音源。部分浏览器已对 WebAudio 指纹识别进行缓解，据报道 Safari 26 默认会扰乱指纹识别脚本的输出，但其他浏览器中仍会出现这一副作用。

hackernews · emctech · 8月20日 10:08 · [社区讨论](https://news.ycombinator.com/item?id=49372583)

**背景**: WebAudio 是一个浏览器 API，允许网页处理和合成音频；但由于不同硬件渲染音频时存在微小差异，这些差异可被用来生成稳定的浏览器指纹。蓝牙多点连接（Bluetooth multipoint）让一副耳机或一个音箱同时连接多台设备，并在它们的音频流之间切换。无声的音频指纹识别流因此可能被当作活跃音源，导致多点连接无法保持空闲状态并等待其他设备播放真正的音频。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.elseif.net/stories/aliexpress-runs-silent-webaudio-fingerprinting-that-breaks-bluetooth-m-4d2c69f">AliExpress silent WebAudio fingerprinting keeps Bluetooth... — elseif</a></li>
<li><a href="https://web-tracking.allenchou.cc/docs/browser-fingerprinting/techniques/audio-fingerprinting/">WebAudio Fingerprinting | Web Tracking 筆記</a></li>
<li><a href="https://www.gblock.app/articles/safari-26-fingerprinting-protection-privacy">Safari 26 Scrambles Every Fingerprinting Script by Default</a></li>
<li><a href="https://www.engadget.com/2226189/heres-why-dont-buy-headphones-bluetooth-multipoint/">Here's Why You Shouldn't Buy New Headphones Without Bluetooth ...</a></li>

</ul>
</details>

**社区讨论**: 评论者的反应混杂着抱怨与技术分析：有人希望无声播放能触发浏览器标签页的扬声器图标，也有人报告在访问速卖通后助听器和车载音响出现异常。开发者指出 Firefox 已在很大程度上缓解了 WebAudio 指纹识别，还有不少用户质疑如果速卖通 App 也造成类似问题，苹果的封闭生态是否能保护用户。整体来看，讨论普遍认为无声音频指纹识别需要更好的检测手段和用户控制。

**标签**: `#WebAudio fingerprinting`, `#privacy`, `#Bluetooth`, `#browser security`, `#AliExpress`

---

<a id="item-4"></a>
## [HTML 也能做到：现代 HTML 特性取代 JavaScript](https://chrisburnell.com/html-can-do-that/) ⭐️ 8.0/10

Chris Burnell 的文章《HTML Can Do That》是一份实用指南，介绍 popover、dialog 和 Invoker Commands API 等现代 HTML 元素与 API，它们可以取代 JavaScript 来实现许多常见的界面模式。 这很重要，因为它帮助前端开发者减少对 JavaScript 的依赖，从而提升性能、可访问性和可维护性。它也标志着整个行业正在向声明式 HTML 和渐进增强的方向转变。 该指南介绍了 popover 属性、dialog 元素和 Invoker Commands API，它们都渲染在浏览器的顶层（top layer）并内置无障碍支持。不过，将 popover 定位到触发元素附近仍然比较困难，而且浏览器支持仍在逐步完善中。

hackernews · encyclopedism · 8月19日 15:11 · [社区讨论](https://news.ycombinator.com/item?id=49362689)

**背景**: popover 属性是一种 HTML 全局属性，可以把任何元素变成弹出层；dialog 元素则原生支持模态和非模态对话框。Invoker Commands API 允许开发者以声明方式为按钮指定行为，从而无需编写 JavaScript 就能调用对话框、弹出层等交互元素。这些特性是更广泛的浏览器原生 UI 基元的一部分，旨在鼓励渐进增强的开发方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Global_attributes/popover">popover HTML global attribute - HTML | MDN</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/dialog">HTML dialog element - HTML | MDN - MDN Web Docs</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Invoker_Commands_API">Invoker Commands API - Web APIs | MDN</a></li>

</ul>
</details>

**社区讨论**: 评论者表示这些特性在生产环境中表现良好，一位开发者说他们的整个应用都在大量使用 popover、dialog 和 invoker commands。主要的保留意见包括：将 popover 定位到触发元素附近比较困难、datalist 作为 combobox 替代品有局限，以及有人希望日期输入能强制使用 ISO 格式等。

**标签**: `#HTML`, `#Web Development`, `#Frontend`, `#Browser APIs`, `#Progressive Enhancement`

---

<a id="item-5"></a>
## [用 125M 模型在设备上自动补全钢琴演奏](https://simedw.com/2026/08/20/midi-autocomplete/) ⭐️ 8.0/10

一个 125M 参数的 Transformer 模型被训练用于在 iPhone 15 上实时自动续写 MIDI 钢琴演奏，完全在设备上运行，速度约为每秒 108 个音符。 这展示了 Transformer 自动补全在音乐领域的新应用，类似于 GitHub Copilot 和 Tabnine 等代码补全工具。这也表明大型语言风格的模型可以在消费级硬件上高效运行，使人人都能使用交互式 AI 辅助音乐创作。 该模型是一个 125M 参数的 Transformer，转换为 Core ML 以实现在设备端推理。开发者提到许多方案没有成功，但最终系统能在 iPhone 15 上实时自动续写。

hackernews · simedw · 8月20日 12:04 · [社区讨论](https://news.ycombinator.com/item?id=49373456)

**背景**: Core ML 是苹果公司用于将机器学习模型集成到应用中的框架，提供统一的模型表示和 API，支持设备端预测和微调。MIDI 是一个连接电子乐器、存储和交换音乐演奏数据（如音符音高、时值和力度）的技术标准。该项目的灵感来源于 Tabnine 等代码自动补全工具，后者利用生成式 AI 根据上下文提供代码补全建议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Core_ML">Core ML</a></li>
<li><a href="https://en.wikipedia.org/wiki/MIDI">MIDI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tabnine">Tabnine</a></li>

</ul>
</details>

**社区讨论**: 评论者将其与古典作曲家的训练方式以及基于 AI 的用户体验设计工具进行类比，指出当生成成本为零时，品味和探索才是关键。一位钢琴家评论者对模型出人意料的方向感到不安，另一些人则好奇训练数据规模和后训练方法。

**标签**: `#machine-learning`, `#music-generation`, `#transformers`, `#on-device-ai`, `#core-ml`

---

<a id="item-6"></a>
## [共享哈希表能否加速 PostgreSQL 并行聚合？](https://postgr.es/p/9sR) ⭐️ 8.0/10

Andrei Lepikhov 测试了共享哈希表能否加速 PostgreSQL 的并行聚合，并将该想法实现为一组可工作的补丁集，在 Google Cloud 的多核实例上进行了基准测试。结果表明该假设只部分成立：将分组查找从 LWLock 下移出解决了最大的瓶颈，但其下至少还隐藏着三个其他问题。 这很重要，因为并行聚合在真实负载中很常见，而现有的 Partial/Finalize 实现对于哈希代价高、分组数多的查询可能比串行执行更慢。如果共享哈希表被证明切实可行，它有望提升查询性能，并改变 PostgreSQL 对聚合的执行计划方式。 在示例查询中，300 万输入行产生近 60 万个分组，约 244 万个部分聚合状态通过 Gather 节点传输，而并行计划最终比串行计划慢近一倍。作者还指出，新发现的三个问题中有两个在论文中不可见，因为论文假设的是线程模型引擎，而非 PostgreSQL 基于进程的架构。

rss · Planet PostgreSQL · 8月20日 17:50

**背景**: PostgreSQL 目前通过两个阶段支持并行聚合：工作进程计算部分聚合，领导者进程完成最终聚合，行数据通过 Gather 节点交换。共享哈希表方案则让所有工作进程直接写入一张由轻量级锁（LWLock）保护的公共表。文章评估了近期一篇论文的观点——只要把分组查找从锁下移出，共享哈希表就是可行的；并将该方案与哈希分区、SQL Server 的 Repartition Streams 等方式进行了比较。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/parallel-plans.html">PostgreSQL: Documentation: 18: 15.3. Parallel Plans</a></li>
<li><a href="https://www.pgedge.com/blog/do-global-hash-tables-strike-back-in-postgresql">Do Global Hash Tables Strike Back in PostgreSQL ?</a></li>
<li><a href="https://www.interdb.jp/pg/pgsql03/07.html">3.7. Parallel Query :: Hironobu SUZUKI @ InterDB</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#parallel aggregation`, `#hash tables`, `#performance`, `#query execution`

---

<a id="item-7"></a>
## [Databricks 收购 Electric，PGlite 嵌入式 PostgreSQL 的开发者](https://postgr.es/p/9sG) ⭐️ 8.0/10

Databricks 已收购 Electric，即 PGlite 的开发者。PGlite 是 PostgreSQL 的 WebAssembly 版本，可运行在浏览器、无服务器环境和 AI 代理沙箱中。据报道，PGlite 的周下载量在约 12 个月内从 100 万增长到 1300 万。 此次收购凸显了嵌入式数据库在 AI 代理架构中日益重要的地位，本地状态管理可降低延迟和耦合度。同时，当每个代理都运行自己的 PostgreSQL 实例时，也带来了“哪个数据库拥有真相”的架构问题。 PGlite 基于 PostgreSQL 的单用户模式编译为 WebAssembly，并以 TypeScript 库的形式打包，可用于浏览器、Node.js、Bun 和 Deno。Electric 还开发了同步技术，将分布式的本地 PGlite 实例连接到中央 PostgreSQL 系统；Databricks 现在将其定位为将 lakehouse 扩展到边缘：PGlite 运行在沙箱中，而中央 Lakebase PostgreSQL 提供共享状态。

rss · Planet PostgreSQL · 8月19日 05:06

**背景**: PGlite 是 PostgreSQL 的 WebAssembly 构建版本，允许完整的 Postgres 数据库在浏览器、边缘函数等环境中无需外部依赖即可运行。它基于 PostgreSQL 的单用户模式，该模式在编译为 WASM 时提供了与数据库交互的输入/输出通道。嵌入式数据库越来越广泛地用于本地优先应用和 AI 代理工作流，以使状态更接近计算。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/electric-sql/pglite">GitHub - electric-sql/pglite: Embeddable Postgres with real-time, reactive bindings. · GitHub</a></li>
<li><a href="https://www.infoq.com/news/2024/05/pglite-wasm-postgres-browser/">Running PostgreSQL in the Browser with WebAssembly - InfoQ</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#WebAssembly`, `#AI Agents`, `#Database`, `#Databricks`

---

<a id="item-8"></a>
## [公民构建，智能体执行，专家治理](https://martinfowler.com/rachels-ramblings/citizens-agents-experts.html) ⭐️ 8.0/10

在这篇文章中，Martin Fowler 认为，非工程师借助 AI 在周末构建应用的能力并不等于企业软件工程，并提出了一个“公民构建、智能体执行、专家治理”的模型。 这篇文章回应了高管中常见的误解——认为 AI 能让工程团队快十倍，并澄清企业软件需要治理、安全性和长期可维护性。它帮助技术与非技术受众理解资深工程师的持久价值。 Fowler 引用了 FOSE 大会的讨论，团队设计规范、让 AI 智能体通宵工作、次日早晨审查结果，并强调人类在做权衡和判断质量。他指出，生产级软件会带来数据保护、依赖失效、可审计性、可扩展性和监控等问题，而这些在演示中不会出现。

rss · Martin Fowler · 8月19日 18:30

**背景**: 公民开发者是指借助无代码或低代码平台构建应用程序的业务用户，他们不具备传统编程技能。相比之下，企业软件工程涉及治理、安全、可扩展性和长期维护，需要经验丰富的工程师来判断设计质量和风险。这篇文章将这个现象与 AI 智能体的兴起联系起来，智能体可以执行编码任务，而人类则负责设计和治理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.creatio.com/glossary/citizen-developer">Who is a Citizen Developer ? | Creatio</a></li>
<li><a href="https://www.infotech.com/research/ss/governance-and-management-of-enterprise-software-implementation">Governance and Management of Enterprise Software Implementation | Info-Tech Research Group</a></li>
<li><a href="https://www.gartner.com/en/articles/ai-agents-transforming-software-engineering">AI Agents: Transforming Software Engineering for CIOs and Leaders | Gartner</a></li>

</ul>
</details>

**标签**: `#AI`, `#software engineering`, `#enterprise software`, `#citizen development`, `#LLMs`

---

<a id="item-9"></a>
## [Bun 1.4 的 Bun.WebView 实现了 shot-scraper 风格的 JSON API](https://simonwillison.net/2026/Aug/20/bun-webview-json-api/) ⭐️ 8.0/10

Simon Willison 基于 Bun 1.4 新增的 Bun.WebView 功能构建了一个 JSON API 原型，它可以加载网页并在页面内执行 JavaScript。这个 TypeScript 服务器受他的 shot-scraper javascript 命令行工具启发，通过 macOS WebKit 或基于 Chrome DevTools Protocol 的 Chromium 来运行无头浏览器。 Bun.WebView 将无头浏览器自动化直接集成到 Bun 运行时中，有可能减少对外部工具（如 Puppeteer 或 Playwright）的依赖。Simon 的原型表明，一个页面执行 JSON API 仅需 192MB–256MB 内存即可运行，这对 AI 智能体与抓取服务很有吸引力。 该原型的 server.ts 托管在 Simon 的 research 仓库中，内存占用使用 cgroups 对复杂网页进行了实测。Bun 1.4 的发布说明还提到它修复了 2900 多个问题，并新增了 Bun.Image、Bun.markdown、Bun.cron() 等多个 API。

rss · Simon Willison · 8月20日 15:37

**背景**: Bun 是一个以速度和内置工具著称的 JavaScript 运行时与工具包。Bun.WebView 是运行时内置的无头浏览器，开发者无需安装 Puppeteer 或 Playwright 即可加载页面、执行 JavaScript、模拟输入并截图。shot-scraper 是 Simon Willison 开发的命令行工具，用于自动化截图和对网页执行 JavaScript。Bun 1.4 是从 Zig 重写为 Rust 之后的第一个稳定版本，因此备受关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bun.com/docs/runtime/webview">WebView | Bun Docs</a></li>
<li><a href="https://github.com/simonw/shot-scraper">GitHub - simonw/shot-scraper: A CLI utility for taking ...</a></li>

</ul>
</details>

**标签**: `#Bun`, `#WebView`, `#JavaScript`, `#JSON API`, `#Tooling`

---

<a id="item-10"></a>
## [Rider 让 AI 代理使用重构引擎，代码修改更安全](https://blog.jetbrains.com/dotnet/2026/08/19/rider-refactoring-code-skill/) ⭐️ 7.0/10

JetBrains Rider 展示了一种新方法：让 AI 代理调用其重构引擎，而不是使用原始 CLI 命令。在一项涉及 15 个 C# 重构任务的实验中，一个前沿模型共进行了 2,513 次工具调用，但结构性重构操作的次数为零。 这很重要，因为让 AI 代理具备原生的重构能力，可以使 AI 辅助的代码转换更安全、更快、成本更低。它也凸显了当前基于 LLM 的编码工具的一大低效之处：它们往往依赖 sed、git 这类文本操作命令，而不是理解代码结构。 实验中，模型将文本通过管道送入交互式命令 468 次，调用 git 422 次、sed 392 次，运行 dotnet build 163 次。重构引擎可以利用全解决方案的语义信息，包括每个标识符绑定到哪个声明、每个调用解析到哪个重载，以及每个引用在解决方案中的位置。

rss · JetBrains .NET Tools (Rider/ReSharper) · 8月19日 15:37

**背景**: JetBrains Rider 中的重构引擎提供自动化、全解决方案的代码重构功能，例如重命名、移动、安全删除符号，以及引入或内联字段、变量和参数。工具调用是 LLM 的一种能力，它让模型能决定何时使用哪个工具并构造参数，使模型从文本预测器转变为软件的控制器。结构性重构将代码视为带有语义绑定的语法树，而基于文本的编辑则可能破坏代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.jetbrains.com/dotnet/2026/08/19/rider-refactoring-code-skill/">Rider Hands AI Agents The Keys To Its Refactoring Engine For Safer, Faster, And Cheaper Results - The JetBrains Blog</a></li>
<li><a href="https://www.jetbrains.com/help/rider/Refactorings__Index.html">Refactorings | JetBrains Rider Documentation</a></li>
<li><a href="https://towardsdatascience.com/tool-calling-explained-how-ai-agents-decide-what-to-do-next/">Tool Calling, Explained: How AI Agents Decide What to Do Next</a></li>

</ul>
</details>

**标签**: `#AI-assisted development`, `#refactoring`, `#JetBrains Rider`, `#LLM`, `#software engineering tools`

---

<a id="item-11"></a>
## [pg_shmemviz：PostgreSQL 共享内存可视化新工具](https://postgr.es/p/9sP) ⭐️ 7.0/10

Bertrand Drouvot 发布了 pg_shmemviz，这是一款开发与调试工具，可将 PostgreSQL 的主共享内存和动态共享内存段捕获为离线快照，并在本地浏览器中展示。它提供了共享内存地图、分配表、结构检查器和物理字节视图的同步联动。 该工具为 PostgreSQL 开发者和 DBA 提供了前所未有的共享内存布局字节级视图，使调试内存问题、理解指针关系以及检查 C 结构体字段和填充变得更加容易。它通过展示物理位置而非仅逻辑分配摘要，补充了 pg_shmem_allocations 和 pg_buffercache 等现有视图。 结构检查器使用来自确切 postgres 可执行文件的 DWARF 调试信息，显示嵌套的 C 结构体、字段偏移、值、编译器填充和数组步长填充。快照可选用 pg_buffercache 包含缓冲缓存摘要，并提供每个缓冲区的详细信息，如关系、分支、块、脏状态和固定后台进程。

rss · Planet PostgreSQL · 8月20日 01:00

**背景**: PostgreSQL 使用共享内存来存储共享缓冲区、锁和进程间协调等关键内部数据。现有的系统视图如 pg_shmem_allocations 和 pg_shmem_allocations_numa（在 PostgreSQL 18 中新增）展示逻辑分配细节和 NUMA 分布，但不显示分配在段内的物理位置、确切的 C 结构体、填充或原始字节。pg_shmemviz 通过捕获实际内存段并使用 DWARF 数据将内存映射到结构体字段来解决这一问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/view-pg-shmem-allocations.html">PostgreSQL : Documentation: 18: 53.27. pg _ shmem _allocations</a></li>
<li><a href="https://www.postgresql.org/docs/current/view-pg-shmem-allocations-numa.html">PostgreSQL: Documentation: 18: 53.28. pg_shmem_allocations_numa</a></li>
<li><a href="https://www.postgresql.org/docs/current/runtime-config-resource.html">PostgreSQL : Documentation: 18: 19.4. Resource Consumption</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#shared memory`, `#visualization`, `#debugging`, `#tools`

---

<a id="item-12"></a>
## [使用事务发件箱和 QStash 构建可重试安全的 HubSpot 同步](https://postgr.es/p/9sH) ⭐️ 7.0/10

这篇文章详细介绍了一种用于将订阅数据同步到 HubSpot 的生产级模式，结合了 PostgreSQL 事务发件箱、基于 HTTP 的 QStash 队列、幂等 worker 和速率限制。文中给出了具体的 SQL 表结构和应用代码，用于在同一数据库事务中存储订阅请求和发件箱事件。 这很重要，因为许多实际集成会在远程系统（HubSpot）已提交更改但本地 worker 丢失响应时失败，从而使重试变得含糊不清。所描述的模式——事务发件箱、幂等键和至少一次处理——可迁移到任何分布式同步管道。 该管道使用两张表：subscription_requests 存储带有幂等键和请求哈希的期望状态，而 hubspot_outbox_events 记录了用于发布的不可变事件。调度器可能多次发布事件，但 worker 是幂等的，调用级速率控制加 Sentry 可观测性使系统保持收敛并受到监控。

rss · Planet PostgreSQL · 8月19日 22:07

**背景**: 事务发件箱模式通过在同一个数据库事务中写入业务变更和发件箱事件，然后由独立的调度器将事件发布到消息代理，从而解决分布式系统中的双重写入问题。QStash 是 Upstash 推出的基于 HTTP 的消息传递与调度平台，专为无服务器和分布式应用设计。幂等 worker 假定任何事件都可能被多次投递，从而使重试安全并最终收敛状态。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://microservices.io/patterns/data/transactional-outbox.html">Pattern : Transactional outbox</a></li>
<li><a href="https://docs.aws.amazon.com/prescriptive-guidance/latest/cloud-design-patterns/transactional-outbox.html">Transactional outbox pattern - AWS Prescriptive Guidance</a></li>
<li><a href="https://qstash.com/">qstash .com</a></li>

</ul>
</details>

**标签**: `#outbox-pattern`, `#hubspot`, `#qstash`, `#distributed-systems`, `#postgresql`

---

<a id="item-13"></a>
## [join_collapse_limit：PostgreSQL 文档化的连接顺序控制](https://postgr.es/p/9sF) ⭐️ 7.0/10

Christophe Pettus 解释了如何将 join_collapse_limit 设置为 1，从而强制 PostgreSQL 规划器按照查询中编写的顺序连接表。这提供了一种文档化的、非技巧性的查询提示替代方案。 PostgreSQL 故意没有原生查询提示，因此这个参数为开发人员和 DBA 提供了一种受支持的方式来影响连接顺序。由于连接顺序会显著影响查询性能，这可以成为优化复杂 SQL 的关键工具。 join_collapse_limit 是一个 GUC 参数，它限制了多少显式 JOIN 结构可以被扁平化为单个 FROM 项列表；将其设置为 1 会保留编写的顺序。默认值是 8，在一个 Stack Overflow 的例子中，将其从 8 提高到 10 将规划时间从约 30 秒缩短到不到 1 毫秒。

rss · Planet PostgreSQL · 8月19日 01:00

**背景**: PostgreSQL 的规划器会基于表统计信息和成本估算自动选择连接顺序，但有时会做出次优选择。GUC（Grand Unified Configuration，全局统一配置）参数是数据库的系统级设置，join_collapse_limit 控制规划器重新排序显式连接的激进程度。将其设置为 1 后，规划器会把查询中编写的连接顺序视为约束而非建议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/explicit-joins.html">PostgreSQL: Documentation: 18: 14.3. Controlling the Planner ...</a></li>
<li><a href="https://runebook.dev/en/docs/postgresql/runtime-config-query/GUC-JOIN-COLLAPSE-LIMIT">PostgreSQL Performance Tuning: The join_collapse_limit Conundrum</a></li>
<li><a href="https://stackoverflow.com/questions/22339836/postgresql-join-collapse-limit-and-time-for-query-planning">join - Postgresql join_collapse_limit and time for query ...</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#query planning`, `#joins`, `#performance tuning`

---

<a id="item-14"></a>
## [ChatGPT 搜索在 GPT-5.6 后大规模采用 site:操作符](https://simonwillison.net/2026/Aug/20/chatgpt-search-now-uses-the-siteoperator-at-scale/) ⭐️ 7.0/10

Promptwatch 的数据显示，ChatGPT 搜索中包含 site:操作符的查询占比从长期稳定的 0.3%–0.5%在 2026 年 8 月 8 日跃升至 16%–17%，与 GPT-5.6 Sol 的推出同步发生。这标志着 ChatGPT 搜索处理域名限定查询的方式发生了重大转变。 这一变化对 SEO 和生成引擎优化（GEO）具有直接影响，因为它揭示了 AI 搜索引擎正越来越多地使用显式域名过滤来塑造回答。品牌和内容创作者必须调整其可见性策略，以适应 AI 驱动搜索行为的这一变化。 这些数据仅反映 Promptwatch 自动跟踪的提示词，可能不代表全部查询构成。Simon Willison 推测 OpenAI 最新的搜索工具已变为类似 search(query, recency, domains)的形式，而不是直接鼓励使用 site:操作符；后续报告还发现，同一次更新后 ChatGPT 中 Reddit 引用大幅减少。

rss · Simon Willison · 8月20日 23:57

**背景**: 生成引擎优化（GEO）是一种通过结构化内容来提高在 ChatGPT、Claude、Gemini 等 AI 工具生成回答中可见性的实践。site:操作符是传统搜索引擎（如 Google）中用于将搜索结果限制在指定域名的经典搜索指令。Promptwatch 是一家 GEO 平台，追踪 AI 搜索引擎对提示词的反应，并发布汇总数据，从而揭示这些产品中原本不可见的设计变化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Generative_engine_optimization">Generative engine optimization - Wikipedia</a></li>
<li><a href="https://promptwatch.com/">Promptwatch | #1 AI Search Visibility & GEO Platform</a></li>
<li><a href="https://developers.google.com/search/docs/monitor-debug/search-operators/all-search-site">How To Use the Site Search Operator | Google Search Central</a></li>

</ul>
</details>

**标签**: `#ChatGPT`, `#search`, `#site:operator`, `#GEO`, `#SEO`

---