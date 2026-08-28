---
layout: default
title: "Horizon 日报：2026-08-28 (ZH)"
date: 2026-08-28
lang: zh
---

> 从 40 条内容中筛选出 11 条重要资讯。

---

1. [英伟达同意以 130 亿美元收购 Hugging Face](#item-1) ⭐️ 9.0/10
2. [提示注入攻击在 80%情况下绕过 Claude Code Auto Mode](#item-2) ⭐️ 9.0/10
3. [Cloudflare 优化 1.1.1.1 缓存，节省 100 TB 内存](#item-3) ⭐️ 8.0/10
4. [小模型已经到来](#item-4) ⭐️ 8.0/10
5. [交互分析揭示 Claude 高频套话词汇'load-bearing'](#item-5) ⭐️ 8.0/10
6. [开发者记录借助 LLM 在 84 天内反编译一款 N64 游戏](#item-6) ⭐️ 8.0/10
7. [为 Agentic AI 构建可靠的数据基础](#item-7) ⭐️ 8.0/10
8. [Qwen3.8-Flash-Next：开放权重 MoE 模型预览 Qwen4 架构](#item-8) ⭐️ 8.0/10
9. [Visual Studio Code 1.135 版本更新发布](#item-9) ⭐️ 7.0/10
10. [Lua 集成补丁让 PostgreSQL psql 支持自定义命令](#item-10) ⭐️ 7.0/10
11. [PostgreSQL 18 使用 UUID v7 将插入性能提升 23 倍](#item-11) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [英伟达同意以 130 亿美元收购 Hugging Face](https://www.businessinsider.com/nvidia-in-talks-to-buy-hugging-face-13-billion-dollars-2026-8) ⭐️ 9.0/10

英伟达已同意以约 130 亿美元收购 Hugging Face，这是领先的开源 AI 模型托管平台。该交易由 The Information 和 TechCrunch 于 2026 年 8 月报道。 这笔收购可能重塑 AI 开发生态，因为英伟达作为占主导地位的 GPU 制造商，将控制用于分发和共享开源 AI 模型的主要平台。这也引发了对开源 AI 未来、模型访问以及潜在反垄断问题的重大关切。 Hugging Face 被开发者广泛用于托管和下载预训练模型，其 Transformers 库是自然语言处理的标准工具。据报道，这笔交易对 Hugging Face 的估值约为 130 亿美元；观察人士指出，英伟达将获得对平台数据（包括硬件使用调查和模型下载模式）的优先访问权。

hackernews · mfiguiere · 8月27日 01:12 · [社区讨论](https://news.ycombinator.com/item?id=49458161)

**背景**: Hugging Face, Inc.是一家总部位于纽约市的美国公司，开发机器学习工具，其中最著名的是用于自然语言处理的 Transformers 库。其平台允许用户分享机器学习模型、数据集和演示，使其成为开源 AI 生态系统的核心枢纽。与此同时，英伟达是用于训练和运行 AI 模型的 GPU 的主要供应商，并一直在围绕其硬件扩展软件和平台产品。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hugging_Face">Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/Open-source_artificial_intelligence">Open-source artificial intelligence - Wikipedia</a></li>
<li><a href="https://aimagazine.com/top10/top-10-open-source-ai-platforms">Top 10: Open Source AI Platforms | AI Magazine</a></li>

</ul>
</details>

**社区讨论**: 评论者反应不一，有人祝贺 Hugging Face 的创始人并希望英伟达能够支持社区，也有人担心失去一个中立的开源中心。还有人对平台数据的优先访问权和潜在的反垄断问题表示担忧，并猜测法国创始人可能会将所得资金再投资于一个新的欧洲 AI 实验室。

**标签**: `#AI`, `#Nvidia`, `#Hugging Face`, `#Acquisition`, `#Open Source`

---

<a id="item-2"></a>
## [提示注入攻击在 80%情况下绕过 Claude Code Auto Mode](https://simonwillison.net/2026/Aug/27/breaking-claude-code-opus-5-auto-mode/) ⭐️ 9.0/10

安全研究员 Johann Rehberger 发现了一种提示注入攻击，可在 80%的情况下绕过 Claude Code Opus 5 Auto Mode 的保护。该攻击通过诱使代理下载并解压包含恶意 struct.py 的 zip 压缩包，从而在导入 base64 时被本地文件劫持。 这一发现挑战了 Anthropic 对 Claude Code auto mode 的安全声明——该模式最近已成为 Pro、Max 和 Team 计划的默认设置。它表明 AI 编程代理仍然容易受到提示注入攻击，凸显了沙箱隔离和网络限制的必要性。 该攻击利用了 Python 模块遮蔽技术：在解压的 zip 中放置 struct.py，使 base64 导入时触发本地文件执行。在几次运行中，auto mode 甚至阻止了 Claude 终止恶意进程的命令，意味着安全分类器反而阻碍了代理将攻击停下。

rss · Simon Willison · 8月27日 22:50

**背景**: 提示注入是一种攻击方式，将恶意指令嵌入 AI 模型处理的内容中，使其偏离预期行为。Claude Code 的 auto mode 通过分类器筛选工具调用，使代理能够无需逐个权限提示自主运行。Python 的导入机制会先搜索当前目录再搜索标准库路径，因此当脚本导入 base64（其内部也会导入 struct）时，本地名为 struct.py 的模块可以遮蔽标准库中的 struct。这种技术被称为模块遮蔽。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/blog/auto-mode">Auto mode for Claude Code | Claude by Anthropic</a></li>
<li><a href="https://code.claude.com/docs/en/auto-mode-config">Configure auto mode - Claude Code Docs</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>

</ul>
</details>

**标签**: `#AI Security`, `#Prompt Injection`, `#Claude Code`, `#Anthropic`, `#Security Research`

---

<a id="item-3"></a>
## [Cloudflare 优化 1.1.1.1 缓存，节省 100 TB 内存](https://blog.cloudflare.com/dns-cache-memory-optimization-1111/) ⭐️ 8.0/10

Cloudflare 工程师重新设计了其 1.1.1.1 DNS 解析器缓存的内存布局，在全球基础设施中减少了约 100 TB 的内存占用。这一成果通过优化 Rust 中的结构体布局、对齐和分配策略实现。 这一优化表明，即使在大规模云服务中，底层系统编程和内存优化依然至关重要，能够带来巨大的成本节省和缓存效率提升。它也为其他 DNS 解析器和高性能网络服务提供了可参考的范例。 该优化涉及对缓存条目字段的紧凑排列，减少填充字节并避免单独分配内存。社区指出，还可以进一步将记录数据直接放在 CacheEntry 成员之后以节省更多内存，但这一点在 Rust 中实现可能并不容易。

hackernews · TangerineDream · 8月27日 17:17 · [社区讨论](https://news.ycombinator.com/item?id=49468083)

**背景**: 1.1.1.1 是 Cloudflare 提供的公共 DNS 解析服务，被数百万用户用于将域名解析为 IP 地址。DNS 缓存会临时存储之前的查询结果，以加快后续解析速度并减少上游流量。要在 Rust 这类内存安全语言中优化缓存的内存布局，需要理解内存对齐、填充字节和分配开销等底层概念。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/1.1.1.1">1.1.1.1 - Wikipedia</a></li>
<li><a href="https://www.keycdn.com/support/dns-cache">What Is DNS Cache and How to Flush It - KeyCDN Support</a></li>
<li><a href="https://www.akamai.com/glossary/what-is-dns-caching">What Is DNS Caching? | How Does DNS Caching Work? | Akamai</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍赞赏这一优化，认为它证明了系统编程仍然重要；也有人讨论是否还有遗漏的布局优化空间。还有人分享了类似的内存优化经验，例如在 MaraDNS 中使用单次 malloc 大幅降低内存占用，并指出结构体对齐问题可能导致大量内存浪费。

**标签**: `#DNS`, `#Memory Optimization`, `#Cloudflare`, `#Systems Programming`, `#Caching`

---

<a id="item-4"></a>
## [小模型已经到来](https://calv.info/small-models-have-arrived) ⭐️ 8.0/10

文章认为，小型语言模型（SLM）已成为前沿模型的实用且性价比高的替代品。文章预测，随着企业和开发者拥抱更小、更高效的模型，对快速、便宜、'足够好用'的人工智能的需求将激增。 这一论点很重要，因为它挑战了 AI 领域'越大越好'的主流叙事。如果小型模型能以更低成本和延迟处理大多数日常任务，它们将推动端侧 AI、降低计算成本，并开启新的消费级和边缘应用。 小型语言模型通常拥有数亿到约 100 亿个参数，远小于拥有数千亿参数的前沿模型。文章指出，本地工作流和边缘计算使得在不依赖大规模云基础设施的情况下运行有能力的 AI 成为可能。

hackernews · tosh · 8月27日 15:56 · [社区讨论](https://news.ycombinator.com/item?id=49466917)

**背景**: 小型语言模型（SLM）是人工智能中注重效率的一个细分领域，其参数数量通常在 3.5 亿至 100 亿之间。前沿模型代表了 AI 的前沿水平，突破了能力边界，但需要巨大的计算资源。边缘计算与 SLM 之间的协同作用越来越强，使得在本地设备上进行超低延迟的推理成为可能。这一背景解释了为什么小型高效模型正成为许多实际应用中的务实选择。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@Er.Devanshu/understanding-small-language-models-slms-definition-architecture-advantages-and-more-5066a7ef5bd4">Understanding Small Language Models ( SLMs ): Definition ... | Medium</a></li>
<li><a href="https://klu.ai/glossary/frontier-models">Frontier AI Models — Klu</a></li>
<li><a href="https://www.linkedin.com/pulse/synergy-between-edge-computing-ai-small-language-models-tom-reyes-wtsjc">The Synergy Between Edge Computing , AI , Small Language Models...</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了实际经验和战略视角。有人描述了在'思考型'模型出现之前，使用 7B 本地模型和 Guidance 库构建编码工作流的经历；还有人指出简单的 OpenAI API 调用便宜得惊人，几个月仅花费 61 美分。其他人则讨论了消费级 AI 公司的缺失，并区分了'IQ 180'创造性工作与'token 输出型'响应性工作。

**标签**: `#AI`, `#Small Language Models`, `#Edge Computing`, `#Cost Efficiency`, `#Local Models`

---

<a id="item-5"></a>
## [交互分析揭示 Claude 高频套话词汇'load-bearing'](https://louisabraham.github.io/load-bearing/) ⭐️ 8.0/10

作者发布了一个交互式网站，分析 Claude 等 LLM 应答中高频出现的'load-bearing'等套话词汇。数据集和分析每天通过 GitHub Actions 自动更新。 这项分析很重要，因为它量化了 LLM 写作中可识别的语言指纹，帮助用户识别和规避 AI'套话'模式。该项目在开发者与写作者社区引发广泛讨论（473 分、230 条评论），丰富了关于 AI 文本检测与风格的讨论。 该网站以简洁的非冗长呈现为特色，一屏尽览；作者计划增加搜索栏并将数据扩大到每天 1000 条 PR。有用户反馈，在 Claude 提示词中加入奥威尔'不滥用常见比喻'的规则后，模型转而给出具体机制解释，而非使用陈词滥调。

hackernews · Labo333 · 8月27日 08:59 · [社区讨论](https://news.ycombinator.com/item?id=49461817)

**背景**: 像 Claude 这样的 LLM 通过人类反馈强化学习训练，而人类标注者往往偏好正式、谨慎、平衡的措辞，导致模型逐渐偏好'load-bearing'、'the crux'、'first-class citizen'等安全但高频的词汇，成为'AI 味'的标志。近期研究也发现学术摘要中类似风格词过量使用，估计 2024 年 10%至 13.5%的摘要经过 LLM 处理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mareksuppa.com/til/load-bearing/">"Load-bearing" is becoming LLM speak · Marek Šuppa</a></li>
<li><a href="https://trend.hulryung.com/en/posts/2026-07-15-1000-claude-llm-overused-words-load-bearing-ai-writing-tics-slop-linguistic-fingerprint-2026/">Why AI Can't Stop Saying 'Load-Bearing' — The Linguistic Fingerprint Hiding in Chatbot Prose | Trend Reader</a></li>
<li><a href="https://arxiv.org/html/2406.07016v1">Delving into ChatGPT usage in academic writing through excess vocabulary</a></li>

</ul>
</details>

**社区讨论**: 评论区整体正面，用户赞赏该展示简洁且不带偏见。有人分享了实用的提示词修改（如奥威尔规则）以减少 LLM 套话，也有人好奇更多句式层面的模式，如'It contains no string'式否定而非标准说法。

**标签**: `#LLM`, `#AI`, `#Claude`, `#language-models`, `#analysis`

---

<a id="item-6"></a>
## [开发者记录借助 LLM 在 84 天内反编译一款 N64 游戏](https://blog.chrislewis.au/decompiling-a-nintendo-64-game-in-84-days/) ⭐️ 8.0/10

在一篇新的博客文章中，开发者 Chris Lewis 详细介绍了他在 84 天内完整反编译一款 Nintendo 64 游戏（评论者确认该游戏为 Snowboard Kids）的过程，其工作流融合了 LLM 辅助等现代逆向工程手段。文章按步骤记录了将游戏编译后代码还原为可读源代码的过程和所用工具。 这件事之所以重要，是因为它展示了 LLM 辅助的逆向工程如何大幅加速反编译工作，使个人开发者也能切实地复活并保存经典游戏。它也进一步引发了关于将专有复古游戏代码做成开源版本是否合法、是否合乎道德的讨论。 这篇博文强调了一种严谨的、项目化的方法：将工作分解为多个里程碑，并利用 LLM 将汇编代码转换为类 C 代码，同时由人工负责验证。社区评论指出，该游戏是 Snowboard Kids，并提到相关项目如 GoldenEye 反编译和 Legend of Dragoon 重编译。

hackernews · knackers · 8月27日 15:01 · [社区讨论](https://news.ycombinator.com/item?id=49466006)

**背景**: 反编译是将可执行二进制代码还原为高级、可读语言的过程。过去，为避免法律问题，许多项目往往采用“净室”式重新实现；而如今很多现代项目直接反编译原始代码并发布为开源，这引发了未解决的版权问题。LLM 最近也进入了这一工作流，帮助逆向工程师快速注释函数、识别数据结构并生成可读的 C 代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Decompiler">Decompiler - Wikipedia</a></li>
<li><a href="https://www.scip.ch/en/?labs.20211202=">Reverse Engineering - Introduction to the World of Disassembling and Decompiling</a></li>

</ul>
</details>

**社区讨论**: 评论者对现代反编译项目表现出高度热情，称赞作者对 Snowboard Kids 所做的工作，并推荐了 Legend of Dragoon 重编译等相关项目。还有人发问：为什么游戏公司自己不利用这些成果来赚钱，同时质疑把原始游戏代码翻译成开源版本的法律地位。另有评论者强调，拥抱 LLM 后，开发者可以变成一台“机器”，只受时间、精力和 token 数量限制。

**标签**: `#decompilation`, `#reverse-engineering`, `#retro-gaming`, `#LLM`, `#software-engineering`

---

<a id="item-7"></a>
## [为 Agentic AI 构建可靠的数据基础](https://martinfowler.com/articles/making-data-ready-for-agentic-ai.html) ⭐️ 8.0/10

Martin Fowler 的网站发布了 Pramod Sadalage 和 Prem Chandrasekaran 撰写的一篇实用指南，介绍如何为代理式 AI（Agentic AI）系统准备准确、可信的数据基础。文中为那些因数据基础薄弱而影响 AI 效果的组织提供了可操作的建议。 随着代理式 AI 系统变得越来越自主，其决策和行动的可靠性完全取决于所访问的数据质量。这篇文章直击一个关键但常被忽视的挑战——组织若要大规模部署可信赖的 AI 智能体，就必须解决这个数据基础问题。 文章作者是 Pramod Sadalage 和 Prem Chandrasekaran，两人都是数据工程与 AI 领域的知名实践者。文章重点讨论数据准确性、信任度和可靠数据基础的建设，而不是模型架构或提示工程。

rss · Martin Fowler · 8月27日 13:11

**背景**: 代理式 AI（Agentic AI）指的是半自主或全自主的人工智能系统，它们能够感知、推理并采取行动，在有限监督下完成特定目标。这类系统高度依赖其访问的基础数据的质量、准确性和可信度。许多组织渴望采用 AI 来提高效率、节省成本，但它们的数据基础往往很脆弱，文章将此比喻为“沙子般的地基”，必须重建。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mitsloan.mit.edu/ideas-made-to-matter/agentic-ai-explained">Agentic AI, explained | MIT Sloan</a></li>
<li><a href="https://aws.amazon.com/what-is/agentic-ai/">What is Agentic AI? - Agentic AI Explained - AWS</a></li>
<li><a href="https://www.ibm.com/think/topics/agentic-ai">What is Agentic AI? | IBM</a></li>

</ul>
</details>

**标签**: `#agentic AI`, `#data engineering`, `#data quality`, `#AI infrastructure`

---

<a id="item-8"></a>
## [Qwen3.8-Flash-Next：开放权重 MoE 模型预览 Qwen4 架构](https://simonwillison.net/2026/Aug/26/qwen38-flash-next/) ⭐️ 8.0/10

Qwen 发布了 Qwen3.8-Flash-Next，这是一个开放权重的多模态混合专家（MoE）模型，作为 Qwen4 架构的早期预览。该模型总参数 125B，但仅激活 6B，运行效率高。 此次发布意义重大，因为让 AI 社区提前接触到 Qwen4 计划的架构思路，同时较小的激活参数规模使其在有限硬件上也能表现出色。开放权重意味着开发者可以自由实验和微调该模型。 根据技术分析，该模型采用混合线性-稀疏注意力机制和内置推测解码，以支持快速的智能体工作负载。Simon Willison 在 NVIDIA DGX Spark 上使用 Unsloth 的 GGUF 量化版本进行了测试，包括 72.5GB 的 UD-IQ1_S 和 78.9GB 的 UD-Q2_K_XL 变体。

rss · Simon Willison · 8月26日 23:52

**背景**: 混合专家（MoE）是一种机器学习技术，将模型划分为多个专门的专家网络，并仅将每个输入路由到相关的专家，从而在较低计算成本下实现更大的总参数量。GGUF 是一种量化格式，通过降低数值精度来减小模型文件大小，使大型模型能够通过 CPU/GPU 卸载在本地硬件上运行。Qwen 是一家定期发布开放权重模型的中国 AI 实验室；Qwen3.8-Flash-Next 被定位为即将推出的 Qwen4 时代的早期架构预览。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://modelfit.io/blog/qwen38-flash-next-open-weights/">Qwen3.8-Flash-Next: the Qwen 4 Architecture Preview Is Open...</a></li>

</ul>
</details>

**标签**: `#AI`, `#Qwen`, `#model release`, `#MoE`, `#open weights`

---

<a id="item-9"></a>
## [Visual Studio Code 1.135 版本更新发布](https://code.visualstudio.com/updates/v1_135) ⭐️ 7.0/10

VS Code 1.135 的更新日志现已发布，介绍了该编辑器的最新功能、改进和问题修复。本次更新延续了 VS Code 每月发布一次的节奏。 VS Code 是目前使用最广泛的开发者工具之一，因此每次月度更新都有可能改善数百万开发者的工作流程。即使是渐进式改进，也可能对日常编码效率产生广泛影响。 1.135 的更新日志可在 Visual Studio Code 官方网站上查看。与大多数月度更新一样，用户应查看日志中列出的具体功能变化、兼容性说明和新的扩展 API。

rss · Visual Studio Code · 8月26日 17:00

**背景**: Visual Studio Code 是微软推出的免费开源代码编辑器，支持多种编程语言，并可通过庞大的扩展市场进行功能扩展。微软大约每月发布一个新版本，每个版本都会在更新页面中总结其变化，包括新命令、设置项以及 API 新增内容。

**标签**: `#VS Code`, `#developer tools`, `#release notes`, `#IDE`

---

<a id="item-10"></a>
## [Lua 集成补丁让 PostgreSQL psql 支持自定义命令](https://postgr.es/p/9tg) ⭐️ 7.0/10

Pavel Stehule 发布了一组补丁，将 Lua 脚本语言集成到 PostgreSQL 的命令行客户端 psql 中。用户因此可以编写自定义的反斜杠命令，例如通过 pg_table_size 函数按大小排序表的 \dt 变体。 该补丁提供了一种在无需等待内核语法更改的情况下扩展 psql 的新方法，让高级用户能够用基于代码的方式灵活地定制工作流程。如果被采用，它可以减少对 pspg 分页器等外部变通方案的依赖，并促进更多社区驱动的 psql 功能增强。 该补丁引入了 psql.registerCommand API，使 Lua 处理器能够解析反斜杠命令选项、执行 SQL 并打印结果集。示例中还展示了如何使用 psql.scanSlashOption 和 psql.connect():escape() 进行选项扫描和字符串转义，并在无法识别选项时回退到标准 \dt 行为。

rss · Planet PostgreSQL · 8月26日 20:34

**背景**: psql 是 PostgreSQL 官方的交互式终端，传统上只支持固定的一组反斜杠命令以及基于 shell 的转义。Lua 是一种轻量、可嵌入的脚本语言，常用于游戏引擎和应用程序。作者此前在无法让内置的 \dt 排序功能被 PostgreSQL 接受后，创建了面向表格的分页器 pspg。这个补丁通过添加通用的 Lua 钩子，而非单一命令增强，重新回到该问题的解决上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://okbob.blogspot.com/2026/08/integration-lua-to-psql-ii.html">Pavel Stehule's blog: integration Lua to psql II</a></li>
<li><a href="https://github.com/okbob/lua-psql">GitHub - okbob/ lua - psql : patch that integrates lua to psql · GitHub</a></li>
<li><a href="https://github.com/okbob/pspg">GitHub - okbob/pspg: Unix pager (with very rich functionality) designed for work with tables. Designed for PostgreSQL, but MySQL is supported too. Works well with pgcli too. Can be used as CSV or TSV viewer too. It supports searching, selecting rows, columns, or block and export selected area to clipboard. · GitHub</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#psql`, `#Lua`, `#Extensibility`, `#Patches`

---

<a id="item-11"></a>
## [PostgreSQL 18 使用 UUID v7 将插入性能提升 23 倍](https://postgr.es/p/9tf) ⭐️ 7.0/10

一位开发者将 PostgreSQL 18.4 中的主键从 UUID v1/v4 切换为 UUID v7，并测得一条每分钟调用 12,000 次的多行插入查询，其平均执行时间最多提升了 23 倍。该更改通过一条 ALTER TABLE 命令完成，并使用较短的锁超时和大量重试来处理所需的排他锁。 这一真实基准测试表明，在高吞吐量的 PostgreSQL 系统中，选择正确的 UUID 版本可以大幅提升写入性能。它为开发者提供了采用 UUID v7 作为新主键的有力理由，尤其是在写入密集、索引页分裂和缓存未命中成为瓶颈的工作负载中。 最大的加速出现在一张数十亿行表上的多行插入查询，达到 23 倍；其他表则分别提升了 6 倍、8 倍、9 倍和 20 倍。由于 ALTER TABLE 需要排他锁，甚至会阻塞 SELECT，作者使用了较短的 lock_timeout 和重试机制来避免服务中断。

rss · Planet PostgreSQL · 8月26日 11:50

**背景**: UUID（通用唯一标识符）是常用作主键的 128 位标识符。UUID v4 是随机生成的，因此新的索引项会分散在 b-tree 索引中，导致更多页分裂和频繁的磁盘读取。UUID v1 基于时间但不具备单调递增性。UUID v7 按时间排序且单调递增，因此新插入的数据可以复用最近访问的“热”索引页，减少 I/O 并提升缓存性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Universally_unique_identifier">Universally unique identifier - Wikipedia</a></li>
<li><a href="https://www.uuidgenerator.net/version7">Version 7 Online UUID Generator Tool</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#UUID`, `#performance`, `#database optimization`, `#indexing`

---