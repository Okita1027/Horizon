---
layout: default
title: "Horizon 日报：2026-08-15 (ZH)"
date: 2026-08-15
lang: zh
---

> 从 34 条内容中筛选出 9 条重要资讯。

---

1. [GLM-5.3 亮相：顶尖编程能力与新兴网络攻击能力](#item-1) ⭐️ 9.0/10
2. [Qwen 3.8 27B 发布：本地推理能力表现出色](#item-2) ⭐️ 8.0/10
3. [走向黑暗：执法黑客的时代来临](#item-3) ⭐️ 8.0/10
4. [RISC-V 设计批评：重蹈过往 ISA 覆辙？](#item-4) ⭐️ 8.0/10
5. [Firefox 成为目前唯一支持完整版 uBlock Origin 的主要浏览器](#item-5) ⭐️ 8.0/10
6. [不要分类，要幻觉：用嵌入映射 LLM 生成的标签](#item-6) ⭐️ 8.0/10
7. [构建 Postgres 扩展以估算查询内存使用量](#item-7) ⭐️ 7.0/10
8. [诊断 pg_stat_statements 中的高基数工作负载：第 6 期](#item-8) ⭐️ 7.0/10
9. [pg_walviz：PostgreSQL WAL 段可视化新工具](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [GLM-5.3 亮相：顶尖编程能力与新兴网络攻击能力](https://z.ai/blog/glm-5.3) ⭐️ 9.0/10

Z.ai 发布了开源旗舰模型 GLM-5.3，展现了前沿的编程表现，并具备自动发现和利用漏洞的新兴网络能力。该版本基于 GLM-5.2 的基础模型，仅通过后训练改进，在 Terminal-Bench 3.0 和 Agents' Last Exam (CLI) 上取得了开源最优结果。 这标志着开源权重模型在进入安全敏感领域方面迈出了重要一步，可能降低防御性安全研究和恶意使用的门槛。其网络能力可能重塑红队测试、漏洞披露以及关于 AI 双重用途的 AI 安全讨论。 根据 Z.ai 文档，GLM-5.3 与 GLM-5.2 使用相同的基础模型，全部提升来自后训练，在 Z.ai Code Bench 上比 GLM-5.2 提升 50%。社区报告提到了真实的红队执行和 cvd.z.ai 上的漏洞披露门户，还与其他前沿模型（如“Sol and Fable”）进行了比较。

hackernews · pella · 8月14日 05:19 · [社区讨论](https://news.ycombinator.com/item?id=49294997)

**背景**: GLM 是 Z.ai 的开放权重大语言模型系列，历来与闭源模型竞争，同时保持免费可用。LLM 中新兴的网络能力是一个日益增长的研究领域，因为模型学会了编写漏洞利用代码、发现漏洞并协助渗透测试，引发了对双重使用的担忧。后训练（如 RLHF 和指令微调等技术）正日益成为共享同一基础模型的模型之间性能差距的主要驱动因素。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.z.ai/guides/llm/glm-5.3">GLM-5.3 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://openlm.ai/glm-5.1/">GLM-5.3 | OpenLM.ai</a></li>
<li><a href="https://arxiv.org/html/2405.03644v1">When LLMs Meet Cybersecurity: A Systematic Literature Review</a></li>

</ul>
</details>

**社区讨论**: 社区反应整体上印象深刻但保持谨慎：用户报告了成功的红队操作（包括插件 0-day 和内核漏洞利用的适配），还有人称赞其文案风格，并指出它仍略逊于“Sol and Fable”。一些用户讨论经济激励和本地量化，一位评论者强调 cvd.z.ai 上正在进行的漏洞扫描规模。

**标签**: `#AI`, `#LLM`, `#Cybersecurity`, `#GLM`, `#Frontier Models`

---

<a id="item-2"></a>
## [Qwen 3.8 27B 发布：本地推理能力表现出色](https://huggingface.co/Qwen/Qwen3.8-27B-FP8) ⭐️ 8.0/10

Qwen 3.8 27B 是 Qwen 3.8 系列新发布的稠密视觉语言模型，已在 Hugging Face 上开源，定位为可本地部署。早期社区测试显示，它是在 Gemma 4 之后第二个能正确通过某用户私有推理基准测试的本地模型。 这一发布意义重大，因为它在可本地运行的模型规模上带来了强大的推理与编程能力，为开发者和研究人员提供了比超大模型或托管服务更实用的选择。社区反响热烈，表明 Qwen 3.8 27B 可能成为端侧及隐私敏感 AI 工作流的标准工具。 根据 Hugging Face 上的说明，Qwen3.8-27B 使用 Qwen3.5 架构，并采用固定的逐步推理提示词进行评估；它支持灵活的思考控制，并在多步智能体任务上具备更强的执行能力。社区成员报告称，在 RTX 5090 上用 ninfer 推理引擎可获得约 138 tokens/秒，约为朴素 llama.cpp 配置的两倍。

hackernews · erdaltoprak · 8月14日 15:00 · [社区讨论](https://news.ycombinator.com/item?id=49299605)

**背景**: Qwen 是阿里巴巴推出的开源模型系列，3.8 代继续聚焦编程、专业工作、研究以及长时程智能体任务。27B 模型尺寸更紧凑、更便于部署，因此很适合在没有云端 API 的情况下在消费级笔记本和工作站上运行。视觉语言模型能够同时处理文本与图像输入，这也解释了用户用“骑自行车的鹈鹕”等生成图像进行测试的缘由。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen/Qwen3.8-27B · Hugging Face</a></li>
<li><a href="https://lmstudio.ai/models/qwen/qwen3.8-27b">qwen/qwen3.8-27b • LM Studio</a></li>
<li><a href="https://www.amd.com/en/blogs/2026/run-qwen-3-8-27b-on-amd-ryzen-ai-max-and-radeon-graphics-cards-day-0.html">Run Qwen 3.8 27B on AMD Ryzen™ AI Max Agentic PCs and Radeon ™ GPUs</a></li>

</ul>
</details>

**社区讨论**: 社区反馈非常积极，有用户称赞 Qwen 3.8 27B 是“在笔记本可运行模型里见过的最棒鹈鹕”，并指出其思维链采用笔记体，与 Qwen 3.6 明显不同。还有用户分享了硬件相关的观察，例如在 RTX 5090 上使用 ninfer 可将吞吐量翻倍，以及相比 Gemma 4 其显存占用更高。

**标签**: `#AI`, `#LLM`, `#Qwen`, `#Local Models`, `#Machine Learning`

---

<a id="item-3"></a>
## [走向黑暗：执法黑客的时代来临](https://blog.cryptographyengineering.com/2026/08/14/everything-is-about-to-go-dark/) ⭐️ 8.0/10

在一篇新的博客文章中，Matthew Green 指出，随着加密技术的普及，执法机构正从电话窃听转向主动黑客攻击。他质疑这一做法是否可持续，因为可利用的软件漏洞数量是有限的。 这一分析意义重大，因为它揭示了长期“走向黑暗”争论中的重大政策转向：与要求后门不同，联邦调查局等机构越来越多地通过黑客手段进入设备和网络。它还引发了关于漏洞披露、漏洞储备以及关键系统安全性的关键问题。 文章借鉴了历史上的窃听实践和 CALEA（通信协助执法法案）框架，来描述当前向“合法黑客”的转变。文章警告说，为执法目的创建的新后门最终可能削弱美国自身的系统，并被外国对手利用。

hackernews · vslira · 8月14日 20:52 · [社区讨论](https://news.ycombinator.com/item?id=49304447)

**背景**: “走向黑暗”问题指的是执法机构有权合法访问加密通信，但缺乏技术手段的情况。从历史上看，像 CALEA 这样的法律要求运营商为窃听提供便利，但不强制解密。随着加密成为消费产品的默认设置，联邦调查局等机构越来越多地转向利用漏洞和黑客攻击，而不是削弱加密。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://carnegieendowment.org/research/2024/04/exploring-law-enforcement-hacking-as-a-tool-against-transnational-cyber-crime">Exploring Law Enforcement Hacking as a Tool Against Transnational Cyber ...</a></li>
<li><a href="https://repository.law.umich.edu/mjlr/vol50/iss2/5/">"Shedding Light on the "Going Dark" Problem and the Encryption Debate" by John Mylan Traylor</a></li>
<li><a href="https://www.fbi.gov/news/testimony/going-dark-encryption-technology-and-the-balances-between-public-safety-and-privacy">Going Dark: Encryption, Technology, and the Balances Between Public Safety and Privacy | Federal Bureau of Investigation</a></li>

</ul>
</details>

**社区讨论**: 评论者意见不一：有人指出，由于 AI 生成的代码，软件漏洞的数量正在增加，对“有用漏洞正在减少”的说法提出质疑。还有人担心政府行为者在开源项目中植入后门，一位读者则分享了计算机化之前物理窃听成本高昂的历史轶事。

**标签**: `#security`, `#privacy`, `#law-enforcement`, `#encryption`, `#hacking`

---

<a id="item-4"></a>
## [RISC-V 设计批评：重蹈过往 ISA 覆辙？](https://dmitry.gr/?r=06.%20Thoughts&proj=12.%20RV) ⭐️ 8.0/10

在一篇新的技术文章中，嵌入式工程师 Dmitry Grinberg 认为 RISC-V 的指令集设计重蹈了 MIPS 等早期 ISA 的覆辙。这篇文章在 Hacker News 上引发了 50 条评论的讨论，争论该批评是否成立，以及开放标准本身的价值。 RISC-V 已成为最重要的开源硬件项目之一，由拥有超过 4500 名成员的 RISC-V International 支持。这项批评之所以重要，是因为基础 ISA 中的设计缺陷日后修复成本高昂，而这场辩论也在影响社区如何权衡架构纯正性与免专利标准带来的好处。 该文章认为 RISC-V 的压缩指令编码、基础整数 ISA 和扩展机制引入了不必要的复杂性和低效问题，与 MIPS 的失误类似。评论者提到了实际难题，例如为了启动 Ubuntu 等常见 Linux 发行版，需要从 RV64IMA 扩展到 RV64GC，甚至引入软浮点库。

hackernews · kaycebasques · 8月14日 22:38 · [社区讨论](https://news.ycombinator.com/item?id=49305492)

**背景**: 指令集架构（ISA）定义了软件与 CPU 之间的接口，使不同实现之间能够保持二进制兼容。RISC-V 是一个自由开放的 ISA，2010 年由加州大学伯克利分校创建，现由非营利组织 RISC-V International 维护；与专有的 x86 和 ARM 不同，实现它无需支付专利费。虽然 RISC-V 广泛用于嵌入式系统，但其不断壮大的生态意味着指令集层面的决策会产生长期影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RISC-V_architecture">RISC-V architecture</a></li>
<li><a href="https://en.wikipedia.org/wiki/Instruction_set_architecture">Instruction set architecture</a></li>

</ul>
</details>

**社区讨论**: 评论者大体上认同部分批评：wren6991 称这些观点“基本切中要害”，尽管 RISC-V 对业余 CPU 设计者来说仍可用；kev009 称之为“基本上是 MIPS 重演”。另一些人如 bjornnn 反驳说，RISC-V 的历史意义在于它是一个开放、无专利束缚的标准，而非技术上的优越；Retr0id 则分享亲身经历，展示扩展泛滥如何使实际使用变得更复杂。

**标签**: `#RISC-V`, `#ISA`, `#CPU architecture`, `#open hardware`, `#technology critique`

---

<a id="item-5"></a>
## [Firefox 成为目前唯一支持完整版 uBlock Origin 的主要浏览器](https://www.pcworld.com/article/3212428/firefox-is-now-the-last-major-browser-that-still-supports-ublock-origin.html) ⭐️ 8.0/10

随着 Chrome、Edge 等基于 Chromium 的浏览器完成向 Manifest V3 的迁移，完整版 uBlock Origin 在这些浏览器中已无法使用。Firefox 成为最后一个仍支持基于 webRequest 的完整版 uBlock Origin 的主要浏览器。 这使 Firefox 成为需要强大实时广告拦截和隐私保护用户的默认选择。同时也加剧了 Google 更严格的扩展模型与 Firefox 更开放做法之间的分化，可能推动注重隐私的用户转向 Firefox。 在 Manifest V3 下，具有拦截能力的 webRequest API 受到限制，因此 uBlock Origin 只能依赖功能较弱的 declarativeNetRequest 替代方案，或仅能作为企业策略扩展安装。用户可尝试 uBlock Origin Lite 或非官方 MV3 移植版（如 r58Playz/uBlock-mv3），但这些方案相比 Firefox 版本都有所限制。

hackernews · DemiGuru · 8月14日 19:03 · [社区讨论](https://news.ycombinator.com/item?id=49303202)

**背景**: uBlock Origin 是由 Raymond Hill 开发的免费开源内容过滤扩展，被广泛认为是最高效的广告拦截器之一。Chrome 的 Manifest V3 扩展平台用 declarativeNetRequest 替代了支持实时拦截的 webRequest API，这给规则数量和动态拦截带来了限制。因此，Google 开始淘汰 Manifest V2 扩展，Edge、Brave 等基于 Chromium 的浏览器也相继跟进，最终使 Firefox 成为唯一保留完整支持的主要浏览器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/UBlock_Origin">UBlock Origin</a></li>
<li><a href="https://en.wikipedia.org/wiki/Manifest_V3">Manifest V3</a></li>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/what-is-mv3">Extensions / Manifest V3 | Chrome for Developers</a></li>

</ul>
</details>

**社区讨论**: 评论者欢迎 Firefox 的这一地位，并指出 Mozilla 会在更新时为一批精选热门扩展审核 uBlock Origin 的代码，这种做法受到用户认可。还有人批评 Google 的扩展改动，并提及了一个非官方 MV3 移植版；也有用户表示 uBlock Origin Lite 目前用起来没有问题。一位网站开发者补充说，现在只有在 Firefox 中才能移除 Google 搜索广告。

**标签**: `#browser`, `#privacy`, `#ad-blocking`, `#manifest-v3`, `#firefox`

---

<a id="item-6"></a>
## [不要分类，要幻觉：用嵌入映射 LLM 生成的标签](https://simonwillison.net/2026/Aug/14/dont-classify-hallucinate/) ⭐️ 8.0/10

Doug Turnbull 提出了一种技术：让 LLM 在不查看现有词汇表的情况下生成全新的、幻觉出来的标签，然后用向量嵌入将这些想象的标签映射到语料库中最接近的真实标签。Simon Willison 指出，这对他博客拥有 1,856 个标签的分类体系来说是一个实用的解决方案，因为该体系太大，无法直接交给 LLM 进行分类。 这种方法解决了当标签词汇表过大而无法放入 LLM 上下文窗口时，分类和打标签中常见的可扩展性问题。它巧妙地将 LLM 的生成输出与基于嵌入的相似性结合起来，为实践者提供了一种高价值、低成本的技术，可将不受控制的生成内容映射回受控词汇表。 示例提示中包含了一些标签形态样本，例如层级类别 'Furniture / Living Room Furniture / Coffee Tables & End Tables / Coffee Tables'，以帮助 LLM 生成有用的幻觉标签。该技术仍然依赖嵌入模型的质量，因为映射效果取决于在想象标签与真实标签列表之间测量的语义相似度。

rss · Simon Willison · 8月14日 21:54

**背景**: 向量嵌入将单词或短语表示为稠密数值向量，语义相近的项在向量空间中位置也相近。这使得系统可以计算任意文本标签之间的相似度。在自然语言处理中，嵌入常用于搜索、聚类和分类。这里描述的技术利用 LLM 的生成能力来推测可能的标签，然后依靠嵌入将这些假设与现有固定标签集进行匹配。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vector_embedding">Vector embedding</a></li>
<li><a href="https://arxiv.org/html/2406.03725">LLMEmbed: Rethinking Lightweight LLM’s Genuine Function in Text Classification</a></li>
<li><a href="https://www.emergentmind.com/topics/embedding-based-classifiers">Embedding-Based Classifiers</a></li>

</ul>
</details>

**标签**: `#LLM`, `#embeddings`, `#classification`, `#tagging`, `#AI`

---

<a id="item-7"></a>
## [构建 Postgres 扩展以估算查询内存使用量](https://postgr.es/p/9sj) ⭐️ 7.0/10

这篇文章提供了一份实战指南，介绍如何构建一个能够估算查询内存消耗并可选记录或阻止查询的 PostgreSQL 扩展。该指南以 PostgreSQL 18 为目标，使用 Docker、PGXS 和规划器级内省，并基于作者此前关于扩展开发的入门文章。 这很重要，因为目前没有工具可以估算查询在连接、排序和分组节点上可能需要的多个内存分配，导致 work_mem 调优困难。这种概念验证扩展可以帮助开发人员和 DBA 更好地理解和控制内存使用，并启发更完善的工具。 该扩展依赖于服务器自身的头文件和 PostgreSQL 18 源码树，并基于官方镜像的 Dockerfile 提供干净的构建环境。这个实现被描述为‘半可用’的概念验证，因为所需的大部分信息位于源代码而非手册中，指南使用 PGXS、控制文件和 SQL 脚本，最初构建一个惰性外壳。

rss · Planet PostgreSQL · 8月14日 16:00

**背景**: PostgreSQL 扩展是向数据库添加功能的软件包，通过 CREATE EXTENSION 加载，并可挂接到查询规划等内部流程中。work_mem 控制排序、连接和哈希操作使用的内存，但每个查询节点会获得自己的分配额度，因此复杂查询可能消耗远超预期的内存。扩展可以使用 planner_hook 等钩子来改变或观察规划器行为，PGXS 是编译扩展的标准构建系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/sql-createextension.html">PostgreSQL: Documentation: 18: CREATE EXTENSION</a></li>
<li><a href="https://www.postgresql.org/docs/current/runtime-config-query.html">PostgreSQL : Documentation: 18: 19.7. Query Planning</a></li>
<li><a href="https://raghunandanbhat.github.io/blog/pg-extension/">How Postgres Extensions Actually work |</a></li>

</ul>
</details>

**标签**: `#postgres`, `#extension`, `#memory`, `#database`, `#development`

---

<a id="item-8"></a>
## [诊断 pg_stat_statements 中的高基数工作负载：第 6 期](https://postgr.es/p/9sa) ⭐️ 7.0/10

在 Postgres in Production 系列第 6 期中，Ryan Booz 解释了高基数工作负载对 pg_stat_statements 的含义，并在 PostgreSQL 17 和 18 上演示了相同的负载。他还提供了具体检查方法，以判断由于 ORM、动态 SQL 和 AI 辅助工具生成的唯一查询，pg_stat_statements 是否正在丢失查询调优所需的数据。 高基数工作负载可能导致 pg_stat_statements 丢弃查询统计信息，使数据库从业者在查询调优时失去依据。随着 ORM、动态 SQL 和 AI 生成代码产生更多唯一查询，这一指导有助于 PostgreSQL 用户识别并缓解日益严重的监控问题。 本集包含在 PostgreSQL 17 和 18 上的并排演示，并使用名为 Bluebox 的工具展示 pg_stat_statements 如何被淹没。还讨论了唯一查询的来源、如何判断自己是否拥有高基数工作负载，以及若不采取措施会发生什么。

rss · Planet PostgreSQL · 8月13日 02:00

**背景**: pg_stat_statements 是 PostgreSQL 内置的扩展，用于跟踪服务器上 SQL 语句的执行统计。它通过将字面常量替换为占位符来规范化查询，使相似语句能够聚合统计；然而，高基数工作负载会产生大量独特的查询形态，可能超出扩展的容量，导致较旧的条目被丢弃。pg_stat_statements_info 视图及相关配置设置有助于检测和处理这类丢失。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pganalyze.com/blog/postgres-in-production-pg-stat-statements-deep-dive-part-6">Diagnosing High Cardinality Workloads in pg_stat_statements</a></li>
<li><a href="https://www.postgresql.org/docs/current/pgstatstatements.html">PostgreSQL: Documentation: 18: F.32. pg_stat_statements — track ...</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#pg_stat_statements`, `#database performance`, `#query tuning`, `#monitoring`

---

<a id="item-9"></a>
## [pg_walviz：PostgreSQL WAL 段可视化新工具](https://postgr.es/p/9sc) ⭐️ 7.0/10

Bertrand Drouvot 发布了 pg_walviz v0.1.0-beta.1，这是一个只读工具，可在本地浏览器中可视化 PostgreSQL WAL 段文件。它以三个同步级别展示 WAL 数据：段概览、记录片段、以及带物理字节的记录检查器。 该工具为开发者和 DBA 提供了罕见的 WAL 页面和记录布局物理视图，使调试和理解 PostgreSQL 预写日志内部机制变得更加容易。虽然它面向小众用户，但弥补了 pg_waldump 等文本工具留下的空白。 pg_walviz 不需要运行中的服务器或数据目录，只需一个 WAL 段文件和匹配的 pg_waldump 二进制文件。它默认绑定 127.0.0.1，支持通过 --no-open 和 --port 进行无头（headless）使用，并提醒不要检查正在写入的 WAL 段或运行中服务器的 pg_wal 目录。

rss · Planet PostgreSQL · 8月13日 01:00

**背景**: 在 PostgreSQL 中，预写日志（WAL）在更改应用之前记录每一次更改，从而保证崩溃安全并支持时间点恢复。WAL 段默认是 16 MB 的文件，内部划分为 8 KB 的页面。pg_waldump 是用于以人类可读形式呈现 WAL 的标准命令行工具，但它不显示物理字节布局。pg_walviz 基于 pg_waldump 的输出，增加了可视化的交互式检查功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bdrouvot.github.io/2026/08/13/welcome-to-pg-walviz-postgresql-wal-segment-visualizer/">Welcome to pg _ walviz : PostgreSQL WAL segment visualizer</a></li>
<li><a href="https://stormatics.tech/blogs/beginners-guide-wal-in-postgresql">Beginner’s Guide to Understanding WAL in PostgreSQL | Stormatics</a></li>
<li><a href="https://www.interdb.jp/pg/pgsql09.html">9. Write Ahead Logging ( WAL ) :: Hironobu SUZUKI @ InterDB</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#WAL`, `#visualization`, `#debugging`, `#tool`

---