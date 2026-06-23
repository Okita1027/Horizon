---
layout: default
title: "Horizon 日报：2026-06-23 (ZH)"
date: 2026-06-23
lang: zh
---

> 从 40 条内容中筛选出 13 条重要资讯。

---

1. [Steam Machine 今日发布，采用反机器人预订系统](#item-1) ⭐️ 8.0/10
2. [社区讨论 Mythos 语言模型的能力，与 Fable 和 Opus 对比](#item-2) ⭐️ 8.0/10
3. [VibeThinker-3B：通过 SFT+GRPO，小模型推理能力超越 Opus 4.5](#item-3) ⭐️ 8.0/10
4. [OpenAI DayBreak：GPT-5.5-Cyber 用于网络安全，但访问受限引发争议](#item-4) ⭐️ 8.0/10
5. [警察局长滥用 Flock 技术跟踪女性，需搜查令](#item-5) ⭐️ 8.0/10
6. [提示注入即角色混淆研究](#item-6) ⭐️ 8.0/10
7. [将 Moebius 图像修复模型移植到浏览器中使用 WebGPU](#item-7) ⭐️ 8.0/10
8. [sqlite-utils 4.0rc1 增加迁移和嵌套事务功能](#item-8) ⭐️ 8.0/10
9. [模型没有偏好，只有上下文](#item-9) ⭐️ 7.0/10
10. [PostgreSQL enable_async_append GUC 详解](#item-10) ⭐️ 7.0/10
11. [PostgreSQL pg_stats：内部统计如何指导查询规划](#item-11) ⭐️ 7.0/10
12. [PostgreSQL 的 effective_io_concurrency 参数演变与影响](#item-12) ⭐️ 7.0/10
13. [Cloudflare 推出无需注册的临时账户用于部署](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Steam Machine 今日发布，采用反机器人预订系统](https://store.steampowered.com/news/group/45479024/view/685257114654870245) ⭐️ 8.0/10

Valve 于 2026 年 6 月 22 日正式推出 Steam Machine，其采用随机化预订系统，旨在防止机器人和黄牛，确保真实买家公平获取。 这标志着 Valve 重新进军专用游戏硬件领域，可能重塑客厅 PC 游戏市场。创新的预订系统可能为公平产品发布和打击倒卖树立新的行业标准。 Steam Machine 采用半定制 Zen 4 六核 CPU（30W TDP）和上一代显卡，价格基于组件成本。预订系统接受多天报名，无先到先得激励，然后随机化排序。

hackernews · theschwa · 6月22日 17:09 · [社区讨论](https://news.ycombinator.com/item?id=48632884)

**背景**: Steam Machine 是 Valve 专为客厅游戏设计的类主机 PC，运行 SteamOS。它延续了 Valve 2015 年未能成功的 Steam Machine 计划。新型号代号“Newell Nucleus”，强调开放性，允许用户安装其他操作系统或应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.lttlabs.com/articles/2026/06/22/the-newell-nucleus-steam-machine-ltt-companion-article">The Newell Nucleus: Steam Machine LTT Companion Article | LTT Labs</a></li>
<li><a href="https://en.wikipedia.org/wiki/Steam_Machine">Steam Machine - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者赞扬了反机器人预订系统以及 Valve 对开放性的承诺，称其“常识性”且“令人耳目一新”。有些注意到对价格和规格的讨论不足，而其他人则欣赏宣传视频中真实的游戏片段。

**标签**: `#steam-machine`, `#valve`, `#gaming-hardware`, `#pc-gaming`, `#hardware-launch`

---

<a id="item-2"></a>
## [社区讨论 Mythos 语言模型的能力，与 Fable 和 Opus 对比](https://swelljoe.com/post/will-it-mythos/) ⭐️ 8.0/10

社区正在积极讨论 Anthropic 的 Mythos 是否是一个称职的大型语言模型，用户分享了详细的使用体验，并与 Fable 和 Opus 等模型进行了比较。该讨论引发了高度关注，获得了 145 分和 85 条评论。 这一讨论反映了人们对前沿大语言模型性能和安全性权衡的极大关注，影响用户信任和模型采用。Mythos、Fable 和 Opus 之间的比较有助于开发者和研究人员了解模型在实际中的表现。 一些评论者认为 Mythos 可能是一个关闭了安全功能的普通大语言模型，其性能与那些不太愿意搜索漏洞的模型相当。另有用户指出 Fable 感觉像是更聪明的旧版 Opus，在后者被“阉割”之前。

hackernews · mindingnever · 6月23日 04:15 · [社区讨论](https://news.ycombinator.com/item?id=48640196)

**背景**: Mythos 是 Anthropic 开发的大型语言模型，虽然被训练为通用模型，但特别适用于网络安全任务。Fable 和 Opus 也是 Anthropic 的模型；Fable 曾被报道功能强大，但因其安全限制可能阻碍其他大语言模型开发而引发争议。大语言模型的安全功能是一个关键问题，模型通常被调整以避免生成有害内容，但这可能会限制其在某些任务（如漏洞检测）中的有效性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.pluralsight.com/resources/blog/ai-and-data/what-is-claude-mythos">What is Claude Mythos? | Pluralsight</a></li>
<li><a href="https://www.interconnects.ai/p/claude-fable-5-and-new-ai-safety">Claude Fable 5 and new AI safety fables - Interconnects AI</a></li>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1u23f8p/anthropics_new_model_fable_will_silently_handicap/">Anthropic's new model Fable will silently handicap work on LLMs [D]</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂：一些用户称赞 Fable 更强大，而另一些用户则感叹 Opus 在更新后性能下降。关于 Mythos 是否只是一个安全约束较少的模型存在争议，有人认为如果移除安全功能，当前模型也能有同样表现。评论者还强调了无偏基准测试的重要性，并建议在不让模型知道要查找什么的情况下进行任务评估。

**标签**: `#AI`, `#LLM`, `#model comparison`, `#safety`, `#performance`

---

<a id="item-3"></a>
## [VibeThinker-3B：通过 SFT+GRPO，小模型推理能力超越 Opus 4.5](https://arxiv.org/abs/2606.16140) ⭐️ 8.0/10

VibeThinker-3B 是一个拥有 3B 参数的小模型，通过结合监督微调（SFT）和 GRPO（一种强化学习算法）的新型训练方法，在 Python 编程任务上的推理能力超越了 Claude Opus 4.5。 这表明小模型在特定推理任务上可以与更大的最先进模型相媲美，可能降低计算成本并支持边缘设备部署。 该模型仅针对 Python 任务进行了评估，在其他语言上表现不佳，训练过程结合了 SFT 和 GRPO，GRPO 是一种在线强化学习算法，能够迭代提升推理能力。

hackernews · timhigins · 6月23日 02:01 · [社区讨论](https://news.ycombinator.com/item?id=48639240)

**背景**: GRPO 是一种强化学习算法，通过使用模型自身生成的数据进行迭代训练来提升推理能力。Opus 4.5 是 Anthropic 目前最智能的模型，在编码和推理方面表现出色。VibeThinker-3B 是一个紧凑的稠密模型，旨在探索小模型在可验证推理上的极限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ghost.oxen.ai/why-grpo-is-important-and-how-it-works/">Why GRPO is Important and How it Works - Oxen.ai</a></li>
<li><a href="https://www.anthropic.com/news/claude-opus-4-5">Introducing Claude Opus 4.5 \ Anthropic</a></li>
<li><a href="https://arxiv.org/abs/2606.16140">[2606.16140] VibeThinker-3B: Exploring the Frontier of ...</a></li>

</ul>
</details>

**社区讨论**: 评论者对结果持谨慎乐观态度，但指出仅限于 Python 的限制；一些人赞赏对小型模型和推理能力的关注，但另一些人质疑小模型是否能在通用智能方面真正匹配大型模型。

**标签**: `#AI`, `#machine learning`, `#reasoning`, `#small language models`, `#research`

---

<a id="item-4"></a>
## [OpenAI DayBreak：GPT-5.5-Cyber 用于网络安全，但访问受限引发争议](https://openai.com/index/daybreak-securing-the-world/) ⭐️ 8.0/10

OpenAI 发布了 DayBreak 网络安全计划，其中包含一个名为 GPT-5.5-Cyber 的专用模型，该模型在网络安全任务上的表现与 Anthropic 的 Mythos 模型相当甚至更好。该模型仅限向经过挑选的“网络防御者”开放，普通付费用户无法使用。 此次发布凸显了前沿 AI 模型在网络安全领域的专业化趋势，但访问限制引发了公平性和透明度的担忧。同时，这也凸显了 OpenAI 与 Anthropic 之间的竞争态势，尤其是在政府监管存在政治偏见的指控背景下。 据报道，GPT-5.5-Cyber 在 CyberGym 基准测试中优于 Mythos 5。该公告发布前几周，Anthropic 的类似模型据称因“安全原因”被政府叫停。Daybreak 计划还包括 Codex Security 和生态系统合作伙伴。

hackernews · AaronO · 6月23日 01:36 · [社区讨论](https://news.ycombinator.com/item?id=48639063)

**背景**: OpenAI 和 Anthropic 是领先的 AI 公司，开发大型语言模型。两者最近都发布了专门用于网络安全的模型：Anthropic 的 Mythos 和 OpenAI 的 GPT-5.5-Cyber。美国政府一直在审查先进 AI 模型的潜在风险，并采取了监管行动。Daybreak 是 OpenAI 的综合网络安全计划，整合了模型、工具和合作伙伴，以帮助防御者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reddit.com/r/singularity/comments/1ucvx1g/an_updated_gpt55_cyber_outperforms_mythos_5_in/">an updated GPT-5.5 Cyber outperforms Mythos 5 in CyberGym</a></li>
<li><a href="https://forums.theregister.com/forum/all/2026/05/01/openai_locks_gpt55cyber_behind_velvet/">OpenAI locks GPT-5.5-Cyber behind velvet rope despite slamming ...</a></li>
<li><a href="https://www.ciodive.com/news/OpenAI-Daybreak-cyber-threats/820036/">OpenAI launches Daybreak to combat cyber threats | CIO Dive</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了付费用户无法使用最佳模型来保护其代码的沮丧。一些用户质疑为什么 Anthropic 的 Mythos 被政府叫停而 OpenAI 的类似模型却被允许，暗示存在政治偏见。其他人要求对 Mythos 和 GPT-5.5-Cyber 进行基准比较。

**标签**: `#OpenAI`, `#GPT-5.5-Cyber`, `#AI security`, `#cybersecurity`, `#AI model release`

---

<a id="item-5"></a>
## [警察局长滥用 Flock 技术跟踪女性，需搜查令](https://ipvm.com/reports/police-chiefs-track) ⭐️ 8.0/10

一份报告揭露，多名警察局长利用 Flock Safety 的车牌自动识别摄像头跟踪他们正在约会或追求的女性，这清楚表明在没有搜查令的情况下滥用监控技术。 这一事件凸显了对执法部门使用的监控技术实行搜查令要求和严格监管的迫切需求，因为此类滥用行为破坏了公众信任和隐私权。 Flock Safety 每月在美国 49 个州的 5000 多个社区进行超过 200 亿次车辆扫描，其摄像头通常在没有明确防止跟踪等滥用行为的政策下安装。

hackernews · jhonovich · 6月22日 19:13 · [社区讨论](https://news.ycombinator.com/item?id=48634694)

**背景**: Flock Safety 提供自动车牌识别（ALPR）摄像头，捕捉车辆位置数据并与警方共享。该技术是更广泛的群众监控趋势的一部分，引发了隐私担忧。报告指出，虽然滥用行为很少见，但一旦发生，这是最常见的违法行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Flock_Safety">Flock Safety - Wikipedia</a></li>
<li><a href="https://www.cnet.com/home/security/when-flock-comes-to-town-why-cities-are-axing-the-controversial-surveillance-technology/">When Flock Surveillance Comes to Your Town: Everything to ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Automatic_license_plate_recognition">Automatic license plate recognition</a></li>

</ul>
</details>

**社区讨论**: 评论者强调需要对监控平台提高透明度并积极监督，并与执法记录仪录像相类比。有人指出滥用行为虽'罕见'却是最常见形式的讽刺意味，并警告不要与警察约会以防安全风险。

**标签**: `#surveillance`, `#privacy`, `#policing`, `#ethics`, `#warrants`

---

<a id="item-6"></a>
## [提示注入即角色混淆研究](https://simonwillison.net/2026/Jun/22/prompt-injection-as-role-confusion/#atom-everything) ⭐️ 8.0/10

研究人员 Charles Ye、Jasmine Cui 和 Dylan Hadfield-Menell 发表论文，证明 LLM 无法可靠区分特权文本（如 <system> 标签）与用户输入，并且模型更注重文本的风格而非实际内容，从而能够实现越狱攻击。 这项研究揭示了当前 LLM 安全架构中的根本性漏洞，表明除非模型实现真正的角色感知，否则提示注入可能是一个无法解决的问题，这对 AI 安全和部署具有重要影响。 研究发现，“去风格化”（destyling），即重写文本使其看起来不像预期的角色标签格式，可将平均攻击成功率从 61% 降至 10%，这一变化对人类几乎不可见，但对 LLM 影响巨大。

rss · Simon Willison · 6月22日 23:59

**背景**: 提示注入是一种网络安全攻击，通过精心设计的输入使 LLM 产生意外行为，绕过安全防护。角色标签如 <system>、<user> 和 <assistant> 最初是格式约定，但后来成为现代 LLM 的安全架构。这项研究表明，模型基于文本风格而非来源混淆这些角色，从而破坏了整个防御策略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>
<li><a href="https://role-confusion.github.io/">Prompt Injection as Role Confusion</a></li>

</ul>
</details>

**标签**: `#prompt injection`, `#LLM security`, `#role confusion`, `#AI safety`

---

<a id="item-7"></a>
## [将 Moebius 图像修复模型移植到浏览器中使用 WebGPU](https://simonwillison.net/2026/Jun/22/porting-moebius/#atom-everything) ⭐️ 8.0/10

Simon Willison 成功将 Moebius 0.2B 轻量级图像修复模型（原本需要 PyTorch 和 NVIDIA CUDA）移植到浏览器中，完全使用 WebGPU 运行。在线演示可在 simonw.github.io/moebius-web 访问。 这表明即使是依赖 CUDA 的机器学习模型也能适配到浏览器中进行推理，大大降低了在网页上部署 AI 图像编辑工具的门槛。它为用户在浏览器中直接进行隐私保护、无需服务器的图像修复创造了可能。 该移植利用了 ONNX Runtime Web 和 WebGPU 后端，模型完全在客户端运行，无需任何服务器调用。该模型有 0.2 亿参数，在修复任务中达到了与 10B 级别模型相当的性能。

rss · Simon Willison · 6月22日 23:43

**背景**: WebGPU 是一种现代 Web 图形 API，允许 Web 应用利用 GPU 进行高性能计算，包括机器学习推理。图像修复是一种通过算法填补图像中缺失或不需要部分的技术，常用于照片修复和编辑。以往，这类模型通常需要强大的桌面 GPU 和 CUDA 软件栈。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebGPU">WebGPU - Wikipedia</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/WebGPU_API">WebGPU API - Web APIs | MDN</a></li>
<li><a href="https://developer.chrome.com/docs/web-platform/webgpu/overview">Overview of WebGPU | Chrome for Developers</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#webgpu`, `#image inpainting`, `#browser`, `#AI`

---

<a id="item-8"></a>
## [sqlite-utils 4.0rc1 增加迁移和嵌套事务功能](https://simonwillison.net/2026/Jun/21/sqlite-utils/#atom-everything) ⭐️ 8.0/10

候选发布版 sqlite-utils 4.0rc1 引入了新的迁移系统，并通过 SQLite 保存点支持嵌套事务。 此版本使 sqlite-utils 成为更强大的工具，支持模式演进和复杂事务逻辑，使依赖 SQLite 进行数据管理的 Python 开发者受益。 嵌套事务通过 SQLite 保存点实现，支持在事务内部分回滚。迁移系统可能使用顺序版本号来跟踪模式变更。

rss · Simon Willison · 6月21日 23:30

**背景**: sqlite-utils 是一个用于创建、查询和操作 SQLite 数据库的 Python 库和命令行工具。迁移功能可自动化随时间的模式变更，而嵌套事务（通过保存点）实现了对数据库写入的更精细控制。SQLite 本身并不原生支持嵌套事务，但保存点提供了一种变通方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/simonw/sqlite-utils">GitHub - simonw/sqlite-utils: Python CLI utility and library for manipulating SQLite databases · GitHub</a></li>
<li><a href="https://sqlite-utils.datasette.io/">sqlite-utils</a></li>

</ul>
</details>

**标签**: `#sqlite-utils`, `#SQLite`, `#migrations`, `#Python`, `#database`

---

<a id="item-9"></a>
## [模型没有偏好，只有上下文](https://devblogs.microsoft.com/blog/models-dont-have-preferences-they-have-context) ⭐️ 7.0/10

这篇文章警告不要将人工智能模型拟人化，认为它们有偏好，并解释模型输出是由上下文驱动的，而非内在偏好。 这很重要，因为许多用户和开发者错误地将模型输出视为固定观点，这可能导致误解和过度依赖 AI 生成的断言。 这篇文章特别驳斥了模型在被询问推荐时'偏好'某个框架（如 React）的观点，强调不同的上下文会产生不同的答案。

rss · Microsoft for Developers · 6月22日 14:53

**背景**: 大型语言模型如 GPT-4 或 Claude 基于训练数据和输入提示生成响应。它们没有信念或偏好；它们的输出是概率性预测。拟人化是与 AI 交互时常见的认知偏差。

**标签**: `#AI`, `#LLMs`, `#prompt engineering`, `#machine learning`

---

<a id="item-10"></a>
## [PostgreSQL enable_async_append GUC 详解](https://postgr.es/p/9n9) ⭐️ 7.0/10

Christophe Pettus 在文章中解释了 PostgreSQL 中的 enable_async_append GUC，这是一个在版本 14 中引入的诊断开关，允许规划器并行地将查询分发到远程分片。 该 GUC 通过将串行分片访问改为并发执行，能显著降低分布式 PostgreSQL 环境中的查询延迟，对使用外部数据封装器和分片的用户尤为有益。 默认值为开启，但它是一个诊断开关而非调优参数，意味着只应在调试或特定测试场景中禁用它。

rss · Planet PostgreSQL · 6月23日 01:00

**背景**: PostgreSQL 的 enable_async_append 在版本 14 中引入，改变了规划器处理包含外部表分区的 Append 节点的方式。未启用时，远程查询串行执行，延迟累加；启用后，查询并发运行，仅等待最慢的分片。这对于基于 FDW 的分片场景最为相关。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pgpedia.info/e/enable_async_append.html">enable_async_append - pgPedia - a PostgreSQL Encyclopedia</a></li>
<li><a href="https://www.cybrosys.com/research-and-development/postgres/how-enableasyncappend-boosts-parallel-performance-in-postgresql">How enable_async_append Boosts Parallel Performance in PostgreSQL</a></li>
<li><a href="https://thebuild.com/blog/all-your-gucs-in-a-row-enableasyncappend/">All Your GUCs in a Row: enable_async_append — The Build</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#GUC`, `#async append`, `#database performance`, `#sharding`

---

<a id="item-11"></a>
## [PostgreSQL pg_stats：内部统计如何指导查询规划](https://postgr.es/p/9mG) ⭐️ 7.0/10

Richard Yen 在 POSETTE 2026 上发表了演讲（现已整理成博客），解释了 PostgreSQL 的 pg_stats 视图和底层 pg_statistic 系统目录如何存储数据摘要，查询规划器基于这些摘要做出基于成本的决策，并通过具体示例进行了说明。 理解 pg_stats 有助于数据库管理员和开发者解读和排查查询计划，从而优化索引设计和查询性能。 博客使用了一个包含 100 万行的 customers 表作为示例，说明即使在 state 列上有索引，如果规划器估计 state='CA' 匹配了较多的行（占表的 17%），它仍可能选择全表扫描。

rss · Planet PostgreSQL · 6月22日 08:00

**背景**: PostgreSQL 的查询规划器采用基于成本的优化模型，依赖存储在 pg_statistic 系统目录（通过 pg_stats 视图暴露）中的统计信息。这些统计信息由 ANALYZE 命令收集，包括不同值的数量、最常见值以及数据分布直方图。规划器比较不同执行策略的估算成本，并选择估算总成本最低的方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/view-pg-stats.html">PostgreSQL: Documentation: 18: 53.29. pg_stats</a></li>
<li><a href="https://www.elysiate.com/blog/postgresql-query-planner-explained-simply">PostgreSQL Query Planner Explained Simply | Elysiate</a></li>
<li><a href="https://www.postgresql.org/docs/current/sql-analyze.html">PostgreSQL: Documentation: 18: ANALYZE</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#pg_stats`, `#query optimization`, `#database internals`

---

<a id="item-12"></a>
## [PostgreSQL 的 effective_io_concurrency 参数演变与影响](https://postgr.es/p/9mD) ⭐️ 7.0/10

Christophe Pettus 解释了 PostgreSQL 中的 effective_io_concurrency 参数如何两次改变含义：从谐波级数主轴数变为直接请求深度，最后变为真正的异步 I/O 控制。 理解这一演变对于数据库管理员和性能调优人员正确配置 PostgreSQL 中的 I/O 并行性至关重要，尤其是在 PostgreSQL 18 引入异步 I/O 的情况下。 该参数最初代表 RAID 阵列中的主轴数，后来被重新解释为并发 I/O 请求数，而在最新版本中则控制异步 I/O 操作的深度。PostgreSQL 18 新增了 io_method 参数来选择底层的 I/O 机制。

rss · Planet PostgreSQL · 6月22日 01:00

**背景**: effective_io_concurrency 是一个 PostgreSQL 配置参数，用于告知查询优化器可以同时执行多少个并发磁盘 I/O 操作。早期版本基于 RAID 配置中的物理主轴数来设定其值，假设是旋转磁盘。随着向 SSD 的转变以及 I/O 子系统的改进，该参数的语义变为直接控制同时 I/O 请求的数量，现在与 PostgreSQL 新的异步 I/O 框架集成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://postgresqlco.nf/doc/en/param/effective_io_concurrency/">PostgreSQL Documentation: effective_io_concurrency parameter</a></li>
<li><a href="https://dba.stackexchange.com/questions/228663/what-is-effective-spindle-count">postgresql - What is effective spindle count - Database...</a></li>
<li><a href="https://pganalyze.com/blog/postgres-18-async-io">Waiting for Postgres 18: Accelerating Disk Reads with Asynchronous I/O</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database tuning`, `#I/O configuration`, `#performance`

---

<a id="item-13"></a>
## [Cloudflare 推出无需注册的临时账户用于部署](https://simonwillison.net/2026/Jun/21/temporary-cloudflare-accounts/#atom-everything) ⭐️ 7.0/10

Cloudflare 宣布推出临时账户，开发者无需注册即可通过 'npx wrangler deploy --temporary' 命令部署 Workers 项目，部署有效期为 60 分钟。 这降低了部署无服务器应用的门槛，非常适合快速实验、演示和 AI 代理工作流，并扩大了 Cloudflare Workers 的可访问性。 部署是临时的，持续 60 分钟后自动过期，除非通过提供的 URL 认领。该功能通过 wrangler CLI 的 --temporary 标志使用。

rss · Simon Willison · 6月21日 22:01

**背景**: Cloudflare Workers 是一个无服务器计算平台，在 Cloudflare 的全球边缘网络上运行代码。Wrangler 是管理 Workers 的命令行工具。临时部署是短期、隔离的环境，常用于测试或预览功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.cloudflare.com/workers/">Overview · Cloudflare Workers docs</a></li>
<li><a href="https://www.cloudflare.com/products/workers/">Cloudflare Workers - Global Serverless Functions Platform</a></li>

</ul>
</details>

**标签**: `#cloudflare`, `#workers`, `#deployment`, `#serverless`, `#AI agents`

---