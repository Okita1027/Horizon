---
layout: default
title: "Horizon 日报：2026-08-27 (ZH)"
date: 2026-08-27
lang: zh
---

> 从 46 条内容中筛选出 11 条重要资讯。

---

1. [英伟达以 130 亿美元收购 Hugging Face](#item-1) ⭐️ 10.0/10
2. [亚马逊 Mechanical Turk 将于 9 月 30 日关闭](#item-2) ⭐️ 9.0/10
3. [Z.ai 发布 GLM-5.3-Flash：体积更小、成本更低、性能接近旗舰](#item-3) ⭐️ 9.0/10
4. [FDA 批准首款转移性胰腺癌靶向疗法](#item-4) ⭐️ 9.0/10
5. [Asahi Linux 通过逆向 ACE3 为 M3 Mac 带来 USB 3.0 和 Thunderbolt 支持](#item-5) ⭐️ 8.0/10
6. [VS Code 推出 Agent Host，实现持久的 AI 代理会话](#item-6) ⭐️ 8.0/10
7. [PostgreSQL 18：UUID v7 主键实现插入性能提升 23 倍](#item-7) ⭐️ 8.0/10
8. [Qwen3.8-Flash-Next：多模态 MoE 模型预览 Qwen4 架构](#item-8) ⭐️ 8.0/10
9. [OpenTelemetry 插件扩展至 IntelliJ IDEA、GoLand、PyCharm 和 WebStorm](#item-9) ⭐️ 7.0/10
10. [PostgreSQL 开发者提议将 Lua 集成到 psql 以实现自定义命令](#item-10) ⭐️ 7.0/10
11. [EVE Online 启动从 Stackless Python 2.7 到 Python 3 的迁移](#item-11) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [英伟达以 130 亿美元收购 Hugging Face](https://www.businessinsider.com/nvidia-in-talks-to-buy-hugging-face-13-billion-dollars-2026-8) ⭐️ 10.0/10

英伟达已同意以 130 亿美元收购 Hugging Face，这是一个领先的开源 AI 模型平台。该交易首先由 The Information 和 TechCrunch 在 2026 年 8 月报道。 这笔里程碑式的交易可能重塑 AI 开发生态，因为英伟达将主导地位从硬件扩展到开源模型的分发与控制。开发者、初创公司以及开源社区都将受到影响，因为谁控制了 AI 模型的核心枢纽，谁就掌握了生态的话语权。 Hugging Face 去年晚些时候曾拒绝了英伟达 5 亿美元、估值 70 亿美元的投资，此前在 2023 年又放弃了一轮 2.35 亿美元、估值 45 亿美元的融资，因此这次 130 亿美元的全盘收购是一个惊人的反转。该交易还引发了反垄断担忧，因为英伟达将获得对平台数据（包括硬件调查和模型下载模式）的特权访问。

hackernews · mfiguiere · 8月27日 01:12 · [社区讨论](https://news.ycombinator.com/item?id=49458161)

**背景**: Hugging Face 是一家总部位于纽约的美国公司，开发用于构建机器学习应用的计算工具，包括广泛使用的 Transformers 库，以及一个供用户共享模型、数据集和演示的平台。它被认为是开源 AI 模型的事实上的中心。英伟达是 AI 芯片的主要供应商，收购 Hugging Face 将使它在开发者依赖的软件层中占据领先地位。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hugging_Face">Hugging Face</a></li>
<li><a href="https://medium.com/@fhirfly/title-exploring-the-best-ai-model-repositories-unleashing-the-power-of-open-source-ai-4ad165bb8077">Exploring the Best AI Model Repositories : Unleashing the... | Medium</a></li>

</ul>
</details>

**社区讨论**: 评论区大多持怀疑态度：GeertB 认为英伟达在开源方面记录不佳，会想要控制整个软件栈；esjeon 则指出对平台数据的特权访问可能构成反垄断问题。也有像 manlymuppet 这样的声音预测开发者将迎来一波免费积分，binarymax 则在祝贺团队之余希望“英伟达能善待社区”，并开玩笑说 130 亿美元应该够付几个月的 S3 出口费。Conol_ai 指出，Hugging Face 在不到一年内从拒绝英伟达 70 亿美元估值的投资，到以 130 亿美元被收购，颇具讽刺意味。

**标签**: `#acquisition`, `#nvidia`, `#huggingface`, `#ai`, `#open-source`

---

<a id="item-2"></a>
## [亚马逊 Mechanical Turk 将于 9 月 30 日关闭](https://www.mturk.com/) ⭐️ 9.0/10

亚马逊宣布其众包微任务平台 Mechanical Turk 将于 9 月 30 日关闭。该服务于 7 月已停止接受新客户。 这标志着众包微任务劳动时代的结束，影响了众多依赖 MTurk 获取收入和进行数据收集的工人与研究者。此次关闭也凸显了 AI 正在颠覆这些曾由人类完成的小任务的平台。 该平台将于 9 月 30 日完全关闭，一位请求者指出，领导 MTurk 的 AWS 高级项目经理在两三年前已转至 Amazon Bedrock 和 SageMaker Model Evaluations。储值账户也已迁移至原生 AWS 计费系统。

hackernews · tmp10423288442 · 8月26日 23:55 · [社区讨论](https://news.ycombinator.com/item?id=49457545)

**背景**: Amazon Mechanical Turk 于 2005 年推出，是一个众包市场，让企业和个人将称为人类智能任务（HITs）的小任务外包给分散的劳动力。这些微任务（如图像识别或数据验证）对人类简单但对计算机困难，该平台在工业界和学术研究中被广泛使用。此次关闭反映了更广泛的趋势：AI 现在可以完成许多非技能型微任务，减少了该领域对人类劳动力的需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Amazon_Mechanical_Turk">Amazon Mechanical Turk - Wikipedia</a></li>
<li><a href="https://docs.aws.amazon.com/AWSMechTurk/latest/AWSMechanicalTurkRequester/WhatIs.html">What is Amazon Mechanical Turk ? - Amazon Mechanical Turk</a></li>
<li><a href="https://www.mturk.com/">Amazon Mechanical Turk</a></li>

</ul>
</details>

**社区讨论**: 评论者情绪复杂，有人指出 AI 涌入和任务套利使 MTurk 在非技能型工作上不再可行，而另一些人强调如今验证 AI 输出需要领域专业知识。一位请求者指出领导层已转向其他 AWS 项目，还有用户分享了 2005 年 MTurk 帮助他们个人的故事。一些人认为在这样一个平台本可以赋能 AI 代理执行真实世界物理任务的时刻关闭它，实在疯狂。

**标签**: `#Mechanical Turk`, `#Amazon`, `#crowdsourcing`, `#AI`, `#platform shutdown`

---

<a id="item-3"></a>
## [Z.ai 发布 GLM-5.3-Flash：体积更小、成本更低、性能接近旗舰](https://z.ai/blog/glm-5.3-flash) ⭐️ 9.0/10

Z.ai 发布了 GLM-5.3-Flash，这是 GLM-5.3 的精简版本，参数数量减半，成本降至五分之一，同时保留了接近旗舰机型的性能。该开源权重模型已上线 Hugging Face，并在国产芯片上提供服务。 此次发布标志着高性价比 AI 推理的重要进展，使高性能大型语言模型对开发者和企业更加可及。它也加剧了中国 AI 实验室（如 Z.ai、DeepSeek 和 Kimi）之间的竞争，并展示了在国产硬件上运行先进模型的进展。 GLM-5.3-Flash 仅在 GLM-5.3 发布 12 天后推出，作为 “Flash” 轻量级版本，参数更少、价格仅为五分之一。社区基准测试显示，它能够以极低的成本匹敌 DeepSeek v4 Pro，其权重可在 huggingface.co/zai-org/GLM-5.3-Flash 获取。

hackernews · Philpax · 8月26日 14:08 · [社区讨论](https://news.ycombinator.com/item?id=49449507)

**背景**: Z.ai 原名智谱 AI，是一家中国人工智能公司，以开发开源权重的大型语言模型 GLM（General Language Model）系列而闻名。GLM 模型基于 Transformer 架构，与 OpenAI 的 GPT 等其他大语言模型类似，在大量数据集上进行预训练以生成文本。GLM-5.3-Flash 这类高性价比模型的发布，体现了中国 AI 实验室快速迭代、降低推理成本的趋势，同时由于先进半导体出口管制，这些实验室常使用国产芯片。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GLM_(AI)">GLM (AI) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Z.ai">Z.ai - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT_(language_model)">GPT (language model)</a></li>

</ul>
</details>

**社区讨论**: Hacker News 社区对此次发布既感到兴奋又持怀疑态度。有用户对快速迭代和高性价比表示赞赏，指出在低成本下超越 DeepSeek v4 Pro 和 Luna；另一些用户则提醒说中国实验室有操纵基准测试的历史，并警告 Z.ai 的服务条款对用户输入和输出授予了过于宽泛的许可。

**标签**: `#AI/ML`, `#GLM`, `#LLM`, `#model release`, `#cost efficiency`

---

<a id="item-4"></a>
## [FDA 批准首款转移性胰腺癌靶向疗法](https://www.fda.gov/news-events/press-announcements/fda-approves-first-class-targeted-therapy-metastatic-pancreatic-cancer) ⭐️ 9.0/10

美国 FDA 批准了首款针对转移性胰腺癌的靶向疗法，这也是 RAS 抑制剂首次获批用于该适应症。这一批准标志着这一治疗选择有限的疾病迎来里程碑式进展。 该批准为转移性胰腺癌患者提供了新的治疗选择，而这类疾病历来难以治疗。它也验证了将 RAS 蛋白作为药物靶点这一长期目标——RAS 曾被认为是“不可成药的”，未来有望推动该类药物在其他 KRAS 突变癌症中的获批。 此次审评速度引人注目，从 FDA 受理新药申请到批准仅用了一个多月，这得益于 FDA 的 CNPV 试点项目。作为一种 RAS 抑制剂，该疗法靶向 KRAS 突变，而 KRAS 突变存在于多种器官的大量癌症中。

hackernews · leopoldj · 8月26日 16:19 · [社区讨论](https://news.ycombinator.com/item?id=49451675)

**背景**: RAS 蛋白是细胞生长的关键调控因子，KRAS 等基因的突变是最常见的癌症驱动因素之一。由于 RAS 蛋白表面光滑、缺乏明确的药物结合口袋，几十年来它一直被认为是“不可成药”的靶点。近年来的药物设计进展使研究者开发出能够与活化状态突变 RAS 结合的 RAS 抑制剂，从而阻断肿瘤生长。此次获批药物专门针对转移性胰腺癌，这类癌症预后极差，传统上主要依赖化疗。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pubmed.ncbi.nlm.nih.gov/39700396/">A Pan-RAS Inhibitor with a Unique Mechanism of Action Blocks Tumor Growth and Induces Antitumor Immunity in Gastrointestinal Cancer - PubMed</a></li>
<li><a href="https://aacrjournals.org/mct/article/24/1/33/750651/Advances-and-Challenges-in-RAS-Signaling-Targeted">Advances and Challenges in RAS Signaling Targeted Therapy in Leukemia | Molecular Cancer Therapeutics | American Association for Cancer Research</a></li>

</ul>
</details>

**社区讨论**: 评论者从个人情感和科学角度表达了看法。有人分享了家人因胰腺癌去世的痛苦经历，并对新药表示欢迎。还有评论强调了该药对 RAS 突变癌症的更广泛意义，以及 FDA 在 CNPV 试点项目下异常快速的审评。

**标签**: `#FDA approval`, `#pancreatic cancer`, `#targeted therapy`, `#RAS inhibitor`, `#medical breakthrough`

---

<a id="item-5"></a>
## [Asahi Linux 通过逆向 ACE3 为 M3 Mac 带来 USB 3.0 和 Thunderbolt 支持](https://asahilinux.org/2026/08/progress-report-7-2/) ⭐️ 8.0/10

Asahi Linux 7.2 版进展报告宣布，所有 M3 系列 Apple Silicon 设备现已获得 USB 3.0 和 Thunderbolt 支持。这是通过逆向苹果的 ACE3 USB-C 控制器实现的，研究发现它与 CD3217 具有几乎相同的寄存器集，但通过 SPMI 接口而非 I2C 访问。 这一里程碑显著提升了 M3 Mac 作为 Linux 机器的可用性，扩大了对日益增长的 ARM 笔记本硬件的支持。它也证明了社区驱动的逆向工程能够在苹果缺乏官方文档的情况下持续填补空白。 ACE3 控制器是德州仪器制造的微控制器，运行完整的 USB 协议栈，并连接到 SPMI 和 JTAG 等内部总线。Asahi 团队的工作同时覆盖了 SPMI 接口和 ACE3 本身，从而为所有 M3 系列设备（包括 M3 Pro 和 M3 Max）带来了 USB 3.0 和 Thunderbolt 支持。

hackernews · pizzaiolo · 8月26日 22:35 · [社区讨论](https://news.ycombinator.com/item?id=49456851)

**背景**: Asahi Linux 是一个开源项目，通过逆向工程苹果未公开文档化的硬件，将 Linux 内核及相关软件移植到 Apple Silicon Mac 上。ACE3 是苹果专有的 USB-C 控制器，也用于 iPhone 15 系列，负责管理电源传输和数据传输。该项目此前已为 Apple Silicon 带来图形、音频及其他外设支持，本次更新将连接功能支持扩展到 M3 一代。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Asahi_Linux">Asahi Linux - Wikipedia</a></li>
<li><a href="https://asahilinux.org/">Asahi Linux</a></li>
<li><a href="https://www.tomsguide.com/phones/iphones/apples-proprietary-usb-c-controller-has-officially-been-hacked-what-you-need-to-know">Apple’s proprietary USB-C controller has officially been ... Apple faces new USB-C threat: The ACE3 hack explained Researchers Hacked into Apple’s New USB-C Controller Security researcher Thomas Roth dumps ROM of ACE3 USB-C ... Apple’s USB-C ACE3 controller hack, what it means for users Apple iPhone USB-C Hack Reveals a Major Security Breakthrough The ACE3 USB Controller Has Been Hacked: What Does This Mean ...</a></li>

</ul>
</details>

**社区讨论**: 评论者对 Asahi 团队的成就表示高度钦佩，有人提到项目在“不稳定的沙地上”取得的进展。一些人担心 Linux 的电源管理和电池续航，另有人质疑英特尔和 AMD 能效的提升是否会减少在 M 系列笔记本上运行 Linux 的需求。一条技术评论指出，ARM 规范要求 WFI 循环保留所有状态，而这并非 Apple Silicon 的默认模式。

**标签**: `#Asahi Linux`, `#Apple Silicon`, `#Linux kernel`, `#Thunderbolt`, `#Reverse engineering`

---

<a id="item-6"></a>
## [VS Code 推出 Agent Host，实现持久的 AI 代理会话](https://code.visualstudio.com/blogs/2026/08/26/agent-host-architecture) ⭐️ 8.0/10

Visual Studio Code 宣布了 Agent Host 架构，这是一个独立进程，通过 Agent Host Protocol（AHP）将 AI 代理与编辑器解耦。它支持持久化、同步的代理会话，可在本地或远程运行，并可在多个窗口和客户端之间共享。 这一里程碑标志着 AI 辅助开发领域的重大架构转变，将 AHP 与 LSP 和 DAP 并列为面向代理工具开放协议。开发者可以在本地启动会话并在远程继续，从而实现更灵活、更协作的 AI 编码工作流。 远程 Agent Host 以独立进程运行，通过 WebSocket 暴露 AHP，并可通过 SSH 或专用开发隧道访问。AHP 基于不可变状态、纯 reducer 和预写日志协调机制，为多个客户端提供 AI 代理会话的同步视图。

rss · Visual Studio Code · 8月26日 00:00

**背景**: Agent Host Protocol 是一种可移植的独立服务器协议，定义了会话服务器如何与其客户端通信。客户端发送的命令会以变更状态的操作形式被返回，从而允许从任何连接的客户端恢复会话。该架构将语言服务器和调试适配器的模型扩展到了 AI 代理领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://code.visualstudio.com/docs/agents/concepts/agent-host">VS Code Agent Host architecture</a></li>
<li><a href="https://github.com/microsoft/agent-host-protocol">GitHub - microsoft/agent-host-protocol: Synchronized multi ...</a></li>
<li><a href="https://microsoft.github.io/agent-host-protocol/">Agent Host Protocol</a></li>

</ul>
</details>

**标签**: `#VS Code`, `#AI agents`, `#architecture`, `#developer tools`, `#agent sessions`

---

<a id="item-7"></a>
## [PostgreSQL 18：UUID v7 主键实现插入性能提升 23 倍](https://postgr.es/p/9tf) ⭐️ 8.0/10

Andrew Atkinson 将多个 PostgreSQL 18.4 表的主键从随机的 UUID v1/v4 改为按时间排序的 UUID v7 默认值，并在每分钟执行 12000 次的高流量多行插入查询上测得最高 23 倍的插入加速。最大提升出现在一个拥有数十亿行的表上，其中有五个查询分别获得了 6x、8x、9x、20x 和 23x 的加速。 由于 UUID v7 嵌入了时间戳，新的主键值是单调递增的，因此 B-tree 索引条目会落到同一个热缓冲缓存页中，从而减少页分裂、WAL 和磁盘 I/O。这对于希望使用 UUID 但又无法承受 UUID v4 插入性能损耗的高写入应用来说，提供了一条实用路径。 每张表的迁移只需执行一条 ALTER TABLE 语句，但它会获取排他锁，甚至阻塞 SELECT；作者通过较短的 lock_timeout 和重试来缓解这一点。大多数表没有明显变化，但受影响最大的查询提升显著，而且 v7 还因页分裂更少而使得索引更小。

rss · Planet PostgreSQL · 8月26日 11:50

**背景**: UUID 是作为主键使用的 128 位标识符。版本 4 是随机的，因此新值会散布在 B-tree 索引中，导致缓存未命中和页分裂。版本 7 编码了 Unix 纪元毫秒时间戳加上随机位，使值可排序且单调递增，从而改善了索引局部性。对于 schema 变更，PostgreSQL 的 DDL 需要排他锁，因此生产团队会使用 lock_timeout 和重试来避免长时间排队和停机。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Universally_unique_identifier">Universally unique identifier - Wikipedia</a></li>
<li><a href="https://postgres.ai/blog/20210923-zero-downtime-postgres-schema-migrations-lock-timeout-and-retries">Zero-downtime Postgres schema migrations need this: lock_timeout and retries | PostgresAI</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#UUID`, `#performance`, `#database`, `#indexing`

---

<a id="item-8"></a>
## [Qwen3.8-Flash-Next：多模态 MoE 模型预览 Qwen4 架构](https://simonwillison.net/2026/Aug/26/qwen38-flash-next/) ⭐️ 8.0/10

Qwen 发布了 Qwen3.8-Flash-Next，这是一个大型开源权重多模态混合专家（MoE）模型，作为 Qwen4 架构的早期预览。尽管其总参数达到 125B，但只有 6B 活跃参数，从而带来显著的性能提升。 此次发布标志着 Qwen 在推动开源权重多模态模型向更高效率发展，并让开发者提前了解 Qwen4 预期采用的架构。6B 活跃参数的设计使大型 MoE 模型在本地推理和实际应用中更加实用。 该模型通过 Unsloth 提供 GGUF 量化版本，包括 Simon Willison 在 NVIDIA DGX Spark 上测试过的 UD-IQ1_S 和 UD-Q2_K_XL 变体。它支持多模态能力，能够生成如鹈鹕插图等图像，并支持高推理强度模式。

rss · Simon Willison · 8月26日 23:52

**背景**: 混合专家（MoE）是一种神经网络架构，对每个词元只激活一部分“专家”子模型，从而在降低计算成本的同时实现大规模模型。GGUF 是一种用于存储量化大型语言模型的文件格式，通过降低模型精度来减小文件大小和内存占用，使其更容易在本地运行。IQ1_S 和 Q2_K_XL 等量化方法以模型质量为代价换取更小的体积，常见于 llama.cpp 等工具中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mixture-of-experts">A Visual Guide to Mixture of Experts ( MoE )</a></li>
<li><a href="https://ggufloader.github.io/what-is-gguf.html">What is GGUF ? Complete Guide to GGUF Format & Quantization</a></li>
<li><a href="https://kaitchup.substack.com/p/choosing-a-gguf-model-k-quants-i">Choosing a GGUF Model: K-Quants, I-Quants, and Legacy Formats</a></li>

</ul>
</details>

**标签**: `#Qwen`, `#LLM`, `#MoE`, `#multimodal`, `#open-weights`

---

<a id="item-9"></a>
## [OpenTelemetry 插件扩展至 IntelliJ IDEA、GoLand、PyCharm 和 WebStorm](https://blog.jetbrains.com/platform/2026/08/opentelemetry-plugin-for-jetbrains-ides/) ⭐️ 7.0/10

JetBrains 在 2026.2 版本中将其 OpenTelemetry 插件扩展到了 IntelliJ IDEA、GoLand、PyCharm 和 WebStorm。此前该插件仅适用于 JetBrains Rider。 这使得使用不同 JetBrains IDE 的开发者能更方便地使用可观测性工具。通过将 OpenTelemetry 集成到编辑器工作流中，可以帮助开发者更高效地调试和排查分布式应用问题。 该插件属于 2026.2 发布周期的一部分，并且公告明确表示 Rider 用户依然可以使用。JetBrains 指出，这次扩展是开发者有计划推进的工作，而非偶然产生的结果。

rss · JetBrains WebStorm · 8月26日 07:40

**背景**: OpenTelemetry 是一个开源的可观测性框架，为采集追踪（traces）、指标（metrics）和日志（logs）提供标准化的 API、SDK 和工具。它旨在帮助开发者监控分布式系统，被广泛视为现代云原生可观测性的默认选择。JetBrains 插件将该能力集成到 IDE 中，可能让开发者无需离开编码环境即可查看遥测数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://opentelemetry.io/docs/what-is-opentelemetry/">What is OpenTelemetry ? | OpenTelemetry</a></li>
<li><a href="https://signoz.io/opentelemetry/">What is OpenTelemetry ? Architecture & Benefits | SigNoz</a></li>

</ul>
</details>

**标签**: `#OpenTelemetry`, `#JetBrains`, `#IDE`, `#Observability`, `#Developer Tools`

---

<a id="item-10"></a>
## [PostgreSQL 开发者提议将 Lua 集成到 psql 以实现自定义命令](https://postgr.es/p/9tg) ⭐️ 7.0/10

Pavel Stehule 发布了一组将 Lua 集成到 psql（PostgreSQL 命令行客户端）的补丁。这些补丁允许用户注册自定义斜杠命令，例如可按大小排序表的 \dt 命令。 这可能会让 psql 更具可扩展性，允许用户无需等待核心语法共识即可定制命令。对于希望在 psql 中实现自定义工作流的 PostgreSQL 高级用户和开发者来说，这非常相关。 该补丁引入了 psql.registerCommand、psql.scanSlashOption、psql.exec、psql.printQuery 和 psql.connect 等 API。示例命令使用 \if :{?LUA_RELEASE} 和 \luacode 代码块有条件地定义新的 \my.dt 命令。

rss · Planet PostgreSQL · 8月26日 20:34

**背景**: psql 是 PostgreSQL 官方的交互式终端客户端，提供诸如 \dt 之类的内置反斜杠命令来列出表。扩展这些命令历来需要核心补丁讨论或外部工具；Pavel Stehule 之前创建了 pspg 分页器，以便按任意列对结果排序。Lua 是一种轻量级脚本语言，经常嵌入到应用程序中，本提案将其嵌入 psql，使用户可以编写自己的命令逻辑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/okbob/pspg">GitHub - okbob/pspg: Unix pager (with very rich functionality ... pspg - Postgres Pager pspg download | SourceForge.net pspg: Terminal pager built for exploring tabular data with ... pspg/tools at master · okbob/pspg · GitHub pspg - Postgres pager - LinuxLinks pspg · Terminal Tools</a></li>
<li><a href="https://github.com/pllua/pllua">GitHub - pllua/pllua: Re-implementation of pllua, embedded Lua for postgresql · GitHub</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#Lua`, `#psql`, `#extensions`

---

<a id="item-11"></a>
## [EVE Online 启动从 Stackless Python 2.7 到 Python 3 的迁移](https://simonwillison.net/2026/Aug/25/eve-online-move-to-python-3/) ⭐️ 7.0/10

EVE Online 官方宣布开始从 Stackless Python 2.7 迁移到 Python 3，这一过程将使用 futurize 脚本处理 240 万行代码。随后团队将手动审查大约 2 万个 Python 2 与 Python 3 行为差异之处。 这标志着游戏行业中规模最大、运行时间最长的 Python 代码库之一迎来了重要里程碑，为类似规模的大型遗留 Python 2 系统提供了切实可行的迁移路径。由于 Python 2 早已停止支持，此次迁移的规模和具体技术方案将受到 Python 社区的高度关注。 本次迁移将使用 futurize 脚本自动转换代码库，随后手动审查行为差异，例如整数除法在 Python 2 中 1 / 2 结果为 0，而在 Python 3 中为 0.5。公告尚未说明 EVE Online 将如何替代 Stackless，不过去年的大会演讲介绍了他们如何在较新游戏 EVE Frontier 中使用 carbonengine/scheduler 库。

rss · Simon Willison · 8月25日 22:59

**背景**: Stackless Python 是 Python 解释器的增强版本，通过称为 tasklet 的微线程提供轻量级并发，EVE Online 自 2003 年上线以来一直依赖该功能。该项目已于 2025 年 2 月正式停止维护，其 GitHub 仓库也已归档。futurize 是 python-future 项目提供的工具，可自动将 Python 2 代码转换为兼容 Python 3 的代码，同时在此过程中保留 Python 2 兼容性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Stackless_Python">Stackless Python</a></li>
<li><a href="https://python-future.org/futurize.html">futurize : Py2 to Py2/ 3 — Python -Future documentation</a></li>
<li><a href="https://github.com/stackless-dev/stackless/wiki">Home · stackless-dev/stackless Wiki · GitHub</a></li>

</ul>
</details>

**标签**: `#Python`, `#migration`, `#EVE Online`, `#Stackless Python`, `#legacy code`

---