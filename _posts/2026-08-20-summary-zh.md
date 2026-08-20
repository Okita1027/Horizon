---
layout: default
title: "Horizon 日报：2026-08-20 (ZH)"
date: 2026-08-20
lang: zh
---

> 从 49 条内容中筛选出 16 条重要资讯。

---

1. [Stripe 以逾 70 亿美元收购 OpenRouter](#item-1) ⭐️ 9.0/10
2. [Go 1.27 引入泛型方法、标准 UUID 包与抗量子密码](#item-2) ⭐️ 9.0/10
3. [Mojo 编程语言正式开源，采用 Apache 2.0 许可证](#item-3) ⭐️ 9.0/10
4. [谷歌用 Google Drive 请求流程取代 Git 标签发布源代码](#item-4) ⭐️ 8.0/10
5. [玩笑域名收购引发探空数据地缘政治之争](#item-5) ⭐️ 8.0/10
6. [用几何与 CUDA 对随机岛屿进行地理定位](#item-6) ⭐️ 8.0/10
7. [Databricks 收购 Electric：PGlite 将 PostgreSQL 带入 AI 代理](#item-7) ⭐️ 8.0/10
8. [Simon Willison：代码行数可成为衡量 AI 编码代理的有意义指标](#item-8) ⭐️ 8.0/10
9. [JetBrains Rider 向 AI 代理开放重构引擎，实现更安全高效的代码变更](#item-9) ⭐️ 7.0/10
10. [使用事务性发件箱和 QStash 构建可靠的 HubSpot 同步](#item-10) ⭐️ 7.0/10
11. [join_collapse_limit：PostgreSQL 有文档支持的查询提示](#item-11) ⭐️ 7.0/10
12. [Kubernetes 的 container_memory_working_set_bytes 指标会误导 Postgres 的 OOM 风险判断](#item-12) ⭐️ 7.0/10
13. [Postgres 19：关于加载、存储和索引的更新建议](#item-13) ⭐️ 7.0/10
14. [10 分钟在 Kubernetes 上部署高可用 PostgreSQL](#item-14) ⭐️ 7.0/10
15. [公民构建，代理执行，专家治理](#item-15) ⭐️ 7.0/10
16. [探索用 smolvm 作为不可信 Python 与 JavaScript 代码的沙箱](#item-16) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Stripe 以逾 70 亿美元收购 OpenRouter](https://openrouter.ai/blog/announcements/openrouter-is-joining-stripe/) ⭐️ 9.0/10

Stripe 正在收购广受欢迎的 AI 模型路由代理 OpenRouter，据报道交易金额超过 70 亿美元。此次收购证实了此前的传闻，也成为 AI 基础设施中间件领域规模最大的退出交易之一。 这笔交易验证了位于开发者和众多相互竞争的 AI 模型提供商之间的 API 中间件商业模式。它可能通过将 Stripe 的支付和记账能力引入模型使用计量、计费和结算，重塑 AI 基础设施与 API 经济。 OpenRouter 是一个将请求发送给模型提供商的代理，其默认路由会选择最便宜的提供商，同时允许用户设置性能下限。除了模型选择，该平台还提供统一 API、图像 API，以及处理密钥轮换和速率限制的功能。

hackernews · rvz · 8月19日 17:32 · [社区讨论](https://news.ycombinator.com/item?id=49364559)

**背景**: OpenRouter 是一个流行的 AI 模型路由代理：开发者无需分别注册每家模型供应商，只需使用一个 API 密钥即可访问众多模型，路由逻辑可以根据价格、质量或其他标准来选择模型。AI 路由器和网关已逐渐成为中间件层，用以应对日益增多的 LLM 提供商、端点、数据格式和计费模式。以在线支付处理闻名的 Stripe，可能会利用 OpenRouter 为 AI 产品和智能体工作负载构建按量计费能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openrouter.ai/docs/faq">OpenRouter FAQ</a></li>
<li><a href="https://inworld.ai/resources/what-is-an-ai-router">What Is an AI Router? LLM Model Routing Explained (2026)</a></li>
<li><a href="https://evolink.ai/blog/what-is-ai-model-routing-guide-for-developers">What Is AI Model Routing? A Practical Guide for Developers | EvoLink</a></li>

</ul>
</details>

**社区讨论**: 评论者大多对该产品及此次交易持积极态度，指出当代理让提供商在单一 API 背后进行价格和质量竞争时，代理也可能价值数十亿美元。也有人对依赖中间商而非开放协议（如 Open Banking）表示担忧；一位长期用户称赞了 OpenRouter 的路由功能，例如带性能下限的最便宜提供商选择。还有评论认为，Stripe 在记账和计费方面的优势可以帮助 AI 产品计量用量、归因成本并与供应商对账。

**标签**: `#AI`, `#Acquisition`, `#Stripe`, `#OpenRouter`, `#API`

---

<a id="item-2"></a>
## [Go 1.27 引入泛型方法、标准 UUID 包与抗量子密码](https://go.dev/blog/go1.27) ⭐️ 9.0/10

Go 1.27 已正式发布，引入了泛型方法、新的标准库 uuid 包以及抗量子密码支持。该版本还通过 Russ Cox 的 uscale 算法改进了浮点数解析与格式化。 泛型方法消除了 Go 泛型长期存在的限制，使 API 设计更具表现力。标准化的 uuid 包减少了对第三方库的依赖，而抗量子支持则让 Go 为未来的量子威胁做好了准备。 泛型方法允许在方法上使用类型参数，但泛型方法实现接口仍不受支持。新的标准 uuid 包无需第三方依赖即可生成和解析 UUID，crypto/mldsa 包则提供抗量子签名。

hackernews · database64128 · 8月19日 18:33 · [社区讨论](https://news.ycombinator.com/item?id=49365405)

**背景**: Go 1.18 为语言引入了泛型，但当时泛型方法因实现复杂而被明确拒绝。UUID 在分布式系统中被广泛用作唯一标识符，此前需要使用 google/uuid 等第三方库。抗量子密码旨在设计能够抵御未来量子计算机攻击的算法，Go 自 1.23 起逐步加入了相关支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@the_atomic_architect/go-generic-methods-go-1-27-6483d7f85e6a">Go Generic Methods in Go 1.27: Proposal 77273 Explained | Medium</a></li>
<li><a href="https://go-cookbook.com/snippets/strings/uuid-package-go-1-27-rc">Go 1.27 RC Preview: Standard - Library UUIDs - Go ... | Go Cookbook</a></li>
<li><a href="https://en.wikipedia.org/wiki/Post-quantum_cryptography">Post - quantum cryptography - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者整体持正面态度，称赞抗量子密码方面的前瞻性工作以及泛型方法带来的易用性改进。有人提到 uscale 浮点解析优化，预测会出现把 google/uuid 迁移到标准库的 PR 浪潮，还有用户希望 Go 博客添加语法高亮。

**标签**: `#Go`, `#release`, `#generics`, `#cryptography`, `#programming languages`

---

<a id="item-3"></a>
## [Mojo 编程语言正式开源，采用 Apache 2.0 许可证](https://simonwillison.net/2026/Aug/18/mojo-is-now-open-source/) ⭐️ 9.0/10

Modular 已将 Mojo 编程语言的编译器和工具链以 Apache 2.0 许可证开源，此前一周刚发布了 1.0 版本。这兑现了自 2023 年 5 月以来的开源承诺。 Mojo 旨在将类似 Python 的易用性与系统级性能结合起来，尤其面向 GPU 和 AI 工作负载。将工具链开源可能会加速采用和社区贡献，从而可能改变 Python 开发者构建高性能 AI 应用的方式。 该项目最初定位为 Python 超集，但这一计划在 2025 年 8 月左右被调整，Modular 表示 Mojo 可能会也可能不会成为完整的 Python 超集。如今，该语言专注于用类似 Python 的语法让 GPU 编程尽可能无痛，而不保证与现有 Python 代码兼容。

rss · Simon Willison · 8月18日 21:39

**背景**: Mojo 是由 Modular 创建的系统编程语言，具有受 Rust 启发的静态类型和借用检查器，但语法让人联想到 Python。它面向 Linux 和 macOS，旨在为 CPU、GPU 及其他加速器编程。此次开源发布包含编译器和工具链，允许开发者查看、修改并在此基础上构建该语言。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language) - Wikipedia</a></li>
<li><a href="https://www.datacamp.com/tutorial/mojo-language-the-new-programming-language-for-ai">Mojo: A Revolutionary New Programming Language for Building AI Applications | DataCamp</a></li>
<li><a href="https://mojolang.org/">Mojo</a></li>

</ul>
</details>

**标签**: `#mojo`, `#open-source`, `#programming-language`, `#ai`, `#compiler`

---

<a id="item-4"></a>
## [谷歌用 Google Drive 请求流程取代 Git 标签发布源代码](https://grapheneos.social/@GrapheneOS/117057099753905023) ⭐️ 8.0/10

谷歌已停止为某些源代码发布 Git 标签，而是要求开发者通过 Google Forms 提交请求，之后由人工提供 Google Drive 链接。GrapheneOS 指出这一流程非常缓慢，且可能违反 GPLv2。 这很重要，因为 GPLv2 要求接收者能够无过多阻碍地获取对应源代码，而人工审批流程会耽误开发者和安全研究人员。这也反映出谷歌在许可义务之下，让 Android 中“开放”的部分变得更难获取的趋势。 Git 标签是指向特定提交的引用，通常用于标记版本发布；取消它们会让精确检出某个版本变得更困难。所请求的源代码通过 Google Drive 而非标准 Git 远程仓库交付，GrapheneOS 表示谷歌处理这些请求的速度已经变得非常慢。

hackernews · Animux · 8月19日 17:47 · [社区讨论](https://news.ycombinator.com/item?id=49364745)

**背景**: Git 标签是指向 Git 历史中特定提交的引用，通常用于标记版本发布。GNU GPL 是一种 copyleft 许可证，保证用户运行、研究、分享或修改软件的自由，但要求分发修改版本的人以相同许可证向接收者提供源代码。GPLv2 是 Linux 内核及 Android 平台部分代码所使用的许可证，因此谷歌的源代码分发行为需要符合其要求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://git-scm.com/book/en/v2/Git-Basics-Tagging">Git - Tagging</a></li>
<li><a href="https://en.wikipedia.org/wiki/GNU_General_Public_License">GNU General Public License - Wikipedia</a></li>
<li><a href="https://www.atlassian.com/git/tutorials/inspecting-a-repository/git-tag">Git Tagging: From Creation to Checkout | Atlassian Git Tutorial</a></li>

</ul>
</details>

**社区讨论**: 评论者意见不一：有人为谷歌辩护，认为称其违反 GPL 是夸大其词；也有人赞同 GrapheneOS，认为这明显违规。还有人讽刺说谷歌最终会通过邮寄方式提供源代码，并分享了 keepandroidopen.org，表达对 Android 开放性整体的担忧。

**标签**: `#open-source`, `#Google`, `#Android`, `#GPL`, `#software-licensing`

---

<a id="item-5"></a>
## [玩笑域名收购引发探空数据地缘政治之争](https://sprocketfox.io/xssfox/2026/08/19/sondehub-and-war/) ⭐️ 8.0/10

文章讲述了一个与 SondeHub 相关的人士出于玩笑购买域名，却意外卷入围绕探空仪数据收集与分析的地缘政治冲突，并收到瑞士探空仪制造商 Meteolabor 的严肃回应。 这个故事表明，像 SondeHub 这样由爱好者推动的开放项目，可能会与国家安全和军事关切发生交集，使无害的技术爱好变成地缘政治的引爆点。它也突显了开源情报日益重要的地位，以及开放数据共享与国家保密之间的紧张关系。 评论中提到，Meteolabor 在邮件里表示其发射机在一段时间后或电池耗尽时会关闭，'原因包括战略考量等'。文章还提到一桩肇事逃逸事件中作者被人联系，评论区将其与'curl 小哥'遭遇黑客调查的经历相比。

hackernews · kareiva · 8月19日 11:21 · [社区讨论](https://news.ycombinator.com/item?id=49360015)

**背景**: 探空仪是由气象气球携带的小型仪器包，在上升穿越大气层时测量温度、湿度、气压等数据，并将数据传回地面站。SondeHub 是一个由社区驱动的开放数据项目，通常利用业余无线电和 OSINT 技术收集、汇总并可视化探空仪遥测数据。开源情报（OSINT）是指从无线电信号、域名注册等公开来源获取信息，如今它既是爱好者的工具，也成为国家行为体的手段。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.osinttechniques.com/">OSINT Techniques - Home</a></li>
<li><a href="https://geo.libretexts.org/Workbench/DeAnza-MET10L/01:_Surface_and_Upper-Air_Weather/1.05:_Vertical_Atmosphere_data_charts">1.5: Vertical Atmosphere data charts - Geosciences LibreTexts</a></li>
<li><a href="https://www.gfdl.noaa.gov/jrl_research_data-quality/">Data Quality & Intercomparison – Geophysical Fluid Dynamics...</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍赞赏这篇文章，monitron 称赞它是没有'LLM 中介'痕迹、直接来自人类大脑的作品，并庆幸没有出现法律威胁。xur17 愉快地回忆约 10 年前与朋友一起用 GPS 记录器和 APRS 发射机施放气象气球并用 habhub 跟踪的经历；Firefishy 提到 OpenStreetMap 基础设施也常收到来自 .mil、.gov 和 GeoTLD 的怪异请求。还有人觉得 Meteolabor '战略考量'的回应很奇葩，并把作者的经历比作'curl 小哥'被当作黑客调查的遭遇。

**标签**: `#geopolitics`, `#OSINT`, `#radiosonde`, `#open data`, `#amateur radio`

---

<a id="item-6"></a>
## [用几何与 CUDA 对随机岛屿进行地理定位](https://yassa9.github.io/osint/gralhix-004/) ⭐️ 8.0/10

一篇博客文章展示了一种 OSINT 技术：将地形特征的几何分析与 CUDA 加速的并行搜索相结合，对一座随机岛屿进行地理定位，大幅加快匹配速度。 该方案展示了 GPU 编程如何应用于传统上靠目视检查或较慢的 CPU 方法完成的地理定位任务，有望惠及开源情报、搜索救援和行星导航等领域。 该方法可能利用从图像中提取的海岸线或地形几何特征，与全球数据库进行比对，并通过 GPU 上的 CUDA 内核执行暴力比较，以便高效处理巨大的搜索空间。

hackernews · yassa9 · 8月19日 12:19 · [社区讨论](https://news.ycombinator.com/item?id=49360545)

**背景**: 开源情报（OSINT）是指通过收集和分析公开可获取的信息来回答诸如“照片在哪里拍摄”等问题。仅凭地形对照片进行地理定位非常困难，因为地球表面有许多相似形状；对卫星影像进行朴素搜索在计算上不可行。CUDA 是 NVIDIA 的并行计算平台和编程模型，允许开发者将 GPU 用于通用计算，使得图像匹配等大规模数据并行算法能以远超 CPU 的速度运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CUDA">CUDA - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞文章风格，并指出了相关技术：用于无人机和导弹的地形轮廓匹配（TERCOM），以及喷气推进实验室（JPL）利用地形相对导航缩小“火星 2020”着陆椭圆。一位评论者指出，太阳的位置可提供方位线索；另一位评论者则认为，这篇文章恰好出现在一篇关于“避免制造可能被警察国家使用的技术”的文章旁边，颇具讽刺意味。

**标签**: `#geolocation`, `#CUDA`, `#geometry`, `#OSINT`, `#computer vision`

---

<a id="item-7"></a>
## [Databricks 收购 Electric：PGlite 将 PostgreSQL 带入 AI 代理](https://postgr.es/p/9sG) ⭐️ 8.0/10

Databricks 宣布收购 Electric，即 PGlite（PostgreSQL 的 WebAssembly 构建版本）背后的公司。PGlite 在约 12 个月内从每周 100 万次下载增长到每周 1300 万次下载，Electric 还开发了同步技术，用于将分布式的 PGlite 实例与中心化 PostgreSQL 连接起来。 此次收购凸显了 PostgreSQL 的一个全新架构角色：在应用程序或 AI 代理沙盒内部运行，而不仅仅作为远程服务器。它还提出了一个关键问题：当每个代理都拥有自己的本地数据库时，哪个数据库拥有真相？这一挑战将影响 AI 基础设施和数据治理。 PGlite 基于 Neon 联合创始人 Stas Kelvich 的开创性 PostgreSQL 到 WASM 工作，Electric 将其变成了一个可嵌入的数据库。Databricks 将这一组合描述为将 PostgreSQL 从 lakehouse 扩展到边缘，PGlite 在代理沙盒中运行，而中心的 Lakebase PostgreSQL 环境则提供共享状态和控制。

rss · Planet PostgreSQL · 8月19日 05:06

**背景**: PGlite 是将 PostgreSQL 编译为 WebAssembly 的产物，使完整的数据库引擎可以在浏览器、Node.js、无服务器环境或 AI 代理沙盒中运行，而无需传统的数据库服务器。AI 代理在运行时会产生大量中间状态，例如检索文档、生成嵌入、制定计划和调用外部工具，如果将所有操作都发送到远程数据库，则会增加延迟和耦合。PGlite 为代理提供了靠近其执行循环的本地 PostgreSQL，而 Electric 的同步技术旨在将这些本地实例与中央记录系统连接起来。这种模式反映了更广泛的 local-first 软件运动，即数据驻留在边缘并与中央基础设施同步。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@premchandak_11/you-dont-need-a-database-server-use-pglite-postgres-in-wasm-91a1268ff69c">You Don’t Need a Database Server. Use PGlite ( Postgres in... | Medium</a></li>
<li><a href="https://noqta.tn/en/tutorials/pglite-postgres-wasm-browser-local-first-2026">PGlite : Run PostgreSQL in the Browser with WebAssembly</a></li>
<li><a href="https://electric.ax/?ref=labnotes.org">Electric | Agents on sync</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#WebAssembly`, `#AI Agents`, `#Databricks`, `#PGlite`

---

<a id="item-8"></a>
## [Simon Willison：代码行数可成为衡量 AI 编码代理的有意义指标](https://simonwillison.net/2026/Aug/19/conceptual-integrity-and-counting-lines-of-code/) ⭐️ 8.0/10

在 2026 年 8 月 19 日的一篇博客文章中，Simon Willison 基于 Talking Postgres 播客的内容提出，代码行数在结合概念完整性时，可以成为衡量 AI 编码代理生产力的有效指标。他还警告说，代理让软件像“温彻斯特神秘屋”一样随意增生，缺乏连贯设计。 这重新定义了 AI 时代的经典软件工程争论，提供了一种细致入微的观点，可能影响工程团队评估 AI 辅助生产力和团队规模的方式。随着 AI 编码代理成为主流，它挑战了人们通常对代码行数指标的否定，并指出了认知容量等新瓶颈。 Willison 提出了一个硬性限制：在 AI 代理出现之前，工程师每天能产出 50 到 200 行可投入生产的代码，而代理能生成上千行调试完毕的代码。他指出，《人月神话》中的“概念完整性”在代理时代更难实现，过去由缓慢编码速度带来的纪律已消失；他还附注称“温彻斯特神秘屋”的灵媒故事存在争议。

rss · Simon Willison · 8月19日 22:46

**背景**: 代码行数（LOC）一直作为生产力指标受到批评，因为它奖励冗长代码、惩罚重构。《人月神话》中普及的“概念完整性”指的是设计连贯、没有意外的软件。AI 编码代理是能根据自然语言提示生成代码的工具，大幅降低了添加功能的成本，若不加以管理便会导致设计退化。这些背景有助于理解为什么 Willison 的论点既及时又具争议性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/from-local-coding-agents-autonomous-development-platforms-t--ta8hf">From local coding agents to autonomous development platforms...</a></li>
<li><a href="https://medium.com/nerd-for-tech/ensuring-conceptual-integrity-in-software-development-fd0b746f44c0">Ensuring Conceptual Integrity in Software Development | Medium</a></li>
<li><a href="https://www.lossless.group/more-about/conceptual-integrity">Conceptual Integrity | Lossless Group</a></li>

</ul>
</details>

**标签**: `#AI coding`, `#software engineering`, `#productivity`, `#lines of code`, `#conceptual integrity`

---

<a id="item-9"></a>
## [JetBrains Rider 向 AI 代理开放重构引擎，实现更安全高效的代码变更](https://blog.jetbrains.com/dotnet/2026/08/19/rider-refactoring-code-skill/) ⭐️ 7.0/10

JetBrains Rider 现在允许 AI 智能体直接调用其内置重构引擎，而不是依赖 sed、git 和 dotnet build 等命令行工具。公告指出，在一次追踪中，一个前沿模型在 2,513 次工具调用中从未执行过任何结构化重构操作。 这解决了基于 LLM 的编程代理长期存在的痛点：它们常常使用低效的 shell 命令，甚至可能破坏代码。该功能将使 AI 辅助重构更安全、更快速、更廉价，并可能促使其他 IDE 厂商向智能体开放原生重构能力。 追踪数据显示，模型使用了 468 次交互式命令管道、422 次 git 调用、392 次 sed 调用和 163 次 dotnet build。在整个过程中，重构引擎一次也未被调用，这凸显了这一集成所填补的关键缺口。

rss · JetBrains .NET Tools (Rider/ReSharper) · 8月19日 15:37

**背景**: 重构是指在不改变代码行为的前提下调整代码结构，通常借助 IDE 的“重命名”“提取方法”“更改签名”等功能安全地完成。大型语言模型通常只能操作文本和 shell 命令，面对结构性变更时容易出错。JetBrains Rider 是面向 .NET 的集成开发环境，多年提供成熟的重构功能，现在这些功能正被开放给 AI 智能体。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.jetbrains.com/help/rider/Refactorings__Index.html">Refactorings | JetBrains Rider Documentation</a></li>

</ul>
</details>

**标签**: `#AI-assisted development`, `#Refactoring`, `#JetBrains Rider`, `#Software engineering`, `#LLM tools`

---

<a id="item-10"></a>
## [使用事务性发件箱和 QStash 构建可靠的 HubSpot 同步](https://postgr.es/p/9sH) ⭐️ 7.0/10

本文介绍如何使用事务性发件箱模式与 QStash 构建一个可重试安全的 HubSpot 同步管道。它通过在同一个数据库事务中写入订阅变更和不可变事件，再由幂等分发器发布，确保至少一次投递且处理安全。 这套方案解决了数据库与消息队列之间双重写入的一致性问题，这是分布式系统中的常见难题。它展示了一种实用且可扩展的架构，能支持多站点集成（例如 40 站点的场景），也可适配其他外部 API 同步需求。 文章给出了 subscription_requests 和 hubspot_outbox_events 的 SQL 表结构，包含幂等键、请求哈希、发布/处理次数和租约过期时间等字段。此外还涉及调用级速率控制、对账机制以及基于 Sentry 的可观测性，以处理边界情况并确保最终收敛到期望状态。

rss · Planet PostgreSQL · 8月19日 22:07

**背景**: 事务性发件箱模式是一种分布式系统设计模式，用于解决双重写入问题：将业务数据和发件箱事件放在同一个数据库事务中，再由独立的分发器将事件发布到消息代理。QStash 是 Upstash 提供的面向无服务器工作负载的 HTTP 消息队列，支持至少一次投递而无需持久连接。幂等键可以确保因重试或崩溃导致的重复投递不会产生重复副作用，从而使重试安全可行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://microservices.io/patterns/data/transactional-outbox.html">Pattern : Transactional outbox</a></li>
<li><a href="https://upstash.com/blog/qstash-announcement">QStash : Messaging for the Serverless | Upstash Blog</a></li>
<li><a href="https://medium.com/@rosgluk/idempotency-in-distributed-systems-that-actually-works-b9c1e789f755">Idempotency in Distributed Systems That Actually Works | Medium</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#Transactional Outbox`, `#QStash`, `#HubSpot`, `#Distributed Systems`

---

<a id="item-11"></a>
## [join_collapse_limit：PostgreSQL 有文档支持的查询提示](https://postgr.es/p/9sF) ⭐️ 7.0/10

Christophe Pettus 解释了将 join_collapse_limit 设为 1 会让 PostgreSQL 完全按照查询中编写的顺序连接表，从而在不用查询提示的情况下提供一种有文档支持的连接顺序控制方式。 这很重要，因为许多 PostgreSQL 用户认为查询提示是不可能的，而 join_collapse_limit 为性能调优提供了一个实用的变通方案。它为开发者和 DBA 提供了一种合法且受支持的干预计划器的手段。 该功能是有文档支持的，而不是实现上的偶然产物，它实际上覆盖了剩余 5% 中可以通过提示模拟的部分。文章还提到了 Tom Lane，表明这一行为是有意设计并持续维护的。

rss · Planet PostgreSQL · 8月19日 01:00

**背景**: PostgreSQL 的计划器通常会自动优化连接顺序，并且该数据库以不支持其他数据库那样的查询提示而闻名。GUC（Grand Unified Configuration）参数如 join_collapse_limit 允许微调计划器的行为；当设为 1 时，它会禁用计划器超出查询指定范围之外重新排序列的能力。理解这一参数有助于 DBA 和开发者在计划器的默认选择不佳的工作负载中影响执行计划。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.enterprisedb.com/postgres-tutorials/how-tune-postgresql-guc-parameters">How to Tune PostgreSQL GUC Parameters</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#query planning`, `#join_collapse_limit`, `#GUC`, `#performance`

---

<a id="item-12"></a>
## [Kubernetes 的 container_memory_working_set_bytes 指标会误导 Postgres 的 OOM 风险判断](https://postgr.es/p/9sE) ⭐️ 7.0/10

Jeremy Schneider 解释了 Kubernetes 的 container_memory_working_set_bytes 指标源于 cgroups v2 memory.stat 中的 current-inactive_file 值，因此用来衡量 Postgres 内存使用并不准确。他提供了复现脚本，并演示了该指标无法预测 Postgres 容器的 OOM 崩溃。 由于 Kubernetes 在内存压力下使用 container_memory_working_set_bytes 来决定 Pod 驱逐和 OOM 杀死，读数不准确可能导致 PostgreSQL 意外重启或数据丢失。这对所有在 Kubernetes 上运行 Postgres 的人都很重要，尤其是在内存 request 小于 limit 的配置下。 该指标只从页缓存中排除了 active file LRU，而作者提出的替代指标把 active 和 inactive file LRU 都排除，表示“不含页缓存”的内存使用量。文章列出了使用 agnhost stress 镜像的 Node E2E 测试，并提供了用于复现测试和图表的 GitHub 仓库。

rss · Planet PostgreSQL · 8月18日 23:28

**背景**: Kubernetes 通过 cgroups v2 的 memory.stat 计算 container_memory_working_set_bytes，具体使用 current-inactive_file，即从总内存使用中减去部分 Linux 页缓存。该指标旨在体现通用负载下可回收的内存，但 PostgreSQL 高度依赖缓存的 I/O 模式会让这种近似产生误导。文章中的压力容器最终在匿名内存达到 cgroup 上限（即 Pod 内存 limit）时发生 OOM。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.baeldung.com/ops/kubernetes-container-memory-metrics">Kubernetes Container Memory Metrics | Baeldung on Ops</a></li>
<li><a href="https://www.alibabacloud.com/blog/container-memory-observability-exploring-workingset-and-pagecache-monitoring_601456">Container Memory Observability: Exploring... - Alibaba Cloud Community</a></li>

</ul>
</details>

**标签**: `#postgres`, `#kubernetes`, `#memory`, `#cgroups`, `#metrics`

---

<a id="item-13"></a>
## [Postgres 19：关于加载、存储和索引的更新建议](https://postgr.es/p/9sD) ⭐️ 7.0/10

在这篇文章中，Christopher Winslett 回顾了 Crunchy Data 之前关于 PostgreSQL 的建议，并解释了 Postgres 19 带来的变化。新版本增加了可自动扩展的异步 I/O 工作进程、并行 autovacuum 以及默认的 LZ4 压缩，同时默认关闭了 JIT；它还让 COPY 更具弹性，并改进了 BRIN 和 skip scan 的使用。 这之所以重要，是因为它更新了 PostgreSQL 工程师沿用多年的最佳实践，影响到索引、存储和大批量加载的决策。随着异步 I/O 的出现，并行扫描与 BRIN 索引之间的性能特征已经改变，因此 DBA 在升级到 Postgres 18 或 19 后需要重新测试并调整配置。 关键的技术要点包括：Postgres 18 引入了异步 I/O，默认 io_method = worker（Linux 5.1+ 可使用 io_uring），Postgres 19 通过 io_min_workers/io_max_workers 让 I/O 工作进程可自动扩展。19 中新增了并行 autovacuum 工作进程，但默认配置保守；JIT 在 19 中默认关闭。文章还建议使用 EXPLAIN (ANALYZE, BUFFERS, IO) 重新评估 BRIN 与并行扫描计划。

rss · Planet PostgreSQL · 8月18日 19:00

**背景**: BRIN（Block Range Index）是一种轻量级索引，适用于某些列与物理存储位置存在自然相关性的超大表；它按块范围存储摘要，而不是逐行条目。PostgreSQL 18 新增了 skip scan（跳过扫描），即使索引首列的不同值很少，也能使用索引；同时引入了异步 I/O（io_method = worker）来重叠磁盘读取，提高扫描和 vacuum 性能。Postgres 19 通过 I/O 工作进程自动扩展和并行 autovacuum 延续了这些改进，并且默认启用 LZ4 压缩以降低存储占用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/brin.html">PostgreSQL : Documentation: 18: 65.5. BRIN Indexes</a></li>
<li><a href="https://pganalyze.com/blog/postgres-18-async-io">Waiting for Postgres 18: Accelerating Disk Reads with Asynchronous I / O</a></li>
<li><a href="https://betterstack.com/community/guides/databases/skip-scans-postgres/">How to Use Skip Scans in PostgreSQL 18 | Better Stack Community</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database`, `#indexing`, `#storage`, `#performance`

---

<a id="item-14"></a>
## [10 分钟在 Kubernetes 上部署高可用 PostgreSQL](https://postgr.es/p/9sA) ⭐️ 7.0/10

这篇文章演示了如何使用 CYBERTEC PG Operator（CPO）0.9.2 在 minikube（Kubernetes 1.30）上部署一个高可用的 PostgreSQL 18.4 集群，只需一个 14 行的 YAML 清单（设置 numberOfInstances: 2）即可获得一个主节点和一个流复制副本。 这意义重大，因为它通过声明式的 Operator 取代了手动配置主节点选举、副本、故障转移和健康检查的复杂过程，降低了在 Kubernetes 上运行生产级高可用 PostgreSQL 的门槛。DevOps 和数据库工程师可以快速采用经过验证的模式，这在 Kubernetes 成为有状态工作负载标准平台的背景下尤为重要。 该教程使用单节点的 minikube，因此需要通过 enable_pod_antiaffinity=false 禁用 Pod 反亲和；在真正的多节点集群上，应保持默认的反亲和设置，以便副本分散到不同节点。每个 Pod 内运行着 Patroni，可以用 `patronictl list` 检查主节点和副本是否处于零延迟流复制状态，并且主节点上的写入可立即在副本上读取。

rss · Planet PostgreSQL · 8月18日 05:07

**背景**: Kubernetes 的 Operator 模式通过让控制器管理自定义资源来扩展 Kubernetes——这里的自定义资源是一个描述所需数据库集群的 PostgreSQL 资源。高可用 PostgreSQL 通常需要主节点选举、流复制副本、自动故障转移和健康检查，手动配置非常复杂。CYBERTEC PG Operator（CPO）将 Patroni 的这些能力打包并以声明式方式提供，用户只需用 YAML 描述集群，其余由 Operator 处理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://kubernetes.io/docs/concepts/extend-kubernetes/operator/">Operator pattern | Kubernetes</a></li>
<li><a href="https://github.com/cybertec-postgresql/CYBERTEC-pg-operator">GitHub - cybertec -postgresql/ CYBERTEC - pg - operator · GitHub</a></li>
<li><a href="https://www.cybertec-postgresql.com/en/products/cybertec-pg-operator/">CYBERTEC PG Operator : Open-Source PostgreSQL for Kubernetes</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#Kubernetes`, `#High Availability`, `#Operator`, `#Tutorial`

---

<a id="item-15"></a>
## [公民构建，代理执行，专家治理](https://martinfowler.com/rachels-ramblings/citizens-agents-experts.html) ⭐️ 7.0/10

Rachel Laycock 解释了为何 AI 赋能的‘公民构建者’创建周末应用并不能转化为企业工程速度的十倍提升，强调了专家治理和稳健工程实践的必要性。

rss · Martin Fowler · 8月19日 18:30

**标签**: `#AI`, `#Software Engineering`, `#Enterprise Software`, `#Productivity`, `#Governance`

---

<a id="item-16"></a>
## [探索用 smolvm 作为不可信 Python 与 JavaScript 代码的沙箱](https://simonwillison.net/2026/Aug/19/smolmachines-untrusted-sandbox/) ⭐️ 7.0/10

西蒙·威利森使用 Claude Code 评估了 smolmachines/smolvm 作为运行不可信 Python 和 JavaScript 代码的快速安全沙箱。由于 Claude Code 环境缺少嵌套虚拟化支持，测试改在暴露 /dev/kvm 的 GitHub Actions 运行器上进行。 安全地执行不可信的用户代码对于 AI 辅助数据转换和多租户应用越来越重要。此次探索评估了 smolvm 能否提供具备 CPU/内存限制、无网络访问和受控文件系统访问的虚拟机级隔离。 smolvm 为每个工作负载提供独立的虚拟机和客户机内核，从而加强客户机与宿主机之间的边界，但它本身并不是一个加固的多用户控制平面。Claude Code 容器（一个 Firecracker 客户机）缺少 /dev/kvm 以及 vmx/svm CPU 标志，因此实际测试套件在支持 KVM 的 GitHub Actions ubuntu 运行器上运行。

rss · Simon Willison · 8月19日 23:16

**背景**: smolvm 是一个发布在 PyPI 上的便携、轻量、自包含的虚拟机工具，可以用相同的 Python 和 CLI 接口启动 Linux 和 Windows 客户机。它的设计目标是通过将每个工作负载放入独立的虚拟机来实现隔离，这适合用于对不可信代码进行沙箱化，但需要宿主机支持硬件虚拟化（KVM）。更广泛的背景是，安全地运行 AI 生成或用户提供的代码（尤其是数据转换等任务）的需求正在不断增长。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/smol-machines/smolvm">GitHub - smol -machines/ smolvm : Portable, lightweight, self-contained...</a></li>
<li><a href="https://pypi.org/project/smolvm/">smolvm · PyPI</a></li>
<li><a href="https://pypi.org/project/smolmachines/">smolmachines · PyPI</a></li>

</ul>
</details>

**标签**: `#sandboxing`, `#security`, `#untrusted-code`, `#AI-assisted-research`, `#Python`

---