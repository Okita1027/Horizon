---
layout: default
title: "Horizon 日报：2026-07-25 (ZH)"
date: 2026-07-25
lang: zh
---

> 从 41 条内容中筛选出 9 条重要资讯。

---

1. [Anthropic 发布 Claude Opus 5，无数据保留要求](#item-1) ⭐️ 9.0/10
2. [英伟达、微软、Meta 呼吁谨慎监管开放权重 AI](#item-2) ⭐️ 9.0/10
3. [伊朗革命卫队声称摧毁亚马逊巴林数据中心](#item-3) ⭐️ 9.0/10
4. [Postgres LISTEN/NOTIFY 通过合理配置可扩展至每秒 6 万次](#item-4) ⭐️ 8.0/10
5. [Claude Opus 5 登顶 AI 智能排行榜](#item-5) ⭐️ 8.0/10
6. [Opus 5 声称拥有最佳的提示注入抵抗力](#item-6) ⭐️ 8.0/10
7. [PyPI 阻止旧版本上传以防止投毒攻击](#item-7) ⭐️ 8.0/10
8. [Christophe Pettus 详解 PostgreSQL full_page_writes](#item-8) ⭐️ 7.0/10
9. [警告：关闭 fsync 可能导致不可恢复的数据损坏](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Anthropic 发布 Claude Opus 5，无数据保留要求](https://www.anthropic.com/news/claude-opus-5) ⭐️ 9.0/10

Anthropic 于 2026 年 7 月 24 日发布了其新旗舰 AI 模型 Claude Opus 5，在编码和知识工作基准测试中取得了最先进的成绩，并取消了通用 API 访问的数据保留要求。 Claude Opus 5 提供了与更昂贵的 Claude Fable 5 相当的尖端智能，价格却便宜约一半，使得先进 AI 更加普及；同时其零数据保留政策对企业及注重隐私的用户是一大优势。 Opus 5 在 Frontier-Bench v0.1 上得分为 43.3%，在 ARC-AGI-3 上得分为 30.2%，约为次优模型的三倍。与 Claude Fable 5 不同，它对通用访问没有数据保留要求，这是敏感应用的关键差异化因素。

hackernews · alvis · 7月24日 16:57 · [社区讨论](https://news.ycombinator.com/item?id=49038433)

**背景**: Claude Opus 模型是 Anthropic 能力最强且最昂贵的产品线。系统卡是部署前的安全披露文件，记录了对模型的评估、风险及缓解措施。零数据保留（ZDR）意味着提示和完成内容在 API 调用生命周期后不再存储，该功能通常需要企业协议，并对受监管行业的合规性至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/system-cards">Model system cards \ Anthropic</a></li>
<li><a href="https://aitoolsreview.co.uk/insights/claude-opus-5">Claude Opus 5: Benchmarks, System Card & Review (July 2026)</a></li>
<li><a href="https://decagon.ai/glossary/what-is-zero-data-retention-ai">What is Zero Data Retention AI? Definition & Vendor Guide | Decagon</a></li>

</ul>
</details>

**社区讨论**: 社区成员称赞无数据保留这一特性，称其为主要卖点。但早期测试结果不一：有用户发现 Opus 5 在图像转 HTML 任务上比 Fable 更准确，而另一用户报告在 C/C++ 代码审查中出现误报，并指出 GPT-5.6-sol 纠正了这些错误。还有评论指出，模型变体的激增正在推动模型路由服务的增长。

**标签**: `#AI`, `#LLM`, `#Claude`, `#Anthropic`, `#machine learning`

---

<a id="item-2"></a>
## [英伟达、微软、Meta 呼吁谨慎监管开放权重 AI](https://www.cnbc.com/2026/07/24/nvidia-microsoft-meta-open-weight-ai-models.html) ⭐️ 9.0/10

英伟达、微软和 Meta 于 2026 年 7 月 24 日联合发布公开信，警告不要过度监管开放权重 AI 模型，认为这可能削弱美国在 AI 领域的领导地位。 这一警告凸显了硅谷在 AI 监管问题上的分歧日益加剧，开放权重支持者与 OpenAI、Anthropic 等闭源倡导者形成对立。结果可能影响创新、安全与全球竞争力之间的平衡。 该信函明确反对限制开放权重模型的呼声，这类模型允许用户下载并在本地运行 AI，信中强调其在促进创新和透明度方面的作用。

hackernews · louiereederson · 7月24日 13:32 · [社区讨论](https://news.ycombinator.com/item?id=49035303)

**背景**: 开放权重模型发布训练后的神经网络权重，允许任何人运行、微调或审计模型，但并非完全开源，因为训练数据和代码可能不公开。随着 DeepSeek 等中国开放权重模型获得关注，美国一些公司推动以国家安全为由进行限制，这场辩论随之激化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>
<li><a href="https://www.ai21.com/glossary/foundational-llm/open-weights-model/">What is an Open-Weights Model? | AI21</a></li>

</ul>
</details>

**社区讨论**: Hacker News 评论者大多支持开放权重的立场，批评 Anthropic 涉嫌资助监管努力，并指出闭源模型被标榜为更安全的讽刺之处。一些人将此事比作 SOPA 抗议，认为开源社区正在动员反对过度监管。

**标签**: `#AI regulation`, `#open-weight models`, `#big tech`, `#policy`, `#open source`

---

<a id="item-3"></a>
## [伊朗革命卫队声称摧毁亚马逊巴林数据中心](https://houseofsaud.com/irgc-claims-destroyed-amazon-bahrain-data-center/) ⭐️ 9.0/10

伊朗伊斯兰革命卫队声称对亚马逊云服务巴林数据中心的摧毁负责，导致整个 me-south-1 区域在 2026 年 7 月下旬离线。 这一事件暴露了集中式云基础设施的地缘政治脆弱性，可能迫使企业重新考虑对单一区域的依赖，尤其是在冲突频发地区。 AWS 区域通常由至少三个相距数公里的数据中心组成；摧毁整个 me-south-1 区域意味着要么是多次协同攻击，要么是一次针对关键电力基础设施的打击。

hackernews · thisislife2 · 7月24日 09:52 · [社区讨论](https://news.ycombinator.com/item?id=49033240)

**背景**: AWS 区域由多个可用区组成，每个可用区包含一个或多个具有独立电源、冷却和网络的数据中心。巴林区域 (me-south-1) 是 AWS 在波斯湾唯一的区域，服务于中东各地的客户。该地区的地缘政治紧张局势长期以来一直引发对云基础设施弹性的担忧。

**社区讨论**: 评论者指出，中东唯一仍在运营的 AWS 区域是特拉维夫，而阿联酋已宕机数月，沙特阿拉伯仍在建设中，这颇具讽刺意味。一些人强调了集中式基础设施对和平稳定的依赖，另一些人则质疑一次打击能否瘫痪整个区域，或者是否需要多次协同攻击。

**标签**: `#AWS`, `#data center`, `#security`, `#geopolitics`, `#cloud infrastructure`

---

<a id="item-4"></a>
## [Postgres LISTEN/NOTIFY 通过合理配置可扩展至每秒 6 万次](https://www.dbos.dev/blog/postgres-listen-notify-scalability) ⭐️ 8.0/10

一篇详细的技术文章证明，通过适当调优，PostgreSQL 的 LISTEN/NOTIFY 机制每秒可处理多达 6 万条通知，推翻了长期以来的“不可扩展”观点。 该发现具有重要意义，因为它挑战了数据库领域的普遍假设，可能扩展 LISTEN/NOTIFY 在高吞吐实时应用中的使用场景，并简化之前依赖外部消息队列的架构。 文章指出性能瓶颈往往源于配置不当而非 LISTEN/NOTIFY 本身的缺陷，并提供了具体策略，如连接池管理、高效负载大小以及避免多队列复用，以实现高吞吐量。

hackernews · KraftyOne · 7月24日 19:05 · [社区讨论](https://news.ycombinator.com/item?id=49040296)

**背景**: PostgreSQL 的 LISTEN/NOTIFY 功能允许客户端应用订阅指定频道，并在其他会话对该频道发出 NOTIFY 命令时接收异步通知。它常用于实时消息传递、缓存失效和构建轻量级消息队列。然而，由于性能问题的传闻，许多开发者认为它不适合生产环境。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/sql-notify.html">PostgreSQL: Documentation: 18: NOTIFY</a></li>
<li><a href="https://www.postgresql.org/docs/current/sql-listen.html">PostgreSQL: Documentation: 18: LISTEN</a></li>

</ul>
</details>

**社区讨论**: 社区讨论反映了细致入微的观点：一些评论者强调“扩展”是一个连续体，每秒 6 万次对许多应用足够但并非全部；另一些人则分享了将 LISTEN/NOTIFY 用作队列时遇到性能瓶颈的真实经验。讨论中还引用了一篇相关批评文章《Postgres LISTEN/NOTIFY 不可扩展》，表明该话题仍存在争议。

**标签**: `#postgres`, `#scalability`, `#databases`, `#notifications`

---

<a id="item-5"></a>
## [Claude Opus 5 登顶 AI 智能排行榜](https://artificialanalysis.ai/models) ⭐️ 8.0/10

Claude Opus 5（自适应推理，最大努力）以 61 分在 Artificial Analysis 智能排行榜上跃居第一，超越了 GPT-5.6 Sol 等其他顶级模型。 这一排名凸显了 Claude Opus 5 在 10 项具有挑战性的基准测试中的强劲表现，但关于其成本与可靠性权衡的争论突显了为实际应用选择模型的复杂性。 该排行榜使用 Artificial Analysis 智能指数 v4.0，聚合了数学、科学、编码、代理任务和推理等 10 项评估结果。Claude Opus 5 在最大努力模式下得分为 61，在高努力模式下与 GPT-5.6 Sol 持平（59 分），但 Opus 5 仍是最昂贵的模型之一，输入/输出分别为每百万 token $5/$25。

hackernews · aarondong · 7月24日 19:45 · [社区讨论](https://news.ycombinator.com/item?id=49040741)

**背景**: Artificial Analysis 智能排行榜基于综合指数对 AI 模型进行排名，涵盖智能、成本、速度等指标。Claude Opus 5 是 Anthropic 于 2026 年 7 月 24 日发布的前沿模型，通过努力程度切换权提供了成本与能力之间的权衡。该排行榜旨在提供超越单一基准的整体视图，但用户对 Claude 的审查和可靠性表示担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/leaderboards/models">LLM Leaderboard - Comparison of AI models from OpenAI ...</a></li>
<li><a href="https://www.datalearner.com/en/leaderboards/external/aa-quality-index">Artificial Analysis Intelligence Index - AI Model Leaderboard ...</a></li>
<li><a href="https://codersera.com/blog/claude-opus-5-launch-guide-2026/">Claude Opus 5: Benchmarks, Pricing & Comparison (2026)</a></li>

</ul>
</details>

**社区讨论**: 社区评论反应不一：一些用户称赞 Opus 5 的高分，但批评其严厉的审查和高成本，认为可靠性比排行榜上的几分更重要。其他人指出 GPT-5.6 和 Kimi K3 以一半的成本获得了相近的分数，并且 AA-Omniscience 指数揭示了知识可靠性的差异。总体情绪谨慎乐观，但对实际可用性仍有较大保留。

**标签**: `#AI`, `#LLM benchmark`, `#Claude Opus 5`, `#model comparison`, `#cost efficiency`

---

<a id="item-6"></a>
## [Opus 5 声称拥有最佳的提示注入抵抗力](https://simonwillison.net/2026/Jul/25/boris-cherny/#atom-everything) ⭐️ 8.0/10

Anthropic 团队成员 Boris Cherny 在 Twitter 上表示，根据系统卡和红队评估，Opus 5 是 Anthropic 目前最不易受提示注入攻击的模型。 提示注入是大语言模型中的一个关键安全漏洞，因此提高抵抗力直接增强了 AI 系统的安全性和可靠性。这一说法将 Opus 5 定位为 AI 安全领域的重要进步，可能影响行业对模型鲁棒性的标准。 该声明基于 Claude Opus 5 系统卡中的发现，具体在第 73 页，涵盖了提示注入评估和红队测试结果。虽然引文中未详细说明具体分数，但 Cherny 强调 Opus 5 '非常难以成功进行提示注入'。

rss · Simon Willison · 7月25日 00:42

**背景**: 提示注入是一种攻击方式，恶意输入旨在覆盖 AI 模型的指令，导致意外行为。这是 LLM 的一个主要问题，尤其是那些具有浏览或文件上传功能的模型。红队测试是一种对抗性测试过程，用于在攻击者之前发现此类漏洞。Anthropic 的系统卡通常会披露安全评估结果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>
<li><a href="https://www.paloaltonetworks.com/cyberpedia/what-is-ai-red-teaming">What Is AI Red Teaming? Why You Need It and How to Implement - Palo Alto Networks</a></li>

</ul>
</details>

**标签**: `#prompt-injection`, `#anthropic`, `#claude`, `#generative-ai`, `#ai`

---

<a id="item-7"></a>
## [PyPI 阻止旧版本上传以防止投毒攻击](https://simonwillison.net/2026/Jul/23/seth-larson/#atom-everything) ⭐️ 8.0/10

自 2026 年 7 月 22 日起，PyPI 拒绝向超过 14 天的旧版本上传新文件。此更改旨在防止攻击者利用被盗的发布令牌篡改长期稳定的版本。 这一主动措施关闭了最近 TeamPCP 等事件中利用的关键供应链攻击途径。它确保一旦版本稳定，就无法通过令牌泄露被事后投毒，从而保护 Python 生态系统。 该限制适用于 PyPI 上的所有项目，并在服务器端强制执行。截至公告发布时，尚未发现针对该特定途径的已知滥用行为，但 PyPI 团队认为这是一种现实威胁。

rss · Simon Willison · 7月23日 04:50

**背景**: PyPI 是 Python 的官方第三方软件仓库，托管超过 50 万个包。最近的供应链攻击，例如 2026 年 3 月针对 LiteLLM 和 Telnyx 的 TeamPCP 活动，利用泄露的 CI/CD 令牌发布恶意版本的合法包。这项新的上传限制旨在通过将令牌滥用的窗口期限制为发布后的 14 天来防止此类攻击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.helpnetsecurity.com/2026/07/23/pypi-secures-package-releases/">PyPI hardens package security with new upload restrictions - Help Net Security</a></li>
<li><a href="https://securitylabs.datadoghq.com/articles/litellm-compromised-pypi-teampcp-supply-chain-campaign/">LiteLLM and Telnyx compromised on PyPI: Tracing the TeamPCP supply chain campaign | Datadog Security Labs</a></li>

</ul>
</details>

**标签**: `#python`, `#security`, `#supply-chain`, `#packaging`

---

<a id="item-8"></a>
## [Christophe Pettus 详解 PostgreSQL full_page_writes](https://postgr.es/p/9qq) ⭐️ 7.0/10

Christophe Pettus 发布了一篇博文，解释了为什么 PostgreSQL 在崩溃后会记录完整页面，并警告不要禁用 full_page_writes 设置。 这一点很重要，因为理解 full_page_writes 对于数据库可靠性和崩溃后的数据完整性至关重要，禁用它会导致静默损坏。 默认开启的 full_page_writes 设置会在检查点后将整个页面写入 WAL，以防止崩溃期间部分写入导致的页面撕裂。

rss · Planet PostgreSQL · 7月25日 01:00

**背景**: PostgreSQL 使用预写日志 (WAL) 进行崩溃恢复。如果在写入过程中发生系统崩溃，部分页面写入可能会损坏数据库。full_page_writes 确保记录整个页面，以便恢复时能完整还原。禁用它可提高性能，但存在无法恢复的损坏风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wiki.postgresql.org/wiki/Full_page_writes">Full page writes - PostgreSQL wiki</a></li>
<li><a href="https://www.rockdata.net/tutorial/tune-full-page-writes/">PostgreSQL Tutorial: The Impact of Full Page Writes</a></li>
<li><a href="https://postgresqlco.nf/doc/en/param/full_page_writes/">PostgreSQL Documentation: full _ page _ writes parameter</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database reliability`, `#configuration`, `#crash recovery`

---

<a id="item-9"></a>
## [警告：关闭 fsync 可能导致不可恢复的数据损坏](https://postgr.es/p/9qo) ⭐️ 7.0/10

PostgreSQL 专家 Christophe Pettus 警告，将 fsync 配置参数设为 off 是 postgresql.conf 中最危险的设置，会导致不可恢复的数据损坏，而不仅仅是糟糕的查询计划。 这一警告对所有 PostgreSQL DBA 至关重要，因为错误的 fsync 设置可能悄然损坏数据，导致无法恢复，并可能造成灾难性的数据丢失。 fsync 参数默认为 on，强制将预写日志（WAL）写入同步到磁盘；关闭它会以牺牲持久性为代价换取微小的性能提升，但会使数据库在崩溃或断电时容易损坏。

rss · Planet PostgreSQL · 7月24日 01:00

**背景**: GUC 是 Grand Unified Configuration（大统一配置）的缩写，是 PostgreSQL 处理服务器配置参数的子系统。fsync 参数控制 PostgreSQL 是否使用 fsync()等系统调用确保数据物理写入磁盘。历史上的“fsyncgate”等事件表明，忽略 fsync 故障可能导致静默损坏。PostgreSQL 的 WAL 默认通过缓冲 I/O 写入，这使得 fsync 对持久性至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/acronyms.html">PostgreSQL: Documentation: 18: Appendix L. Acronyms</a></li>
<li><a href="https://postgresqlco.nf/doc/en/param/fsync/">PostgreSQL Documentation: fsync parameter</a></li>
<li><a href="https://danluu.com/fsyncgate/">Fsyncgate: errors on fsync are unrecovarable</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database`, `#fsync`, `#data integrity`, `#configuration`

---