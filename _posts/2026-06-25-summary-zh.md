---
layout: default
title: "Horizon 日报：2026-06-25 (ZH)"
date: 2026-06-25
lang: zh
---

> 从 52 条内容中筛选出 14 条重要资讯。

---

1. [OpenAI 与博通联合推出首款自研 AI 芯片“Jalapeño”](#item-1) ⭐️ 9.0/10
2. [Krea 2：开源权重 12B 文生图模型发布](#item-2) ⭐️ 9.0/10
3. [使用 JAX 和 Vision Transformer 的自对弈强化学习智能体在 Generals.io 中超越人类](#item-3) ⭐️ 9.0/10
4. [Anthropic 指控阿里巴巴非法提取 Claude AI 模型能力](#item-4) ⭐️ 8.0/10
5. [高通以 40 亿美元收购 AI 初创公司 Modular](#item-5) ⭐️ 8.0/10
6. [微软 Agent Experience 系列：处理未见过的代码](#item-6) ⭐️ 7.0/10
7. [PostgreSQL 新配置优化 GROUP BY 和 DISTINCT](#item-7) ⭐️ 7.0/10
8. [AI 智能体架构：超越记忆，迈向规划、工具与反思](#item-8) ⭐️ 7.0/10
9. [PostgreSQL 的计算与存储分离之路](#item-9) ⭐️ 7.0/10
10. [不要更改 PostgreSQL checkpoint_timeout，应设置告警](#item-10) ⭐️ 7.0/10
11. [pg_clickhouse 0.3.2 新增对 PostgreSQL 19 Beta1 的支持](#item-11) ⭐️ 7.0/10
12. [Tomas Vondra 分享关于 random_page_cost 的最新思考](#item-12) ⭐️ 7.0/10
13. [Tom MacWright：LLM 生成的求职申请无法展现求职者特质](#item-13) ⭐️ 7.0/10
14. [Datasette 1.0a35 新增模式管理 JSON API](#item-14) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [OpenAI 与博通联合推出首款自研 AI 芯片“Jalapeño”](https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/) ⭐️ 9.0/10

OpenAI 与博通联合发布了专为大语言模型设计的定制 AI 推理芯片“Jalapeño”，从设计到量产仅用九个月，由台积电代工。 这标志着 OpenAI 首次涉足定制芯片领域，通过垂直整合可减少对英伟达等 GPU 供应商的依赖，并显著提升推理效率与成本效益。 “Jalapeño”芯片是一款专为 OpenAI 的 LLM 工作负载优化的纯推理处理器，其开发部分借助了 OpenAI 自身模型加速设计与优化过程。该芯片整合了博通的网络方案和 Celestica 的系统集成。

hackernews · jamdesk · 6月24日 17:47 · [社区讨论](https://news.ycombinator.com/item?id=48663324)

**背景**: AI 推理芯片是专门用于高效运行已训练模型的处理器，不同于侧重计算吞吐量的训练芯片。定制芯片能让企业根据自身模型架构定制硬件，相比通用 GPU 可能实现更高的能效比和更低的延迟。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/openai-broadcom-jalapeno-inference-chip/">OpenAI and Broadcom unveil LLM-optimized inference chip</a></li>
<li><a href="https://www.cnbc.com/2026/06/24/openai-and-broadcom-reveal-jalapeno-first-ai-chip-in-partnership.html">OpenAI and Broadcom reveal Jalapeno, first AI chip in partnership - CNBC</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：部分评论者对声称的 AI 加速设计流程表示怀疑，认为可能只是营销噱头；也有评论者确认了台积电代工等制造细节。此外还有技术讨论，比如将权重固化到硅片中以实现极致吞吐量的替代方案。

**标签**: `#AI`, `#hardware`, `#OpenAI`, `#custom silicon`, `#inference`

---

<a id="item-2"></a>
## [Krea 2：开源权重 12B 文生图模型发布](https://www.krea.ai/blog/krea-2-technical-report) ⭐️ 9.0/10

Krea AI 发布了 Krea 2，这是一个拥有 120 亿参数、开源权重的文生图扩散模型，并附有详尽的技术报告，涵盖数据整理、架构和训练流程。模型提供两个版本：标准版 Krea 2 以及经过引导和时间步蒸馏的 Krea 2 Turbo，可实现更快的推理速度。 作为最先进的开源权重图像生成模型，Krea 2 使开发者和研究人员能在本地运行高质量文生图，减少对封闭 API 的依赖。详尽的技术报告分享了数据整理、训练基础设施和后训练管线等方面的见解，推动了开放研究。 模型权重以宽松许可证形式发布在 Hugging Face 和 GitHub 上，Turbo 变体仅需 8 步推理即可取得出色效果。技术报告深入探讨了分布式训练基础设施、用于提示扩展的强化学习管线等鲜有详细讨论的主题。

hackernews · mattnewton · 6月23日 15:31 · [社区讨论](https://news.ycombinator.com/item?id=48646659)

**背景**: 文生图扩散模型通过迭代去噪随机噪声，从自然语言描述生成图像。开源权重模型允许研究人员和开发者在自己的硬件上检查、修改和部署模型，促进了 AI 研究的透明性和可复现性。Krea 2 延续了这一趋势，加入了 Stable Diffusion 和 FLUX 等其他开源模型的行列。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.krea.ai/blog/krea-2-technical-report">Krea 2 Technical Report - Krea</a></li>
<li><a href="https://github.com/krea-ai/krea-2">GitHub - krea-ai/krea-2: Official inference code for Krea 2</a></li>
<li><a href="https://news.ycombinator.com/item?id=48646659">Krea 2 : SOTA open-weights 12B image model | Hacker News</a></li>

</ul>
</details>

**社区讨论**: Hacker News 社区反响积极，许多人称赞详尽的技术报告和开源权重的发布。用户指出 Krea 2 Turbo 在可本地部署的模型中表现出色，但也有人认为它仍不如 Ideogram 4 等专有模型。作者积极在评论区回答问题，增强了互动。

**标签**: `#image generation`, `#open-source`, `#text-to-image`, `#deep learning`, `#technical report`

---

<a id="item-3"></a>
## [使用 JAX 和 Vision Transformer 的自对弈强化学习智能体在 Generals.io 中超越人类](https://www.reddit.com/r/MachineLearning/comments/1uei2yg/i_made_a_superhuman_generalsio_agent_with/) ⭐️ 9.0/10

一个使用 JAX 和 Vision Transformer 架构重新实现的自对弈强化学习智能体，在 Generals.io 的 1v1 排行榜上达到了超越人类的水平并排名第一。整个流程（包括快速的 JAX 模拟器）已开源，并附有详细的博客指南。 这项工作表明，通过 Vision Transformer 和 JAX 扩展模型容量和计算效率可以超越人工设计的先验知识。开源发布为研究不完美信息实时策略游戏的研究人员和开发者提供了宝贵资源。 智能体从 NumPy/Torch 重新实现为 JAX，并将架构从 CNN 切换为 Vision Transformer，专注于扩展而非临时修补。博客详细介绍了死胡同、决策依据和实用技巧，JAX 模拟器可独立作为 RTS 环境使用。

reddit · r/MachineLearning · /u/shrekofspeed · 6月24日 16:18

**背景**: Generals.io 是一款快节奏的多人战略游戏，玩家需要占领领土并击败对手。自对弈强化学习通过让智能体与自身副本对战来逐步提升。JAX 是一个用于机器学习的高性能数值计算库，Vision Transformer（ViT）将 transformer 自注意力机制应用于图像块，是卷积神经网络的一种替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://www.generals.io/">generals.io</a></li>
<li><a href="https://en.wikipedia.org/wiki/JAX_(software)">JAX (software) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vision_transformer">Vision transformer - Wikipedia</a></li>

</ul>
</details>

**标签**: `#reinforcement learning`, `#self-play`, `#game AI`, `#JAX`, `#vision transformer`

---

<a id="item-4"></a>
## [Anthropic 指控阿里巴巴非法提取 Claude AI 模型能力](https://www.reuters.com/world/china/anthropic-says-alibaba-illicitly-extracted-claude-ai-model-capabilities-2026-06-24/) ⭐️ 8.0/10

Anthropic 指控阿里巴巴通过模型蒸馏技术从其 Claude AI 模型中提取能力，并以低于成本的价格转售提取后的模型访问权限。 此案凸显了人工智能领域新兴的知识产权纠纷，尤其是在模型蒸馏方面，并可能为全球范围内如何保护与许可 AI 模型能力树立先例。 据报道，中国转售商通过合并账户、支付欺诈以及将模型输出和推理链作为训练数据转售，以比 Anthropic 官方 API 价格低 70-90% 的价格提供 Claude 代币。Anthropic 称这种做法为非法蒸馏。

hackernews · htrp · 6月24日 19:48 · [社区讨论](https://news.ycombinator.com/item?id=48664814)

**背景**: 模型蒸馏是一种技术，通过让较小的“学生”模型学习较大的“教师”模型的输出来模仿其性能，且成本更低。Claude 是 Anthropic 开发的最先进的大型语言模型。AI 公司通常抓取公开网页数据用于训练，但从竞争对手的模型中提取能力用于商业转售引发了法律和伦理问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (language model ) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论褒贬不一：有人将此次指控比作历史上的知识产权纠纷（例如苹果 vs. 施乐），指出 Anthropic 本身也在未经许可的情况下使用网络数据训练 Claude。也有人将蒸馏视为巧妙利用漏洞，认为并无不妥。

**标签**: `#AI`, `#model distillation`, `#intellectual property`, `#Anthropic`, `#Alibaba`

---

<a id="item-5"></a>
## [高通以 40 亿美元收购 AI 初创公司 Modular](https://www.reuters.com/business/qualcomm-buy-ai-startup-modular-2026-06-24/) ⭐️ 8.0/10

2026 年 6 月 24 日，高通宣布以 40 亿美元收购 AI 基础设施初创公司 Modular，旨在强化其 AI 软件栈并扩展至基于 RISC-V 的处理器。 此次收购使高通能在 AI 推理和数据中心市场与英伟达竞争，同时加速其从 ARM 架构向开源 RISC-V 架构的转移。 这笔 40 亿美元的交易使高通获得 Modular 的 MAX 推理引擎和 Mojo 编程语言，但部分观察人士指出，Modular 创始人此前曾批评硬件公司未能构建有效的 AI 软件栈。

hackernews · timmyd · 6月24日 13:49 · [社区讨论](https://news.ycombinator.com/item?id=48659798)

**背景**: Modular 是由 Chris Lattner（LLVM、Clang 和 Swift 的创建者）创立的 AI 基础设施初创公司，开发了面向 AI 工作负载的类 Python 语言 Mojo。RISC-V 是一种免费开放标准的指令集架构（ISA），正逐渐成为专有 ARM 和 x86 架构的替代方案。高通的收购符合其从移动芯片向 AI 和边缘计算多元化的战略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/06/24/qualcomm-ai-chip-modular-software.html">Qualcomm inks deal for AI startup Modular to bolster software ...</a></li>
<li><a href="https://www.modular.com/company/about">Modular: About Us</a></li>
<li><a href="https://en.wikipedia.org/wiki/RISC-V_architecture">RISC-V architecture</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些人认为此举对高通的 RISC-V 和 AI 战略具有合理性，而另一些人则质疑协同效应，因为 Modular 创始人曾批评硬件公司的 AI 软件栈，且高通当前产品组合与英伟达主导的高端 AI 推理市场存在差距。

**标签**: `#acquisition`, `#AI`, `#Qualcomm`, `#Modular`, `#RISC-V`

---

<a id="item-6"></a>
## [微软 Agent Experience 系列：处理未见过的代码](https://devblogs.microsoft.com/blog/when-the-model-has-never-seen-your-code) ⭐️ 7.0/10

微软发布了其 Agent Experience（AX）系列中的第五篇文章，聚焦于如何让 AI 编程代理有效处理从未见过的代码库，包括测量和迭代策略。 这很重要，因为实际代码库与训练数据不同，开发者需要实用指导来确保 AI 代理在其特定环境中可靠且有用，从而提高生产力并减少错误。 该文章是一个系列的一部分，涵盖了代理堆栈中可控的方面、如何衡量自定义扩展的影响以及迭代以获得更好的结果。摘要中未提供具体的技术细节或代码示例。

rss · Microsoft for Developers · 6月24日 14:04

**背景**: Agent Experience（AX）是关于创建 AI 代理可以有效解释和操作的数字环境。AI 编程代理是基于自然语言指令自主规划、编写、测试和调试代码的系统，不同于传统助手仅建议代码片段。微软的这个系列旨在帮助开发者优化使用此类代理的工作流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.synclovis.com/articles/what-is-agent-experience-ax-in-ai-and-why-it-matters-to-you/">What Is Agent Experience ( AX ) in AI – And Why... - Synclovis Systems</a></li>
<li><a href="https://cloud.google.com/discover/what-is-agentic-coding">What is agentic coding? How it works and use cases</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#developer experience`, `#code generation`, `#AI-assisted programming`, `#machine learning`

---

<a id="item-7"></a>
## [PostgreSQL 新配置优化 GROUP BY 和 DISTINCT](https://postgr.es/p/9nj) ⭐️ 7.0/10

PostgreSQL 17 和 18 引入了两个新的配置参数：enable_group_by_reordering 和 enable_distinct_reordering，它们允许查询规划器重新排序 GROUP BY 和 DISTINCT 的键，以匹配已有的排序顺序，从而降低比较开销并消除不必要的排序。 这些优化无需修改模式即可显著提升聚合和去重操作的查询性能，受益于调优 PostgreSQL 工作负载的 DBA 和开发者。 enable_group_by_reordering 在 PostgreSQL 17 中添加，而 enable_distinct_reordering 更新，在 PostgreSQL 18 中引入；两者默认启用，如果重新排序导致次优计划，可以禁用。

rss · Planet PostgreSQL · 6月25日 01:00

**背景**: PostgreSQL 的查询规划器可以为 GROUP BY 选择哈希聚合或分组聚合。分组聚合要求输入按分组键排序；以前，它按查询中指定的顺序比较键，如果顺序与可用索引不匹配，可能开销很大。新的 GUC 允许规划器重新排序键以匹配索引的自然顺序，从而避免显式排序并降低比较开销。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thebuild.com/blog/all-your-gucs-in-a-row-enabledistinctreordering-and-enablegroupbyreordering/">All Your GUCs in a Row: enable_distinct_reordering and enable_group_by ...</a></li>
<li><a href="https://pgpedia.info/e/enable_distinct_reordering.html">enable_distinct_reordering - pgPedia - a PostgreSQL Encyclopedia</a></li>
<li><a href="https://blog.anayrat.info/en/2024/01/26/group-by-reordering/">New feature in PostgreSQL 17: GROUP BY reordering</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database optimization`, `#SQL`, `#query performance`, `#GUC`

---

<a id="item-8"></a>
## [AI 智能体架构：超越记忆，迈向规划、工具与反思](https://postgr.es/p/9ni) ⭐️ 7.0/10

Vibhor Kumar 指出，仅靠记忆不足以支撑企业级 AI 智能体，规划、工具使用和反思才是执行业务流程的关键。文章提供了具体指导：将执行计划视为可持久化的工件、设计安全的工具接口、并在运行前定义成功标准。 这一观点将 AI 智能体的开发从无状态对话系统转向可审计的企业级参与者。它澄清了关于工具设计和反思的常见误解，帮助从业者避免脆弱的即兴发挥，构建适合生产部署的系统。 关键原则包括：将执行计划视为可版本化、可暂停的工件；绝不允许模型对生产数据生成并执行任意 SQL；在智能体运行前定义“好”与“坏”的结果。文章全程以 PostgreSQL 为例说明企业级智能体模式。

rss · Planet PostgreSQL · 6月24日 16:30

**背景**: AI 智能体将大语言模型与记忆、规划、工具使用和反思等能力相结合来执行任务。记忆提供上下文，规划将目标分解为步骤，工具与外部系统交互，反思则允许自我修正。许多早期智能体实现缺乏稳健的规划和安全护栏，导致在企业环境中行为不可靠。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mayursurani.medium.com/the-reflection-pattern-how-ai-agents-learn-from-themselves-239ce164aa14">The Reflection Pattern: How AI Agents Learn from... | Medium</a></li>
<li><a href="https://www.agentik-os.com/glossary/reflection-agent">Reflection Agent — AI Glossary | Agentik {OS}</a></li>
<li><a href="https://www.eduhubspot.com/blogs/pmp/project-planning-to-execution-how-project-management-artifacts-shape-the-Journey-for-success">From Project Planning to Execution: How Project Artifacts ...</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#planning`, `#tool use`, `#reflection`, `#enterprise systems`

---

<a id="item-9"></a>
## [PostgreSQL 的计算与存储分离之路](https://postgr.es/p/9ng) ⭐️ 7.0/10

Shaun Thomas 的文章探讨了在 PostgreSQL 中实现分层存储的挑战和多种方法，即通过将计算与存储分离，将冷数据迁移到廉价的对象存储，同时将热数据保留在本地。 这解决了数据库中存储成本管理的关键问题，使得资源利用更高效，并可能使 PostgreSQL 成为能够统一查询本地和远程任意规模数据的引擎。 文章审视了声明式分区、表空间、外部数据包装器和表访问方法等技术，以及 Parquet 和 Iceberg 等列式格式，并提到 Neon 作为完全替换存储引擎的示例。

rss · Planet PostgreSQL · 6月24日 10:05

**背景**: 传统数据库将所有数据存储在昂贵的块存储上，即使是很少访问的冷数据也不例外。计算与存储分离意味着将查询处理层与数据存储层分开，从而允许将数据存储在更廉价的对象存储上。分层存储会自动将冷数据迁移到更便宜的存储，同时将热数据保留在快速的本地存储上。像 Parquet 和 Iceberg 这样的列式存储格式通过按列而非按行存储数据来优化分析查询。

**标签**: `#PostgreSQL`, `#storage tiering`, `#compute-storage separation`, `#columnar storage`

---

<a id="item-10"></a>
## [不要更改 PostgreSQL checkpoint_timeout，应设置告警](https://postgr.es/p/9ne) ⭐️ 7.0/10

Jeremy Schneider 建议不要增加 PostgreSQL 默认的 5 分钟 checkpoint_timeout，警告这会延长故障恢复时间。他建议启用 log_checkpoints 并设置总检查点时间超过 15 分钟的告警。 这一指导帮助数据库管理员避免常见错误配置，防止短暂宕机演变为数小时的灾难。正确监控检查点对于数据库可用性和满足恢复时间目标至关重要。 告警可以通过解析日志中的检查点消息或检查距离上次检查点消息的时间来构建，后者更为稳健。Schneider 还警告不要在有检查点问题的情况下重启数据库，正如一次 40 小时宕机事件所示。

rss · Planet PostgreSQL · 6月24日 08:20

**背景**: PostgreSQL 检查点将脏页从缓存写入磁盘，并管理其他任务如 fsync 批处理和 archive_timeout 的强制执行。增加 checkpoint_timeout 会降低检查点频率，但会增加恢复时间（RTO），因为崩溃后需要重放更多 WAL。log_checkpoints 自 PostgreSQL 15 起默认启用，用于记录检查点活动以便监控。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.rockdata.net/tutorial/tune-checkpoints/">PostgreSQL Tutorial: Tuning Checkpoints - Redrock Postgres</a></li>
<li><a href="https://runebook.dev/en/docs/postgresql/runtime-config-wal/GUC-CHECKPOINT-TIMEOUT">PostgreSQL checkpoint _ timeout : Common Issues and Solutions</a></li>
<li><a href="https://pgpedia.info/l/log_checkpoints.html">log_checkpoints - pgPedia - a PostgreSQL Encyclopedia</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#checkpoint`, `#database administration`, `#performance tuning`, `#RTO`

---

<a id="item-11"></a>
## [pg_clickhouse 0.3.2 新增对 PostgreSQL 19 Beta1 的支持](https://postgr.es/p/9nc) ⭐️ 7.0/10

pg_clickhouse 0.3.2 现在支持 PostgreSQL 19 Beta1，并改进了 TLS 连接、正则表达式下推和二进制协议压缩。该版本还包含各种错误修复，并为最终的 PostgreSQL 19 版本做好准备。 此更新确保将 PostgreSQL 与 ClickHouse 集成的用户能够从第一天起就利用最新的 PostgreSQL 19 功能。它加强了事务工作负载与分析工作负载之间的桥梁，使依赖实时分析的数据工程师和分析师受益。 该扩展需要对源代码进行小幅修改，以适应 PostgreSQL 19 的元组和数组优化、移除旧类型定义以及添加新头文件。该版本可在 PGXN、GitHub 和 Docker 上获取。

rss · Planet PostgreSQL · 6月23日 16:14

**背景**: pg_clickhouse 是一个 PostgreSQL 扩展，允许直接从 PostgreSQL 查询 ClickHouse（一种分析型数据库）。它使用户能够运行 SQL 查询，将分析操作无缝下推到 ClickHouse 以加快处理速度。这种集成对于混合事务/分析处理（HTAP）场景特别有用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://clickhouse.com/docs/integrations/postgresql">PostgreSQL | ClickHouse Docs</a></li>
<li><a href="https://clickhouse.com/blog/introducing-pg_clickhouse">Introducing pg_clickhouse: A Postgres extension for querying ClickHouse</a></li>
<li><a href="https://github.com/ClickHouse/pg_clickhouse">GitHub - ClickHouse/pg_clickhouse: Interfaces to query ClickHouse databases from PostgreSQL · GitHub</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#ClickHouse`, `#pg_clickhouse`, `#database`, `#extension`

---

<a id="item-12"></a>
## [Tomas Vondra 分享关于 random_page_cost 的最新思考](https://postgr.es/p/9na) ⭐️ 7.0/10

Tomas Vondra 发布了一篇更新，继之前在 POSETTE 会议上的演讲和社区讨论之后，重新思考了 PostgreSQL 中 random_page_cost 参数的调整，以反映现代存储的特性。 这一讨论对数据库管理员和数据库工程师非常重要，因为调整 random_page_cost 可以大幅提升查询计划的质量，尤其是在现代 SSD 和 NVMe 存储上，默认值已经过时。 Vondra 之前的文章建议将 random_page_cost 从默认值 4 调低，而本次更新很可能基于新的见解对该建议进行了细化。该演讲是为 POSETTE 2026 预先录制的。

rss · Planet PostgreSQL · 6月23日 09:00

**背景**: 在 PostgreSQL 中，random_page_cost 参数影响查询规划器对随机 I/O 与顺序 I/O 成本的估计。默认值 4 假设的是类似机械硬盘的行为，但现代 SSD 的随机访问延迟远低于此，因此调整该参数可以带来更好的索引使用和更快的查询。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pganalyze.com/blog/5mins-postgres-tuning-random-page-cost">Tuning random_page_cost and how index correlation affects ... - pganalyze</a></li>
<li><a href="https://www.postgresql.org/docs/current/runtime-config-query.html">PostgreSQL: Documentation: 18: 19.7. Query Planning</a></li>
<li><a href="https://www.scality.com/topics/what-is-sequential-vs-random-io/">What is Sequential vs Random I/O? - scality.com</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database tuning`, `#storage`, `#performance`

---

<a id="item-13"></a>
## [Tom MacWright：LLM 生成的求职申请无法展现求职者特质](https://simonwillison.net/2026/Jun/24/tom-macwright/#atom-everything) ⭐️ 7.0/10

Tom MacWright 观察到，最近许多求职申请明显由 LLM 共同撰写，附带的个人作品集、GitHub 项目和提交信息也都是 LLM 生成的，这些内容千篇一律，无法展现申请者的个性或技能。 这凸显了一个日益严重的问题：AI 生成的内容削弱了招聘中的真实性，使雇主更难评估真正的候选人，并可能贬低申请中的人类努力。 MacWright 指出，这些申请是通用且非个人化的，只透露出申请者对某些工具的熟悉度，而他觉得无法了解申请背后的这个人。

rss · Simon Willison · 6月24日 18:13

**背景**: LLM（大型语言模型，如 GPT-4）越来越多地被用于生成简历、求职信和代码。虽然它们可以节省时间，但过度依赖会导致内容缺乏个人风格和原创性，在重视真实性的招聘环境中可能适得其反。

**标签**: `#ai`, `#careers`, `#hiring`, `#llm`, `#authenticity`

---

<a id="item-14"></a>
## [Datasette 1.0a35 新增模式管理 JSON API](https://simonwillison.net/2026/Jun/23/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a35 引入了新的“创建表”和“修改表”JSON API 来管理数据库模式。该版本还添加了全面的模板上下文文档，作为稳定的 API。 这些 API 允许在 Datasette 中以编程方式修改模式，使其成为更强大的数据探索和管理工具。模板上下文文档稳定了自定义模板开发，使整个 Datasette 生态系统受益。 “创建表”API 支持定义列、主键、自定义类型、约束、默认值和单列外键。“修改表”API 允许添加、重命名、重新排序、删除列，以及更改类型、默认值和约束，还包括一个“删除表”按钮。

rss · Simon Willison · 6月23日 21:34

**背景**: Datasette 是一个用于探索和发布 SQLite 数据库的开源工具。在此版本之前，模式更改需要手动执行 SQL 命令或使用外部工具。新的 JSON API 将模式管理直接引入 Datasette 的界面和 API，简化了数据库管理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.datasette.io/en/latest/json_api.html">JSON API - Datasette documentation</a></li>
<li><a href="https://simonwillison.net/2026/Jun/23/datasette/">Release: datasette 1.0a35 - simonwillison.net</a></li>

</ul>
</details>

**标签**: `#datasette`, `#sqlite`, `#data-exploration`, `#json-api`, `#open-source`

---