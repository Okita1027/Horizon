---
layout: default
title: "Horizon 日报：2026-06-30 (ZH)"
date: 2026-06-30
lang: zh
---

> 从 30 条内容中筛选出 11 条重要资讯。

---

1. [火箭实验室收购铱星公司，达成里程碑交易](#item-1) ⭐️ 9.0/10
2. [最高法院：地理围栏搜查令需受第四修正案保护](#item-2) ⭐️ 9.0/10
3. [.self 顶级域名提案：支持自托管但面临挑战](#item-3) ⭐️ 8.0/10
4. [因藏匿 zines 被判 30 年引发言论自由担忧](#item-4) ⭐️ 8.0/10
5. [WATaBoy：将 GB 指令即时编译为 WASM，性能超越原生解释器](#item-5) ⭐️ 8.0/10
6. [相同行不同 SUM：PostgreSQL 中浮点非确定性](#item-6) ⭐️ 8.0/10
7. [Ornith-1.0：开源权重 LLM 实现编码基准最佳](#item-7) ⭐️ 8.0/10
8. [索引唯一扫描仍读取堆的原因](#item-8) ⭐️ 7.0/10
9. [PostgreSQL 19 填补升级流程中的序列同步缺口](#item-9) ⭐️ 7.0/10
10. [灾难恢复是流程：最佳运行手册工程实践](#item-10) ⭐️ 7.0/10
11. [PostgreSQL 增量排序的利弊分析](#item-11) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [火箭实验室收购铱星公司，达成里程碑交易](https://investors.rocketlabcorp.com/news-releases/news-release-details/rocket-lab-acquire-iridium-historic-deal-creating-fully) ⭐️ 9.0/10

火箭实验室宣布收购铱星通信公司，首次将发射服务提供商与卫星星座运营商合并。 这种垂直整合可能重塑航天业，为火箭实验室提供有保障的发射需求和盈利的卫星业务，类似于 SpaceX 与星链的模式。 交易包括铱星公司的频谱资产和卫星网络，可用于未来由火箭实验室建造的铱星星座替换。此次收购反映了向垂直整合航天公司的战略转变。

hackernews · everfrustrated · 6月29日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=48719485)

**背景**: 铱星公司运营着 66 颗低轨卫星组成的星座，提供全球语音和数据通信。火箭实验室是一家以电子火箭闻名的小型发射提供商，并已扩展到卫星制造领域。航天领域的垂直整合指一家公司同时控制发射和卫星运营，以降低成本和依赖性。

**社区讨论**: 社区反应不一：一些人认为此次收购是确保发射需求和增长的战略妙招，而另一些人则对太空垃圾增加和低轨商业化表示担忧。还有对火箭实验室从新西兰起源转向美国公司的讨论。

**标签**: `#space industry`, `#acquisition`, `#Rocket Lab`, `#Iridium`, `#satellite communications`

---

<a id="item-2"></a>
## [最高法院：地理围栏搜查令需受第四修正案保护](https://www.theguardian.com/us-news/2026/jun/29/supreme-court-geofence-warrants-case-decision) ⭐️ 9.0/10

美国最高法院裁定，地理围栏搜查令需受第四修正案的宪法保护，这是数字隐私领域的里程碑式裁决。该裁决可能要求执法部门在获取科技公司的位置数据前，必须基于可能原因申请搜查令。 这一裁决加强了对数百万智能手机用户的隐私保护，限制了政府进行大规模基于位置的监控的能力。它为法院如何将第四修正案应用于现代数字证据收集树立了重要先例。 该案涉及谷歌在抢劫时间段内向执法部门提供了银行附近 150 米范围内 19 台设备的位置数据。最高法院认为，这种未经个性化怀疑的大规模收集行为违反了第四修正案。

hackernews · cdrnsf · 6月29日 15:54 · [社区讨论](https://news.ycombinator.com/item?id=48720924)

**背景**: 地理围栏搜查令，也称为反向位置搜查令，是一种允许执法部门向谷歌等公司请求特定时间段内特定地理区域内所有设备位置数据的搜查令。与传统针对特定人员的搜查令不同，地理围栏搜查令“反向运行”，通过设备与犯罪现场的接近程度来识别未知嫌疑人。第四修正案保护公民免受不合理的搜查和扣押，要求搜查令必须具体且基于可能原因。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Geofence_warrant">Geofence warrant - Wikipedia</a></li>
<li><a href="https://www.congress.gov/crs_external_products/LSB/PDF/LSB11274/LSB11274.4.pdf">PDF Geofence Warrants and the Fourth Amendment - Congress.gov</a></li>
<li><a href="https://govfacts.org/tech-innovation/digital-rights-privacy/digital-surveillance/geofence-warrants-how-police-use-your-phones-location-to-solve-crimes/">Geofence Warrants: How Police Use Your Phone's Location to Solve Crimes</a></li>

</ul>
</details>

**社区讨论**: 评论者强调了法院在意见书中引用事实来源的做法，并讨论了更广泛的影响。有人指出，照片元数据经常在没有法律程序的情况下泄露位置数据，而地理围栏搜查令现在需要宪法保护，这具有讽刺意味。

**标签**: `#privacy`, `#supreme court`, `#geofence warrants`, `#constitutional law`, `#location data`

---

<a id="item-3"></a>
## [.self 顶级域名提案：支持自托管但面临挑战](https://hccf.onmy.cloud/2026/06/21/reclaiming-our-digital-selves-hccfs-vision-for-a-human-centered-top-level-domain/) ⭐️ 8.0/10

一项关于新顶级域名 .self 的提案已发布，旨在为个人提供免费子域名用于自托管。该计划试图创建一个以人为本的 TLD，并包含反抢注措施和身份验证。 如果成功，.self 可能使个人重新掌控自己的在线身份，减少对中心化平台的依赖。然而，它必须克服像 .tk 这类之前免费 TLD 所面临的声誉和滥用问题。 该提案包括每人一个免费域名、子域名分配，以及对非活跃域名的挑战机制。资金和反滥用政策的执行仍是未解决问题，作者建议采用捐赠和社区治理。

hackernews · HumanCCF · 6月29日 19:49 · [社区讨论](https://news.ycombinator.com/item?id=48724230)

**背景**: 顶级域名（TLD）是域名最后的部分，如 .com 或 .org。自托管指个人运行自己的服务器，而非使用第三方服务。之前的免费 TLD（如 Freenom 提供的 .tk）由于缺乏监管，与垃圾邮件和钓鱼活动关联，导致被主要平台屏蔽。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48724230">.self: A new top-level domain designed to support self-hosting | Hacker News</a></li>
<li><a href="https://en.wikipedia.org/wiki/.tk">.tk - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者表达了怀疑，引用 .tk TLD 作为一个警示故事，免费域名吸引了滥用者。一些人建议整合声誉系统或要求身份证明以减少抢注。其他人质疑财务可持续性，并提出了替代方案，如微软的 Vega 用于身份管理。

**标签**: `#domains`, `#self-hosting`, `#TLD`, `#privacy`, `#internet governance`

---

<a id="item-4"></a>
## [因藏匿 zines 被判 30 年引发言论自由担忧](https://theintercept.com/2026/06/26/daniel-sanchez-estrada-zines-prairieland-free-speech/) ⭐️ 8.0/10

一名男子因藏匿联邦搜查令所追查的 zines（政治小册子）而被判处 30 年监禁，这些 zines 与一起导致联邦探员被枪击的 Antifa 抗议活动有关。 此案凸显了言论自由权与妨碍司法之间的紧张关系，对非暴力证据篡改行为判处 30 年重刑引发了关于量刑公正性的担忧。 被告藏匿的 zines 已公开多年，搜查令针对的是抗议活动的文件——该抗议中使用烟花引诱 ICE 急救人员，导致一名探员中枪。

hackernews · xrd · 6月28日 21:42 · [社区讨论](https://news.ycombinator.com/item?id=48711981)

**背景**: 此案涉及联邦搜查令，与一场 Antifa 抗议活动的证据有关。被告并非枪手，但其妻子要求他藏匿材料。30 年刑期针对的是妨碍司法和证据篡改，而非 zines 的内容。

**社区讨论**: 评论存在分歧：一些人认为在暴力犯罪背景下，因证据篡改而重判是合理的；另一些人则视其为对言论自由的攻击。多位评论者强调，案件忽略了枪击事件的背景。

**标签**: `#free speech`, `#legal`, `#civil liberties`, `#social media`

---

<a id="item-5"></a>
## [WATaBoy：将 GB 指令即时编译为 WASM，性能超越原生解释器](https://humphri.es/blog/WATaBoy/) ⭐️ 8.0/10

WATaBoy 是一款创新的 Game Boy 模拟器，采用即时编译（JIT）技术将 Game Boy 指令转换为 WebAssembly（WASM），性能超越了原生解释器。这表明将 JIT 编译到 WASM 可能比直接解释原生代码更快。 该方案可以在允许 WebAssembly 但限制原生 JIT 的平台（如 iOS）上实现高性能模拟。同时，它也展示了 WebAssembly 作为动态重编译目标的潜力，对复古游戏等领域具有广泛影响。 WATaBoy 的 JIT 编译器在运行时将 Game Boy 操作码转换为 WASM 模块，利用宿主浏览器或引擎的 WebAssembly 运行时实现接近原生的速度。该项目是一项本科作品，并指出在此工作负载下 Firefox 比 Chrome/Safari 慢约 25%。

hackernews · energeticbark · 6月29日 15:02 · [社区讨论](https://news.ycombinator.com/item?id=48720190)

**背景**: 即时编译（JIT）在运行时编译代码以提高执行速度，结合了解释的灵活性和原生代码的性能。WebAssembly（WASM）是一种专为网络高性能设计的二进制格式，得到所有主流浏览器的支持。Game Boy 模拟需要解释自定义的 SM83 CPU 指令集，计算强度较高。通过 JIT 编译到 WASM，WATaBoy 避免了指令解释的开销，转而依赖优化的 WASM 运行时。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/JIT_compilation">JIT compilation</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly</a></li>
<li><a href="https://gbdev.io/gb-opcodes/optables/">Game Boy CPU (SM83) instruction set</a></li>

</ul>
</details>

**社区讨论**: 社区评论指出，使用 JavaScript 的 eval 或 new Function 是编写 JIT 最简单的方法，并引用 Andrew Kelley 关于 NES 静态重编译的文章，认为 JIT 是解决方案。有人指出 iOS 仅允许在浏览器中使用 JIT，因此该方法在 iOS 上可行。一位评论者称赞该项目并指出 Firefox 性能较慢，另一位解释 WASM 开销（约 20%）远小于解释器开销（约 1000%），因此结果并不意外。

**标签**: `#JIT compilation`, `#WebAssembly`, `#emulation`, `#Game Boy`, `#WASM`

---

<a id="item-6"></a>
## [相同行不同 SUM：PostgreSQL 中浮点非确定性](https://postgr.es/p/9nx) ⭐️ 8.0/10

即使数据相同且无并发修改，PostgreSQL 中对 double precision 列的重复 SUM 查询也可能返回不同结果，原因是并行聚合和非结合性浮点加法。 这揭示了一个影响数据库从业者的细微可重复性问题，特别是那些在报告、分析或仪表板中使用浮点数据的人；它强调当涉及并行性时，“不要将货币存储为浮点数”的规则是不够的。 非确定性发生的根源在于浮点加法不具有结合性，且并行查询执行会以不可预测的顺序对部分结果求和；PostgreSQL 的默认并行设置可能仅需 500 万行数据即可触发此问题。

rss · Planet PostgreSQL · 6月28日 19:45

**背景**: 浮点数是有限精度的近似值；由于舍入，加法和乘法不具有结合性。当 SUM 查询并行运行时，每个工作者计算部分和，最终结果取决于这些部分和的组合顺序。这不是 Bug，而是 IEEE 754 算术的固有特性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://boringsql.com/posts/same-rows-different-sum/">Same rows, different SUM | boringSQL</a></li>
<li><a href="https://developer.nvidia.com/blog/controlling-floating-point-determinism-in-nvidia-cccl/">Controlling Floating-Point Determinism in NVIDIA CCCL | NVIDIA Technical Blog</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#floating-point`, `#database`, `#SQL`, `#precision`

---

<a id="item-7"></a>
## [Ornith-1.0：开源权重 LLM 实现编码基准最佳](https://simonwillison.net/2026/Jun/29/ornith/#atom-everything) ⭐️ 8.0/10

DeepReinforce 发布了 Ornith-1.0，这是一个基于 Gemma 4 和 Qwen 3.5 构建的 MIT 开源权重 LLM 系列（9B 密集、31B 密集、35B MoE、397B MoE），在同等规模的开源模型中取得了编码基准测试的最佳结果。 此次发布通过提供许可宽松、表现优异的编码模型，增强了开源 AI 生态系统，可能使更广泛的用户群体获得智能编码能力，并减少对专有模型的依赖。 该模型支持自我支架（self-scaffolding），即无需外部组件即可将复杂任务分解为子步骤，并提供 GGUF 格式以便本地推理。早期用户报告显示其在多步骤工具使用任务（如导航代码库和生成图像）上表现良好。

rss · Simon Willison · 6月29日 16:17

**背景**: 自我支架是一种让 LLM 在内部将任务分解为显式子步骤的技术，无需外部工具即可提升推理能力。混合专家（MoE）架构每次只激活部分参数，从而在保持低推理成本的同时支持更大模型。GGUF 是一种量化 LLM 的文件格式，针对使用 LM Studio 等工具的本地执行进行了优化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/29/ornith/">Ornith-1.0: Self - Scaffolding LLMs for Agentic Coding</a></li>
<li><a href="https://www.lesswrong.com/posts/mAwxebLw3nYbDivmt/scaffolded-llms-less-obvious-concerns">Scaffolded LLMs : Less Obvious Concerns — LessWrong</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>

</ul>
</details>

**标签**: `#LLM`, `#open-source`, `#coding`, `#agentic AI`, `#model release`

---

<a id="item-8"></a>
## [索引唯一扫描仍读取堆的原因](https://postgr.es/p/9nM) ⭐️ 7.0/10

Christophe Pettus 解释了 PostgreSQL 中索引唯一扫描在物理上可行的情况下，仍可能因可见性检查而几乎每行都读取堆。 这澄清了一个常见误解，帮助数据库工程师优化查询，避免因索引唯一扫描导致意外的性能下降。 堆读取是因为索引唯一扫描必须通过可见性映射验证行可见性；如果表页面并非全部可见，PostgreSQL 会获取堆元组。GUC 参数 enable_indexonlyscan 控制是否使用这种扫描类型。

rss · Planet PostgreSQL · 6月30日 01:00

**背景**: 索引唯一扫描允许 PostgreSQL 仅从索引回答查询，当索引包含所有需要的列且可见性映射表明行可见时，避免堆访问。为了高效工作，通常使用覆盖索引（通过 INCLUDE 子句）。GUC 参数 enable_indexonlyscan 是多个规划器开关之一，用于启用或禁用特定的扫描类型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/indexes-index-only-scans.html">PostgreSQL : Documentation: 18: 11.9. Index - Only Scans and...</a></li>
<li><a href="https://pgpedia.info/g/guc.html">GUC - Grand Unified Configuration - pgPedia - a PostgreSQL ...</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#indexing`, `#performance`, `#GUC`

---

<a id="item-9"></a>
## [PostgreSQL 19 填补升级流程中的序列同步缺口](https://postgr.es/p/9nL) ⭐️ 7.0/10

PostgreSQL 19 通过出版物中的新 ALL SEQUENCES 子句实现了逻辑复制的自动序列同步，填补了在接近零停机升级过程中无法复制序列状态的长期缺口。 该功能通过确保升级过程中序列数据的完整性，消除了数据库管理员在切换窗口期的压力，使接近零停机的 PostgreSQL 升级更加可靠和实用。 该功能要求发布者使用 CREATE PUBLICATION upgrade_pub FOR ALL TABLES, ALL SEQUENCES，订阅者相应地创建订阅。它由 Amit Kapila 通过三个提交实现。

rss · Planet PostgreSQL · 6月30日 00:38

**背景**: PostgreSQL 升级通常使用 pg_upgrade 结合逻辑复制实现接近零停机。然而，逻辑复制传统上只复制表，不复制序列，导致故障切换后序列值出现缺口。pg_createsubscriber 帮助将物理副本转换为逻辑订阅者，但此前序列并未同步。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bytebase.com/blog/postgres-19-feature-preview-logical-replication-sequence/">Postgres 19 Feature Preview: Sequence Synchronization for Logical Replication | Bytebase</a></li>
<li><a href="https://www.depesz.com/2025/11/11/waiting-for-postgresql-19-sequence-synchronization-in-logical-replication/">Waiting for PostgreSQL 19 – Sequence synchronization in logical replication. – select * from depesz;</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database upgrade`, `#sequence synchronization`, `#pg_upgrade`

---

<a id="item-10"></a>
## [灾难恢复是流程：最佳运行手册工程实践](https://postgr.es/p/9nK) ⭐️ 7.0/10

Richard Yen 的续篇指出，灾难恢复依赖于经过演练的运行手册和流程，而非仅仅依靠工具，并指出了运行手册设计中的常见反模式。 这很重要，因为许多团队拥有备份和复制，但由于未经过测试的运行手册而在实际恢复中失败，导致宕机时间延长和数据丢失。 该文章详细描述了反模式，如庞大的 wiki 页面、过时的命令、缺乏回滚标准、所有权不明确以及模糊的指令，强调运行手册必须具有程序性和确定性。

rss · Planet PostgreSQL · 6月29日 08:00

**背景**: 灾难恢复（DR）涉及在故障后恢复 IT 系统的流程。关键指标是 RPO（恢复点目标）和 RTO（恢复时间目标）。运行手册是处理事件的逐步指南，但常常失败，因为它们是由专家在平静环境下编写的，而非为凌晨 3 点压力大、疲惫的操作员准备的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.pagerduty.com/resources/automation/learn/what-is-a-runbook/">What is a Runbook ? | PagerDuty</a></li>
<li><a href="https://www.linkedin.com/pulse/understanding-rpo-rto-disaster-recovery-petros-tsehay-c0vpe">Understanding RPO and RTO in Disaster Recovery</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#disaster recovery`, `#runbooks`, `#operational excellence`, `#database administration`

---

<a id="item-11"></a>
## [PostgreSQL 增量排序的利弊分析](https://postgr.es/p/9ny) ⭐️ 7.0/10

Christophe Pettus 的文章探讨了 PostgreSQL 的 enable_incremental_sort 特性，指出它利用预排序数据提升性能，但也警告在倾斜数据上因成本估算错误可能导致优化器选择糟糕的执行计划。 这对数据库性能工程师至关重要，因为增量排序（自 PostgreSQL 13 起默认启用）是一种强大的优化，能减少排序开销，但若在倾斜数据上误解其成本模型，可能导致严重的性能下降。 增量排序在 PostgreSQL 13 中引入，由 enable_incremental_sort 参数控制，默认开启。该特性在输入已部分排序时效果最佳，但倾斜数据上的成本估算不准确会导致规划器高估其收益并选择次优计划。

rss · Planet PostgreSQL · 6月29日 01:00

**背景**: 增量排序是一种查询优化技术，它利用已有的行顺序增量式地排序数据，避免对所有行进行全排序。数据倾斜指列中值分布不均匀，某些值出现频率远高于其他值，这使得 PostgreSQL 规划器难以进行准确的成本估算。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@chaitanya.vcs22/postgres-incremental-sorting-and-its-improvements-f0d1d719497f">Postgres Incremental Sorting and its Improvements | Medium</a></li>
<li><a href="https://www.cybrosys.com/research-and-development/postgres/step-by-step-guide-to-postgresql-incremental-sorting-for-faster-queries">Step-by-Step Guide to PostgreSQL Incremental Sorting for Faster...</a></li>
<li><a href="https://stormatics.tech/blogs/incremental-sort-in-postgresql-a-developers-guide">Incremental Sort in PostgreSQL : A Developer's Guide - Stormatics</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#query optimization`, `#incremental sort`, `#database performance`, `#cost estimation`

---