---
layout: default
title: "Horizon 日报：2026-08-02 (ZH)"
date: 2026-08-02
lang: zh
---

> 从 40 条内容中筛选出 13 条重要资讯。

---

1. [无状态 MCP 重新引起了我的兴趣（并启发了 mcp-explorer 和 datasette-mcp）](#item-1) ⭐️ 9.0/10
2. [Seedance 2.5](#item-2) ⭐️ 8.0/10
3. [Diátaxis：将技术文档分为四类的文档框架](#item-3) ⭐️ 8.0/10
4. [Lean 内核健全性漏洞 #14576 的事后分析](#item-4) ⭐️ 8.0/10
5. [谷歌如何加速了 RSS 订阅的衰落](#item-5) ⭐️ 8.0/10
6. [NetBSD 11.0 发布：更快的虚拟化与防火墙改进](#item-6) ⭐️ 8.0/10
7. [PostgreSQL 19 将新增 SQL 属性图查询（SQL/PGQ）](#item-7) ⭐️ 8.0/10
8. [DeepSeek 发布 V4 Flash：304B 参数模型，智能体能力显著增强](#item-8) ⭐️ 8.0/10
9. [Simon Willison 在 Oxide and Friends 播客探讨开源权重 AI 革命](#item-9) ⭐️ 8.0/10
10. [Christophe Pettus：将所有 GUC 排成一行：hot_standby_feedback](#item-10) ⭐️ 7.0/10
11. [PostgreSQL 18 的 extension_control_path 让扩展可实现容器化部署](#item-11) ⭐️ 7.0/10
12. [开发者变“指挥家”：AI 重塑软件开发角色](#item-12) ⭐️ 7.0/10
13. [OpenAI 称 Astra 模型解决十个长期数学难题](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [无状态 MCP 重新引起了我的兴趣（并启发了 mcp-explorer 和 datasette-mcp）](https://simonwillison.net/2026/Jul/31/stateless-mcp/#atom-everything) ⭐️ 9.0/10

Simon Willison 讨论了无状态 MCP 更新（MCP 2.0）如何重新激发了他的兴趣，并促成了新工具 mcp-explorer 和 datasette-mcp 的诞生。

rss · Simon Willison · 7月31日 23:13

**标签**: `#MCP`, `#AI Agents`, `#Protocol`, `#Developer Tools`, `#Simon Willison`

---

<a id="item-2"></a>
## [Seedance 2.5](https://seed.bytedance.com/en/blog/one-take-creation-flexible-referencing-introducing-seedance-2-5) ⭐️ 8.0/10

字节跳动宣布 Seedance 2.5，一款高质量的 AI 视频生成模型，引发社区对其能力和市场方向的广泛讨论。

hackernews · njaremko · 8月1日 20:45 · [社区讨论](https://news.ycombinator.com/item?id=49138302)

**标签**: `#AI video generation`, `#ByteDance`, `#Seedance`, `#generative AI`, `#model release`

---

<a id="item-3"></a>
## [Diátaxis：将技术文档分为四类的文档框架](https://diataxis.fr/) ⭐️ 8.0/10

Diátaxis 文档框架在 Hacker News 上再次受到关注，其作者 Daniele Procida 宣布正在积极将该框架翻译成多种语言，并已提供进行中的翻译版本。 Diátaxis 为技术团队提供了一种实用且共享的文档分类方法，有助于提高文档的可发现性和一致性，已被 Canonical 等组织用于 Ubuntu 文档，进一步推动了以用户为中心的技术写作趋势。 该框架定义了四种内容类型：教程（面向学习）、操作指南（面向任务）、参考（面向信息）和解释（面向理解）。虽然每个页面通常应属于其中一个类别，但真实文档可能具有复杂的层级结构，Diátaxis 网站为此提供了专门讨论页面。

hackernews · ryanseys · 8月1日 20:33 · [社区讨论](https://news.ycombinator.com/item?id=49138188)

**背景**: Diátaxis 是由 Daniele Procida 创建的一个文档框架，它为技术文档规定了一种轻量、务实的结构，基于四种不同的内容类型。该框架旨在系统化地满足用户需求，使读者更容易在正确的时间找到正确的信息。它已在开发者文档社区中获得广泛关注，并被 Ubuntu 等知名项目采用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://diataxis.fr/">Diátaxis</a></li>
<li><a href="https://ubuntu.com/blog/diataxis-a-new-foundation-for-canonical-documentation">Diátaxis , a new foundation for Canonical documentation | Ubuntu</a></li>
<li><a href="https://blog.sequinstream.com/we-fixed-our-documentation-with-the-diataxis-framework/">We fixed our documentation with the Diátaxis framework</a></li>

</ul>
</details>

**社区讨论**: 评论者大多称赞 Diátaxis 明确了文档结构和写作口吻，并列举了在大型代码库交接和文档重构中的成功案例。作者在评论中介绍了多语言翻译项目；也有观点提醒不要将其奉为教条，还有人提到，让 LLM 遵循“diataxis”能方便地生成不错的初版文档。

**标签**: `#documentation`, `#technical-writing`, `#developer-experience`, `#framework`

---

<a id="item-4"></a>
## [Lean 内核健全性漏洞 #14576 的事后分析](https://leodemoura.github.io/blog/2026-8-1-postmortem-for-kernel-soundness-bug-14576/) ⭐️ 8.0/10

Leo de Moura 于 2026 年 8 月 1 日发布了 Lean 内核健全性漏洞 #14576 的事后剖析，该漏洞可让一个 False 的证明同时绕过 Lean 官方内核和独立的 nanoda 检查器。分析详细说明了技术根因，并解释了为何独立验证仍然有效，但用户需要同时更新两个检查器。 这很重要，因为证明助手内核的健全性漏洞会破坏形式化验证所依赖的基础信任。该事后剖析提供了一个具体例子，说明精心构造的证明甚至能绕过独立检查器，提醒我们验证结果应被视为极强但并非绝对可靠的保证。 该漏洞利用被精心构造以触发两个不同实现中的缺陷：一个是 Lean 内核的缺陷，另一个是独立检查器 nanoda 的缺陷，因此只有在两个工具都更新到修复版本后，独立内核检查才能继续保持健全。根本原因属于实现缺陷，而非 Lean 底层元理论的问题。

hackernews · juhopitk · 8月1日 18:32 · [社区讨论](https://news.ycombinator.com/item?id=49137060)

**背景**: 像 Lean 这样的证明助手依赖一个小的、受信任的内核来检查每个证明项是否有效；周围的自动化代码可能复杂且有缺陷，但内核本应保证健全性。健全性漏洞意味着内核接受了一个无效证明，甚至可能推导出 False，从而破坏系统的逻辑一致性。历史上，Coq、Isabelle、Agda 等证明助手都曾出现过健全性漏洞，因此这并非前所未有，但每次事件都会受到严肃对待。诸如 nanoda 之类的独立检查器被用作第二道防线，用另一套实现重新验证证明。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lawrencecpaulson.github.io/2026/07/30/Collatz.html">Why is it all in the kernel ?</a></li>
<li><a href="https://sourcefeed.dev/a/the-collatz-disproof-that-beat-two-proof-checkers-2">The Collatz 'Disproof' That Beat Two Proof Checkers — SourceFeed</a></li>
<li><a href="https://math-cs-compass.com/Mathematics/Discrete/formal_methods.html">Formal Methods: Machine- Verified Proof - MATH-CS COMPASS</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为这种漏洞虽然严重但属意料之中，指出所有证明助手都有健全性问题，验证结果是极强而非绝对的保证。也有人质疑复杂内核背后的理念，认为 Metamath 更简单的设计会更加可靠；还有人提出为证明 False 设置赏金以增强信任等想法。

**标签**: `#Lean`, `#formal verification`, `#soundness`, `#proof assistants`, `#security`

---

<a id="item-5"></a>
## [谷歌如何加速了 RSS 订阅的衰落](https://openrss.org/blog/how-google-helped-destroy-adoption-of-rss-feeds) ⭐️ 8.0/10

2023 年，openrss.org 发布了一篇分析文章，认为谷歌的一系列决策——尤其是 2013 年关闭 Google Reader——是 RSS 订阅采用率下降的重要原因。这篇文章引发了社区的热烈讨论，获得了 403 个点赞和 141 条评论。 这件事很重要，因为它展示了一个占主导地位的科技公司的战略选择如何重塑开放网络，并把用户推向集中式平台或'围墙花园'。这一分析回应了关于开放标准与企业控制生态系统之间持续存在的争论，并提醒人们：基础设施的决策会带来持久的文化和技术影响。 Google Reader 是一个免费的 RSS/Atom 聚合器，于 2013 年 7 月 1 日正式关闭；谷歌给出的理由是用户减少，但当时的批评者指出，谷歌同时在大力推广 Google+。RSS 本身仍然是一种轻量级、开放的基于 XML 的格式，几乎不会带来性能或资源成本；这篇文章认为，RSS 的衰落更多源于企业的激励机制，而非技术上的局限。

hackernews · pudgywalsh · 8月1日 18:07 · [社区讨论](https://news.ycombinator.com/item?id=49136821)

**背景**: RSS（Really Simple Syndication）是一种开放的 XML 格式，允许用户订阅网站的内容更新，并通过阅读器接收信息。Google Reader 于 2005 年推出，曾是最受欢迎的阅读器之一；它在 2013 年的关闭象征着开放、去中心化的内容分发逐渐让位于由算法驱动的社交媒体和移动应用。openrss.org 在 2023 年发表的这篇文章重新审视了这段历史，探讨谷歌在关闭 Reader 以及推广自家平台上的决策如何推动了这一转变。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Google_Reader">Google Reader - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/RSS">RSS - Wikipedia</a></li>
<li><a href="https://www.wired.com/2013/06/why-google-reader-got-the-ax/">Why Google Reader Really Got the Axe | WIRED</a></li>

</ul>
</details>

**社区讨论**: 评论者们表达了对 2000 年代初互联网的怀念，并对谷歌关闭 Reader 的理由表示沮丧；有评论称这个理由'明显是假的'，并指出谷歌当时在同时推广 Google+。也有人认为，像 Hacker News 这样中心化的社交网络最终仍会占据主导地位；还有评论者指出 RSS 至今仍被广泛支持，而且实现几乎不需要成本，因此呼吁网站继续提供 RSS 订阅。

**标签**: `#RSS`, `#Google`, `#Open Web`, `#Web History`, `#Technology`

---

<a id="item-6"></a>
## [NetBSD 11.0 发布：更快的虚拟化与防火墙改进](https://blog.netbsd.org/tnf/entry/netbsd_11_0_released) ⭐️ 8.0/10

NetBSD 11.0 已正式发布，带来了 npf 防火墙的重大改进、面向 x86 的新 MICROVM 内核（约 10 毫秒启动）以及 64 位 RISC-V 支持。该版本还扩展了 Linux 系统调用仿真。 这一重要版本巩固了 NetBSD 作为可移植、轻量级开源操作系统的地位，尤其是在虚拟化和嵌入式领域。它也重新引发了社区对 BSD 系统相对于 Linux 的相关性的思考。 新的 MICROVM 内核利用 PVH 启动和 VirtIO MMIO 实现极快的启动速度，而 npf 新增了二层以及用户/组过滤功能。该版本还引入了 64 位 RISC-V 移植，并扩展了 Linux 系统调用仿真。

hackernews · jaypatelani · 8月1日 17:56 · [社区讨论](https://news.ycombinator.com/item?id=49136736)

**背景**: NetBSD 是一款免费且高度可移植的类 Unix 操作系统，以支持众多硬件平台著称。11.0 是一个重大版本，此前的候选版本逐步加入了 64 位 RISC-V 支持等特性。其 npf 防火墙与 MICROVM 内核旨在提升虚拟化和网络环境下的性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.netbsd.org/releases/formal-11/NetBSD-11.0.html">Announcing NetBSD 11.0 RC7 (July 21, 2026)</a></li>
<li><a href="https://www.osnews.com/story/145663/netbsd-11-0-released/">NetBSD 11.0 released – OSnews</a></li>
<li><a href="https://news.tuxmachines.org/n/2026/02/09/NetBSD_11_0_RC1_available.shtml">Tux Machines — NetBSD 11 . 0 RC1 available!</a></li>

</ul>
</details>

**社区讨论**: 评论者总体持正面态度，赞赏 npf 二层过滤和约 10 毫秒的 MICROVM 启动。一位用户好奇 BSD 系统相对 Linux 的整体现状和发展势头，另一位则希望 AI 能帮助 BSD 这类小众系统成为实用的日常系统。还有人注意到发布说明中对未解决问题措辞的谦逊态度。

**标签**: `#NetBSD`, `#BSD`, `#Operating Systems`, `#Open Source`, `#Release`

---

<a id="item-7"></a>
## [PostgreSQL 19 将新增 SQL 属性图查询（SQL/PGQ）](https://postgr.es/p/9q_) ⭐️ 8.0/10

2026 年 3 月 16 日，Peter Eisentraut 向 PostgreSQL 19 提交了 SQL 属性图查询（SQL/PGQ）支持。该补丁新增了 GRAPH_TABLE 表函数、CREATE/ALTER/DROP PROPERTY GRAPH 命令，以及新的系统目录和信息模式视图。 这是让图查询成为主流关系数据库一等公民功能的重要一步。它遵循 ISO/IEC 9075-16:2023 标准，用户无需单独的图数据库即可执行标准化的图模式匹配。 该实现包含用于图模式匹配的 GRAPH_TABLE 表函数和属性图 DDL 命令。它还引入了多个新的系统目录和信息模式视图来管理属性图。

rss · Planet PostgreSQL · 7月31日 16:57

**背景**: 属性图数据模型由节点和边（关系）组成，节点和边都可以以键值对的形式拥有属性。SQL/PGQ 是 SQL:2023 标准（ISO/IEC 9075-16）的一部分，它将属性图的创建和查询直接在 SQL 中标准化，并借鉴了 Cypher 和 PGQL 等早期图查询语言。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blogs.oracle.com/database/property-graphs-in-oracle-database-23ai-the-sql-pgq-standard">Property Graphs in Oracle Database 23ai: The SQL / PGQ Standard</a></li>
<li><a href="https://en.wikipedia.org/wiki/Property_graph">Property graph - Wikipedia</a></li>
<li><a href="https://datasets.ldbcouncil.org/event/eighteenth-tuc-meeting/day1/6.+PGQ+Standard+final.pdf">The SQL / PGQ Standard : SQL</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#SQL/PGQ`, `#graph queries`, `#SQL standard`, `#database`

---

<a id="item-8"></a>
## [DeepSeek 发布 V4 Flash：304B 参数模型，智能体能力显著增强](https://simonwillison.net/2026/Jul/31/deepseek-v4-flash-0731/#atom-everything) ⭐️ 8.0/10

DeepSeek 发布了 DeepSeek-V4-Flash-0731，这是一个 304B 参数的模型，智能体（agentic）能力大幅增强。该模型定价为每百万输入 token 0.14 美元、每百万输出 token 0.27 美元，Artificial Analysis 将其排在 428B 参数的 MiniMax M3 之前。 这可能是目前市场上性价比最高的模型，每个任务的成本比同类竞品低一个数量级。它表明中国实验室继续压低大模型价格，同时保持有竞争力的基准测试表现。 该模型在 Hugging Face 上的大小为 167GB，可通过 OpenRouter 访问。独立测试显示，输出质量高度依赖推理强度：默认等级生成的鹈鹕图画质量较差，而将 reasoning_effort 设为 high 后结果明显更好。

rss · Simon Willison · 7月31日 23:59

**背景**: 智能体（agentic）能力指大语言模型进行推理、行动和交互的能力，使其能够自动化复杂流程并充当自主智能体。Artificial Analysis 智能指数（Intelligence Index）是一个综合基准分数，涵盖推理、知识、科学、编程和智能体任务，范围从 0 到 100。DeepSeek V4 系列属于高效开放权重模型浪潮的一部分，这些模型与规模更大的专有系统竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2503.23037">[2503.23037] Agentic Large Language Models, a survey</a></li>
<li><a href="https://artificialanalysis.ai/evaluations/artificial-analysis-intelligence-index">Artificial Analysis Intelligence Index | Artificial Analysis</a></li>

</ul>
</details>

**标签**: `#deepseek`, `#llm`, `#ai`, `#model-release`, `#machine-learning`

---

<a id="item-9"></a>
## [Simon Willison 在 Oxide and Friends 播客探讨开源权重 AI 革命](https://simonwillison.net/2026/Jul/31/oxide-and-friends/#atom-everything) ⭐️ 8.0/10

Simon Willison 与 Oxide and Friends 主持人 Bryan Cantrill 和 Adam Leventhal 一同探讨开源权重 AI 革命，话题涉及 Kimi K3 的前沿级性能、意外网络攻击事件，以及一份几乎获得所有主要 AI 公司（仅 Anthropic 除外）签署的行业公开信。该期节目还提到，录制后仅数天便出现了 DeepSeek V4 Flash 和 Anthropic 自身的网络事件。 本期节目凸显了 AI 行业的一个关键转折：开源权重模型正在与专有前沿系统正面竞争，这可能让最先进的 AI 技术更加普及，并重塑行业竞争格局。这份获得广泛签署的行业公开信表明，开放性已成为主流政策议题，各大玩家纷纷就其与 AI 领导力和安全性的关系表态。 Moonshot AI 的 Kimi K3 是一款 2.8 万亿参数的开源权重多模态模型，拥有 100 万 token 上下文窗口，在 OpenRouter 上输入价格为每百万 token 2.90 美元。节目还提到 DeepSeek V4 Flash——一款总参数 2840 亿、激活参数 130 亿的混合专家模型，并以新预测收尾：教皇将在年底前就开放模型发表评论。

rss · Simon Willison · 7月31日 21:33

**背景**: 开源权重模型是指公开已训练参数的 AI 系统，任何人都可以无限制地下载和使用，但通常不包含完整的训练流程。这类模型介于完全开源 AI 与封闭专有系统之间，让开发者得以基于前沿能力进行构建，同时也引发了关于安全与问责的讨论。随着 Kimi K3 和 DeepSeek V4 Flash 等模型的发布，它们已接近甚至追平领先封闭模型的性能，这场争论也随之升温。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-flash">DeepSeek V 4 Flash - API Pricing & Benchmarks | OpenRouter</a></li>

</ul>
</details>

**标签**: `#open weights`, `#AI`, `#podcast`, `#Simon Willison`, `#Kimi K3`

---

<a id="item-10"></a>
## [Christophe Pettus：将所有 GUC 排成一行：hot_standby_feedback](https://postgr.es/p/9r4) ⭐️ 7.0/10

解释了 hot_standby_feedback 如何防止清理冲突，但不能防止锁或删除冲突，用主库膨胀换取更少的备库查询取消。

rss · Planet PostgreSQL · 8月1日 01:00

**标签**: `#PostgreSQL`, `#hot_standby_feedback`, `#replication`, `#database administration`

---

<a id="item-11"></a>
## [PostgreSQL 18 的 extension_control_path 让扩展可实现容器化部署](https://postgr.es/p/9r0) ⭐️ 7.0/10

PostgreSQL 18 引入了新的 GUC 参数 extension_control_path，允许扩展的控制文件和 SQL 脚本存放在服务器目录之外。结合 dynamic_library_path，扩展就可以被打包成独立的 OCI 容器镜像并进行挂载。 该特性将扩展的版本管理和升级与 PostgreSQL 服务器镜像解耦，使多个集群可以共享一个精简且未修改的数据库镜像，同时独立更新像 pgvector 这样的扩展。不过，实际收益取决于扩展与服务器内部机制的耦合程度，因此并非所有扩展都适用。 extension_control_path 接受的是 sharedir 级别的路径，而不是扩展子目录的直接路径；同时 $system 占位符必须保留在路径中，否则服务器将无法访问自带的扩展。由于 PostgreSQL 的内部 ABI 在不同主版本间会变化，每个扩展镜像需要按主版本分别构建并打上对应标签，不能在 PG 17 和 PG 18 之间通用。

rss · Planet PostgreSQL · 7月31日 10:08

**背景**: 在 PostgreSQL 18 之前，dynamic_library_path 可以把共享库文件放到服务器目录之外，但扩展控制文件（.control）和 SQL 脚本必须位于服务器的 share 目录中。新的 extension_control_path GUC 弥补了这一缺口，与 Kubernetes 的 ImageVolume 或 Docker 的镜像挂载功能配合，可以将 OCI 镜像挂载到运行中的容器内。文章指出，容器边界只对与服务器启动序列、进程树或存储子系统耦合不深的扩展有实际帮助，而 PG 16/17 只能通过较为脆弱的 init 容器方式来实现类似效果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/message-id/E1tumbY-003Dl3-2o@gemulon.postgresql.org">PostgreSQL : pgsql: extension _ control _ path</a></li>
<li><a href="https://kubernetes.io/docs/tasks/configure-pod-container/image-volumes/">Use an Image Volume With a Pod | Kubernetes</a></li>
<li><a href="https://runebook.dev/en/docs/postgresql/runtime-config-client/GUC-EXTENSION-CONTROL-PATH">postgresql - The Twin Paths: extension _ control _ path and...</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#containers`, `#extensions`, `#database-administration`, `#Kubernetes`

---

<a id="item-12"></a>
## [开发者变“指挥家”：AI 重塑软件开发角色](https://martinfowler.com/rachels-ramblings/conductor-developer.html) ⭐️ 7.0/10

Martin Fowler 网站上的这篇文章认为，AI 在软件开发中的角色正从生产力工具转向“编排层”。优秀开发者如今并行协调多个 AI 代理，人类注意力成为软件交付流程中的新瓶颈。 这一重新定义很重要，因为它把焦点从“用 AI 写代码有多快”转向培养开发者的编排、评估和全局判断能力。当 AI 代理承担更多编码任务时，团队在招聘、培训和任务组织上都会受到影响。 作者指出，顶尖开发者通常并行运行 8 到 12 个 AI 代理，超过这个数量后，人本身就成了瓶颈。她把开发者比作管弦乐队的指挥，比如 Jacob Collier——不是亲自演奏每种乐器，而是塑造整体演出。

rss · Martin Fowler · 7月31日 13:48

**背景**: AI 编程助手已从自动补全工具发展为能独立生成和修改代码的自主代理。文章中提到的 FOSE（未来软件工程）活动一直在讨论当代理编写更多代码时如何保证设计质量。传统上，开发者依靠“深工作”和心流状态来编写软件；文章认为，这种状态正被并行编排多个工作流的持续管理所取代。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://conf.researchr.org/track/icse-2023/fose">ICSE 2023 - FoSE - Future of Software Engineering - ICSE 2023</a></li>
<li><a href="https://www.linkedin.com/pulse/ai-orchestrated-software-development-worksfor-once-connor-ms-cccm-9e7ec">AI Orchestrated Software Development That Works(For Once)</a></li>

</ul>
</details>

**标签**: `#AI`, `#software-development`, `#future-of-work`, `#DevOps`

---

<a id="item-13"></a>
## [OpenAI 称 Astra 模型解决十个长期数学难题](https://simonwillison.net/2026/Aug/1/ten-advances-in-mathematics/#atom-everything) ⭐️ 7.0/10

OpenAI 宣布其下一代主要模型 Astra 的内部版本解决了数学与理论计算机科学领域十个长期悬而未决的开放问题，按 GPT-5.6 Sol 的 token 价格计算，每个问题花费不到 2000 美元。 这意义重大，因为它提供了迄今较清晰的证据，表明前沿 AI 模型能够以极低成本产出可审计的研究成果，可能加速数学向人机协作模式的转变。它可能影响数学家、AI 研究者，以及将 AI 系统作为发现基础设施出售的新兴市场。 OpenAI 在 openai/ten-proofs 仓库中发布了 Lean 4 形式化证明、描述解决方案的论文，以及一份由 LLM 根据未公开推理轨迹重建证明过程的 PDF。然而，公司未披露具体使用的提示词，也未说明有多少问题尝试后未能解决。

rss · Simon Willison · 8月1日 20:34

**背景**: 这一公告紧跟在 Anthropic 的类似展示之后：其 Claude Mythos Preview 花费约 10 万美元的 token 成本发现了密码学弱点。陶哲轩曾将 AI 描述为“大数学”的催化剂，即未来大规模、去中心化的人机协作，由 AI 承担大部分技术性繁重工作。Lean 4 是一种交互式定理证明器，常用于对数学证明进行形式化验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://runtimewire.com/article/openai-astra-ten-open-math-problems">OpenAI says unreleased Astra model solved 10 open... - RuntimeWire</a></li>
<li><a href="https://scalevise.com/resources/openai-public-materials-no-astra-model/">OpenAI Public Materials Do Not List Astra</a></li>
<li><a href="https://openrouter.ai/openai/gpt-5.6-sol">GPT - 5 . 6 Sol - API Pricing & Benchmarks | OpenRouter</a></li>

</ul>
</details>

**标签**: `#AI`, `#mathematics`, `#OpenAI`, `#research`, `#theoretical computer science`

---