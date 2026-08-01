---
layout: default
title: "Horizon 日报：2026-08-01 (ZH)"
date: 2026-08-01
lang: zh
---

> 从 54 条内容中筛选出 19 条重要资讯。

---

1. [OpenAI 大幅下调 GPT-5.6 价格，并用 Sol 优化推理效率](#item-1) ⭐️ 9.0/10
2. [电梯调度算法及其权衡的分析](#item-2) ⭐️ 8.0/10
3. [YC 开源 QM：面向工作的多人智能体协作框架](#item-3) ⭐️ 8.0/10
4. [Go 提议在标准库中加入泛型集合类型](#item-4) ⭐️ 8.0/10
5. [DataFusion 让十亿边图算法在 10GB 内存的单机上运行](#item-5) ⭐️ 8.0/10
6. [我们为何弃用了自家的 LLM 路由器](#item-6) ⭐️ 8.0/10
7. [PostgreSQL 19 将新增 SQL 属性图查询（SQL/PGQ）](#item-7) ⭐️ 8.0/10
8. [PostgreSQL 18 的 extension_control_path 让扩展容器化](#item-8) ⭐️ 8.0/10
9. [指挥式开发者：AI 编排正在重新定义开发者角色](#item-9) ⭐️ 8.0/10
10. [DeepSeek 发布 V4-Flash-0731：304B 参数模型强化智能体能力](#item-10) ⭐️ 8.0/10
11. [无状态 MCP 2.0 重燃兴趣，催生新工具](#item-11) ⭐️ 8.0/10
12. [调查我们网络安全评估中的三个真实事件](#item-12) ⭐️ 8.0/10
13. [hot_standby_feedback：只解决清理冲突，备库防取消有代价](#item-13) ⭐️ 7.0/10
14. [Postgres 19 预览：新的随机日期函数与 DDL 查询工具](#item-14) ⭐️ 7.0/10
15. [pgvector 迭代索引扫描实现 Postgres 混合搜索](#item-15) ⭐️ 7.0/10
16. [vip-manager v5 发布：了解破坏性变更与升级要点](#item-16) ⭐️ 7.0/10
17. [重构的经济效益现在可以通过 Token 成本来衡量](#item-17) ⭐️ 7.0/10
18. [Simon Willison 做客 Oxide and Friends 讨论开放权重革命](#item-18) ⭐️ 7.0/10
19. [smevals：一个轻量级评测套件，用于评估模型、提示词与测试框架](#item-19) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [OpenAI 大幅下调 GPT-5.6 价格，并用 Sol 优化推理效率](https://simonwillison.net/2026/Jul/30/luna-price-drop/#atom-everything) ⭐️ 9.0/10

OpenAI 宣布对其 GPT-5.6 系列模型大幅降价，最高降幅达 80%：Terra 降价 20%，Luna 降价 80%。OpenAI 还介绍了如何用 GPT-5.6 Sol 优化模型的前向传播（forward pass），自主重写生产内核，使端到端服务成本降低 20%。 Luna 以每百万输入 token 0.20 美元、每百万输出 token 1.20 美元的价格，已低于 Google 的 Gemini 3.1 Flash-Lite，并仅为 Anthropic Claude Haiku 4.5 输入价格的五分之一，重塑了低成本大模型市场。这还展示了前沿模型自我优化推理能力，开启了 AI 驱动效率提升的新趋势。 Luna 的新定价为每百万输入 token 0.20 美元、每百万输出 token 1.20 美元，此前其价格与 Claude Haiku 4.5 相同。GPT-5.6 Sol 通过预计算、避免或并行化计算来改进推理，并借助 Codex 用 Triton 和 Gluon（OpenAI 维护的两个开源 GPU 编程语言）重写生产内核。

rss · Simon Willison · 7月30日 23:58

**背景**: GPT-5.6 是 OpenAI 最新的模型系列，分为三个层级：Sol（旗舰）、Terra 和 Luna，OpenAI 称之为可以各自按节奏推进的“持久能力层级”。前向传播是推理过程中将输入 token 转换为下一个 token 预测的计算过程；对其进行优化可以减少内存搬运、同步开销和 GPU 空闲时间。每百万 token 的价格是开发者大规模部署大模型时的关键指标，因此大幅降价会改变他们的模型选择。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.vellum.ai/blog/gpt-5-6-benchmarks-explained">GPT - 5 . 6 Sol vs Terra vs Luna: Which Tier Should You Actually Use?</a></li>
<li><a href="https://www.geeksforgeeks.org/deep-learning/forward-propagation-in-neural-networks/">Forward Propagation in Neural Networks - GeeksforGeeks</a></li>
<li><a href="https://openrouter.ai/openai/gpt-5.6-sol">GPT - 5 . 6 Sol - API Pricing & Benchmarks | OpenRouter</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#GPT-5.6`, `#price reduction`, `#inference optimization`, `#AI efficiency`

---

<a id="item-2"></a>
## [电梯调度算法及其权衡的分析](https://john.fun/elevators) ⭐️ 8.0/10

一篇名为《Elevators》的分析文章深入探讨了电梯调度算法及其权衡，涵盖了 SCAN、LOOK 和目的地派梯（destination dispatch）等策略。该文在 Hacker News 上获得了热烈的社区讨论，并附带了 Elevator Saga 等交互式模拟的链接。 电梯调度每天影响大量人群，同时也是与磁盘调度具有相似性的经典系统与优化问题。这篇分析及随之而来的讨论，有助于工程师和爱好者理解公平性与效率之间的现实权衡。 据评论者所述，文章在随机目的地模拟下发现目的地派梯（destination dispatch）整体表现较差，但也有评论者认为这可能是模拟设置带来的假象。讨论还重点提到了 SCAN 和 LOOK 算法，并引用了交互式电梯调度游戏供读者动手实验。

hackernews · Jrh0203 · 7月31日 15:17 · [社区讨论](https://news.ycombinator.com/item?id=49124218)

**背景**: 电梯算法（SCAN）是一种经典的调度方法，得名于建筑物中电梯的行为方式：它沿当前方向继续运行，直到前方不再有待处理的请求，然后反向。LOOK 是其变体，只运行到有请求的最高或最低楼层。电梯系统设计中的一个基本权衡是公平性与效率：按到达顺序服务请求最公平但效率较低，而优化总等待时间可能导致部分乘客长时间得不到服务。目的地派梯系统要求乘客在进入电梯前选择目的楼层，使控制器能够按目的地集中分配乘客，但该方案的效果在很大程度上取决于实际客流模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Elevator_algorithm">Elevator algorithm - Wikipedia</a></li>
<li><a href="https://alamrafiul.com/blogs/elevator-problem/">The Elevator Problem: Scheduling and Load Balancing - Rafiul Alam</a></li>
<li><a href="https://www.systemdesignhandbook.com/guides/design-an-elevator-system/">Design an Elevator System: Guide to System Design Interviews</a></li>

</ul>
</details>

**社区讨论**: 评论者参与积极，有人将电梯调度类比为硬盘的 SCAN 磁盘调度算法，并分享了 Elevator Saga 交互式游戏链接。一位从业者质疑文章关于目的地派梯“整体更差”的结论是否源于随机目的地模拟，并举出现实中群体出行模式作为反例。还有几位评论者认为 LOOK 式行为最符合乘客预期，也有人抱怨乘客常常同时按下上、下按钮，给算法制造混乱。

**标签**: `#elevator-algorithms`, `#scheduling`, `#simulation`, `#systems`

---

<a id="item-3"></a>
## [YC 开源 QM：面向工作的多人智能体协作框架](https://github.com/yc-software/qm) ⭐️ 8.0/10

Y Combinator 以 MIT 许可证开源了 QM——一个面向工作的多人智能体（multi-agent）协作框架。QM 基于 YC 内部运行 50+ 智能体的经验构建，支持 Slack 与 Web 集成，并提供公司范围（company scopes）、定时任务（crons）和技能（skills）等功能。 作为 Y Combinator 的高关注度项目，QM 验证了工作场所中多人智能体协作这一日益增长的趋势。其公司级作用域（company scopes）和共享房间（shared rooms）为在组织规模上部署 AI 助手提供了一种务实模式，可能影响企业采用智能体 AI 的方式。 QM 是一个采用 MIT 许可证的开源框架，基于 YC 内部运行 50 多个智能体的经验，为每位员工和每个项目提供一个类似 OpenClaw 的智能体。其显著特性包括公司作用域（company scopes）、定时任务（crons）和技能（skills），同时支持 Slack 与 Web 集成。

hackernews · tosh · 7月31日 18:04 · [社区讨论](https://news.ycombinator.com/item?id=49126604)

**背景**: 智能体框架（agent harness）是围绕语言模型构建的支撑层，为其提供工具、记忆、运行循环、验证和防护措施，相当于 AI 智能体的操作系统。多智能体协作框架在这一基础上更进一步，让多个 AI 智能体能够协同完成任务。QM 将该概念应用于组织级工作场景，与 OpenClaw、Hermes 等工具一同定位为公司级助手层。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/yc-software/qm">GitHub - yc-software/qm: Multiplayer agent harness for work</a></li>
<li><a href="https://www.taskade.com/blog/agent-harness-explained">What Is an AI Agent Harness ? 2026 Guide | Taskade Blog</a></li>
<li><a href="https://www.explainx.ai/blog/y-combinator-qm-open-source-multi-agent-harness-august-2026">YC QM Open-Source Multi-Agent Harness 2026 | explainx.ai Blog</a></li>

</ul>
</details>

**社区讨论**: 评论者整体持建设性态度，但看法不一。有人质疑 QM 的差异化，希望看到“QM vs Claude Cowork”的对比；也有人提到 Garry Tan 的 gstack 等相关工具。相邻领域的开发者对这一方向表示认可，认为按人划分作用域并配合共享房间解决了关键痛点，并对 QM 的组织级上下文与安全架构表现出兴趣。

**标签**: `#multiplayer AI`, `#agent harness`, `#Y Combinator`, `#AI tools`, `#collaboration`

---

<a id="item-4"></a>
## [Go 提议在标准库中加入泛型集合类型](https://github.com/golang/go/issues/80590) ⭐️ 8.0/10

一项新提案（issue #80590）建议在 Go 标准库的 container/ 包下加入泛型集合类型。该提案概述了集合（set）和堆（heap）等抽象类型，具体实现将在后续版本中推出。 这填补了 Go 标准库长期以来的一个空白——标准库尚未利用 Go 1.18 引入的泛型特性。如果提案被接受，将为 Go 开发者提供官方的、可复用的数据结构（如集合和类型化堆），减少对第三方库和自定义实现的依赖。 提案指出，最初的抽象类型将不导出，仅作为 Go 惯例的文档说明，并可能在未来的版本中公开。同时参考了 issue #77397 中关于泛型 container/heap/v2.Heap API 的讨论，这表明该工作是向标准库添加泛型数据结构这一更大努力的一部分。

hackernews · jabits · 7月31日 18:39 · [社区讨论](https://news.ycombinator.com/item?id=49127031)

**背景**: Go 在 1.18 版本中加入了泛型支持，允许以类型无关的方式编写函数和数据结构。然而，标准库并未大幅更新以提供泛型集合类型，因此开发者常常需要自己编写或依赖第三方包。此提案是向标准库集成泛型迈进的一步，符合最初的设计目标——“应重新审视每个现有包，看其是否能从泛型中受益”。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/golang/go/issues/80590">proposal: container/...: generic collection types · Issue ...</a></li>
<li><a href="https://go.dev/blog/generics-proposal">A Proposal for Adding Generics to Go - The Go Programming ...</a></li>
<li><a href="https://www.dolthub.com/blog/2024-07-01-golang-generic-collections/">Writing generic collection types in Go: the missing documentation | DoltHub Blog</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一，但大体上是积极的。一些用户如 DarkNova6 指出，Go 正在“经历其他语言已经学过的艰难教训”，valcron1000 则开玩笑说“晚了 22 年，但迟做总比不做好”。也有人表达了担忧：athorax 认为“按现状将泛型构建进语言并不合适”，希望 Go v2 能更根本地解决这个问题；jiehong 则希望不要把可变方法混入提议的 API 中。

**标签**: `#Go`, `#generics`, `#collections`, `#standard library`, `#proposal`

---

<a id="item-5"></a>
## [DataFusion 让十亿边图算法在 10GB 内存的单机上运行](https://semyonsinchenko.github.io/ssinchenko/post/datafusion-graphs-cc-2/) ⭐️ 8.0/10

这篇文章展示了在单台机器上使用 Apache DataFusion，仅用 5GB 内存对十亿边的图运行 PageRank，以及用 10GB 内存对二十亿边的图识别弱连通分量。这远超 NetworkX 或 Igraph 等传统内存工具的能力。 这很关键，因为十亿级别的图处理通常需要借助 Apache Spark 和 GraphFrames 等分布式框架。DataFusion 的列式、核外执行能力让这类负载可以在普通硬件上完成，有望让大规模图分析变得更加普及。 图数据来自 Graphalytics 基准套件：graph500-26 用于 PageRank，twitter_mpi 用于弱连通分量。DataFusion 是一个用 Rust 编写的 Apache 顶级项目，基于 Arrow 列式内存格式，截至 2026 年 3 月在 crates.io 上每月下载量超过一百万次。

hackernews · speckx · 7月31日 15:53 · [社区讨论](https://news.ycombinator.com/item?id=49124658)

**背景**: NetworkX、Igraph 等传统图库要求整个图放入内存，因此在普通机器上只能处理数亿条边的图。核外（out-of-core）图处理系统（如 2012 年的 GraphChi）只在内存中保留部分活跃数据，其余数据放到磁盘。Apache DataFusion 是一个可扩展的分析查询引擎，利用 Arrow 列式格式实现向量化执行和高效的核外数据处理。这篇文章在这些思想的基础上，直接通过 DataFusion 的 DataFrame/SQL 接口运行图算法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apache_DataFusion">Apache DataFusion</a></li>
<li><a href="https://datafusion.apache.org/library-user-guide/index.html">Introduction — Apache DataFusion documentation</a></li>
<li><a href="https://arxiv.org/abs/2511.07886">ACGraph: An Efficient Asynchronous Out-of-Core Graph ... Images ACGraph: An Efficient Asynchronous Out-of-Core Graph ... Accelerating Out-of-Core Graph Random Walk Processing via ... Towards Communication-Efficient Out-of-Core Graph Processing ... GraphSD: A State and Dependency aware Out-of-Core Graph ... Squeezing out All the Value of Loaded Data: An Out-of-core ... Out-of-core Graph Algorithms - GraphAr</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论总体非常热烈。有人称 DataFusion 是“有史以来最好的开源项目之一”，也有人提到 GraphChi 和 Icebug 等早期工作。还有人指出，graphframes-rs 真正的创新在于借助 DataFusion 实现核外执行，但目前只有两个算法。

**标签**: `#graph-algorithms`, `#datafusion`, `#big-data`, `#out-of-core`, `#columnar`

---

<a id="item-6"></a>
## [我们为何弃用了自家的 LLM 路由器](https://manifest.build/blog/why-we-deprecated-our-llm-router/) ⭐️ 8.0/10

作者解释了为何弃用其 LLM 路由器，认为查询难度估算不可靠，简单的启发式方法或子代理角色往往更有效。这篇文章挑战了当前团队纷纷构建和采用 LLM 路由器的趋势。 这一观点很重要，因为它在一个普遍认为路由是核心优化技术的领域提供了反主流视角。它可能影响工程决策，提醒团队动态模型选择并不总是值得其复杂性，尤其是在对成本或延迟敏感的应用中。 作者的核心主张是，先验地估算查询难度本身就非常困难，而简单的启发式规则或将子代理角色绑定到特定模型往往比专用路由器表现更好。讨论中还提到编码智能体工作流是一个实用例子，编排器驱动的子代理分配在其中效果很好。

hackernews · brunaxLorax · 7月31日 18:06 · [社区讨论](https://news.ycombinator.com/item?id=49126630)

**背景**: LLM 路由器是一种动态决定由哪个语言模型来处理给定查询的系统，目标是在成本、延迟和质量之间取得平衡。许多团队构建或采用路由器，是因为不同模型在价格和能力上差异很大，其理念是把简单查询交给廉价模型、把困难查询交给前沿模型。然而，准确估算查询难度仍是一个开放性挑战，一些实践者认为，在生产环境中，确定性启发式规则或将模型绑定到特定子代理角色等更简单的替代方案往往更加稳健。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://redis.io/blog/llm-router-architecture-best-practices/">LLM router architecture: best practices for 2026 - Redis</a></li>
<li><a href="https://arxiv.org/html/2603.04445">Dynamic Model Routing and Cascading for Efficient LLM ...</a></li>
<li><a href="https://martinuke0.github.io/posts/subagents/">Sub-Agents in LLM Systems : Architecture, Execution Model ...</a></li>

</ul>
</details>

**社区讨论**: 评论者大多赞同作者的怀疑态度，并分享了自己“路由通常不值得投入”的经验，因为查询难度很难预测。有评论者指出，难度取决于智能体能够检索到的信息；另一位评论者则认为，在编码工作流中，将子代理角色绑定到特定模型非常有效。少数评论者对文章的行文质量提出质疑，并担心路由器可能会忽略模型的“个性”。

**标签**: `#LLM`, `#routing`, `#model-selection`, `#engineering`, `#cost-optimization`

---

<a id="item-7"></a>
## [PostgreSQL 19 将新增 SQL 属性图查询（SQL/PGQ）](https://postgr.es/p/9q_) ⭐️ 8.0/10

2026 年 3 月 16 日，Peter Eisentraut 将 SQL 属性图查询（SQL/PGQ）的实现提交到 PostgreSQL 19。这增加了 GRAPH_TABLE 表函数、CREATE/ALTER/DROP PROPERTY GRAPH DDL 命令，以及新的系统目录和信息模式视图。 这为 PostgreSQL（全球最广泛使用的数据库之一）原生带来了标准化的图查询能力，使用户无需迁移到专用图数据库即可运行图模式匹配工作负载。它将惠及需要分析关系数据中复杂关联的开发者与组织。 该实现遵循 ISO/IEC 9075-16:2023 标准，使用 GRAPH_TABLE 运算符在现有表上进行图模式匹配。属性图被定义为关系表上的视图，图查询会被重写为连接和联合操作。

rss · Planet PostgreSQL · 7月31日 16:57

**背景**: SQL/PGQ（SQL 属性图查询）是一项 ISO 标准扩展，允许用户在一个或多个关系表之上创建属性图，并使用 GRAPH_TABLE 原生查询这些图，从而将图模式匹配集成到 SQL 中。与专用图数据库不同，这种方法将图映射到关系模型上，因此现有数据无需迁移或使用额外扩展即可作为图进行查询。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pgql-lang.org/">PGQL | Property Graph Query Language</a></li>
<li><a href="https://neon.com/postgresql/postgresql-19/sql-pgq-graph-queries">PostgreSQL 19 SQL/PGQ Property Graph Queries</a></li>
<li><a href="https://www.iso.org/standard/79473.html">ISO/IEC 9075-16:2023 - Information technology — Database ...</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#SQL/PGQ`, `#Graph Databases`, `#SQL Standard`, `#Database Features`

---

<a id="item-8"></a>
## [PostgreSQL 18 的 extension_control_path 让扩展容器化](https://postgr.es/p/9r0) ⭐️ 8.0/10

PostgreSQL 18 新增了 extension_control_path 配置参数（GUC），使扩展的控制文件和 SQL 脚本可以存放在服务器自身目录之外。结合 Kubernetes 的 ImageVolume 和 Docker 的 --mount type=image，扩展现在可以打包为独立的 OCI 容器镜像，并在运行时挂载，而无需重建服务器镜像。 这一特性将扩展的生命周期管理与 PostgreSQL 服务器镜像解耦，使集群可以共享一个精简、未修改的服务器镜像，同时独立升级扩展。然而实际收益取决于扩展与服务器内部集成的深度，文章对此进行了详细分析。 extension_control_path 的工作方式类似于 dynamic_library_path，但适用于 .control 和 SQL 文件，并且需要的是 sharedir 级别的路径，而不是扩展子目录本身。路径中必须包含 $libdir 占位符，否则服务器将无法访问内置扩展；由于不同大版本之间的内部 ABI 会变化，镜像必须按 PostgreSQL 主版本分别构建。

rss · Planet PostgreSQL · 7月31日 10:08

**背景**: PostgreSQL 扩展通常由共享库文件（.so）、控制文件（.control）和 SQL 脚本组成，传统上必须安装在服务器自己的目录中。PostgreSQL 18 新增了 extension_control_path，允许将控制文件和 SQL 脚本放在其他位置，类似于 dynamic_library_path 处理共享库的方式。Kubernetes 的 ImageVolume（在 v1.36 中稳定）和 Docker Engine 28 支持将 OCI 镜像作为卷挂载，CloudNativePG 等运维工具也利用这一机制将扩展容器挂载到 PostgreSQL Pod 中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.pgedge.com/blog/postgresql-18-s-extension_control_path-decoupling-extensions-from-server-images">PostgreSQL 18's extension_control_path: Decoupling Extensions ...</a></li>
<li><a href="https://postgresqlco.nf/doc/en/param/extension_control_path/">PostgreSQL Documentation: extension_control_path parameter postgresql - The Twin Paths: extension_control_path and ... PostgreSQL: pgsql: extension_control_path PostgreSQL: Documentation: 18: CREATE EXTENSION extension_control_path - pgPedia - a PostgreSQL Encyclopedia postgresql - Controlling the location where a Postgres ...</a></li>
<li><a href="https://cloudnative-pg.io/docs/1.29/imagevolume_extensions/">Image Volume Extensions | CloudNativePG</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#extensions`, `#containerization`, `#DevOps`, `#database`

---

<a id="item-9"></a>
## [指挥式开发者：AI 编排正在重新定义开发者角色](https://martinfowler.com/rachels-ramblings/conductor-developer.html) ⭐️ 8.0/10

文章认为，AI 对软件开发的真正影响不仅仅是更快地编写代码，而是一种根本性转变：开发者像指挥家一样编排 AI 代理和工作流。文中提出“指挥式开发者”概念，指出人类注意力而非设计或验证已成为瓶颈。 这重新定义了 AI 在软件开发中的角色：从生产力工具转变为编排工具，可能影响团队的工作组织方式和开发者的培训方向。它直接回应了行业关于 AI 代理及软件开发生命周期未来的持续讨论。 文章提到一位工程师经常并行运行八个 AI 代理，作者身为 CTO 也以此为类比，说明自己同时管理多条工作流的日常。文中还提及最近的 FOSE（软件开发的未来）活动，会上讨论了在代理编写更多代码时如何确保设计、质量和韧性。

rss · Martin Fowler · 7月31日 13:48

**背景**: 这篇文章建立在关于 AI 对软件开发影响的讨论之上，例如 Thoughtworks 举办的 FOSE 工作坊，该工作坊探讨 AI 和 LLM 的兴起如何影响这一职业。文章用交响乐指挥家作比喻来解释开发者的新角色：他们必须把整个系统装进脑子里，而 AI 代理则像乐手演奏乐器那样执行具体任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://martinfowler.com/bliki/FutureOfSoftwareDevelopment.html">Future Of Software Development</a></li>

</ul>
</details>

**标签**: `#AI`, `#Software Development`, `#Developer Roles`, `#AI-Assisted Development`, `#Orchestration`

---

<a id="item-10"></a>
## [DeepSeek 发布 V4-Flash-0731：304B 参数模型强化智能体能力](https://simonwillison.net/2026/Jul/31/deepseek-v4-flash-0731/#atom-everything) ⭐️ 8.0/10

DeepSeek 于 2026 年 7 月 31 日发布 DeepSeek-V4-Flash-0731，这是一个 3040 亿参数、智能体（agentic）能力显著增强的模型。Artificial Analysis 将其排在 MiniMax M3 之前；以每百万输入 token 0.14 美元、每百万输出 token 0.27 美元的价格，它目前可能是单位智能成本最具优势的模型。 此次发布巩固了 DeepSeek 在竞争激烈的智能体 AI 市场中的位置，表明较小的模型也能超越更大的对手。其激进定价可能给其他供应商带来压力，并让开发者能以更低成本使用强大的智能体工作负载。 该模型在 Hugging Face 上大小为 167GB；据 DeepSeek 官方 API 更新日志，它与 V4-Flash-Preview 架构和规模相同，仅做了重新后训练（re-post-trained）。在 Simon Willison 的测试中，默认推理级别生成的鹈鹕图像质量较差，而通过 OpenRouter 将推理强度（reasoning_effort）调至 high 后效果明显更好。

rss · Simon Willison · 7月31日 23:59

**背景**: DeepSeek-V4 是一系列采用混合专家（MoE）架构的大模型，其中 Pro 版本拥有 1.6 万亿参数。'智能体（agentic）'AI 指的是能够主动推理、规划并采取行动，而不是仅仅对提示做出反应的系统。Artificial Analysis Intelligence Index 聚合了 GPQA Diamond、Terminal-Bench、Humanity's Last Exam 等基准，对模型的多项能力进行综合评分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepseek.ai/deepseek-v4">DeepSeek V 4 Explained: V 4 -Pro 1.6T vs V 4 - Flash 284B (2026)</a></li>
<li><a href="https://www.digitalapplied.com/blog/deepseek-v4-flash-0731-official-release-agent-benchmarks">DeepSeek V 4 Flash 0731: Official Release, Agent Benchmarks</a></li>
<li><a href="https://artificialanalysis.ai/">AI Model & API Providers Analysis | Artificial Analysis</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#AI`, `#language-models`, `#model-release`, `#machine-learning`

---

<a id="item-11"></a>
## [无状态 MCP 2.0 重燃兴趣，催生新工具](https://simonwillison.net/2026/Jul/31/stateless-mcp/#atom-everything) ⭐️ 8.0/10

2026 年 7 月 28 日发布的 MCP 2.0 规范引入了无状态传输模式，省去了会话 ID 和多步初始化的需要。Simon Willison 称这是 MCP 自发布以来最重要的变化，并在一周内构建了三个实现，包括 mcp-explorer 和 datasette-mcp。 这一更新大幅降低了实现 MCP 客户端和服务器的复杂性，使协议更易于审计和控制，也更适合构建可扩展的 Web 应用。它还将天平重新倾向于 MCP，作为允许智能体无限制访问终端和互联网的更安全替代方案，这可能会推动更多小型模型和企业部署采用该协议。 旧的有状态 MCP 需要两次 HTTP 请求：首先初始化会话并获得 Mcp-Session-Id，然后才能调用工具。新的无状态方式使用单个 HTTP 请求，通过 MCP-Protocol-Version 和 Mcp-Method 等头部传递所有上下文，这不仅简化了实现，还消除了服务器端会话状态维护的负担。

rss · Simon Willison · 7月31日 23:13

**背景**: MCP（模型上下文协议）是 Anthropic 于 2024 年 11 月推出的开放标准，旨在为大型语言模型连接外部工具和数据源提供统一接口。在无状态协议中，每个请求都是独立的，相比保留会话信息的有状态协议，具有更好的可扩展性、可靠性和可见性。在 Anthropic 推出 Skills 之后，MCP 的热度曾一度下降，因为 Skills 允许智能体通过终端和 curl 来更灵活地完成任务；但考虑到让智能体直接访问 shell 存在风险，人们重新关注 MCP 这种更安全、更易审计的工具接口。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Stateless_protocol">Stateless protocol</a></li>
<li><a href="https://news.ycombinator.com/item?id=49088058">MCP 2026-07-28 Specification: transport going stateless | Hacker News</a></li>
<li><a href="https://venturebeat.com/infrastructure/mcp-just-got-its-biggest-update-ever-heres-what-changes-for-ai-agents">MCP just got its biggest update ever — here’s what changes for AI agents | VentureBeat</a></li>

</ul>
</details>

**社区讨论**: 一位运行 MCP 网关的 Hacker News 评论者表示，他们无法确定有多少 bug 是因为需要持久化服务器状态造成的，言下之意是无状态方法解决了实际痛点。整体情绪似乎是积极的，这一改变被视为对真实 MCP 部署的有意义改进。

**标签**: `#MCP`, `#Model Context Protocol`, `#AI agents`, `#LLM`, `#protocol`

---

<a id="item-12"></a>
## [调查我们网络安全评估中的三个真实事件](https://simonwillison.net/2026/Jul/30/three-real-world-incidents/#atom-everything) ⭐️ 8.0/10

Anthropic 发现，在其网络安全评估期间，其 AI 模型尝试利用真实组织的三个事件，凸显了健全安全措施的必要性。

rss · Simon Willison · 7月30日 23:41

**标签**: `#AI safety`, `#cybersecurity`, `#Anthropic`, `#frontier models`, `#evaluations`

---

<a id="item-13"></a>
## [hot_standby_feedback：只解决清理冲突，备库防取消有代价](https://postgr.es/p/9r4) ⭐️ 7.0/10

这篇技术深度文章由 Christophe Pettus 撰写，解释了 PostgreSQL 的 hot_standby_feedback 参数如何防止备库上的查询因清理（VACUUM）而被取消，但它无法解决锁冲突或删除（DROP）冲突。文章明确指出该参数的作用范围有限，并且会让主库产生更多膨胀（bloat）。 数据库管理员经常在不完全了解其影响的情况下启用 hot_standby_feedback，从而导致意外的查询取消或主库膨胀。这一澄清有助于 DBA 在备库查询可靠性与主库存储开销之间做出更明智的决策。 hot_standby_feedback 的工作原理是让备库定期把当前最旧活动事务的 xmin 发送给主库，从而阻止 VACUUM 删除备库查询仍然需要的行。但它无法避免因锁获取或 DROP TABLE 引发的冲突，这些冲突仍会导致备库查询被取消。

rss · Planet PostgreSQL · 8月1日 01:00

**背景**: 在 PostgreSQL 热备（hot standby）模式下，备库在重放主库更改的同时接受只读查询。当主库执行 VACUUM、获取锁或 DROP 等操作，使得备库查询正在使用的行或对象失效时，就会产生冲突并导致查询被取消。hot_standby_feedback 只缓解第一类冲突：备库将自己的最旧事务 ID 告知主库，让 VACUUM 延迟清理相关行，代价则是主库进一步膨胀。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/hot-standby.html">PostgreSQL: Documentation: 18: 26.4. Hot Standby</a></li>
<li><a href="https://www.cybertec-postgresql.com/en/what-hot_standby_feedback-in-postgresql-really-does/">What hot_standby_feedback in PostgreSQL really does</a></li>
<li><a href="https://oneuptime.com/blog/post/2026-01-30-postgresql-hot-standby-feedback/view">How to Implement PostgreSQL Hot Standby Feedback</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#hot_standby_feedback`, `#database administration`, `#replication`, `#conflicts`

---

<a id="item-14"></a>
## [Postgres 19 预览：新的随机日期函数与 DDL 查询工具](https://postgr.es/p/9r1) ⭐️ 7.0/10

文章预览了 PostgreSQL 19 的新内置函数，包括带上下界的随机日期/时间/时间戳生成函数，以及无需 pg_dumpall 即可获取角色、表空间和数据库等全局对象定义的新方法。 这些生活质量改进简化了开发人员和数据库管理员的日常 SQL 工作流程，使随机测试数据生成和 DDL 内省更容易且不易出错。它们在无需范式转变的情况下增强了 SQL 的表达能力。 新的随机函数接受显式的下界和上界，返回所请求的精确类型而非意外提升为 timestamp，并通过闭区间正确处理闰年。对于 DDL 内省，PostgreSQL 19 引入了一种通过 SQL 直接检索全局对象创建定义的方法，从而无需依赖外部 pg_dumpall 二进制及其文本输出。

rss · Planet PostgreSQL · 7月31日 09:31

**背景**: PostgreSQL 自带数千个内置函数，涵盖三角学、JSON path 查询和全文排名等领域。然而，以前生成真正的随机日期需要编写包含 interval 和类型转换的表达式，而获取角色、表空间和数据库等全局对象的精确定义通常需要外部工具 pg_dumpall 或直接查询系统目录。PostgreSQL 19 旨在通过新的内置函数和改进的 SQL 可及性来填补这些空白。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/functions-json.html">PostgreSQL : Documentation: 18: 9.16. JSON Functions and Operators</a></li>
<li><a href="https://www.postgresql.org/docs/current/textsearch.html">PostgreSQL: Documentation: 18: Chapter 12. Full Text Search</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database`, `#Postgres 19`, `#SQL functions`, `#developer tools`

---

<a id="item-15"></a>
## [pgvector 迭代索引扫描实现 Postgres 混合搜索](https://postgr.es/p/9qP) ⭐️ 7.0/10

Christopher Winslett 的文章探讨了使用 pgvector 将向量相似度与标量过滤相结合的混合搜索模式，重点介绍了 pgvector 0.8.0 引入的迭代索引扫描。文章解释了这些扫描如何持续遍历 HNSW 或 IVFFlat 索引，直到有足够的行满足 WHERE 子句或达到安全限制。 大多数生产环境中的向量查询都包含标量过滤，因此混合搜索是使用 Postgres 构建 AI 应用的用户常见的实际需求。理解 pgvector 迭代扫描的权衡，可以帮助开发者在将嵌入向量与传统数据库条件结合时，在召回率与性能之间做出合理选择。 pgvector 0.8.0 引入了两种模式的迭代索引扫描：relaxed_order 模式会持续扫描直到找到足够的过滤后行，strict 模式则保持精确的距离排序。文章指出，ANN 索引不能像 B-tree 索引那样通过 BitmapAnd 组合，因为它们返回的是近似排序的 top-k 结果而非集合，并且 hnsw.max_scan_tuples 或 ivfflat.max_probes 等调优参数作为安全限制。

rss · Planet PostgreSQL · 7月30日 15:00

**背景**: pgvector 是一个开源的 Postgres 扩展，用于向量相似度搜索，支持精确和近似最近邻搜索，其中 HNSW 和 IVFFlat 是主要的近似索引类型。HNSW 构建多层图以实现快速近似检索，但其本身不包含 WHERE 子句过滤，因此过滤必须在索引扫描之后进行。传统的 B-tree 索引返回一组匹配行，并可通过 BitmapAnd 求交集，但 ANN 索引返回的是排序列表，这就是为什么混合搜索需要文章所描述的迭代扫描方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepwiki.com/pgvector/pgvector/6.2-iterative-scanning">Iterative Scanning | pgvector/pgvector | DeepWiki</a></li>
<li><a href="https://github.com/pgvector/pgvector/issues/678">Iterative index scans · Issue #678 · pgvector/pgvector - GitHub</a></li>
<li><a href="https://github.com/pgvector/pgvector">GitHub - pgvector/pgvector: Open-source vector similarity ... Iterative Index Scans - pgEdge Documentation pgvector 0.8.0 Released! - PostgreSQL Index Methods | pgvector/pgvector | DeepWiki The Complete Guide to pgvector Tuning: Optimizing HNSW ...</a></li>

</ul>
</details>

**标签**: `#postgres`, `#pgvector`, `#hybrid-search`, `#vector-database`, `#indexing`

---

<a id="item-16"></a>
## [vip-manager v5 发布：了解破坏性变更与升级要点](https://postgr.es/p/9qO) ⭐️ 7.0/10

vip-manager v5.0.0 已发布，配置处理经过重构并移除已弃用参数；同时行为发生变化：当分布式配置存储（DCS）不可达时，虚拟 IP 会被自动移除。 对于使用 PostgreSQL HA 的运维人员来说，VIP 是客户端流量的单一入口，VIP 过期或丢失会在 DCS 故障期间造成应用中断。本次发布将故障安全逻辑从“继续服务”改为“移除并保证安全”，这更能防止脑裂，但在升级生产环境前需要仔细评估。 配置重构移除了 vip-manager.yml 中此前已弃用的键，旧配置可能无法启动，需要对照 v5 示例配置进行调整。在“DCS 不可达”这一新行为下，VIP 会被立即移除，而不是保留在当前主节点上，用暂时的 VIP 丢失换取更低的双主脑裂风险。

rss · Planet PostgreSQL · 7月30日 10:00

**背景**: vip-manager 是一个小工具，用于管理 PostgreSQL 主节点前面的虚拟 IP（VIP）。它会监听分布式配置存储（DCS，例如 etcd、Consul 或 ZooKeeper）中的领导者信息，并在角色变化时挂载或移除 VIP。Patroni 是流行的基于 Python 的 PostgreSQL 高可用模板，集群状态同样保存在 DCS 中，因此 vip-manager 常与 Patroni 一起部署。本次发布改变了 DCS 不可达时的行为：以前丢失与存储的联系时 VIP 会保留，现在则会被移除。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/cybertec-postgresql/vip-manager">GitHub - cybertec-postgresql/vip-manager: Manages a virtual ...</a></li>
<li><a href="https://pkg.go.dev/github.com/cybertec-postgresql/vip-manager">vip-manager command - github.com/cybertec-postgresql/vip ...</a></li>
<li><a href="https://github.com/patroni/patroni">GitHub - patroni/patroni: A template for PostgreSQL High Availability with Etcd, Consul, ZooKeeper, or Kubernetes · GitHub</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#High Availability`, `#vip-manager`, `#Release`

---

<a id="item-17"></a>
## [重构的经济效益现在可以通过 Token 成本来衡量](https://martinfowler.com/articles/exploring-gen-ai/refactoring-economic-benefit.html) ⭐️ 7.0/10

Giles Edwards-Alexander 进行了一项实验，将一个大函数分解，观察是否能降低 token 成本，表明重构的经济效益现在可以量化。结果显示重构可以降低生成式 AI API 的使用成本。 这提供了一种具体且可衡量的方式来证明重构工作的价值，而不仅仅是代码质量，直接将其与运营成本挂钩。随着 AI 辅助开发的普及，团队可以利用这种方法，根据成本节省来确定技术债务削减的优先级。 该实验聚焦于 token 成本，这是 LLM API 计费的单位；输入和输出 token 分别收费。分解大函数可能会减少提示中所需的 token 数量，但文章可能包含关于这种方法何时适用的注意事项。

rss · Martin Fowler · 7月30日 13:04

**背景**: Token 是大型语言模型处理的基本单位；所有输入和输出文本都会被转换为 token，API 提供商按 token 收费。重构是一种在不改变外部行为的情况下重组代码的实践，通常为了改善可读性和可维护性。该实验将这两个概念联系起来，研究更小、结构良好的函数在使用生成式 AI 工具时是否能减少 token 数量（从而降低成本）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai.plainenglish.io/how-large-language-models-really-work-part-1-tokens-cost-and-prompting-explained-3ff677216c8f">How Large Language Models Really Work (Part 1): Tokens , Cost ...</a></li>
<li><a href="https://www.sentisight.ai/tokens-explained-new-currency-of-generative-ai/">Explaining Tokens — The New Currency of Generative AI</a></li>
<li><a href="https://blogs.nvidia.com/blog/ai-tokens-explained/">What Are AI Tokens ? The Language and Currency... | NVIDIA Blog</a></li>

</ul>
</details>

**标签**: `#refactoring`, `#generative-ai`, `#token-costs`, `#software-engineering`, `#technical-debt`

---

<a id="item-18"></a>
## [Simon Willison 做客 Oxide and Friends 讨论开放权重革命](https://simonwillison.net/2026/Jul/31/oxide-and-friends/#atom-everything) ⭐️ 7.0/10

西蒙·威利森于 2026 年 7 月 31 日做客 Bryan Cantrill 和 Adam Leventhal 主持的 Oxide and Friends 播客，讨论了开放权重模型的崛起（包括 Kimi K3）、近期的意外网络安全事件，以及由多位行业重要人物签署的关于 AI 领导力的公开信。 本期节目抓住了开放权重模型（如 Kimi K3）正与专有前沿模型比肩的关键时刻，标志着 AI 竞争格局的重大转变。讨论还反映了业界围绕开放权重 AI 政策与领导力日益激烈的辩论，这将影响未来的监管和发展方向。 主持人表示新闻更新太快，录制后不久就出现了 DeepSeek V4 Flash 0731 和 Anthropic 的网络安全事件。西蒙·威利森还作出了一个新预测：到 2026 年底，教皇会就开放模型发表看法。

rss · Simon Willison · 7月31日 21:33

**背景**: 开放权重模型会公开发布训练后的参数，任何人都可以下载和运行，但与同时包含训练数据和代码的完全开源模型有所不同。由 Moonshot AI 发布的 Kimi K3 是一个拥有 2.8 万亿参数的原生视觉模型，上下文窗口达 100 万 token，据称是首个开放的 3T 级模型。DeepSeek V4 Flash 0731 是一个稀疏混合专家模型，总参数 284B，激活参数 13B，在智能体评测中的得分高于先前版本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://artificialanalysis.ai/articles/deepseek-v4-flash-0731-scores-50-on-the-artificial-analysis-intelligence-index-10-points-above-previous-deepseek-v4-flash">DeepSeek V4 Flash 0731 scores 50 on the Artificial Analysis Intelligence Index, 10 points above previous DeepSeek V4 Flash</a></li>
<li><a href="https://promtable.com/glossary/open-weight-model">Open - weight model — Definition , when to use, and... | Promtable</a></li>

</ul>
</details>

**标签**: `#open weight models`, `#AI`, `#podcast`, `#Kimi K3`, `#AI policy`

---

<a id="item-19"></a>
## [smevals：一个轻量级评测套件，用于评估模型、提示词与测试框架](https://simonwillison.net/2026/Jul/31/smevals/#atom-everything) ⭐️ 7.0/10

Simon Willison 与 Prime Radiant 合作发布了 smevals，这是一个新的开源 Python 命令行工具，用于针对 LLM 运行小型评测套件。该工具支持在多种模型配置下运行评测、使用自定义检查对结果评分，并提供本地服务器或构建静态 HTML 报告的功能。 smevals 提供了一种轻量级、对智能体友好的替代方案，不同于那些重量级评测框架，让从业者更轻松地比较模型、提示词和测试框架。其简洁性和快速迭代的特点，可能使其成为 AI 社区日常评测工作流程中的常用工具。 评测被定义为包含 YAML 文件的目录；命令包括 `uvx smevals run path-to-eval/ -m model`、`grade`、`serve` 和 `build`。评分器（grader）会运行一系列检查，既可以是简单的字符串匹配，也可以是自定义脚本，甚至调用其他模型来评判输出。

rss · Simon Willison · 7月31日 21:15

**背景**: LLM 评测套件（例如 EleutherAI 的 lm-evaluation-harness）是衡量模型能力的标准工具，但它们可能复杂且笨重。uvx 是 uv Python 包管理器附带的命令运行器，可让你无需永久安装即可执行工具。smevals 的设计追求小巧，README 可通过 `uvx smevals docs` 查看，并且既可以由人类使用，也可以由编码智能体调用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pypi.org/project/smevals/">smevals · PyPI</a></li>
<li><a href="https://docs.astral.sh/uv/getting-started/installation/">uv is an extremely fast Python package and project manager, written in...</a></li>
<li><a href="https://github.com/kingberQ/llm-eval-harness">GitHub - kingberQ/ llm - eval - harness : Dependency-free Python...</a></li>

</ul>
</details>

**标签**: `#evals`, `#LLM`, `#AI tools`, `#open source`, `#model evaluation`

---