---
layout: default
title: "Horizon 日报：2026-06-28 (ZH)"
date: 2026-06-28
lang: zh
---

> 从 46 条内容中筛选出 10 条重要资讯。

---

1. [DeepSeek 开源 DSpark，通过投机解码加速大模型推理](#item-1) ⭐️ 10.0/10
2. [OpenAI 预览 GPT-5.6 系列模型](#item-2) ⭐️ 9.0/10
3. [为何物理媒介所有权仍然重要](#item-3) ⭐️ 8.0/10
4. [数据分布中的可疑间断点分析](#item-4) ⭐️ 8.0/10
5. [别再为不会发生的崩溃而惩罚你的 PostgreSQL](#item-5) ⭐️ 8.0/10
6. [OpenRA 为现代系统重建经典 C&C](#item-6) ⭐️ 7.0/10
7. [金融科技工程手册引发货币表示方法关键讨论](#item-7) ⭐️ 7.0/10
8. [PostgreSQL 13 哈希聚合写入磁盘引起回归](#item-8) ⭐️ 7.0/10
9. [前沿 AI 经济学：利润窗口狭窄与基础设施风险](#item-9) ⭐️ 7.0/10
10. [6000 次尝试黑客 AI 助手均失败，显示提示注入防御力](#item-10) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [DeepSeek 开源 DSpark，通过投机解码加速大模型推理](https://github.com/deepseek-ai/DeepSpec/blob/main/DSpark_paper.pdf) ⭐️ 10.0/10

DeepSeek 发布了 DSpark 论文，并在 Hugging Face 上开源了 DeepSeek-V4-Flash-DSpark 和 DeepSeek-V4-Pro-DSpark 模型，这些模型直接集成了投机解码模块，在保持输出质量的同时加速推理。 这是一项重要的开源贡献，展示了中国 AI 实验室在创新和透明度方面的领先地位，有望让社区更广泛地获得更快的 LLM 推理能力。该技术可将延迟降低两到三倍而不影响准确性，惠及多种应用场景。 该投机解码模块采用“草稿-目标”方法，每个步骤可生成多个 token：较小的草稿模型提出候选 token，较大的目标模型通过单次前向传播进行验证。社区反馈称 Hugging Face 模型已内置该模块，可立即使用。

hackernews · aurenvale · 6月27日 09:18 · [社区讨论](https://news.ycombinator.com/item?id=48696585)

**背景**: 投机解码是一种用于自回归大语言模型（LLM）的推理时优化技术，每次解码步骤可生成多个 token，而非仅一个。较小的草稿模型提出候选 token 序列，较大的目标模型通过改进的拒绝采样方案进行验证，在保持原始输出分布的同时将延迟降低大约两到三倍。该名称类比 CPU 中的投机执行，即处理器在结果未知前沿预测分支执行指令。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Speculative_decoding">Speculative decoding</a></li>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-speculative-decoding-for-reducing-latency-in-ai-inference/">An Introduction to Speculative Decoding for Reducing Latency in AI ...</a></li>

</ul>
</details>

**社区讨论**: 社区反响非常积极，许多用户称赞 DeepSeek 在发布详细论文和开源模型的同时，而美国实验室却对其方法保密。有用户报告了 DeepSeek V4 pro 的出色实际体验，指出其速度快、可靠性高且成本低。有评论者询问该方法是否比 2022 年最初的投机解码论文更新或更好。

**标签**: `#speculative decoding`, `#LLM inference`, `#DeepSeek`, `#AI optimization`, `#open-source`

---

<a id="item-2"></a>
## [OpenAI 预览 GPT-5.6 系列模型](https://simonwillison.net/2026/Jun/26/openai/#atom-everything) ⭐️ 9.0/10

OpenAI 宣布了 GPT-5.6 系列的有限预览，包括三个不同的模型：Sol（旗舰）、Terra（均衡）和 Luna（快速/经济）。该预览最初仅向一小群受信任的合作伙伴开放。 此次发布标志着 OpenAI 的下一次重大模型升级，引入了分层定价和性能选项，以满足不同用例和预算的需求。不同的成本结构可能会使高级 AI 功能的访问更加民主化。 每 100 万 token 的定价：Sol（输入 $5 / 输出 $30），Terra（输入 $2.50 / 输出 $15），Luna（输入 $1 / 输出 $6）。GPT-5.6 还引入了可预测的提示缓存，支持显式缓存断点和 30 分钟的最小缓存寿命；缓存写入按未缓存输入率的 1.25 倍计费。

rss · Simon Willison · 6月26日 17:10

**背景**: OpenAI 开发了多代 GPT 模型，其中 GPT-5.5 是之前的旗舰型号。新的 GPT-5.6 系列引入了三个层级：Sol 作为最强大的型号，Terra 作为均衡选项，Luna 作为经济型选择。提示缓存是一种通过重用先前计算的输出来降低延迟和成本的技术。

**标签**: `#OpenAI`, `#GPT-5.6`, `#AI Models`, `#Machine Learning`, `#Pricing`

---

<a id="item-3"></a>
## [为何物理媒介所有权仍然重要](https://dervis.de/physical/) ⭐️ 8.0/10

文章论证了物理媒介是唯一真正的内容所有权形式，而数字购买只是可撤销的许可。它将物理光盘的永久性与数字流媒体和下载的暂时性进行了对比。 在消费者日益转向数字媒体、却往往不知道自己只持有可撤销许可的情况下，这一话题至关重要。它重新点燃了关于数字权利和消费者保护的讨论，尤其是在索尼 PlayStation 商店移除内容等事件之后。 文章引用了数字储物柜服务 Ultraviolet 的失败，以及索尼将于 2026 年从 PlayStation 账户中移除已购买的 Studio Canal 电影。这些例子凸显了许可协议如何使数字所有权失效。

hackernews · cemdervis · 6月27日 11:32 · [社区讨论](https://news.ycombinator.com/item?id=48697335)

**背景**: 数字版权管理（DRM）限制了数字内容的使用方式。当您“购买”数字媒体时，通常购买的是许可，服务提供商可以撤销该许可。DVD 和蓝光等物理媒介则让您拥有实物副本，不受远程删除或访问控制的影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_rights_management">Digital rights management - Wikipedia</a></li>
<li><a href="https://www.accio.com/blog/sonys-digital-license-crisis-how-gaming-giants-risk-customer-trust">Sony’s Digital License Crisis: How Gaming Giants Risk ...</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认同该观点，但对物理媒介的必要性存在争议，部分人主张 GOG 和 Bandcamp 等无 DRM 的数字选项。另一些人认为盗版是合法的所有权形式。Ultraviolet 案例经常被引证为数字撤销的证据。

**标签**: `#digital rights`, `#media ownership`, `#DRM`, `#consumer protection`, `#piracy`

---

<a id="item-4"></a>
## [数据分布中的可疑间断点分析](https://danluu.com/discontinuities/) ⭐️ 8.0/10

Dan Luu 在 2020 年撰写的文章探讨了数据分布中可疑的间断点如何揭示人类行为和测量偏差，以马拉松完成时间在整数附近聚集和税收福利悬崖为例。 识别这些间断点有助于数据科学家避免误解并改进数据清洗，同时为人类心理学以及税收和评分系统中的激励缺陷提供见解。 文章使用统计可视化突出了马拉松时间每 30 分钟的堆积、英国和印度的税收悬崖，以及波兰语言考试成绩中的可疑尖峰。

hackernews · tosh · 6月27日 13:32 · [社区讨论](https://news.ycombinator.com/item?id=48698151)

**背景**: 数据中的间断点通常出现在阈值或激励导致行为调整时，或测量方法引起四舍五入时。例如，马拉松跑者追求整数完成时间，而税收制度在收入阈值处造成边际税率突变。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=28452926">Suspicious Discontinuities | Hacker News</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC3518030/">Accounting for Heaping in Retrospectively Reported Event Data – A Mixture-Model Approach - PMC</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了个人轶事，例如半马跑者努力在 2:30 内完赛，以及英国税收悬崖等额外例子。讨论普遍赞同文章的发现，并提供了更多真实世界的证据。

**标签**: `#statistics`, `#data analysis`, `#behavioral economics`, `#human-computer interaction`, `#anomaly detection`

---

<a id="item-5"></a>
## [别再为不会发生的崩溃而惩罚你的 PostgreSQL](https://postgr.es/p/9nu) ⭐️ 8.0/10

一篇新的技术文章纠正了一个常见误解：增加 PostgreSQL 的 checkpoint_timeout 不会导致崩溃恢复时间变长。文章指出，如果拥有副本，恢复时间根本不是问题，更长的超时反而能提升性能。 这很重要，因为许多生产数据库因过于频繁的检查点而遭受不必要的性能下降，该建议澄清了影响成千上万 PostgreSQL 用户的关键权衡。 PostgreSQL 默认的 checkpoint_timeout 是 5 分钟（300 秒），将其降低到 1 分钟会导致过多的 I/O 和性能下降。文章强调，如果有一个同步副本，崩溃恢复在副本上进行，而不是主库。

rss · Planet PostgreSQL · 6月27日 00:00

**背景**: PostgreSQL 使用预写式日志（WAL）来确保数据持久性。检查点是周期性事件，将脏缓冲区刷新到磁盘，其频率由 checkpoint_timeout（默认 5 分钟）和 max_wal_size 控制。更长的超时意味着检查点频率降低，从而减少 I/O，但可能增加崩溃后的恢复时间。然而，如果有副本，崩溃后主库可以被丢弃，快速故障转移到副本，使得主库的恢复时间无关紧要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/wal-configuration.html">PostgreSQL: Documentation: 18: 28.5. WAL Configuration</a></li>
<li><a href="https://medium.com/@jramcloud1/04-postgresql-17-performance-tuning-checkpoints-explained-4972e78f4e56">04 - PostgreSQL 17 Performance Tuning: Checkpoints Explained | by Jeyaram Ayyalusamy | Medium</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#performance`, `#checkpoint`, `#replication`, `#database administration`

---

<a id="item-6"></a>
## [OpenRA 为现代系统重建经典 C&C](https://www.openra.net/) ⭐️ 7.0/10

OpenRA 是一个开源项目，为现代操作系统重建了经典命令与征服游戏（如红色警戒和沙丘 2000），并改进了平衡性和新增功能。 该项目保留了经典即时战略游戏，使其能在当前硬件上运行，同时增强了游戏公平性。其忠实社区维持了这些游戏的活力。 OpenRA 包含重新平衡的单位和地图、现代用户界面以及多人游戏支持。它是免费开源的，在 GitHub 上活跃开发。

hackernews · tosh · 6月27日 12:10 · [社区讨论](https://news.ycombinator.com/item?id=48697560)

**背景**: 命令与征服（C&C）是 1990 年代的经典即时战略系列。OpenRA 是一个粉丝制作的引擎，在不使用原始代码的情况下，以更好的平衡性和更高分辨率等现代增强功能重现了原始游戏。

**社区讨论**: 社区评论普遍积极，赞扬 OpenRA 改进的平衡性和现代功能。一位用户强调火炮现在可以有效对抗特斯拉线圈，另一位指出 EA 容忍该项目甚至开源了老游戏。讨论反映了对游戏保护和社区努力的强烈赞赏。

**标签**: `#open-source`, `#gaming`, `#RTS`, `#strategy games`

---

<a id="item-7"></a>
## [金融科技工程手册引发货币表示方法关键讨论](https://w.pitula.me/fintech-engineering-handbook/) ⭐️ 7.0/10

近期发布的《金融科技工程手册》旨在描述金融科技软件工程中的模式，但很快受到社区批评，认为其内容肤浅且可能有害，尤其是在货币表示方面。 货币表示是金融科技中的基本问题，该讨论强调了能防止代价高昂错误的最佳实践。这场辩论对进入金融科技领域的工程师非常有价值。 该手册建议将货币值存储为整数这一点受到赞扬，但其中关于浮点小数和汇率处理的内容受到批评。社区成员强调使用整数进行存储，并注意货币精度。

hackernews · signa11 · 6月27日 10:28 · [社区讨论](https://news.ycombinator.com/item?id=48696982)

**背景**: 在金融科技中准确表示货币值至关重要；使用浮点数可能因 IEEE 754 限制而引入舍入误差。最佳实践建议将金额存储为整数（例如分），并使用不可变日志进行审计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://w.pitula.me/fintech-engineering-handbook/">Fintech Engineering Handbook</a></li>
<li><a href="https://news.ycombinator.com/item?id=48696982">Fintech Engineering Handbook | Hacker News</a></li>
<li><a href="https://www.ancisoft.com/blog/what-class-to-use-for-money-representation/">What Class to Use for Money Representation? Avoid Rounding ...</a></li>

</ul>
</details>

**社区讨论**: 评论者如 xlii 和 lxgr 强烈建议不要使用浮点数或小单位精度策略存储货币，指出边缘情况和对账挑战。Lanstin 补充说，对账是必不可少的，可以捕捉舍入误差，而 jdw64 则质疑什么才是真正擅长编程。总体情绪是手册肤浅但讨论富有洞察力。

**标签**: `#fintech`, `#engineering`, `#best practices`, `#monetary representation`, `#community discussion`

---

<a id="item-8"></a>
## [PostgreSQL 13 哈希聚合写入磁盘引起回归](https://postgr.es/p/9nt) ⭐️ 7.0/10

PostgreSQL 13 引入了内存安全的哈希聚合功能，允许其将数据溢出到磁盘，但这一变更意外导致某些工作负载在升级后出现查询性能回退。 该回归问题很重要，因为许多 PostgreSQL 用户依赖哈希聚合实现高效的 GROUP BY 操作；升级到 PostgreSQL 13 的数据库管理员可能会在不知原因的情况下遇到性能下降。 该回归问题特别影响哈希表超过可用内存时使用 HashAggregate 的查询，导致优化器选择磁盘溢出策略，该策略可能比 GroupAggregate 等替代方案更慢。

rss · Planet PostgreSQL · 6月27日 01:00

**背景**: PostgreSQL 13 之前的版本中，如果哈希聚合耗尽内存，查询会被中止；13 版通过 `agg_refill_hash_table` 函数分批将数据写入磁盘，使其内存安全。`enable_hashagg` GUC 参数控制优化器是否考虑哈希聚合。`temp_file_limit` 设置也会影响溢出是否导致失败。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/message-id/20190703001753.s5e5cme3ucjgeu6c@development">PostgreSQL: Re: Memory-Bounded Hash Aggregation agg_refill_hash_table - PostgreSQL Symbol Document Re: Spilling hashed SetOps and aggregates to disk - PostgreSQL All Your GUCs in a Row: enable_hashagg — The Build PostgreSQL Temp File Size Threshold Fix | StackEngine PostgreSQL query optimization: avoiding HashAggregate spills PostgreSQL Aggregate and Window Function Tuning - mydba.dev</a></li>
<li><a href="https://ryogrid.github.io/create_pg_super_document/a/agg_refill_hash_table.html">agg_refill_hash_table - PostgreSQL Symbol Document</a></li>
<li><a href="https://www.postgresql.org/message-id/20200409114855.h4hh7e2wt77p56sv@development">PostgreSQL: Re: Default setting for enable_hashagg_disk</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#hash aggregation`, `#database optimization`, `#upgrade`

---

<a id="item-9"></a>
## [前沿 AI 经济学：利润窗口狭窄与基础设施风险](https://simonwillison.net/2026/Jun/26/dean-w-ball/#atom-everything) ⭐️ 7.0/10

Dean W. Ball 指出，前沿 AI 模型在发布后只有很短的窗口期来收回成本，而且大规模基础设施投资假设了一个全球市场，但政府限制可能导致该市场无法实现。 这一分析质疑了当前 AI 行业繁荣的可持续性，对价值数十亿美元的数据中心的经济合理性以及 AI 监管和出口管制的潜在政策影响提出了问题。 Ball 指出，几个月后，前沿模型会变成次前沿模型，竞争出现，利润率压缩。他还引用了前美国 AI 主管 David Sacks 的说法，即基础设施建设对美国经济至关重要，但质疑了对全球可寻址市场的假设。

rss · Simon Willison · 6月26日 22:25

**背景**: 前沿 AI 模型是最先进的通用模型，训练需要巨大的计算预算（约 10^26 次浮点运算），成本高达数百万美元。其经济可行性取决于在被更新模型或竞争超越之前的短时间内收回成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/glossary/frontier-models/">What Are Frontier AI Models and How They Work | NVIDIA Glossary</a></li>
<li><a href="https://thebizanalyst.substack.com/p/the-economics-of-frontier-ai-models">The Economics of Frontier AI models: A Primer</a></li>
<li><a href="https://www.datacamp.com/blog/frontier-models">Frontier Models Explained: What Defines the Cutting Edge of AI | DataCamp</a></li>

</ul>
</details>

**标签**: `#AI economics`, `#frontier models`, `#AI infrastructure`, `#policy`

---

<a id="item-10"></a>
## [6000 次尝试黑客 AI 助手均失败，显示提示注入防御力](https://simonwillison.net/2026/Jun/26/hack-my-ai-assistant/#atom-everything) ⭐️ 7.0/10

费尔南多·伊拉拉扎瓦尔发起了一项挑战：试图通过电子邮件从 OpenClaw AI 助手中窃取秘密的 6000 次尝试全部失败，这表明前沿模型 Opus 4.6 对提示注入攻击具有强大的抵抗力。 这一现实世界的测试表明，前沿模型通过提示注入进行利用的难度显著增加，这是 AI 助手面临的主要安全问题。它为 Claude Opus 4.6 等模型中的安全措施的有效性提供了经验证据。 该挑战花费了 500 美元的代币费用，并因大量入站邮件导致谷歌账户被暂停。模型的系统提示中包含明确的防提示注入指令，测试使用的是 Opus 4.6 变体。

rss · Simon Willison · 6月26日 18:33

**背景**: 提示注入是一种网络安全利用方式，精心设计的输入会使大型语言模型产生非预期行为，绕过安全防护。这种攻击对于能够访问敏感数据或执行操作的 AI 助手尤其危险。该测试突显了 AI 实验室在训练模型抵抗此类攻击方面的持续努力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (language model)</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论线程获得了积极反馈，既有合理的怀疑，也有作者费尔南多的真诚回应。许多评论者讨论了测试的局限性及其对 AI 安全的更广泛影响。

**标签**: `#AI security`, `#prompt injection`, `#language models`, `#AI safety`

---