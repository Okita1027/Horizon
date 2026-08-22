---
layout: default
title: "Horizon 日报：2026-08-22 (ZH)"
date: 2026-08-22
lang: zh
---

> 从 37 条内容中筛选出 12 条重要资讯。

---

1. [.NET MAUI 10.0.100 发布：含 209 项修复与改进](#item-1) ⭐️ 8.0/10
2. [美国公民因在边境删除手机数据面临重罪指控](#item-2) ⭐️ 8.0/10
3. [科学家发布迄今最大宇宙二维地图](#item-3) ⭐️ 8.0/10
4. [意外发现：废弃 ENUM 基础设施泄露大量军事基地电话路由查询](#item-4) ⭐️ 8.0/10
5. [DeepSeek-v4-flash-vision-exp](#item-5) ⭐️ 8.0/10
6. [全局哈希表在 PostgreSQL 中能否卷土重来？](#item-6) ⭐️ 8.0/10
7. [UUID v7 修复 PostgreSQL 随机主键索引问题](#item-7) ⭐️ 7.0/10
8. [拆分事务型 API：网络边缘与 PostgreSQL 事务权威](#item-8) ⭐️ 7.0/10
9. [显式插入 ID 为何让 PostgreSQL 序列失步](#item-9) ⭐️ 7.0/10
10. [pg_shmemviz：在浏览器中可视化 PostgreSQL 共享内存的新工具](#item-10) ⭐️ 7.0/10
11. [编码代理让原生界面变便宜：别再写 TUI 了](#item-11) ⭐️ 7.0/10
12. [ChatGPT 搜索现大规模使用 site: 运算符](#item-12) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [.NET MAUI 10.0.100 发布：含 209 项修复与改进](https://github.com/dotnet/maui/releases/tag/10.0.100) ⭐️ 8.0/10

.NET MAUI 团队发布了 10.0.100 版本，这是一个包含 209 个提交的稳定性版本，修复了多个 bug 并提升了 Android、iOS、Mac Catalyst 和 Windows 平台上的性能。主要修复包括 ActivityIndicator 卡住不动、动画线程安全问题以及阴影变换相关问题。 此版本提升了 .NET MAUI（一个被广泛使用的跨平台 UI 框架）的可靠性，帮助开发者通过单一的 C# 代码库交付更稳定的移动和桌面应用。这也体现了微软在 .NET 10 生态系统中对质量和性能的持续投入。 值得注意的修复包括：iOS/Mac Catalyst 上 ActivityIndicator 在 IsRunning 设为 false 后仍然可见的问题；Windows 上 PlatformTicker 的 IsRunning 始终返回 false 的问题；以及 AnimationExtensions 中可能导致动画 ID 重复的线程安全问题。此外，该版本还包含内部 CI 和 AI 代理工作流的改进，例如 Trim/NativeAOT 安全规则和自动化视觉回归对比。

github · kubaflo · 8月20日 16:50

**背景**: .NET MAUI（多平台应用 UI）是微软的开源框架，允许开发者通过单一的 C# 和 XAML 代码库构建原生 Android、iOS、macOS 和 Windows 应用。它是 Xamarin.Forms 的下一代产品，属于 .NET 10 发布浪潮的一部分。本次 10.0.100 更新看起来是一个补丁级的稳定性版本，重点在于修复 bug 和改善开发者工作流，而非引入新功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/dotnet/maui/what-is-maui?view=net-maui-10.0">What is .NET MAUI? - .NET MAUI | Microsoft Learn</a></li>
<li><a href="https://github.com/dotnet/maui">GitHub - dotnet/maui: .NET MAUI is the .NET Multi-platform App UI, a framework for building native device applications spanning mobile, tablet, and desktop. · GitHub</a></li>

</ul>
</details>

**标签**: `#.NET MAUI`, `#release`, `#mobile development`, `#cross-platform`, `#framework`

---

<a id="item-2"></a>
## [美国公民因在边境删除手机数据面临重罪指控](https://www.nytimes.com/2026/08/21/us/politics/samuel-tunick-deleted-phone-felony.html) ⭐️ 8.0/10

据《纽约时报》2026 年 8 月 21 日报道，美国公民塞缪尔·图尼克（Samuel Tunick）因在边境检查期间删除手机数据而面临重罪指控。此案正在引发关于美国边境数字隐私与法律权利的公众辩论。 此案考验旅客在穿越边境时是否能够合法保护敏感数字数据，而边境无证搜查设备很常见。判决结果可能影响法院如何在国家安全关切与个人隐私权之间取得平衡，并波及经常旅行者、记者和商务人士。 具体重罪指控源于在边境检查期间删除数据，但摘要中并未说明完整法律细节。评论者提到了一些技术对策，例如诱饵启动分区、过境前进行设备镜像，以及使用功能极简的“一次性手机”来避免暴露敏感数据。

hackernews · floathub · 8月21日 12:10 · [社区讨论](https://news.ycombinator.com/item?id=49386895)

**背景**: 根据美国长期以来的边境搜查原则，海关与边境保护人员可以在没有搜查令的情况下检查电子设备，将其视为行李或其他随身物品。然而，法院对这项权力的边界意见不一，尤其是在设备加密或在搜查过程中删除数据的情况下。即使设备所有者认为数据是私密的，删除证据仍可能被以妨碍司法等罪名起诉。

**社区讨论**: 评论者提出了一系列技术对策，例如使用诱饵密码启动到一个独立分区并悄悄清除真实数据，以及在过境前创建手机的加密镜像。还有人指出，档案页面现在被意大利政府的审查系统屏蔽，另有人建议出行时只携带仅有登机牌和娱乐内容的功能极简“一次性手机”。

**标签**: `#privacy`, `#border search`, `#civil liberties`, `#legal`, `#digital security`

---

<a id="item-3"></a>
## [科学家发布迄今最大宇宙二维地图](https://newscenter.lbl.gov/2026/08/10/scientists-release-biggest-2d-map-of-the-universe/) ⭐️ 8.0/10

研究人员发布了迄今最全面的宇宙二维地图，该地图基于 Legacy Survey 项目制作，并附带一个免费公开的天空浏览器。这一交互式工具让任何人都能探索覆盖大半天区的数十亿个天体。 这次发布为天文学家和公众提供了前所未有的宇宙视角，有助于未来的研究、教育和科普推广。预计该地图在未来数年内仍将是最全面的二维宇宙地图。 该项目提供了海量的天空图像数据集，可通过 viewer.legacysurvey.org 上的 Legacy Survey Sky Viewer 访问。虽然这张地图以二维形式记录星系及其他天体的角位置，但要将其转化为三维地图还需要加上距离测量。

hackernews · NKosmatos · 8月21日 18:36 · [社区讨论](https://news.ycombinator.com/item?id=49392200)

**背景**: 天文巡天通过多波段的天空成像来编目星系、恒星和其他天体。Legacy Survey 是一项地基成像项目，覆盖了大部分天区；与此同时，Vera C. Rubin 天文台的时空遗产巡天（Legacy Survey of Space and Time）等互补项目也正在进行中。二维地图展示的是天体在天球上的出现位置，而要计算它们的距离则需要红移等额外测量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://phys.org/news/2026-03-world-biggest-astronomy-camera-universe.html">World's biggest astronomy camera seeks to answer pressing...</a></li>

</ul>
</details>

**社区讨论**: 用户的评论总体非常热情，大家都在浏览查看器并就宇宙尺度的发现开玩笑。一位评论者担心经济逆风会减少未来对天文学的投资，另一位则询问如何将这幅地图扩展到三维，指出距离测量是缺失的关键环节。

**标签**: `#astronomy`, `#data release`, `#universe map`, `#science`, `#survey`

---

<a id="item-4"></a>
## [意外发现：废弃 ENUM 基础设施泄露大量军事基地电话路由查询](https://lina.sh/blog/hijacking-e164-arpa) ⭐️ 8.0/10

一名安全研究人员意外发现，e164.arpa 下废弃的 ENUM 基础设施仍在响应电话号码映射查询，使其记录到数十万条通话路由查询。被捕获的查询中包含发往军事基地的流量，暴露出一个现实存在的隐私与安全漏洞。 这一发现之所以重要，是因为电话号码路由数据可能揭示通话关系，而涉及军事基地的查询更引发国家安全担忧。它表明，被废弃或未完全部署的电信基础设施可能多年保持可达并泄露敏感数据，影响运营商、企业和政府机构。 ENUM 是 IETF 定义的协议，通过 e164.arpa 域中类似 DNS 的查找，将 E.164 电话号码映射为 URI。虽然面向公众的 User ENUM 并未普及，但面向运营商的基础设施/运营商 ENUM 仍以私有形式存在，而被废弃的节点可在未经授权的情况下响应查询。

hackernews · gavide · 8月21日 13:11 · [社区讨论](https://news.ycombinator.com/item?id=49387570)

**背景**: ENUM（电话号码映射）旨在利用现有 E.164 号码和 DNS 基础设施，将 IP 世界与传统电话系统连接起来。基础设施 ENUM（有时称为运营商 ENUM）用于服务提供商之间的路由和互联，而公共 User ENUM 原本面向终端用户服务。随着时间推移，许多公共 ENUM 部署被废弃，但相关域名服务器和区域并未全部注销，从而可能被意外或恶意利用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Telephone_number_mapping">Telephone number mapping - Wikipedia</a></li>
<li><a href="https://www.rfc-editor.org/rfc/rfc5067">RFC 5067: Infrastructure ENUM Requirements</a></li>
<li><a href="https://one.oecd.org/document/DSTI/ICCP/CISP(2007)14/REV2/en/pdf">Microsoft Word - ENUM DSTI-ICCP-CISP_2007_14-_REV1.doc</a></li>

</ul>
</details>

**社区讨论**: 评论者惊讶于作者没有被起诉，并指出向当局报告这类发现通常会带来麻烦。有人指出 ENUM 并未完全消亡，它以付费的私有号码携带查询服务等形态存续；还有人希望作者进一步测试这些查询是否会导致真正的 SIP 呼叫接通。总体氛围是对揭露这一被遗忘的基础设施漏洞表示赞赏，也有评论批评相关机构直到涉及军方号码后才采取行动。

**标签**: `#security`, `#privacy`, `#telephony`, `#ENUM`, `#infrastructure`

---

<a id="item-5"></a>
## [DeepSeek-v4-flash-vision-exp](https://api-docs.deepseek.com/guides/vision/) ⭐️ 8.0/10

DeepSeek 发布了其 v4-flash 模型的实验性视觉版本，引发了社区对其能力和局限性的广泛讨论。

hackernews · dares2573 · 8月21日 10:33 · [社区讨论](https://news.ycombinator.com/item?id=49386163)

**标签**: `#deepseek`, `#vision-model`, `#ai`, `#machine-learning`, `#llm`

---

<a id="item-6"></a>
## [全局哈希表在 PostgreSQL 中能否卷土重来？](https://postgr.es/p/9sR) ⭐️ 8.0/10

Andrei Lepikhov 测试了最近论文《Global Hash Tables Strike Back!》中提出的假设：共享哈希表能否在 PostgreSQL 中加速并行聚合。他实现了一个可用的补丁集，在 Google Cloud 的多核实例上进行了测量，发现虽然锁下查找是最大的问题，但至少还有另外三个因素限制性能。 这项实证研究通过真实测量和一个可用的补丁对研究假设提出了质疑，为 PostgreSQL 开发者提供了细致的见解。它表明 LWLock 上的竞争并不是共享内存聚合中唯一的瓶颈，这可能会影响未来的并行查询优化。 文章分析了一个在十三个可变长度字段上进行分组的查询：输入 300 万行、输出近 60 万个分组，并行计划耗时约 25 秒，而串行计划约 12 秒。Gather 节点会重新对所有键进行哈希和比较，而该补丁揭示了除锁查找之外的至少三个隐藏成本因素，其中两个源于 PostgreSQL 基于进程而非线程的模型。

rss · Planet PostgreSQL · 8月20日 17:50

**背景**: PostgreSQL 目前通过两个阶段实现并行聚合：每个 worker 计算部分聚合结果，然后 Gather 节点在 Finalize Aggregate 步骤中合并这些部分状态。理论上，共享哈希表可以让所有 worker 写入同一个公共聚合结构，但这需要使用轻量级锁（LWLock）来保护该表，这可能会成为瓶颈。研究论文《Global Hash Tables Strike Back!》认为，将分组查找从锁下移出可以使共享哈希表变得可行，而文章直接在 PostgreSQL 中检验了这一主张。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.pgedge.com/blog/do-global-hash-tables-strike-back-in-postgresql">Do Global Hash Tables Strike Back in PostgreSQL?</a></li>
<li><a href="https://arxiv.org/pdf/2505.04153">Global Hash Tables Strike Back! An Analysis of Parallel GROUP BY...</a></li>
<li><a href="https://www.postgresql.org/docs/current/parallel-plans.html">PostgreSQL : Documentation: 18: 15.3. Parallel Plans</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database internals`, `#parallel aggregation`, `#hash tables`, `#performance`

---

<a id="item-7"></a>
## [UUID v7 修复 PostgreSQL 随机主键索引问题](https://postgr.es/p/9sX) ⭐️ 7.0/10

本文解释了随机 UUID v4 主键如何降低 PostgreSQL 中 B-tree 索引的性能，并介绍了作为时间有序替代方案的 UUID v7（RFC 9562）。UUID v7 在高位嵌入毫秒时间戳，使插入操作主要追加到索引最右侧页面。 这很重要，因为主键的选择直接影响数据库的插入吞吐量、索引膨胀和内存效率，尤其在规模化场景下。设计分布式或高写入系统的数据库从业者需要理解随机 UUID 与时间有序 UUID 之间的权衡，以避免隐藏的性能退化。 UUID v4 值是随机分布的，每次插入都会命中不可预测的叶子页面，导致频繁的页面分裂和索引碎片化。UUID v7（RFC 9562）使用 48 位存储毫秒级 Unix 时间戳，包含版本/变体字段、12 位亚毫秒单调性信息，以及用于唯一性的随机位。

rss · Planet PostgreSQL · 8月21日 19:03

**背景**: 自增整数等代理键简单快速，但在分布式系统中需要中心化协调。UUID 无需协调即可提供算法上唯一的值，但随机 UUID（v4）会破坏 B-tree 的局部性，因为 B-tree 索引保持排序顺序，并受益于顺序插入。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@sonal.sadafal/postgresql-uuid-performance-random-v4-vs-time-ordered-v7-a-deep-dive-067b2de044ef">PostgreSQL UUID Performance: Random (v4) vs Time-Ordered (v7 ...</a></li>
<li><a href="https://wildandfreetools.com/blog/uuid-v7-time-ordered-sortable-guide/">UUID v7 Explained: Time-Ordered, Sortable, and Better Than v4</a></li>
<li><a href="https://thirdwaveweb.com/why-b-tree-index-fragmentation-is-killing-your-queries-and-three-tools-that-actually-fix-it/">Why B-Tree Index Fragmentation Is Killing Your Queries (And ...</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#UUID`, `#primary keys`, `#indexing`, `#database design`

---

<a id="item-8"></a>
## [拆分事务型 API：网络边缘与 PostgreSQL 事务权威](https://postgr.es/p/9sW) ⭐️ 7.0/10

在一篇新文章中，Alexey Evlampiev 提出，事务型 API 的网络边缘（调用者认证、HTTP 适配）与事务操作（校验、授权、执行、结果整形）应当分离，由 PostgreSQL 负责事务这一半。文章引入“事务操作”作为设计单位，REST 仅是它的一个绑定。 这重新定义了“只用 Postgres”的趋势：在存储组件都迁入 PostgreSQL 后，API 层依然留在外部；将事务边界移入数据库可获得唯一权威和可执行证明。后端系统可以原子地测试端到端操作与状态变迁，简化一致性、授权和回滚测试。 文章聚焦于有价值行为是对 PostgreSQL 状态进行事务决策的 API，而非通用 CRUD。每个事务操作被定义为一个具名数据库操作，包含类型化契约、授权策略、声明事务、实现和测试，使每个声明的结果都能在同一事务中得到证明。

rss · Planet PostgreSQL · 8月21日 00:00

**背景**: 近年来，PostgreSQL 整合了队列、缓存、搜索索引和向量存储等存储角色，但 API 层通常仍留在应用框架中。事务型 API 分为两半：网络边缘负责认证和 HTTP 适配，而事务边界负责解析、校验、授权、执行和整形结果。PostgreSQL 的事务管理系统是这些决策的底层权威；将该边界移入数据库后，测试可以在一个快照中端到端调用操作并回滚所有内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/transactions.html">PostgreSQL: Documentation: 18: Chapter 67. Transaction Processing</a></li>
<li><a href="https://stackoverflow.com/questions/12778209/are-postgresql-functions-transactional">database - Are PostgreSQL functions transactional? - Stack ... Code sample</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#transactional API`, `#architecture`, `#backend design`

---

<a id="item-9"></a>
## [显式插入 ID 为何让 PostgreSQL 序列失步](https://postgr.es/p/9sV) ⭐️ 7.0/10

一篇新的技术文章演示了向 bigserial 或 identity 列插入显式主键值时，底层序列并不会随之推进，导致后续由数据库生成 ID 的插入操作因重复键错误而失败。文章提供了在 PostgreSQL 18.6 上可复现的示例，并解释了如何用 setval 修正序列。 这是数据加载过程中常见的陷阱，在迁移或种子脚本之后可能让应用处于隐患状态，错误要到第一次真实插入时才出现。理解这一行为有助于数据库开发者避免莫名其妙的重复键错误，并正确重置序列同步。 即使显式插入了 id 为 1 到 3 的三行数据，序列仍显示 last_value=1 且 is_called=false，因此下一次 nextval 会返回 1。在空表上使用 setval(seq, max(id))不会有任何效果，因为传入 NULL 时 setval 会直接返回；is_called 标志决定传入的数字是下一个值还是最后一个已用值。

rss · Planet PostgreSQL · 8月21日 00:00

**背景**: 在 PostgreSQL 中，serial 和 identity 列依赖序列（sequence）为列提供默认值。当客户端显式提供 id 时，默认的 nextval 表达式根本不会被评估，因此序列停留在原位置，而表数据却在不断增长。当应用后续省略 id 时，序列会生成一个表中已存在的值，于是产生重复键错误。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/sql-createsequence.html">PostgreSQL: Documentation: 18: CREATE SEQUENCE</a></li>
<li><a href="https://wiki.postgresql.org/wiki/Fixing_Sequences">Fixing Sequences - PostgreSQL wiki</a></li>
<li><a href="https://www.cybertec-postgresql.com/en/fixing-out-of-sync-sequences-in-postgresql/">Fixing out-of-sync sequences in PostgreSQL | CYBERTEC PostgreSQL | Services & Support</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database`, `#sequences`, `#data-loading`, `#debugging`

---

<a id="item-10"></a>
## [pg_shmemviz：在浏览器中可视化 PostgreSQL 共享内存的新工具](https://postgr.es/p/9sP) ⭐️ 7.0/10

Bertrand Drouvot 推出了 pg_shmemviz，这是一个新的调试工具，可以将 PostgreSQL 的主共享内存和动态共享内存段捕获为离线快照，并在本地浏览器中展示。它沿用了现有工具 pg_walviz 的方法，提供物理布局、字节级导航、以及分配、结构字段、填充和原始字节的同步视图。 对于需要调试或分析共享内存内部的 PostgreSQL 开发者来说，这个工具非常有价值，它可以更直观地显示分配在物理上的位置以及指针引用如何映射到实际数据。它通过为共享内存检查增加可视化和交互维度，补充了 pg_shmem_allocations 和 pg_buffercache 等现有视图。 该界面包含共享内存地图、分配表、结构检查器和物理字节视图，所有视图保持同步，选择某个分配或字段会更新其他面板。它利用精确匹配的 postgres 可执行文件中的 DWARF 信息来显示嵌套 C 结构、字段偏移、编译器填充和数组步幅填充，并针对统计信息、WAL、进程、SLRU、dynahash 和 DSM 注册表结构提供专门的发现机制。该工具目前处于 beta 阶段，主要面向 PostgreSQL 20devel。

rss · Planet PostgreSQL · 8月20日 01:00

**背景**: PostgreSQL 使用共享内存进行进程间通信并存储共享数据结构，如缓冲区缓存、锁表和统计信息。现有的系统视图（如 pg_shmem_allocations 和 pg_buffercache）提供部分信息，但无法展示物理布局或字节级细节。pg_shmemviz 基于 pg_walviz 的概念——后者用于可视化 WAL 段——将这种方法扩展到共享内存。该工具将离线快照加载到浏览器中，并利用 DWARF 调试信息来映射结构和指针。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/bdrouvot/pg_shmemviz">GitHub - bdrouvot/pg_shmemviz</a></li>
<li><a href="https://github.com/bdrouvot/pg_walviz">GitHub - bdrouvot/pg_walviz</a></li>
<li><a href="https://bdrouvot.github.io/2026/08/13/welcome-to-pg-walviz-postgresql-wal-segment-visualizer/">Welcome to pg_walviz: PostgreSQL WAL segment visualizer</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#shared memory`, `#visualization`, `#debugging`, `#developer tools`

---

<a id="item-11"></a>
## [编码代理让原生界面变便宜：别再写 TUI 了](https://simonwillison.net/2026/Aug/21/stop-making-tuis/) ⭐️ 7.0/10

Thomas Ptacek 发文认为，AI 编码代理已让原生用户界面的开发成本低到足以取代 TUI，即使是小型个人工具也应如此。Simon Willison 表示赞同，并提到他自己用 vibe coding 写的 macOS 菜单栏应用（监控带宽和 GPU）至今仍在每天使用。 这反映了 AI 辅助编程降低 GUI 开发门槛的普遍趋势，可能会让 TUI 在个人工具中不再那么必要。它也可能促使开发者重新考虑默认的工具形态，转而用原生应用完成那些以前只值得写一个 CLI 的任务。 原文发布于 sockpuppet.org，日期为 2026 年 8 月 20 日，Ptacek 呼吁开发者“把你那 500 个用完即弃的 CLI 中的一个变成原生应用”。Willison 提到他早在 2026 年 3 月就写过用 SwiftUI 开发的菜单栏应用，并说自己“已经找不到借口”不为其他项目做界面了。

rss · Simon Willison · 8月21日 16:07

**背景**: TUI（文本用户界面）是一种基于终端的界面，使用文本和视觉元素与程序交互，介于纯命令行界面和完整图形界面之间。AI 编码代理是能够跨项目自主编写、修改、调试和重构代码的工具；“vibe coding”则指用自然语言描述意图，让 AI 生成代码，通常很少人工审查。这篇文章的核心论点是：传统上比 CLI 昂贵得多的 GUI 开发，在 AI 帮助下已经便宜到值得为小型个人脚本也做一个原生界面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dev.to/devasservice/introduction-to-textual-building-modern-text-user-interfaces-in-python-6c2">Introduction to Textual : Building Modern Text User Interfaces in Python</a></li>
<li><a href="https://agentic.ai/best/coding-agents">Best AI Coding Agents in 2026</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding - Wikipedia</a></li>

</ul>
</details>

**标签**: `#TUI`, `#GUI`, `#coding-agents`, `#vibe-coding`, `#native-apps`

---

<a id="item-12"></a>
## [ChatGPT 搜索现大规模使用 site: 运算符](https://simonwillison.net/2026/Aug/20/chatgpt-search-now-uses-the-siteoperator-at-scale/) ⭐️ 7.0/10

Promptwatch 的数据显示，包含 site: 运算符的 ChatGPT 搜索查询占比在 8 月 8 日从约 0.3%–0.5% 跃升至 16%–17%，正好与 OpenAI 的 GPT-5.6 发布重合。这表明 OpenAI 改变了大规模处理限定域名搜索的方式。 这对 SEO 和生成式引擎优化（GEO）从业者意义重大，因为它表明 ChatGPT 越来越多地默认使用域名限定搜索，从而改变网站在 AI 助手中的被发现方式。这也标志着 AI 搜索行为的转变，可能影响 Reddit 等大型网站的流量模式。 这些数据来自 Promptwatch 的自动化跟踪，仅反映其监控范围内的提示词。OpenAI 在 8 月 6 日的公告中仅表示 GPT-5.6 Sol 会‘更可靠地处理事实’，但未透露细节；Willison 猜测搜索工具现在可能形如 search(query, recency, domains)，而不是直接鼓励使用 site: 运算符。

rss · Simon Willison · 8月20日 23:57

**背景**: site: 运算符是一种标准搜索运算符，用于将结果限制在特定网站内，长期以来一直用于传统搜索引擎。生成式引擎优化（GEO）是一种提升品牌在 ChatGPT 等 AI 工具生成答案中可见度的做法。Promptwatch 是一个 GEO 平台，跟踪 ChatGPT、Claude、Gemini 等平台的 AI 搜索可见度，并利用汇总数据来发现这些工具的行为变化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://promptwatch.com/about">About - Promptwatch</a></li>
<li><a href="https://en.wikipedia.org/wiki/Generative_engine_optimization">Generative engine optimization - Wikipedia</a></li>
<li><a href="https://developers.google.com/search/docs/monitor-debug/search-operators/all-search-site">How To Use the Site Search Operator | Google Search Central | Documentation | Google for Developers</a></li>

</ul>
</details>

**标签**: `#AI search`, `#ChatGPT`, `#GEO`, `#SEO`, `#Generative Engine Optimization`

---