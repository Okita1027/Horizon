---
layout: default
title: "Horizon 日报：2026-08-19 (ZH)"
date: 2026-08-19
lang: zh
---

> 从 38 条内容中筛选出 14 条重要资讯。

---

1. [Mojo 编程语言以 Apache 2 协议开源](#item-1) ⭐️ 9.0/10
2. [Qwen 3.8 27B 智能指数 52 分，追平规模大得多的模型](#item-2) ⭐️ 9.0/10
3. [用铁路网络当作平板扫描仪](#item-3) ⭐️ 8.0/10
4. [Cursor 推出 Origin，面向 AI 时代的 GitHub 替代品](#item-4) ⭐️ 8.0/10
5. [内存价格一年飙涨 500%，引发效率之争](#item-5) ⭐️ 8.0/10
6. [苹果以 5%佣金取代欧盟核心技术费，更新应用政策](#item-6) ⭐️ 8.0/10
7. [Postgres 19：我们写作建议的变化更新](#item-7) ⭐️ 8.0/10
8. [在 Next.js 中利用幂等键防止重复提交表单](#item-8) ⭐️ 8.0/10
9. [AirTag 追踪：一批稀有书籍最终流入亚马逊 AI 训练设施](#item-9) ⭐️ 8.0/10
10. [pgColumnar 1.0-alpha2 发布：支持 Iceberg 与对象存储](#item-10) ⭐️ 8.0/10
11. [Jeremy Schneider：为什么 Postgres 会破坏 Kubernetes 的 container_memory_working_set_bytes 指标](#item-11) ⭐️ 7.0/10
12. [解析 PostgreSQL 17 故障转移槽同步功能](#item-12) ⭐️ 7.0/10
13. [PostgreSQL 会锁定表上的所有索引，包括未使用的索引](#item-13) ⭐️ 7.0/10
14. [在 Kubernetes 上使用 CloudNativePG PostgreSQL 后端运行 OpenBao](#item-14) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Mojo 编程语言以 Apache 2 协议开源](https://simonwillison.net/2026/Aug/18/mojo-is-now-open-source/) ⭐️ 9.0/10

Modular 已将 Mojo 编程语言及其工具链以 Apache 2 许可证开源，紧随上周 Mojo 1.0 的发布。这兑现了该公司自 2023 年 5 月以来的最初承诺。 Mojo 是面向 AI 和异构计算的高性能语言，其编译器开源可能加速 AI/ML 工具链和编译器生态系统的创新。开发者现在可以查看、修改并为该语言的实现做出贡献。 Mojo 构建在 MLIR 编译器框架之上，而非直接依赖 LLVM，因此可以面向 CPU、GPU、TPU 及其他加速器。大约在 2025 年 8 月，原先作为 Python 超集的目标被放弃；Mojo 现在采用受 Python 启发的语法，但它是拥有静态类型和借用检查器（borrow checker）的独立语言。

rss · Simon Willison · 8月18日 21:39

**背景**: Mojo 是 Modular 公司开发的一种系统级编程语言，专为高性能 AI 基础设施而设计。它结合了 Rust 风格的语义（如静态类型和借用检查器）与类似 Python 的语法。由于构建在 MLIR 之上，Mojo 可以更有效地利用 SIMD 等优化，并生成面向多种加速器的代码，因此非常适合 AI 工作负载。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language)</a></li>
<li><a href="https://mojolang.org/">Mojo</a></li>

</ul>
</details>

**标签**: `#mojo`, `#programming-language`, `#open-source`, `#ai`, `#compiler`

---

<a id="item-2"></a>
## [Qwen 3.8 27B 智能指数 52 分，追平规模大得多的模型](https://simonwillison.net/2026/Aug/17/qwen-38-27b-scores-52/) ⭐️ 9.0/10

Qwen 3.8 27B 在 Artificial Analysis Intelligence Index 上获得 52 分，追平 GPT-5.6 Luna (max)，仅比 GLM-5.2 和 DeepSeek V4 Pro 0813 低 1 分。作为一个 270 亿参数的模型，能与拥有数千亿甚至万亿参数的顶级模型比肩，这是效率上的重大里程碑。 这表明模型效率正在大幅提升，小型本地模型也能具备前沿级别的智能。它可能改变部署选择，降低先进 AI 应用的成本和硬件门槛。 Artificial Analysis Intelligence Index 是一个综合基准，涵盖推理、编码、知识、指令跟随、科学推理和多步任务。该模型在评估中生成了 1.6 亿个词元，远高于中位数的 4300 万，这可能影响成本比较。

rss · Simon Willison · 8月17日 23:58

**背景**: Artificial Analysis Intelligence Index 是一个综合得分，衡量语言模型在推理、编码、指令跟随等多个维度的能力。它目前包含九项评估，如 GDPval-AA v2、Terminal-Bench v2.1、SciCode 和 Humanity's Last Exam。该指数常被用来在模型大小、速度和成本背景下比较模型的智能水平。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/evaluations/artificial-analysis-intelligence-index">Artificial Analysis Intelligence Index | Artificial Analysis</a></li>
<li><a href="https://artificialanalysis.ai/models/qwen3-8-27b">Qwen 3 . 8 27 B - Intelligence, Performance & Price Analysis</a></li>

</ul>
</details>

**标签**: `#qwen`, `#llms`, `#ai`, `#model-efficiency`, `#benchmark`

---

<a id="item-3"></a>
## [用铁路网络当作平板扫描仪](https://philo.gay/linecam/) ⭐️ 8.0/10

一个名为 linecam 的实验项目利用列车运动和固定相机，通过狭缝扫描（slit-scan）摄影将铁路走廊变成一台巨大的平板扫描仪。该技术连续捕捉经过的风景条带，生成引人注目且常常出人意料的图像。 这个项目展示了将现有基础设施重新利用为成像设备的创造性做法，为摄影、计算机视觉和创意编程开辟了新的可能性。它也与探索狭缝扫描技术的艺术家和工程师群体产生共鸣，表明简单的想法也能带来新颖的视觉体验。 该项目通过固定相机并利用列车的运动提供扫描动作，每一帧为最终图像贡献一条狭窄的垂直条带。由此产生的“错误”镜头——即运动或时机不完美的部分——往往在主观上比计划好的镜头更有趣，为作品增添了偶然性。

hackernews · otherayden · 8月18日 12:43 · [社区讨论](https://news.ycombinator.com/item?id=49344825)

**背景**: 狭缝扫描摄影是一种在长时间曝光过程中，让一条窄缝在相机和被摄物体之间移动，从而产生随时间拉伸或扭曲图像的技术。它在 20 世纪 60 年代开始广为人知，最著名的应用是斯坦利·库布里克的《2001 太空漫游》中的“星门”段落。在这个项目中，铁轨本身充当了狭缝机构，而列车的运动则提供了扫描动作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Slit-scan_photography">Slit-scan photography - Wikipedia</a></li>
<li><a href="https://www.photodoto.com/slit-scan-photography-how-to/">Slit Scan Photography: How to do it and What can You Achieve</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了先例和相关实验：有人描述 2008 年与 Ward Cunningham 在波特兰铁路旁使用早期 iSight 相机进行类似装置，另有人通过手动拼接帧来制作动画。其他人指出那些非刻意的“错误”画面更有趣，还有用户提供了一个基于浏览器的狭缝扫描工具，并提议用镜子技巧测量列车速度。

**标签**: `#slit-scan`, `#creative-coding`, `#computer-vision`, `#photography`, `#experimental`

---

<a id="item-4"></a>
## [Cursor 推出 Origin，面向 AI 时代的 GitHub 替代品](https://cursor.com/changelog/origin-code-hosting) ⭐️ 8.0/10

Cursor 在 2026 年 6 月 16 日的 Compile 大会上发布了 Origin，这是一个定位为 GitHub 替代品的全新 Git forge 与代码托管平台。该产品由 Graphite 团队打造，目前仅有一个带标语“面向代理时代的 Git forge”的候补名单落地页。 Origin 标志着一家重要的 AI 代码编辑器公司进入开发者日常依赖的基础设施领域，有可能重塑开发者工具链。同时，它也引发了开发者对中心化所有权的担忧，尤其是因为 Cursor 现在归 SpaceX 和 Elon Musk 所有。 产品页面目前未提供任何技术细节，只有候补名单注册和标语“代码的演进速度已经超过了任何现有基础设施的设计能力”。Origin 由 Graphite 团队打造，Graphite 是 Cursor 在 2026 年 SpaceX 以 600 亿美元收购 Cursor 之前收购的堆叠式 diff 代码审查公司。

hackernews · tomasreimers · 8月17日 17:02 · [社区讨论](https://news.ycombinator.com/item?id=49334209)

**背景**: Cursor 是一款 AI 驱动的 IDE，是 Visual Studio Code 的分支，由 Anysphere 开发；Anysphere 在被 SpaceX 于 2026 年年中收购前估值达到 293 亿美元。Origin 是一个“Git forge”，即托管 Git 仓库并协作编写代码的平台，类似于 GitHub、GitLab，或 Radicle、Forgejo 等去中心化替代品。此次发布将 Origin 定位为面向 AI 代理产生的大量代码、而非仅为人类开发者设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.eesel.ai/blog/what-is-cursor-origin">What is Cursor Origin? Cursor's Git forge for the agentic era | eesel AI</a></li>
<li><a href="https://www.learncursor.dev/guides/cursor-origin">Cursor Origin Guide · Learn Cursor</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cursor_(code_editor)">Cursor (code editor)</a></li>

</ul>
</details>

**社区讨论**: 开发者的反应总体持怀疑态度：多名评论者担心中心化所有权以及 Elon Musk 的关联，称其为“供应链风险”，还有人主张采用 Radicle 或 Forgejo 等去中心化替代方案。Origin 团队的开发者 Tomas Reimers 也加入了讨论，表示愿意回答问题，态度开放。

**标签**: `#Cursor`, `#GitHub alternative`, `#code hosting`, `#developer tools`, `#AI`

---

<a id="item-5"></a>
## [内存价格一年飙涨 500%，引发效率之争](https://www.tomshardware.com/pc-components/ram/memory-prices-climb-500-percent-in-12-months-up-to-10x-the-lowest-ever-tracked-prices-128gb-of-ddr5-now-usd3-399) ⭐️ 8.0/10

过去 12 个月内存价格上涨了 500%，128GB DDR5 模组现价高达 3399 美元，是最低记录价格的 10 倍。这一剧烈涨幅引起了硬件买家和软件开发者的广泛关注。 内存价格飙升使升级内存变得更加昂贵，可能迫使消费者更长时间地保留现有硬件，并推动开发者优化内存使用。这或许标志着软件工程重新重视内存效率，此前多年内存占用问题一直被忽视。 此次涨价幅度达到 DDR5 内存历史最低记录价格的 10 倍。社区成员指出，由于更换部件变得难以负担，即便是老旧的设备也可能需要继续使用。

hackernews · haunter · 8月17日 17:52 · [社区讨论](https://news.ycombinator.com/item?id=49334960)

**背景**: 内存价格通常受供需周期影响而波动，但近期的上涨因人工智能需求的增长和生产限制而进一步加剧。DDR5 是现代计算机中使用的最新一代动态随机存取存储器，其价格直接影响新电脑、服务器和笔记本电脑的成本。

**社区讨论**: 评论者对消费者面临的财务负担表示担忧，同时有人希望这一局面能促使开发者重新关注内存使用。有用户认为，随着个人电脑变得越来越昂贵，这可能加速转向终端式计算的趋势。

**标签**: `#memory`, `#hardware`, `#pricing`, `#software-engineering`, `#economics`

---

<a id="item-6"></a>
## [苹果以 5%佣金取代欧盟核心技术费，更新应用政策](https://www.apple.com/newsroom/2026/08/apple-announces-changes-for-apps-in-the-european-union/) ⭐️ 8.0/10

苹果宣布了对欧盟应用政策的调整，将按安装次数收取的核心技术费（Core Technology Fee）改为对 App Store 之外分发应用的数字交易收取 5%佣金。该公告于 2026 年 8 月发布在苹果新闻室，同时取消了初始获取费和商店服务费，并继续要求替代分发的应用通过公证（Notarization）审查。 这是一项影响欧盟开发者的重大政策转变，因为它用与数字交易挂钩的、更简单的收入分成佣金，取代了备受批评的按安装收费模式。这可能会降低安装量大的应用的成本，并减少替代应用市场面临的摩擦，但苹果的公证要求仍然保留。 在旧条款下，核心技术费对年首次安装量超过 100 万次之后的部分，按每次 0.50 欧元收取。新的 5%佣金适用于在 App Store 之外分发的应用中的数字交易，苹果仍要求将这些应用交由公证进行基线审查。此外，从 2026 年 10 月 1 日起，欧盟的阅读器应用（reader apps）可以在不提供可操作链接的情况下推广应用外优惠。

hackernews · newusertoday · 8月18日 16:21 · [社区讨论](https://news.ycombinator.com/item?id=49348055)

**背景**: 欧盟的《数字市场法》（DMA）要求苹果在欧盟允许替代应用市场和替代支付方式。2024 年，苹果为符合 DMA 的应用推出了替代商业条款，其中包括核心技术费：年首次安装量超过 100 万次后，每次安装收取 0.50 欧元。公证（Notarization）是苹果在应用分发前进行的自动化安全审查，用于检查恶意或有问题行为。这项新公告解决了苹果与欧盟委员会在商业条款和替代分发方面的一些分歧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.apple.com/support/core-technology-fee/">Core Technology Fee - Support - Apple Developer</a></li>
<li><a href="https://www.ithinkdiff.com/apple-eu-app-store-fee-structure-october-2026/">Apple Replaces €0.50 Core Technology Fee with 5% Commission</a></li>
<li><a href="https://developer.apple.com/support/dma-and-apps-in-the-eu/">Changes for apps in the European Union - Support - Apple Developer</a></li>

</ul>
</details>

**社区讨论**: 评论者总体上欢迎苹果改用更简单的 5%佣金以及阅读器应用规则的改进，但也有人质疑：既然苹果已经收取年度开发者计划费用，是否还需要再收佣金。还有人指出公证仍然是强制要求，并提到开发者门户网站上有关于新条款的详细说明。

**标签**: `#Apple`, `#EU regulation`, `#App Store`, `#developer fees`, `#policy`

---

<a id="item-7"></a>
## [Postgres 19：我们写作建议的变化更新](https://postgr.es/p/9sD) ⭐️ 8.0/10

Christopher Winslett 的文章重新审视了 Crunchy Data 针对 PostgreSQL 19（当前处于测试阶段）的加载、存储、索引和分区建议。文章涵盖异步 I/O 改进、默认 LZ4 压缩、新的 BRIN 索引能力、skip scan 以及更平滑的分区操作。 这一点很重要，因为 PostgreSQL 19 改变了多个长期存在的默认值和性能特征，因此针对 Postgres 10/11 编写的建议已不完全准确。数据库工程师需要更新后的、针对具体版本的建议，以免白白损失性能。 Postgres 19 在 Postgres 18 的异步 I/O 基础上增加了自动调节的 I/O worker（io_min_workers/io_max_workers）、改进的预读以及用于可观测性的 EXPLAIN (ANALYZE, IO)。它还新增了并行 autovacuum（autovacuum_max_parallel_workers），并默认关闭 JIT，因此依赖运行时编译的分析型负载需要显式重新开启。

rss · Planet PostgreSQL · 8月18日 19:00

**背景**: PostgreSQL 是一个开源关系型数据库，具有多种索引类型；BRIN（Block Range Index）是一种面向超大型表的空间高效索引，通过按块范围存储摘要信息来工作。PostgreSQL 18 中的异步 I/O 让后端可以并发发出多个磁盘读取，而不必逐个等待，从而加速顺序扫描、位图堆扫描和 vacuum。JIT（即时编译）用于在运行时编译查询表达式，Postgres 19 因其成本模型不可靠而默认将其关闭。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Block_Range_Index">Block Range Index - Wikipedia</a></li>
<li><a href="https://www.postgresql.org/docs/current/brin.html">PostgreSQL: Documentation: 18: 65.5. BRIN Indexes</a></li>
<li><a href="https://betterstack.com/community/guides/databases/postgresql-asynchronous-io/">PostgreSQL 18 Asynchronous I/O: A Complete Guide</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database internals`, `#performance`, `#indexing`, `#partitioning`

---

<a id="item-8"></a>
## [在 Next.js 中利用幂等键防止重复提交表单](https://postgr.es/p/9sz) ⭐️ 8.0/10

本文提供了一份生产级指南，介绍如何在 Next.js 中利用幂等键、PostgreSQL 唯一约束、事务性发件箱事件和请求指纹来防止重复提交表单。文章演示了完整的幂等契约，包括使用 crypto.randomUUID() 在客户端生成密钥，以及在服务端进行冲突检测。 重复提交表单是常见的分布式系统问题，可能导致重复线索、重复邮件和不一致的 CRM 数据。这种方法超越了前端禁用按钮的做法，提供了服务端保证，使 Web 应用更加可靠和生产就绪。 幂等契约要求客户端为每个逻辑提交生成一个新密钥，并在重试时复用该密钥，而服务端将该密钥与规范化请求的指纹一起存储，并施加唯一约束。如果相同密钥携带不同数据到达，服务端会返回 409 Idempotency Conflict；事务性发件箱可确保下游副作用只执行一次。

rss · Planet PostgreSQL · 8月17日 20:00

**背景**: 幂等性是指重复的相同请求与单个请求具有相同效果的特性，这对于客户端在超时后可能重试请求的分布式系统至关重要。事务性发件箱模式在更新业务实体的同一数据库事务中将消息存储在表中，然后由独立进程可靠地将消息发送到消息代理。这些模式广泛应用于 Stripe 等 API 中，Stripe 支持幂等键以安全地重试请求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.stripe.com/api/idempotent_requests">Idempotent requests | Stripe API Reference</a></li>
<li><a href="https://microservices.io/patterns/data/transactional-outbox.html">Microservices Pattern: Pattern: Transactional outbox</a></li>

</ul>
</details>

**标签**: `#idempotency`, `#PostgreSQL`, `#Next.js`, `#web development`, `#distributed systems`

---

<a id="item-9"></a>
## [AirTag 追踪：一批稀有书籍最终流入亚马逊 AI 训练设施](https://simonwillison.net/2026/Aug/17/we-tracked-a-shipment-of-rare-books-it-ended-at-an-amazon-ai-tra/) ⭐️ 8.0/10

404 Media 将一枚 Apple AirTag 藏在一本稀有书籍中，并通过 Biblio 平台上的一笔约 1,000 本书的大宗订单进行追踪，最终发现该包裹被送至拉斯维加斯亚马逊 LAS8 设施的 VGT3 区域。亚马逊员工的论坛讨论证实，该站点会破坏性地扫描大量书籍用于 AI 训练。 这项调查提供了确凿的实物证据，表明 AI 公司正在批量购买书籍用于训练数据，证实了此前仅停留在传闻层面的怀疑。它还将亚马逊直接卷入大规模破坏性扫描，加剧了未经许可使用书籍所引发的版权与伦理担忧。 书商于 7 月在二手与稀有书交易平台 Biblio 上接到这笔订单，并同意将 404 Media 提供的 AirTag 藏入其中一本书中。照片显示，LAS8 设施 VGT3 入口处有一个恐龙与书的标识，员工讨论也称该流程属于破坏性扫描。

rss · Simon Willison · 8月17日 15:21

**背景**: AI 公司需要海量文本语料来训练大语言模型，而书籍因长篇、高质量的内容而受到重视。自 2025 年前后起，书商们不断报告有匿名、对价格不敏感的买家大量购书，普遍认为这些书籍被用于 AI 训练。Biblio 成立于 2003 年，是一个连接读者与专业古旧书商的在线市场。这篇报道的特别之处在于，它利用实体追踪设备端到端地追踪了一本书的物流全程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Biblio.com">Biblio.com - Wikipedia</a></li>
<li><a href="https://www.biblio.com/">Used Books and Rare Books from Antiquarian Booksellers - Biblio</a></li>

</ul>
</details>

**标签**: `#AI training`, `#Amazon`, `#investigative journalism`, `#copyright`, `#books`

---

<a id="item-10"></a>
## [pgColumnar 1.0-alpha2 发布：支持 Iceberg 与对象存储](https://www.reddit.com/r/PostgreSQL/comments/1vrsok0/pgcolumnar_10alpha2_released_iceberg_support/) ⭐️ 8.0/10

pgColumnar 1.0-alpha2 于 2026-08-18 发布，新增了对 Apache Iceberg 的只读支持、对 S3 兼容对象存储的读写访问，以及一个新的维护守护进程。本次发布还包含大量优化器、统计信息、性能和安全性方面的改进。 该版本让 PostgreSQL 可以直接查询 Apache Iceberg 表——一种在数据湖中广泛使用的开放表格式——无需复制数据，从而将 PostgreSQL 与现代化大数据生态连接起来。同时，它使 S3 兼容对象存储成为分析型工作负载的一等公民，拓宽了 Postgres 用户的部署选择。 Iceberg 支持为只读，可通过元数据路径、REST catalog 或外部表使用；支持位置删除、等值删除和格式版本 3 的删除向量。对象存储访问支持 s3://、http:// 和 https:// URL，并使用 AWS SigV4 签名；原生 PGCN v1 磁盘格式保持不变，只需一条升级命令。

reddit · r/PostgreSQL · /u/linuxhiker · 8月18日 15:39

**背景**: pgColumnar 是一个用于 PostgreSQL 的列式表访问方法扩展，支持列式存储和分析。Apache Iceberg 是一种面向大型分析数据集的高性能开源表格式，最初由 Netflix 于 2017 年开发，现已被众多引擎和厂商支持。PostgreSQL 12 引入的表访问方法接口使得 pgColumnar 等扩展能够以自定义方式存储和读取表数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apache_Iceberg">Apache Iceberg</a></li>
<li><a href="https://iceberg.apache.org/">Apache Iceberg - Apache Iceberg™</a></li>
<li><a href="https://www.postgresql.fastware.com/blog/postgresql-table-access-methods">What are table access methods, and what is their importance to PostgreSQL?</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#columnar storage`, `#Apache Iceberg`, `#object storage`, `#pgColumnar`

---

<a id="item-11"></a>
## [Jeremy Schneider：为什么 Postgres 会破坏 Kubernetes 的 container_memory_working_set_bytes 指标](https://postgr.es/p/9sE) ⭐️ 7.0/10

本文解释了为什么 Postgres 会导致 Kubernetes 的 container_memory_working_set_bytes 指标不准确。这可能导致内存使用误判和 OOM 崩溃。

rss · Planet PostgreSQL · 8月18日 23:28

**标签**: `#Postgres`, `#Kubernetes`, `#memory metrics`, `#cgroups`, `#DevOps`

---

<a id="item-12"></a>
## [解析 PostgreSQL 17 故障转移槽同步功能](https://postgr.es/p/9sx) ⭐️ 7.0/10

文章介绍了 PostgreSQL 17 新增的故障转移槽同步特性，该特性使备用服务器上的逻辑复制槽保持同步，从而减少提升后订阅者需要进行的全量重新同步。 该特性显著改善了逻辑复制的高可用性，使故障转移更快、对订阅者的干扰更小。依赖逻辑复制在 HA 环境中进行部分数据复制的 PostgreSQL 用户将直接受益。 该特性依赖一个槽同步工作进程，即使主节点仍在运行，也会持续同步启用了故障转移的槽（failover = true）。在主备切换后，备用节点可以接管为新主节点，而不会丢失逻辑复制槽。

rss · Planet PostgreSQL · 8月18日 00:43

**背景**: 逻辑复制是一种基于复制标识（通常是主键）来复制数据对象及其变更的方法，它依靠主节点上的复制槽来跟踪订阅者的位置。在带有备用节点的高可用架构中，如果主节点发生故障并且备用节点被提升，旧主节点上的逻辑复制槽将会丢失，迫使订阅者从头开始重新同步。PostgreSQL 17 通过持续将槽状态同步到备用节点来解决此问题，使故障转移变得无缝。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.pgedge.com/blog/setting-up-failover-slots-in-postgresql-17">Setting Up Failover Slots in PostgreSQL-17</a></li>
<li><a href="https://www.decodable.co/blog/failover-replication-slots-with-postgres-17">Failover Replication Slots with Postgres 17</a></li>
<li><a href="https://www.postgresql.org/docs/current/logical-replication.html">PostgreSQL: Documentation: 18: Chapter 29. Logical Replication</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#logical replication`, `#high availability`, `#failover`, `#replication slots`

---

<a id="item-13"></a>
## [PostgreSQL 会锁定表上的所有索引，包括未使用的索引](https://postgr.es/p/9ss) ⭐️ 7.0/10

PostgreSQL 在执行查询时会锁定表上的所有索引，即使查询根本不使用这些索引。这一由 Christophe Pettus 指出的反直觉行为经常让开发者和数据库管理员感到意外。 理解这一锁定行为对于诊断 PostgreSQL 中的并发问题、锁竞争和性能瓶颈至关重要。它还会影响 schema 设计决策，例如创建多少个索引，因为每个索引都会给表上的每次查询增加额外的锁开销。 根据 PostgreSQL 文档，核心系统在索引扫描期间会获取索引上的 AccessShareLock，在更新索引时获取 RowExclusiveLock。但这里描述的行为意味着，对表的每次查询都会锁定所有索引，无论是否使用，这与 PostgreSQL 为保证一致性而管理索引锁定的方式有关。

rss · Planet PostgreSQL · 8月17日 16:00

**背景**: 在 PostgreSQL 中，锁对于确保并发读写期间的数据一致性至关重要。虽然表数据本身支持无阻塞读写访问，但索引锁用于保护索引结构免受并发修改。标题 'Sixteen Locks' 模仿了 '640K 对任何人都应该足够了' 的说法，强调即使是数量不多的索引，每次查询也会锁定每一个索引。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/index-locking.html">PostgreSQL: Documentation: 18: 63.4. Index Locking Considerations</a></li>
<li><a href="https://www.postgresql.org/docs/current/locking-indexes.html">PostgreSQL: Documentation: 18: 13.7. Locking and Indexes</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database locking`, `#indexes`, `#database internals`

---

<a id="item-14"></a>
## [在 Kubernetes 上使用 CloudNativePG PostgreSQL 后端运行 OpenBao](https://postgr.es/p/9sq) ⭐️ 7.0/10

这篇 CNPG Recipe 介绍了如何在 Kubernetes 上部署 OpenBao，并使用 CloudNativePG 作为其 PostgreSQL 存储后端。它通过 CloudNativePG 1.30 引入的 DatabaseRole CRD 签发 TLS 客户端证书，从而构建一个无密码且完全开源的栈。 这很重要，因为它展示了一套完全开源、无供应商锁定的 Kubernetes 机密管理方案，直接回应了锁定风险和密码泛滥的问题。DevOps 和平台工程师可从中获得一份实用蓝图，通过 TLS 客户端证书在 OpenBao 与 PostgreSQL 之间实现免密码认证。 该栈的每一层都是开源的：Kubernetes、CloudNativePG 和 OpenBao，并且任何地方都不存储密码。本 recipe 由 ControlPlane 的 Rob Kenefeck 共同撰写。

rss · Planet PostgreSQL · 8月17日 08:48

**背景**: OpenBao 是一种开源软件解决方案，用于管理、存储和分发敏感数据，例如机密、证书和密钥。CloudNativePG 是一个 Kubernetes Operator，负责管理高可用 PostgreSQL 集群的完整生命周期，并于 2025 年 1 月作为 Sandbox 项目被 CNCF 接受。TLS 客户端证书认证使 PostgreSQL 能够通过受信任 CA 签发的证书来验证客户端身份，从而无需共享密码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openbao.org/">OpenBao</a></li>
<li><a href="https://cloudnative-pg.io/">CloudNativePG - PostgreSQL Operator for Kubernetes</a></li>

</ul>
</details>

**标签**: `#Kubernetes`, `#PostgreSQL`, `#OpenBao`, `#CloudNativePG`, `#TLS`

---