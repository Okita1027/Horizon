---
layout: default
title: "Horizon 日报：2026-07-01 (ZH)"
date: 2026-07-01
lang: zh
---

> 从 46 条内容中筛选出 13 条重要资讯。

---

1. [美国解除对 Anthropic 的 Claude Fable 5 和 Mythos 5 的出口管制](#item-1) ⭐️ 10.0/10
2. [Claude Code 嵌入隐藏的隐写标记](#item-2) ⭐️ 9.0/10
3. [Anthropic 发布 Claude Sonnet 5，增强智能体能力](#item-3) ⭐️ 8.0/10
4. [Anthropic 推出用于科学研究的 Claude Science](#item-4) ⭐️ 8.0/10
5. [通过 WebAssembly 将 Kubernetes 移植到浏览器](#item-5) ⭐️ 8.0/10
6. [PostgreSQL 18 和 19 新增时态键和针对部分的更新/删除](#item-6) ⭐️ 8.0/10
7. [序列同步填补 PostgreSQL 升级关键缺口](#item-7) ⭐️ 8.0/10
8. [Ornith-1.0：面向智能体编程的自脚手架大型语言模型](#item-8) ⭐️ 8.0/10
9. [Percona Operator 现支持社区 Docker 镜像](#item-9) ⭐️ 7.0/10
10. [PostgreSQL 中表过多导致 OOM 和 CPU 问题](#item-10) ⭐️ 7.0/10
11. [SQL 标准会议接受 QUALIFY 和 INSERT BY NAME](#item-11) ⭐️ 7.0/10
12. [理解 PostgreSQL 索引扫描中的堆读取问题](#item-12) ⭐️ 7.0/10
13. [shot-scraper video 可录制自动化网页演示](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [美国解除对 Anthropic 的 Claude Fable 5 和 Mythos 5 的出口管制](https://twitter.com/AnthropicAI/status/2072106151890809341) ⭐️ 10.0/10

美国商务部已解除对 Anthropic 的 Claude Fable 5 和 Mythos 5 人工智能模型的出口管制，允许恢复面向一般用户的访问。 这一政策转变影响国家安全和全球人工智能竞争，这些前沿模型在监管上常被比作核技术。 Claude Fable 5 在 FrontierBench 上得分最高，擅长长程推理，而 Mythos 5 是功能更强的变体，已部分恢复对特定客户的访问。

hackernews · Pragmata · 6月30日 23:55 · [社区讨论](https://news.ycombinator.com/item?id=48740771)

**背景**: Anthropic 的 Claude 平台与 OpenAI 的 ChatGPT 和 Google 的 Gemini 竞争。Fable 5 是面向消费市场的版本，能够进行深度推理和独立完成复杂任务。出口管制最初是由于担心先进 AI 被滥用而实施的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://www.bbc.com/news/articles/cdr42623e1do">Fable and Mythos : Anthropic says US lifts export ban on its advanced...</a></li>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/introducing-claude-fable-5-and-claude-mythos-5">Introducing Claude Fable 5 and Claude Mythos 5</a></li>

</ul>
</details>

**社区讨论**: 评论反映了不同观点：有人认为对美国前沿模型的信任已受损，有人质疑在中国模型取得进展的情况下出口管制是否有效，还有人认为解除管制是一种倒退，使情况更糟。

**标签**: `#AI regulation`, `#export controls`, `#Anthropic`, `#national security`, `#frontier models`

---

<a id="item-2"></a>
## [Claude Code 嵌入隐藏的隐写标记](https://thereallo.dev/blog/claude-code-prompt-steganography) ⭐️ 9.0/10

有博客分析发现，Anthropic 的智能编程工具 Claude Code 在发出的请求中嵌入了隐藏的隐写标记。 这一发现引发了关于人工智能公司未披露做法的重要透明度和道德问题，可能影响用户信任和隐私，尤其对于依赖该工具的开发者而言。 这些标记是通过逆向工程检测到的，根据社区推测，其设计意图可能是识别来自特定实体（例如进行模型蒸馏的中国公司）的请求。

hackernews · kirushik · 6月30日 15:44 · [社区讨论](https://news.ycombinator.com/item?id=48734373)

**背景**: 隐写术是将数据隐藏在其他数据中以避免检测的技术。在此背景下，Claude Code 在用户请求中不可见地添加标记以追踪使用情况。Claude Code 是 Anthropic 的 AI 代理，可帮助开发者在终端中直接编写和编辑代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**社区讨论**: 评论显示反应不一：一些人淡化严重性，认为意图是正当的（例如检测模型窃取），而另一些人批评 Anthropic 缺乏透明度且实现粗糙。少数用户表达了对 Anthropic 的不信任，并建议使用开源的替代方案如 Codex CLI。

**标签**: `#steganography`, `#AI`, `#trust`, `#security`, `#Anthropic`

---

<a id="item-3"></a>
## [Anthropic 发布 Claude Sonnet 5，增强智能体能力](https://www.anthropic.com/news/claude-sonnet-5) ⭐️ 8.0/10

Anthropic 发布了 Claude Sonnet 5，这是一款强调自主规划和工具使用等智能体能力的新模型。该模型引入了多个努力级别，成本和性能各不相同，社区基准测试对此进行了详细说明。 此次发布凸显了智能体 AI 在现实应用中的日益重要地位，能够实现更自主的任务完成。它展示了更小、更快的模型如何提供先进的智能体功能，从而可能降低开发者的成本。 社区基准测试显示，Claude Sonnet 5 的性能达到 GLM-5.2 水平，成本翻倍但速度翻倍，在常识问答、工具调用和谜题解决方面存在弱点。每任务成本图表表明，对于较高努力级别，Opus 可能更具成本效益。

hackernews · marinesebastian · 6月30日 17:59 · [社区讨论](https://news.ycombinator.com/item?id=48736605)

**背景**: 智能体 AI 指的是能够自主追求目标、使用工具和规划行动的系统，与被动问答模型形成对比。Anthropic 的 Claude 模型系列包括 Opus（更大、能力更强）和 Sonnet（更快、效率更高）等变体，针对不同用例进行了优化。Claude Sonnet 5 在此系列基础上发展，侧重于智能体任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ea-crux-project.vercel.app/knowledge-base/capabilities/agentic-ai/">Agentic AI | LongtermWiki</a></li>
<li><a href="https://zhukov.live/what-is-agentic-ai-understanding-agentic-ai-5f011521bc08">What is Agentic AI ? Understanding... | by Volodymyr Zhukov | Medium</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些人质疑与 Opus 相比的价值主张，指出在高努力级别下 Opus 可能更具成本效益。另一些人则欣赏其在智能体辅助开发中的速度，但对漏洞发现等方面的性能下降表示担忧。

**标签**: `#AI`, `#Large Language Models`, `#Anthropic`, `#Claude`, `#Machine Learning`

---

<a id="item-4"></a>
## [Anthropic 推出用于科学研究的 Claude Science](https://claude.com/product/claude-science) ⭐️ 8.0/10

Anthropic 推出了 Claude Science，这是一款专为科学研究设计的产品，运行本地服务器并集成 HPC 集群和数据库。 这之所以重要，是因为它在制药实验室等管控严格的环境中实现了安全、高性能的 AI 辅助数据科学，填补了 AI 在科学计算应用中的空白。 Claude Science 采用本地服务器加 Web UI 的架构，区别于其他 Claude 产品，并集成了 HPC 工具和数据库，实现无缝的科学工作流程。

hackernews · lebovic · 6月30日 17:07 · [社区讨论](https://news.ycombinator.com/item?id=48735770)

**背景**: HPC（高性能计算）为复杂的科学和 AI 工作负载提供巨大的计算能力。现代大语言模型越来越多地用于数据分析和可视化，但通常缺乏与科学基础设施的直接集成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High-performance_computing">High-performance computing - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/hpc-ai">High Performance Computing (HPC) and AI | IBM</a></li>

</ul>
</details>

**社区讨论**: 社区成员在实际任务（如计算生物学）中测试了 Claude Science，认为它能产生合理但并非卓越的结果，同时存在一些注意事项，如对非哺乳动物目标使用哺乳动物设计规则。其他人则称赞本地服务器架构能够安全访问敏感数据。

**标签**: `#Claude Science`, `#Anthropic`, `#scientific computing`, `#HPC`, `#AI for science`

---

<a id="item-5"></a>
## [通过 WebAssembly 将 Kubernetes 移植到浏览器](https://ngrok.com/blog/i-ported-kubernetes-to-the-browser) ⭐️ 8.0/10

ngrok 的一位开发者创建了 'webernetes' 项目，该项目利用 WebAssembly 将 Kubernetes 完全移植到浏览器中运行，用户无需安装任何软件即可与模拟的 Kubernetes 集群进行交互。 这使得 Kubernetes 的教育和实验更加便捷，学习者无需搭建真实集群的繁琐步骤，即可探索 Kubernetes 概念。 该项目实际上并未在浏览器中运行容器，而是使用 Rust 编写的轻量级实现并编译为 WebAssembly，模拟 Kubernetes API 响应和行为。

hackernews · peterdemin · 6月30日 20:48 · [社区讨论](https://news.ycombinator.com/item?id=48738985)

**背景**: WebAssembly (Wasm) 是一种二进制指令格式，可在网页浏览器中实现高性能代码执行。Kubernetes 是一个容器编排平台，通常在服务器集群上运行。将 Kubernetes 移植到浏览器需要在不依赖底层基础设施的情况下模拟其控制平面和 API。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly</a></li>
<li><a href="https://en.wikipedia.org/wiki/Ngrok">Ngrok</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为该项目很酷，但指出其在实际使用中的局限性。一些人认为标题具有误导性，因为它实际上并未运行容器，其他人则强调了重新实现 Kubernetes 逻辑的维护负担。使用 AI 生成代码并通过 Kubernetes 进行验证的工作流程也受到了赞赏。

**标签**: `#Kubernetes`, `#WebAssembly`, `#Education`, `#Browser`, `#ngrok`

---

<a id="item-6"></a>
## [PostgreSQL 18 和 19 新增时态键和针对部分的更新/删除](https://postgr.es/p/9nR) ⭐️ 8.0/10

PostgreSQL 18 引入了使用 WITHOUT OVERLAPS 子句的时态主键和唯一约束，以及使用 PERIOD 子句的外键，而 PostgreSQL 19 则通过 UPDATE/DELETE FOR PORTION OF 扩展了时态数据操作的支持。 这些特性为 PostgreSQL 带来了原生的时态数据完整性和操作能力，减少了管理随时间变化的数据时所需的复杂应用程序逻辑，并符合 SQL:2011 标准。 WITHOUT OVERLAPS 子句确保主键或唯一约束中的时间段不重叠，而外键中的 PERIOD 则强制跨时态关系的参照完整性。UPDATE/DELETE FOR PORTION OF 允许仅修改行有效期的特定时间段。

rss · Planet PostgreSQL · 6月30日 16:00

**背景**: 时态数据库管理随时间变化的数据，存储带有有效期段的多个版本记录。SQL:2011 标准定义了具有时态键和操作的应用程序时间周期表，PostgreSQL 正在实现这些功能，以简化时间序列和历史数据管理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/19/ddl-temporal-tables.html">PostgreSQL: Documentation: 19: 5.7. Temporal Tables</a></li>
<li><a href="https://www.depesz.com/2026/04/02/waiting-for-postgresql-19-add-update-delete-for-portion-of/">Waiting for PostgreSQL 19 – Add UPDATE / DELETE FOR PORTION ...</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#temporal database`, `#database features`, `#time-series`, `#SQL`

---

<a id="item-7"></a>
## [序列同步填补 PostgreSQL 升级关键缺口](https://postgr.es/p/9nL) ⭐️ 8.0/10

PostgreSQL 工程师 vignesh C 提出了一种序列同步机制，确保在使用 pg_createsubscriber 进行升级时序列被正确复制，填补了逻辑复制中长期存在的空白。 这使得近零停机 PostgreSQL 升级真正可靠，避免了因序列不同步导致的应用程序错误（如重复键违例），惠及管理大规模数据库升级的 DBA 和系统工程师。 该解决方案可能依赖于额外的 WAL 记录或同步步骤，在切换期间捕获并应用序列状态。它专门针对使用 pg_createsubscriber 将物理备库转换为逻辑订阅者后再进行升级的工作流程。

rss · Planet PostgreSQL · 6月30日 00:38

**背景**: pg_upgrade 支持 PostgreSQL 的二进制升级，而 pg_createsubscriber（PostgreSQL 17 引入）可将物理备库转换为逻辑订阅者，实现近零停机升级。但逻辑复制默认不复制序列状态，导致新主库上的序列可能滞后，引发冲突。序列同步通过确保升级后序列值保持一致来解决此问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.fastware.com/blog/closing-a-critical-gap-in-postgresql-upgrade-workflows-with-sequence-synchronization">Closing a critical gap in PostgreSQL upgrade workflows with...</a></li>
<li><a href="https://www.postgresql.fastware.com/blog/an-introduction-to-postgresql-pg-createsubscriber">An introduction to PostgreSQL pg_createsubscriber</a></li>
<li><a href="https://www.postgresql.org/docs/current/app-pgcreatesubscriber.html">PostgreSQL: Documentation: 18: pg_createsubscriber</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database upgrade`, `#logical replication`, `#sequence synchronization`, `#pg_upgrade`

---

<a id="item-8"></a>
## [Ornith-1.0：面向智能体编程的自脚手架大型语言模型](https://simonwillison.net/2026/Jun/29/ornith/#atom-everything) ⭐️ 8.0/10

DeepReinforce 发布了 Ornith-1.0 系列开源模型（MIT 许可），基于 Gemma 4 和 Qwen 3.5 构建，提供 9B、31B、35B MoE 和 397B MoE 等多种规模，在编程基准测试中达到同类开源模型的最佳性能。 该发布为开源社区带来了强大的智能体编程能力，其自脚手架训练框架联合学习任务解决与脚手架构建，有望加速 AI 辅助软件开发，减少对闭源模型的依赖。 该模型采用自改进训练策略，推理时学会构建自己的脚手架，并包含一个冻结的评判者（frozen judge）以防止奖励欺骗。它可通过 LM Studio 本地运行，初步测试显示其在多步智能体任务（如代码库导航）中表现熟练。

rss · Simon Willison · 6月29日 16:17

**背景**: 智能体编程（Agentic coding）指使用自主 AI 代理在最少人工干预下规划、编写、测试和修改代码。自脚手架（self-scaffolding）是一种技术，模型学会生成自己的中间步骤或“脚手架”（如工具调用、子目标）来解决复杂任务，而不是依赖固定提示。MoE（混合专家）是一种模型架构，将模型划分为多个专门的子网络，每次只激活相关专家以提高效率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/29/ornith/">Ornith-1.0: Self-Scaffolding LLMs for Agentic Coding</a></li>
<li><a href="https://deep-reinforce.com/ornith_1_0.html">Ornith-1.0: Self-Scaffolding LLMs for Agentic Coding</a></li>
<li><a href="https://www.explainx.ai/blog/ornith-1-0-self-scaffolding-agentic-coding-llm-2026">Ornith-1.0: Self-Scaffolding Open Models for Agentic Coding</a></li>

</ul>
</details>

**社区讨论**: Simon Willison 的初步印象是积极的：35B GGUF 模型在本地运行良好，熟练处理智能体工具调用，甚至能画出可识别的鹈鹕。该发布被视为开源 LLM 领域的重要补充，编程性能具有竞争力。

**标签**: `#LLM`, `#open-source`, `#coding`, `#agentic`, `#deepreinforce`

---

<a id="item-9"></a>
## [Percona Operator 现支持社区 Docker 镜像](https://postgr.es/p/9nQ) ⭐️ 7.0/10

Percona Operator for PostgreSQL 3.0.0 推出了社区 Docker 镜像的技术预览版，允许用户使用官方 PostgreSQL 包构建的镜像来运行 operator，而非 Percona 的发行版镜像。该功能将在 3.1.0 版本中正式支持。 此举解决了 Kubernetes 上 PostgreSQL operator 的关键信任与锁定问题，消除了对容器镜像分发和许可的厂商依赖。用户获得了对镜像供应链的完全控制，降低了厂商政策意外变更的风险。 社区 Docker 镜像由 PostgreSQL 全球开发组 (PGDG) 提供的包构建，并可托管在用户控制的注册表中。该方法不包含 Percona 特有的功能（如透明数据加密 TDE），这是有意为之的权衡。

rss · Planet PostgreSQL · 6月30日 14:09

**背景**: Kubernetes operator 依赖容器镜像来运行数据库集群，信任这些镜像意味着信任厂商的注册表和许可。近期历史显示，厂商可以在不更改开源源代码的情况下更改容器镜像条款，引发了社区的怀疑。Percona 的社区 Docker 镜像允许用户从官方上游包构建并控制自己的镜像，从而重建信任。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/percona/percona-postgresql-operator">GitHub - percona/percona-postgresql-operator: Percona Operator for PostgreSQL · GitHub</a></li>
<li><a href="https://docs.percona.com/percona-operator-for-postgresql/3.0.0/index.html">Percona Operator for PostgreSQL</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#Kubernetes`, `#Docker`, `#Percona Operator`, `#container images`

---

<a id="item-10"></a>
## [PostgreSQL 中表过多导致 OOM 和 CPU 问题](https://postgr.es/p/9nN) ⭐️ 7.0/10

Laurenz Albe 发表了一篇技术深度分析文章，指出 PostgreSQL 中过多的表会触发 Linux OOM killer 并导致长时间运行的查询占用 CPU。该分析基于一个真实客户案例，其中内存上下文转储显示过多表导致了系统目录缓存膨胀。 这很重要，因为许多 PostgreSQL 用户可能没有意识到过多的表会严重降低性能和稳定性，甚至导致崩溃。该文章提供了可操作的建议来避免这些问题，对设计数据库模式的 DBA 和开发人员很有帮助。 具体问题是 CacheMemoryContext 中的系统目录缓存膨胀，当表数量达到数千时可能消耗数百 MB 内存。Albe 建议保持表数量可控、谨慎使用分区并监控目录膨胀。

rss · Planet PostgreSQL · 6月30日 05:00

**背景**: Linux OOM 杀手是一种内核机制，当内存严重不足时终止进程，通常由内存过量使用引起。PostgreSQL 的系统目录存储所有表、索引和其他对象的元数据；每个表都会在目录表中添加条目，过多的条目会导致缓存内存膨胀。这种膨胀可能导致 OOM 杀手杀死 PostgreSQL，或者由于目录查找的 CPU 占用增加而降低性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Out_of_memory">Out of memory - Wikipedia</a></li>
<li><a href="https://www.netdata.cloud/blog/postgresql-database-bloat/">How to monitor and fix Database bloats in PostgreSQL ? | Netdata</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database performance`, `#table design`, `#performance tuning`

---

<a id="item-11"></a>
## [SQL 标准会议接受 QUALIFY 和 INSERT BY NAME](https://postgr.es/p/9nP) ⭐️ 7.0/10

ISO SQL 标准工作组在 2026 年 6 月的斯德哥尔摩会议上接受了 QUALIFY 子句和 INSERT BY NAME 选项，使这些功能更接近正式标准化。 这些新增功能简化了复杂查询并提高了 SQL 和 PostgreSQL 用户的使用体验，减少了嵌套子查询和列排序的需要。 QUALIFY 子句在窗口函数之后进行过滤，消除了子查询包装；而 INSERT BY NAME 按名称匹配列而非位置，BY POSITION 作为显式默认选项。

rss · Planet PostgreSQL · 6月30日 04:00

**背景**: ISO/IEC JTC1 SC32 WG3 是负责数据库语言 SQL 和 GQL 标准化的国际委员会。该工作组以就近机场代码命名其现场会议。接受的提案先进入工作草案，最终才会成为正式标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://jtc1info.org/technology/subcommittees/data-mgmt-and-interchange/database-languages/">Database languages - JTC 1</a></li>
<li><a href="https://en.wikipedia.org/wiki/GQL_Graph_Query_Language">GQL Graph Query Language</a></li>

</ul>
</details>

**标签**: `#SQL`, `#PostgreSQL`, `#Database Standards`, `#ISO`, `#WG3`

---

<a id="item-12"></a>
## [理解 PostgreSQL 索引扫描中的堆读取问题](https://postgr.es/p/9nM) ⭐️ 7.0/10

Christophe Pettus 解释了 PostgreSQL 中关于索引扫描的一个常见误解：即使在物理上可行，由于可见性映射问题，它们仍可能对每一行进行堆读取。 这一见解对 PostgreSQL 性能调优至关重要，因为不必要的堆读取会抵消索引扫描的优势并增加 I/O 开销。 索引扫描依赖可见性映射来跳过堆获取；如果映射显示页面并非全可见，PostgreSQL 仍需读取堆来检查 MVCC 可见性。

rss · Planet PostgreSQL · 6月30日 01:00

**背景**: 索引扫描在 PostgreSQL 9.2 中引入，允许仅从索引数据满足查询，减少 I/O。可见性映射跟踪哪些堆页面仅包含对所有活动事务可见的元组。当页面全可见时，无需堆获取；否则需要它们来确保事务可见性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wiki.postgresql.org/wiki/Index-only_scans">Index - only scans - PostgreSQL wiki</a></li>
<li><a href="https://www.pgmustard.com/blog/2019/03/04/index-only-scans-in-postgres">Index - only scans in Postgres - pgMustard</a></li>
<li><a href="https://medium.com/@borhadeshardul/the-silent-killer-of-index-only-scans-a-deep-dive-into-heap-fetches-and-lossy-pages-8386e33677d8">The Silent Killer of Index - Only Scans : A Deep Dive into Heap Fetches...</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#index-only scan`, `#performance`, `#GUCs`

---

<a id="item-13"></a>
## [shot-scraper video 可录制自动化网页演示](https://simonwillison.net/2026/Jun/30/shot-scraper-video/#atom-everything) ⭐️ 7.0/10

shot-scraper 1.10 中的新命令 `shot-scraper video` 接受一个 storyboard YAML 文件，并使用 Playwright 录制网页应用程序操作的视频，从而使编码智能体能够演示其成果。 这简化了为网页应用创建视频演示的过程，特别有助于需要展示其输出的 AI 编码智能体，增强了自动化工作流的可信度和可验证性。 该命令包含如 `--auth` 用于认证会话和 `--mp4` 用于输出 MP4 等选项；storyboard YAML 定义了包含点击、暂停和 JavaScript 注入等操作的场景，以实现精细控制。

rss · Simon Willison · 6月30日 16:54

**背景**: shot-scraper 是一个基于 Playwright 构建的命令行工具，用于自动截图，最初由 Simon Willison 于 2022 年为文档截图而创建。新的 video 命令将其功能扩展到视频录制，使开发者能够创建完整的演示。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2022/Mar/10/shot-scraper/">shot-scraper: automated screenshots for documentation, built on Playwright</a></li>
<li><a href="https://github.com/simonw/shot-scraper">GitHub - simonw/shot-scraper: A command-line utility for taking automated screenshots of websites · GitHub</a></li>

</ul>
</details>

**标签**: `#shot-scraper`, `#Playwright`, `#video recording`, `#coding agents`, `#demos`

---