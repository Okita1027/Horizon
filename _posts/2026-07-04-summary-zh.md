---
layout: default
title: "Horizon 日报：2026-07-04 (ZH)"
date: 2026-07-04
lang: zh
---

> 从 50 条内容中筛选出 12 条重要资讯。

---

1. [飞马间谍软件感染调查间谍软件的希腊欧洲议会议员](#item-1) ⭐️ 9.0/10
2. [AMD MI355X 在 GLM5.2 上达 2626 tok/s，成本低于 Blackwell 两倍以上](#item-2) ⭐️ 8.0/10
3. [本地运行 LLM 指南：高昂成本与实际权衡](#item-3) ⭐️ 8.0/10
4. [Wordgard：ProseMirror 作者推出的新富文本编辑器](#item-4) ⭐️ 8.0/10
5. [PostgreSQL 通过严格内存过量使用避免 OOM 杀手](#item-5) ⭐️ 8.0/10
6. [开源 AI 差距地图索引 421 个产品](#item-6) ⭐️ 8.0/10
7. [嵌套循环连接：仅在规划器错误估算行数时成为性能灾难](#item-7) ⭐️ 7.0/10
8. [指南：通过 pg_hardstorage 追溯 PostgreSQL 备份到恢复](#item-8) ⭐️ 7.0/10
9. [AI 冲击下课程销量暴跌 50%以上](#item-9) ⭐️ 7.0/10
10. [Simon Willison 2026 年 6 月简讯](#item-10) ⭐️ 7.0/10
11. [用 DSPy 优化 Datasette Agent 的 SQL 提示](#item-11) ⭐️ 7.0/10
12. [理解才能参与：AI 辅助编程的新理念](#item-12) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [飞马间谍软件感染调查间谍软件的希腊欧洲议会议员](https://citizenlab.ca/research/member-of-committee-investigating-spyware-hacked-with-pegasus/) ⭐️ 9.0/10

公民实验室确认，飞马间谍软件感染了一名希腊欧洲议会议员，该议员曾参与调查间谍软件问题的委员会。感染发生在 2022 年 10 月和 2023 年 3 月。 此次间谍活动直接针对欧盟机构，破坏民主监督。它凸显了持续存在的国家支持监视风险，以及加强议员网络安全保护的必要性。 法医分析以高度置信度发现该议员的 iPhone 多次被感染。首次感染与已知针对流亡记者的飞马间谍活动重叠，表明某客户拥有跨国家监视授权。

hackernews · ledoge · 7月3日 20:38 · [社区讨论](https://news.ycombinator.com/item?id=48779683)

**背景**: 飞马是由以色列 NSO 集团开发的强大间谍软件，能够远程、隐蔽地监视移动设备。它已被各国政府广泛滥用来针对记者、活动家和政治家。公民实验室是揭露数字威胁的领先研究机构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Citizen_Lab">Citizen Lab</a></li>
<li><a href="https://citizenlab.ca/">The Citizen Lab - The Citizen Lab</a></li>

</ul>
</details>

**社区讨论**: 评论者将此事件与希腊持续的政治丑闻联系起来，许多政界人士被黑，可能由总理办公室策划。其他人指出讽刺之处：调查间谍软件的人自己被监视，并批评欧盟成员国滥用飞马。

**标签**: `#spyware`, `#cybersecurity`, `#Pegasus`, `#European Parliament`, `#surveillance`

---

<a id="item-2"></a>
## [AMD MI355X 在 GLM5.2 上达 2626 tok/s，成本低于 Blackwell 两倍以上](https://www.wafer.ai/blog/glm52-amd) ⭐️ 8.0/10

AMD 的 MI355X GPU 在 GLM5.2 语言模型上实现了每节点 2626 tokens/秒的推理速度，并声称成本比 Nvidia 的 Blackwell 低两倍以上。 这一基准测试表明 AMD 正在成为 AI 推理领域的有力竞争者，可能为 Nvidia GPU 提供高性价比的替代方案，尤其适用于 Nvidia 供应受限的美国以外数据中心。 2626 tok/s 的吞吐量是聚合值而非单请求延迟，基准测试使用了量化模型（FP8 到 MXFP4）并假设 60% 的缓存命中率，可能影响准确度。

hackernews · latchkey · 7月3日 21:49 · [社区讨论](https://news.ycombinator.com/item?id=48780417)

**背景**: GLM5.2 是 Z.ai（原智谱 AI）最新发布的开源大语言模型，采用 MIT 许可证。AMD MI355X 是面向推理优化的数据中心 GPU，属于 Instinct 系列，与 Nvidia 的 Blackwell 和 Rubin 竞争。成本比较往往取决于量化和缓存策略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GLM_5.2">GLM 5.2</a></li>
<li><a href="https://en.wikipedia.org/wiki/Amd_MI355X">Amd MI355X</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.2">GLM - 5 . 2 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>

</ul>
</details>

**社区讨论**: 评论者质疑 60% 缓存命中率的假设是否合理，并指出从 FP8 切换到 MXFP4 时存在明显的准确度下降。还有人澄清 2600 tok/s 是聚合值而非实际吞吐量，并要求提供每瓦性能指标以进行公平比较。

**标签**: `#AMD`, `#GPU`, `#inference`, `#cost-efficiency`, `#benchmark`

---

<a id="item-3"></a>
## [本地运行 LLM 指南：高昂成本与实际权衡](https://github.com/jamesob/local-llm) ⭐️ 8.0/10

Jamesob 在 GitHub 上发布了一份实用指南，介绍如何在本地运行最先进的 LLM，详细说明了从 3000 美元到 5.5 万美元的硬件配置。社区讨论指出了高昂成本，并质疑本地方案相对于云订阅的可行性。 这凸显了本地 AI 控制与云成本效益之间的持久困境。对大多数个人和小团队而言，高端本地 LLM 的前期硬件投资仍然高得令人望而却步，相比之下云 API 则价格低廉。 该指南的旗舰配置起始预算 4 万美元，但实际上配备四块 1.2 万美元的 GPU 后总价约 5.5 万美元。更便宜的选择如两块 RTX 3090（约 3000 美元）拥有 48GB 显存，可运行 Qwen3.6-27B，但社区指出量化通常会降低模型质量。

hackernews · livestyle · 7月3日 15:03 · [社区讨论](https://news.ycombinator.com/item?id=48775921)

**背景**: 在本地运行大型语言模型需要大量显存和计算能力。量化技术通过降低数值精度（例如从 FP16 降至 INT4）来减少内存占用，但可能降低输出质量。云订阅如 Claude Opus（每月 200 美元）无需硬件开销即可轻松访问顶级模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://julsimon.medium.com/what-to-buy-for-local-llms-april-2026-a4946a381a6a">What to Buy for Local LLMs (April 2026) | by Julien Simon | Medium</a></li>
<li><a href="https://www.sitepoint.com/definitive-guide-local-llms-2026-privacy-tools-hardware/">Guide to Local LLMs in 2026: Privacy, Tools & Hardware</a></li>
<li><a href="https://fungies.io/local-llm-vs-cloud-cost-2026/">Local LLM vs Cloud API: The Complete 2026 Cost Breakdown & Break-Even ...</a></li>

</ul>
</details>

**社区讨论**: 评论者算出 5.5 万美元的配置相当于 16.8 年的 Claude Opus 订阅费，质疑其合理性。有人建议采用 128GB 统一内存来运行 DeepSeek V4 flash 等替代方案，也有人警告量化剪枝后的模型在基准测试外往往表现不佳。

**标签**: `#LLM`, `#local inference`, `#hardware`, `#cost analysis`, `#community discussion`

---

<a id="item-4"></a>
## [Wordgard：ProseMirror 作者推出的新富文本编辑器](https://wordgard.net/) ⭐️ 8.0/10

ProseMirror 的创建者 Marijn Haverbeke 发布了 Wordgard 0.1，这是一个新的开源 JavaScript 富文本编辑器库，整合了自 ProseMirror 稳定九年来所学到的经验。 Wordgard 代表了基于 Web 的富文本编辑的重大演进，提供了更可定制且聚焦于模式的方法，可能简化需要结构化内容编辑的应用程序的开发。 Wordgard 没有从 ProseMirror 升级的路径，共享许多概念，但切换需要大量重做。它针对的是符合特定模式的内容编辑，而非通用的所见即所得编辑。

hackernews · indy · 7月3日 08:50 · [社区讨论](https://news.ycombinator.com/item?id=48772573)

**背景**: 富文本编辑器允许用户在网页浏览器中格式化文本，而无需编写 HTML。ProseMirror 是一个知名的编辑器库，能生成干净、语义化的文档。Wordgard 是同一位作者的新一代作品，旨在解决限制并提高对结构化内容的可定制性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wordgard.net/">Wordgard</a></li>
<li><a href="https://marijnhaverbeke.nl/blog/wordgard-0.1.html">Wordgard Release 0.1</a></li>
<li><a href="https://wordgard.net/docs/guide/">Wordgard System Guide</a></li>
<li><a href="https://prosemirror.net/">ProseMirror</a></li>

</ul>
</details>

**社区讨论**: Hacker News 社区表现出浓厚兴趣，用户讨论了与 ProseMirror 的差异、缺乏升级路径，并称赞编辑器的设计。一些人提到 ProseMirror 在类型定义方面的挑战，并赞赏 Wordgard 在更好的静态类型支持方面的潜力。

**标签**: `#rich-text editor`, `#web development`, `#ProseMirror`, `#open-source`

---

<a id="item-5"></a>
## [PostgreSQL 通过严格内存过量使用避免 OOM 杀手](https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit) ⭐️ 8.0/10

Ubicloud 的博客文章提倡在 PostgreSQL 服务器上使用严格内存过量使用（vm.overcommit_memory=2），以防止在内存压力下 Linux OOM 杀手终止数据库进程。 这对生产环境中的 PostgreSQL 运维人员意义重大，因为一个简单的配置更改就能显著提高数据库稳定性。内存过量使用策略的权衡对 Linux 系统的可靠性有广泛影响。 严格过量使用防止内核过度承诺内存，当内存耗尽时 malloc()返回 NULL 而不是让 OOM 杀手稍后终止进程。但如评论所指，如果已调整过量使用比率，模式 2 可能破坏 fork()，因此测试至关重要。

hackernews · furkansahin · 7月3日 13:00 · [社区讨论](https://news.ycombinator.com/item?id=48774509)

**背景**: Linux 默认使用内存过量使用，允许进程请求超过物理内存的内存。当实际内存耗尽时，OOM 杀手会选择并终止一个进程以释放内存。PostgreSQL 由于其大型共享缓冲区常常成为受害者。严格过量使用（vm.overcommit_memory=2）禁用过量使用，使分配立即失败而不是依赖 OOM 杀手，从而可以防止灾难性系统挂起。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit">PostgreSQL and the OOM Killer: Why We Use Strict Memory ...</a></li>
<li><a href="https://www.baeldung.com/linux/memory-overcommitment-oom-killer">Linux Memory Overcommitment and the OOM Killer - Baeldung</a></li>

</ul>
</details>

**社区讨论**: 社区情绪总体积极但谨慎。一位评论者指出 Linux 默认设置有问题，另一位警告如果已调整过量使用比率，模式 2 可能导致故障。Ubicloud 的作者同意技术内容但承认标题可能过于强烈，并且严格过量使用在某些场景下有意想不到的副作用。另一位用户分享了在模式间切换导致不稳定的个人经历。

**标签**: `#PostgreSQL`, `#Linux`, `#memory management`, `#OOM killer`, `#database operations`

---

<a id="item-6"></a>
## [开源 AI 差距地图索引 421 个产品](https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/#atom-everything) ⭐️ 8.0/10

Current AI（2025 年 2 月在巴黎 AI 行动峰会上成立的非营利组织）发布了开源 AI 差距地图 v0.1，该地图索引了 AI 堆栈中的 421 个产品（包括 266 个软件工具和库、85 个模型、50 个数据集和 20 个硬件项目）。 这一全面的地图有助于识别开源 AI 生态系统中的差距，指导在哪里建设、投资和弥补关键空白，并为全球 AI 社区提供了宝贵的资源。 底层数据以 MIT 许可证发布在 GitHub 上，包括 1,184 个 YAML 文件和 16,185 个跟踪仓库，可通过 Datasette Lite 进行探索。

rss · Simon Willison · 7月3日 22:04

**背景**: Current AI 是一个旨在构建 AI 公共选项的全球合作组织，已获 4 亿美元承诺资金支持。差距地图评估了从基础模型到推理后端的超过 24,626 个项目，评估其开放性、能力和采用情况。它将产品分为三个层次的 14 个类别：模型组件、产品/用户体验和基础设施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://map.currentai.org/">Current AI - Open Source AI Gap Map</a></li>
<li><a href="https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/">Open Source AI Gap Map - simonwillison.net</a></li>
<li><a href="https://www.currentai.org/blogs/introducing-the-gap-map-v0-1">Introducing the Gap Map v0.1 - currentai.org</a></li>

</ul>
</details>

**标签**: `#open source AI`, `#ecosystem mapping`, `#AI infrastructure`, `#non-profit`

---

<a id="item-7"></a>
## [嵌套循环连接：仅在规划器错误估算行数时成为性能灾难](https://postgr.es/p/9n_) ⭐️ 7.0/10

Christophe Pettus 在题为《All Your GUCs in a Row: enable_nestloop》的博客中提出，嵌套循环连接本身并非性能灾难；只有当 PostgreSQL 规划器错误估算行数时，才会导致性能问题。 这一见解帮助数据库管理员和开发者避免完全禁用嵌套循环连接，从而通过改进基数估算而非全面配置变更来实现更好的查询优化。 文章指出，将 enable_nestloop 设置为 off 可能会在嵌套循环适用的情况下损害性能，例如当外表行数很少时。

rss · Planet PostgreSQL · 7月3日 01:00

**背景**: 嵌套循环连接是一种基本的连接方法，对于外表中的每一行，扫描内表以查找匹配。PostgreSQL 查询规划器通过估算行数来选择最佳连接策略；估算错误可能导致性能低下。enable_nestloop 配置参数允许用户完全禁用这一连接类型。该文是解释各种全局统一配置（GUC）参数的系列文章之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thebuild.com/blog/all-your-gucs-in-a-row-enable_nestloop/">All Your GUCs in a Row : enable_nestloop — The Build</a></li>
<li><a href="https://stackoverflow.com/questions/594930/what-are-the-pitfalls-of-setting-enable-nestloop-to-off">postgresql - What are the pitfalls of setting enable _ nestloop to OFF</a></li>

</ul>
</details>

**社区讨论**: 新闻条目中未提供评论，但 Stack Overflow 的讨论表明，禁用 enable_nestloop 是一种常见但有时错误的做法。

**标签**: `#PostgreSQL`, `#query optimization`, `#database performance`, `#join types`, `#GUC`

---

<a id="item-8"></a>
## [指南：通过 pg_hardstorage 追溯 PostgreSQL 备份到恢复](https://postgr.es/p/9o4) ⭐️ 7.0/10

Hans-Juergen Schoenig 发布了一份详细指南，追踪 PostgreSQL 备份通过 pg_hardstorage 的完整生命周期，从数据捕获到恢复，解释了存储库布局、WAL 处理和元数据。 该指南帮助数据库管理员、SRE 和平台团队理解备份数据如何在系统中流动，这对故障排除、验证备份策略和准备恢复至关重要。 该指南涵盖了内容寻址存储、分块、去重、清单设计、完整性验证、损坏处理、崩溃安全性和垃圾回收。pg_hardstorage 是一个开源、Apache 2.0 的 PostgreSQL 备份工具，使用原生 WAL 流和单个静态 Go 二进制文件。

rss · Planet PostgreSQL · 7月2日 07:54

**背景**: PostgreSQL 管理员需要健壮的备份和恢复工具。pg_hardstorage 是一个来自 CYBERTEC 的相对较新的企业级备份工具，提供持续的 WAL 流和基础备份。该指南侧重于存储库背后的架构决策，而不仅仅是命令使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/cybertec-postgresql/pg_hardstorage">GitHub - cybertec-postgresql/pg_hardstorage: pg_hardstorage — enterprise-grade PostgreSQL backup: continuous WAL streaming + base backups, single static Go binary, PostgreSQL 15–18, Apache 2.0.</a></li>
<li><a href="https://www.pghardstorage.org/">pg_hardstorage — PostgreSQL backup, done right.</a></li>
<li><a href="https://www.cybertec-postgresql.com/en/products/pg-hardstorage/">pg_hardstorage – Open-Source PostgreSQL Backup | CYBERTEC</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#backup`, `#recovery`, `#pg_hardstorage`

---

<a id="item-9"></a>
## [AI 冲击下课程销量暴跌 50%以上](https://simonwillison.net/2026/Jul/3/josh-w-comeau/#atom-everything) ⭐️ 7.0/10

知名课程创作者 Josh W. Comeau 报告称，其新课程发布销量仅达平时三分之一，现有课程销售额同比下滑超过 50%。 这来自一位信誉良好的创作者，提供了关于 AI 如何颠覆开发者教育的具体数据：学习者因工作不确定性而犹豫投资，并转向大型语言模型获取免费个性化辅导。 Comeau 将销量下降归因于‘双重打击’：对开发者工作可能很快消失的恐惧，以及 LLM 提供个性化辅导减少了对付费课程的需求。他还指出多位课程创作者都观察到收入下降 50%以上。

rss · Simon Willison · 7月3日 21:25

**背景**: 大型语言模型（LLM）是在大量文本数据上训练的 AI 系统，能够生成、总结和分析文本。ChatGPT 等聊天工具已被广泛用于学习编程和解决问题，且通常免费。这扰乱了付费教程和课程市场，因为学习者无需购买传统资源即可获得即时帮助。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model_emergent_abilities">Large language model emergent abilities</a></li>
<li><a href="https://www.geeksforgeeks.org/artificial-intelligence/large-language-model-llm/">Large Language Model ( LLM ) - GeeksforGeeks</a></li>

</ul>
</details>

**标签**: `#AI impact`, `#developer education`, `#course sales`, `#LLM`, `#job market`

---

<a id="item-10"></a>
## [Simon Willison 2026 年 6 月简讯](https://simonwillison.net/2026/Jul/3/june-newsletter/#atom-everything) ⭐️ 7.0/10

Simon Willison 的 2026 年 6 月简讯涵盖了近期 AI 模型发布，包括 Claude Fable 5、GPT-5.6、GLM-5.2，以及从 tokenmaxxing 向 valuemaxxing 的转变。 这份精心策划的简讯汇集了来自一位知名技术人士的重要 AI 动态，帮助读者了解模型发布、出口限制以及 tokenmaxxing 衰落等行业趋势。 该简讯仅面向赞助者，订阅费为每月 10 美元，可提前一个月获得免费版本的访问权。内容包括 Claude Fable 5（Anthropic 最强大的视觉模型）、GLM-5.2（领先的开源权重模型）以及 tokenmaxxing 的终结。

rss · Simon Willison · 7月3日 14:50

**背景**: Tokenmaxxing 是指以最大化 AI 令牌使用量作为生产力指标的做法，但企业正转向强调结果的 valuemaxxing。GLM-5.2 是 Z.ai 推出的约 750B 参数的混合专家开源模型，在编程基准测试中表现优异。Claude Fable 5 是 Anthropic 的最新一代先进模型，在视觉和推理任务上表现出色。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Token_maxxing">Token maxxing - Wikipedia</a></li>
<li><a href="https://ollama.com/library/glm-5.2">GLM - 5 . 2 is Z.ai’s flagship model for the era of long-horizon tasks.</a></li>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI`, `#machine learning`, `#newsletter`, `#tech news`, `#open models`

---

<a id="item-11"></a>
## [用 DSPy 优化 Datasette Agent 的 SQL 提示](https://simonwillison.net/2026/Jul/2/dspy-datasette-agent-prompts/#atom-everything) ⭐️ 7.0/10

Simon Willison 使用 DSPy 框架自动评估和改进了 Datasette Agent 的 SQL 查询功能中的系统提示，发现了诸如在模式列表中包含列名等有前景的改进方向。 这展示了一种结合 DSPy 进行自动评估和提示优化的实用工作流程，可以显著提高 Datasette Agent 等工具中 AI 生成 SQL 查询的可靠性和准确性。 Willison 使用 Claude Code for web 与 Claude Fable 5 进行实验，DSPy 测试使用了 GPT 4.1 mini 和 nano 模型。一个关键发现是原始提示缺少列名，导致代理猜测列名并陷入错误重试循环。

rss · Simon Willison · 7月2日 18:25

**背景**: DSPy（Declarative Self-improving Python）是斯坦福大学开发的开源框架，通过将任务表达为结构化签名而不是脆弱的提示来构建 AI 系统。Datasette Agent 是 Datasette 的 AI 助手，Datasette 是一款用于探索和查询数据的工具，它通过生成 SQL 查询来回答用户的问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dspy.ai/">DSPy</a></li>
<li><a href="https://agent.datasette.io/">Datasette Agent: an AI assistant for Datasette to help explore and ...</a></li>
<li><a href="https://datasette.io/blog/2026/datasette-agent/">Datasette Agent, an extensible AI assistant for Datasette</a></li>

</ul>
</details>

**标签**: `#dspy`, `#prompt engineering`, `#datasette`, `#sql`, `#AI-assisted development`

---

<a id="item-12"></a>
## [理解才能参与：AI 辅助编程的新理念](https://simonwillison.net/2026/Jul/2/understand-to-participate/#atom-everything) ⭐️ 7.0/10

Geoffrey Litt 在 AIE 大会上提出了“理解才能参与”的概念，认为开发者必须深入理解 AI 生成的代码变更，才能保持活跃的创意合作，避免认知债务。 这个概念突出了一个关键风险：随着 AI 编程代理能力增强，如果缺乏深入理解，开发者将失去有效引导项目的能力，导致认知债务和长期软件脆弱性。 Litt 的演讲强调开发者需要思维中拥有“丰富的概念集”才能创造性地思考代码变更，并且理解必须足够深入，以便能够积极参与创意过程，而非被动接受。

rss · Simon Willison · 7月2日 17:07

**背景**: 认知债务指开发者对软件工作原理的理解与实际复杂性之间的差距。随着 AI 编程助手生成更多代码，开发者容易落后，积累认知债务，使得未来修改更困难、风险更高。“理解才能参与”这一框架提供了主动应对之道：通过投入理解来保持主动权。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/2/understand-to-participate/">Understand to participate | Simon Willison’s Weblog</a></li>
<li><a href="https://itbrief.asia/story/ai-coding-boom-deepens-cognitive-debt-says-thoughtworks">AI coding boom deepens cognitive debt , says Thoughtworks</a></li>

</ul>
</details>

**标签**: `#AI-assisted programming`, `#cognitive debt`, `#code understanding`, `#software engineering`

---