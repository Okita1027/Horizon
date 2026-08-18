---
layout: default
title: "Horizon 日报：2026-08-18 (ZH)"
date: 2026-08-18
lang: zh
---

> 从 37 条内容中筛选出 14 条重要资讯。

---

1. [DuckDB v2.0 预览版发布，引发数据社区热议](#item-1) ⭐️ 9.0/10
2. [Qwen3.8 27B 在 Artificial Analysis 获 52 分，超越更大模型](#item-2) ⭐️ 9.0/10
3. [Rust 原生 GPU 卸载：可移植、安全且快速](#item-3) ⭐️ 8.0/10
4. [AI 生成的 Copilot Autofix 在 Snowflake Jira 工作流中引入漏洞](#item-4) ⭐️ 8.0/10
5. [如何关闭或避开强制 AI 功能：一份指南引发热议](#item-5) ⭐️ 8.0/10
6. [AirTag 追踪稀有书籍订单至亚马逊 AI 训练设施](#item-6) ⭐️ 8.0/10
7. [Qwen 3.8 27B：本地运行出色，但默认过度思考](#item-7) ⭐️ 8.0/10
8. [Dario Amodei：AI 遭公众不信任折射更广泛的信任危机](#item-8) ⭐️ 8.0/10
9. [在 Kubernetes 上使用 CloudNativePG PostgreSQL 后端运行 OpenBao](#item-9) ⭐️ 7.0/10
10. [PostgreSQL 为何跳过索引？调整 random_page_cost 至 1.1 可提速](#item-10) ⭐️ 7.0/10
11. [Postgres 19 图查询：固定深度等同连接，变深度仍需递归 CTE](#item-11) ⭐️ 7.0/10
12. [PostgreSQL 17：传统列优于 JSONB+GIN，唯多键包含查询例外](#item-12) ⭐️ 7.0/10
13. [覆盖索引：PostgreSQL 17 写入开销增加 28%，读取加快 1.26 倍](#item-13) ⭐️ 7.0/10
14. [Flyway validate 检查的是文件完整性，而非数据库结构](#item-14) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [DuckDB v2.0 预览版发布，引发数据社区热议](https://duckdb.org/2026/08/17/duckdb-20-highlights) ⭐️ 9.0/10

DuckDB 于 2026 年 8 月 17 日发布了 v2.0 预览版，这是其嵌入式分析数据库的一次重大版本更新。该公告迅速引发广泛关注，在 Hacker News 上获得了 517 个点赞和 91 条评论。 DuckDB 已成为数据工程和分析领域的常用工具，因此 v2.0 的重大版本更新可能会带来显著的性能提升和新功能。对于大量使用 DuckDB 从流处理管道到大规模分析负载的开发者社区来说，这次预览具有重要意义。 社区讨论中提到了 v2.0 中代号为 “Quack” 的功能，并称赞 DuckDB 的超内存（out-of-core）处理能力。一位评论者指出，该项目在不到六个月内产生了约 10,000 次提交，凸显了其快速的开发节奏。

hackernews · ibotty · 8月17日 13:46 · [社区讨论](https://news.ycombinator.com/item?id=49330781)

**背景**: DuckDB 是一种进程内分析数据库引擎，专为快速执行复杂 SQL 查询而设计，通常直接嵌入应用程序或与 Python 和 R 一起使用。它以可移植性、简单性以及能够处理大于可用内存的数据集而著称。v2.0 的发布标志着该项目在多年增量更新后的一个重要里程碑。

**社区讨论**: 社区反响非常积极，用户纷纷分享实际应用案例，包括构建流处理系统以及在多家公司引入 DuckDB。一些评论者对 Quack 等特定功能表示期待，同时也有用户提出疑问，询问 AI 是否推动了项目如此快速的开发节奏。

**标签**: `#duckdb`, `#database`, `#data-engineering`, `#analytics`, `#release`

---

<a id="item-2"></a>
## [Qwen3.8 27B 在 Artificial Analysis 获 52 分，超越更大模型](https://artificialanalysis.ai/models/qwen3-8-27b) ⭐️ 9.0/10

开源权重稠密视觉语言模型 Qwen3.8 27B 在 Artificial Analysis Intelligence Index 上获得 52 分，与 DeepSeek V4 Flash 0731 持平，并超过所有中等规模模型（40B–150B）。这个分数远高于可比模型的中位数 9。 一个 27B 模型能与 Claude Opus 4.6 等规模大得多的前沿模型匹敌，意味着重大效率突破，可能降低获得高级 AI 能力的成本和硬件门槛。它能在游戏 PC 上流畅运行，让接近前沿的性能惠及个人和小型机构。 在评测过程中，Qwen3.8 27B 生成了 1.6 亿个 token，而中位数为 4300 万，说明其输出非常冗长。Artificial Analysis Intelligence Index 是仅限文本、仅限英语的基准套件，因此图像输入、语音输入和多语言能力会单独评测。

hackernews · anana_ · 8月17日 17:25 · [社区讨论](https://news.ycombinator.com/item?id=49334544)

**背景**: Artificial Analysis Intelligence Index 是用于对 AI 模型在推理、知识和指令遵循方面排序的纯文本英语基准套件。Qwen 是阿里巴巴的开源权重模型系列；Qwen3.8 27B 是基于 Qwen 3.5 架构的紧凑型稠密视觉语言模型，支持编码、专业工作、研究和长周期智能体任务。它的体积小且为稠密架构，因此可以在游戏 PC 等消费级硬件上本地运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/models/qwen3-8-27b">Qwen 3 . 8 27 B - Intelligence, Performance & Price Analysis</a></li>
<li><a href="https://lmstudio.ai/models/qwen/qwen3.8-27b">qwen/ qwen 3 . 8 - 27 b • LM Studio</a></li>
<li><a href="https://artificialanalysis.ai/methodology/intelligence-benchmarking">Artificial Analysis Intelligence Benchmarking Methodology</a></li>

</ul>
</details>

**社区讨论**: 评论者对一个 27B 模型能匹敌甚至超越大得多的前沿模型表示惊叹和难以置信，有人说这“既好笑又有点可怕”。动手使用过的用户形容它聪明且异常“智能体化”，甚至会执着地解决问题，令人联想到 GPT-5.6-Sol-max；还有人表示会进行大量测试。也有观点指出，虽然它的分数超过 Opus 4.6，但 Opus 的世界知识更好；另外一位用户关于内部基准的评论被截断。

**标签**: `#AI`, `#machine learning`, `#Qwen`, `#benchmarks`, `#efficiency`

---

<a id="item-3"></a>
## [Rust 原生 GPU 卸载：可移植、安全且快速](https://arxiv.org/abs/2608.13759) ⭐️ 8.0/10

一篇新研究论文（arXiv:2608.13759）提出一个原生构建于 Rust 编译器（rustc）和 LLVM 后端中的零开销、多厂商 GPU 编译框架，无需外部绑定即可在 GPU 上卸载执行 Rust 代码。这项工作利用 Rust 的所有权和别名保证，通过 LLVM 的 Offload 基础设施实现自动数据移动。 目前 Rust 开发者进行 GPU 编程时不得不依赖外部绑定或特定厂商的工具（如 ROCm 绑定、CUDA 绑定），这会带来维护和兼容性负担。该项目与 Rust 官方 2025H2 目标相关，可能让 Rust 成为可移植 GPU 计算的一等语言，直接解决 HPC 和 AI/LLM 推理工作负载中的一大痛点。 该实现基于 LLVM 的 “offload” 项目，也就是 OpenMP 用来在 GPU 上运行 C++/Fortran 的同一套基础设施；它支持自动、高效的数据移动，后续还会提供可选的、更高级的 unsafe 接口以提供更高控制度。rust-lang/goals 文档指出，后端仍需继续改进如何将 Rust 代码降低到 GPU，并会在 Rust 测试套件中加入越来越复杂的计算内核。

hackernews · linggen · 8月17日 17:54 · [社区讨论](https://news.ycombinator.com/item?id=49334991)

**背景**: GPU 卸载（GPU offload）是指将程序中计算密集的部分从 CPU 卸载到 GPU 上并行执行。传统上这需要用厂商语言编写内核，并通过 CUDA/ROCm 或图形 API 等绑定/运行时来调用，这在 Rust 中是一个很大的痛点。Rust GPU 项目（最初由 Embark Studios 发起，现已转由社区维护）通过编译器后端让 Rust 成为 GPU 着色器的一等语言；而本次的 offload 工作则直接在 rustc 和 LLVM 中实现，采用不同的、更通用的方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2608.13759">[2608.13759] GPU Offload in Rust: Portable, Safe, and Fast</a></li>
<li><a href="https://rustc-dev-guide.rust-lang.org/offload/internals.html">GPU offload internals - Rust Compiler Development Guide</a></li>
<li><a href="https://github.com/rust-lang/goals/blob/main/src/2025h2/finishing-gpu-offload.md">goals/src/2025h2/finishing-gpu-offload.md at main · rust-lang/goals</a></li>

</ul>
</details>

**社区讨论**: 社区总体态度积极但谨慎：一位构建自定义 LLM 推理引擎的用户称绑定是“一个很大的头痛”，并表示会从第一天就尝试；另一位用户则询问是否已发布任何代码。一条更技术性的评论质疑为何走 LLVM 路线，而不是直接从 MIR 生成 PTX/HIP，并指出已有基于 Vulkan 和 SPIR-V 的解决方案；还有评论者询问该项目是否主要面向 HPC 和自包含的异构主机二进制文件。

**标签**: `#Rust`, `#GPU`, `#LLVM`, `#Systems Programming`, `#Research`

---

<a id="item-4"></a>
## [AI 生成的 Copilot Autofix 在 Snowflake Jira 工作流中引入漏洞](https://www.wiz.io/blog/red-agent-snowflake-copilot-cicd-bug) ⭐️ 8.0/10

Wiz 的研究人员报告称，GitHub Copilot Autofix 在 Snowflake 的 GitHub Actions 工作流中引入了一个脚本注入漏洞，该漏洞随后被利用以攻破 Snowflake 的 Jira 自动化流程。这一不安全的模式——将 issue 标题和正文未转义地插入 `run:` 代码块——后来被 zizmor 静态分析工具标记出来。 这起事件表明，AI 生成的安全修复本身也可能成为攻击载体，而不仅仅是一般 AI 生成的代码存在风险。它强调了即使补丁最初由机器建议，拥有高权限令牌的 CI/CD 工作流仍必须进行静态分析和人工审查。 受影响的文件是 jira_issue.yml；在第 24 行，该工作流将 GitHub issue 的标题和正文未转义地回显到 shell 命令中，导致可通过 `${{ ... }}` 表达式展开进行模板注入。GitHub 文档将这种情况归类为脚本注入风险，因为不受信任的 pull request 或 issue 内容可能触发 action 并执行任意命令。

hackernews · galnagli · 8月17日 14:18 · [社区讨论](https://news.ycombinator.com/item?id=49331423)

**背景**: GitHub Actions 是一种 CI/CD 服务，仓库通过 YAML 文件定义自动化工作流。`run:` 步骤会执行 shell 命令，而 `${{ github.event.issue.title }}` 之类的 GitHub 表达式会在脚本执行前被求值，因此攻击者如果能够控制 issue 标题，就可以逃逸出预期命令并执行任意代码。GitHub Copilot Autofix 是一种智能代理功能，可为代码扫描警报建议补丁；在这个案例中，它建议的补丁没有正确转义用户可控数据，从而引入了漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.github.com/en/code-security/concepts/code-scanning/autofix-for-code-scanning">About autofix for code scanning - GitHub Docs</a></li>
<li><a href="https://docs.github.com/en/actions/reference/security/secure-use">Secure use reference - GitHub Docs</a></li>
<li><a href="https://www.wiz.io/blog/github-actions-security-guide">Hardening GitHub Actions: Lessons from Recent Attacks | Wiz Blog</a></li>

</ul>
</details>

**社区讨论**: 评论者大多对编写该修复的开发者表示理解，同时认为 GitHub Actions 工作流应始终使用 zizmor 等静态分析工具进行检查。有评论者指出，AI 降低了生成改动的成本，但并没有降低审查成本，瓶颈正从代码生成转向验证；还有评论者对 Copilot 是否真的导致了该漏洞提出质疑。

**标签**: `#AI security`, `#GitHub Actions`, `#CI/CD`, `#vulnerability`, `#Copilot`

---

<a id="item-5"></a>
## [如何关闭或避开强制 AI 功能：一份指南引发热议](https://www.librarian.net/notoai/) ⭐️ 8.0/10

librarian.net 发布了一份题为“如何关闭或避免侵入式 AI”的实用指南，并提供了短链接 NoToAI.org，帮助用户在各平台关闭或绕过 AI 功能。该指南迅速在 Hacker News 上引发关注，获得了 248 分和 151 条评论。 这一事件反映了用户对 AI 功能被强行整合进日常软件的不满情绪日益增长，可能促使企业重新思考如何部署这类工具。其重要性在于，围绕用户控制与 AI 强制使用的讨论，可能会影响未来的产品设计和隐私政策。 指南作者 jessamyn 欢迎补充建议，评论区也指出了额外选项，如 LibreWolf、Waterfox 和 Codeberg。一个突出的抱怨是 Apple CarPlay 即使对音乐和地图等非 AI 功能也要求启用 Siri，说明缺乏备用状态会让用户被锁定在功能之外。

hackernews · ColinWright · 8月17日 14:07 · [社区讨论](https://news.ycombinator.com/item?id=49331220)

**背景**: 科技公司越来越多地将 AI 助手和生成式功能嵌入操作系统、浏览器和移动应用中，通常没有简单的关闭方式。一些不想使用 AI 的用户发现自己被锁定在基本功能之外，比如 CarPlay 必须使用 Siri 的示例。因此，社区维护指南以及部分用户转而使用 Linux 或替代浏览器来避开 AI 集成。

**社区讨论**: 评论者普遍对公司强制推行 AI 功能表示不满，有人说“市场确实可以长期保持非理性”。不少人建议改用 Linux 或 LibreWolf、Waterfox 等替代浏览器，而指南作者也积极参与并乐于接受建议。

**标签**: `#AI`, `#privacy`, `#user-control`, `#browsers`, `#Linux`

---

<a id="item-6"></a>
## [AirTag 追踪稀有书籍订单至亚马逊 AI 训练设施](https://simonwillison.net/2026/Aug/17/we-tracked-a-shipment-of-rare-books-it-ended-at-an-amazon-ai-tra/) ⭐️ 8.0/10

404 Media 将一个苹果 AirTag 藏在一本稀有书籍中，该书属于 Biblio 上约 1000 本书的批量订单，并追踪到拉斯维加斯亚马逊 LAS8 设施的 VGT3 角落。调查证实，大量匿名书籍订单正被送往一个以破坏性方式扫描书籍以获取 AI 训练数据的亚马逊设施。 这项调查提供了具体的实物证据，证明 AI 公司如何从纸质书籍中获取训练数据，引发了重大的版权和伦理问题。它揭露了 AI 数据获取背后不透明的供应链，影响了作者、出版商、书商以及更广泛的 AI/ML 社区。 被追踪的书籍被送至位于拉斯维加斯东北部的亚马逊 LAS8 设施的 VGT3 区域，该入口处展示着一个恐龙抓书的标志。亚马逊员工之间的在线论坛讨论证实，VGT3 以破坏性方式扫描大量书籍。

rss · Simon Willison · 8月17日 15:21

**背景**: 据报道，AI 公司一直批量购买二手书籍，以获取高质量文本来训练大型语言模型，通常随后将书籍粉碎以保密。报道称，这些购买通常通过中间人进行，以避免公众反弹。Biblio.com 是一个主要的二手和稀有书籍在线市场，提供近 1 亿种图书，因此成为此类批量订单的常见来源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/ai-companies-are-reportedly-shredding-millions-of-books-to-train-models-tech-giants-outsource-to-middlemen-to-secretly-buy-up-books-for-training-material">AI companies are reportedly shredding millions of books after using them to train AI models — tech giants outsource to middlemen to secretly buy up books for training material | Tom's Hardware</a></li>
<li><a href="https://futurism.com/artificial-intelligence/ai-companies-destroying-rare-books">AI Companies Are Buying Antique Books, Ingesting Their Contents to Train Models, and Then Destroying Them at Incredible Scale, Even If Almost No Copies Remain</a></li>
<li><a href="https://www.theatlantic.com/technology/2026/08/ai-companies-buying-used-books-for-data/688167/">Someone Is Mysteriously Snapping Up Used Books Around the World - The Atlantic</a></li>

</ul>
</details>

**社区讨论**: 亚马逊员工之间的在线论坛讨论证实了 404 Media 的调查结果，确认 VGT3 设施大规模进行破坏性书籍扫描。在总结的内容中未提供具体的反对意见或其他观点。

**标签**: `#AI training data`, `#copyright`, `#investigation`, `#Amazon`, `#books`

---

<a id="item-7"></a>
## [Qwen 3.8 27B：本地运行出色，但默认过度思考](https://simonwillison.net/2026/Aug/16/qwen-38-27b/) ⭐️ 8.0/10

阿里巴巴 Qwen 实验室发布了 Qwen 3.8 27B，这是一款采用 Apache 2 许可、拥有 270 亿参数的视觉能力大语言模型。Simon Willison 的测试显示，其基准成绩明显超过 Qwen 3.6 27B 以及闭源模型 Qwen 3.7-Plus，但默认的 xhigh 推理强度会导致严重过度思考——例如为一个简单的 SVG 提示生成了 21 分钟、22,276 个推理 token 的思维链。 27B 这一规模非常适合在消费级笔记本上运行强大模型，且宽松的 Apache 2 许可使其可自由用于商业项目。此次发布表明，开源权重模型继续挑战闭源竞争对手，但也凸显了默认推理强度设置会显著影响实际使用体验。 该模型默认使用 xhigh 推理强度，LM Studio 的 17GB Q4_K_M 量化版本保留了这一默认值；在 LM Studio 默认的 8,192 token 上下文限制下，模型光是思考简单任务就会耗尽 token。Simon Willison 在 128GB M5 Max MacBook Pro 和 NVIDIA DGX Spark 上运行了该模型，生成的最佳“骑自行车鹈鹕”SVG 花了 21 分钟，用了 22,276 个推理 token 和 3,223 个输出 token。

rss · Simon Willison · 8月16日 22:00

**背景**: Apache 2.0 是一种宽松的开源许可证，允许自由使用、修改和分发，包括用于商业目的。“27B”指神经网络中约 270 亿个参数，这些参数大致决定了模型的能力和资源需求；27B 模型小到可以运行在高配笔记本电脑上。Qwen 模型包含一个“reasoning_effort”（推理强度）设置，控制模型在回答前思考多长时间；量化（如 Q4_K_M）则通过压缩权重降低文件体积，同时尽量减小质量损失。在 AI 行业中，像 GPT-4 这样的“闭源权重”模型不公开内部权重，而“开源权重”模型会公开权重，便于本地部署和定制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apache_License">Apache License</a></li>
<li><a href="https://llm-explorer.com/model/Qwen/Qwen3.8-27B,3HAoLr0dKuoKi0dZxTZefY">Qwen3.8 27 B by Qwen — VRAM 55.6GB | LLM Explorer</a></li>
<li><a href="https://www.emergentmind.com/topics/closed-weight-systems">Closed - Weight Systems in Agentic LLMs</a></li>

</ul>
</details>

**标签**: `#LLM`, `#Qwen`, `#open-source`, `#AI`, `#model release`

---

<a id="item-8"></a>
## [Dario Amodei：AI 遭公众不信任折射更广泛的信任危机](https://simonwillison.net/2026/Aug/16/dario-amodei/) ⭐️ 8.0/10

Anthropic 首席执行官 Dario Amodei 在最近的一条推文中表示，公众对 AI 的不信任主要不是源于 AI 领袖的风险警示，而是反映出对机构更深层的信任危机。他认为 Anthropic 应专注于真正兑现承诺的益处，例如治愈癌症，而不是靠营销宣传。 Amodei 的论述反驳了“AI 领袖的末日预言加剧公众恐惧”这一常见叙事，并将讨论焦点拉回到实际的成果交付上。作为行业顶尖人物，他的表态可能影响 AI 公司对待问责与公众沟通的方式。 Amodei 明确拒绝了采用正面包装的华丽营销活动的想法，并称“AI 将治愈癌症”这类说法是陈词滥调，缺乏说服力。他承认包括 Anthropic 在内的 AI 公司最准确的批评是尚未兑现造福世界的重大承诺。

rss · Simon Willison · 8月16日 15:05

**背景**: 近年来，随着生成式 AI 工具的快速部署，公众对 AI 的信任度有所下降，同时 AI 公司领袖也接二连三发出关于存在性风险的严厉警告。Amodei 的言论出现在一场持续争论中：这些警告本身是否要对公众负面认知负责，行业又应如何应对。他的回应认为，根本原因是几十年来公众对企业、政府和科技行业信任的持续下降。

**标签**: `#AI`, `#trust`, `#Anthropic`, `#public perception`, `#Dario Amodei`

---

<a id="item-9"></a>
## [在 Kubernetes 上使用 CloudNativePG PostgreSQL 后端运行 OpenBao](https://postgr.es/p/9sq) ⭐️ 7.0/10

Gabriele Bartolini 与 Rob Kenefeck 发布了 CNPG Recipe 27，这是一份在 Kubernetes 上部署 OpenBao、并以 CloudNativePG 管理的 PostgreSQL 作为其后端存储的分步指南。该方案完全通过 CloudNativePG 1.30 中新增的 DatabaseRole CRD 使用 TLS 客户端证书进行身份验证，整个技术栈中不再有密码。 该方案展示了一个完全开源、无厂商锁定的秘密管理技术栈，基于 CNCF 项目构建，对云原生和安全从业者很有吸引力。它也突显了新的 DatabaseRole CRD 支持声明式、GitOps 友好的数据库角色来为机器身份认证的能力。 OpenBao 是 HashiCorp Vault 的社区驱动分支，由 Linux 基金会旗下的 OpenSSF 维护。该方案使用 TLS 客户端证书进行身份验证，整个技术栈中没有密码，且由来自 ControlPlane 的 Rob Kenefeck 共同撰写。

rss · Planet PostgreSQL · 8月17日 08:48

**背景**: OpenBao 是一个开源秘密管理器，用于存储和分发 API 密钥、密码、证书等敏感数据。CloudNativePG 是一个 Kubernetes 算子，负责管理 PostgreSQL 集群的完整生命周期，其 1.30 版本引入了 DatabaseRole CRD 以声明式管理数据库角色。Kubernetes 是 CNCF 项目，因此这是一个全开源的技术栈。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openbao.org/">OpenBao</a></li>
<li><a href="https://cloudnative-pg.io/docs/1.30/">CloudNativePG</a></li>
<li><a href="https://byteiota.com/cloudnativepg-1-30-databaserole-crd-kubernetes-postgres/">CloudNativePG 1.30: DatabaseRole CRD and Two CVE... | byteiota</a></li>

</ul>
</details>

**标签**: `#Kubernetes`, `#OpenBao`, `#CloudNativePG`, `#PostgreSQL`, `#Secrets Management`

---

<a id="item-10"></a>
## [PostgreSQL 为何跳过索引？调整 random_page_cost 至 1.1 可提速](https://postgr.es/p/9sw) ⭐️ 7.0/10

Alexander Ioffe 解释称，PostgreSQL 默认的 random_page_cost=4.0 仍针对旋转硬盘时代设计，可能导致优化器跳过有用的索引。将该值调低至 1.1 后，示例查询的执行时间从 125.98 毫秒降至 68.69 毫秒。 这很重要，因为大多数 PostgreSQL 实例仍沿用 25 年前的成本默认值，与现代 SSD 硬件不匹配，导致索引使用次优、查询变慢。仅更改一个参数即可在不修改代码的情况下，为索引密集型负载带来显著的性能提升。 random_page_cost 参数默认值为 4.0，反映的是 HDD 的高寻道延迟，而 SSD 的随机读成本要低得多。将其设为 1.1 能更接近 SSD 的行为，但最佳取值仍取决于具体的存储硬件和工作负载特征。

rss · Planet PostgreSQL · 8月17日 00:00

**背景**: PostgreSQL 的查询优化器使用 random_page_cost 等成本参数来估算不同执行策略的代价，并选择代价最低的方案。默认假设为旋转硬盘，使随机访问看起来远贵于顺序访问，从而可能抑制索引扫描。许多用户不知道这一默认值已 25 年未变，而硬件早已过渡到 SSD。将 random_page_cost 调整至与实际硬件匹配，可以显著改变优化器的选择并提升查询性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/postgresqls-randompagecost-isnt-just-disk-latency-default-pachot-fphre">PostgreSQL ’s " random _ page _ cost " isn’t just about disk latency...</a></li>
<li><a href="https://pgpedia.info/r/random_page_cost.html">random _ page _ cost - pgPedia - a PostgreSQL Encyclopedia</a></li>
<li><a href="https://hotpath.rs/blog/postgresql-performance-issues">Easy to Overlook PostgreSQL Query Performance Issues</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#query performance`, `#index tuning`, `#cost model`, `#database optimization`

---

<a id="item-11"></a>
## [Postgres 19 图查询：固定深度等同连接，变深度仍需递归 CTE](https://postgr.es/p/9sv) ⭐️ 7.0/10

Alexander Ioffe 在 PostgreSQL 19beta1 上对新的 SQL/PGQ 图查询进行了基准测试，发现固定深度图查询的执行计划与手写连接完全相同，而变深度遍历仍会编译为递归 CTE。Apache AGE 则在 Cypher 包装器下执行同样的索引遍历。 这很重要，因为 SQL/PGQ 是新的 ISO SQL:2023 标准特性，让关系数据库无需单独的图引擎即可处理图工作负载。该结果表明，Postgres 的查询优化器会将简单图查询当作普通连接处理，但复杂路径遍历仍需要递归 CTE 或 Apache AGE 等专门工具。 基准测试使用 ExoBench 的本地模式，针对 PostgreSQL 19beta1 运行。固定深度查询生成与手写连接完全相同的计划，因此没有性能损失，而变深度遍历仍依赖递归 CTE；Apache AGE 则用 Cypher 包装相同的索引遍历。

rss · Planet PostgreSQL · 8月17日 00:00

**背景**: SQL/PGQ（SQL Property Graph Queries，SQL 属性图查询）是 ISO/IEC SQL:2023 标准的一部分，允许直接在 SQL 中将现有关系数据作为属性图进行查询，而无需 Neo4j 等独立图数据库。PostgreSQL 19 正在加入对该标准的支持，让用户可以借助普通 SQL 语法运行图式查询。图中的固定深度查询本质上就是模式匹配连接，而变深度遍历需要反复沿着边行走，因此通常会使用递归 CTE 或 Cypher 等图查询语言。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.enterprisedb.com/blog/representing-graphs-postgresql-sqlpgq">Representing graphs in PostgreSQL with SQL / PGQ | EDB</a></li>
<li><a href="https://blogs.oracle.com/database/property-graphs-in-oracle-database-23ai-the-sql-pgq-standard">Property Graphs in Oracle Database 23ai: The SQL / PGQ Standard</a></li>
<li><a href="https://age.apache.org/">Apache AGE</a></li>

</ul>
</details>

**标签**: `#postgres`, `#graph-queries`, `#performance`, `#sql-pgq`, `#benchmarks`

---

<a id="item-12"></a>
## [PostgreSQL 17：传统列优于 JSONB+GIN，唯多键包含查询例外](https://postgr.es/p/9su) ⭐️ 7.0/10

Alexander Ioffe 在 PostgreSQL 17 上的性能分析表明，传统关系型列在所有测试场景中均优于 JSONB 搭配 GIN 索引的组合，唯一的例外是多键包含查询。这一发现挑战了“JSONB+GIN 是灵活模式工作负载最佳默认选择”的常见假设。 这项分析为数据库模式设计提供了具体指导：开发人员在许多情况下可以通过使用原生关系型列获得比 JSONB 更好的性能。然而，多键包含查询的例外说明 JSONB 的 GIN 索引在动态查询 JSON 文档的场景中仍然具有独特价值。 该基准测试运行在 PostgreSQL 17 上，比较了传统列、带 GIN 索引的 JSONB 以及 JSONB 路径查询。在大多数场景下列胜出，但多键包含查询（即同时匹配多个键的值的查询）使用 JSONB+GIN 更快，因为 GIN 索引可以仅用一个索引处理这类查询。

rss · Planet PostgreSQL · 8月17日 00:00

**背景**: PostgreSQL 的 JSONB 数据类型以二进制格式存储 JSON 文档，而 GIN（通用倒排索引）索引可以使用 @> 等操作符加速包含查询。JSON 路径表达式于 PostgreSQL 12 引入，提供了一种用于从 JSONB 提取数据的 SQL/JSON 查询语言。在关系型列和 JSONB 之间选择是一个常见的模式设计决策，尤其是对于属性变化或动态的工作负载。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hasurahq.medium.com/postgres-containment-operators-part-2-performance-comparison-with-mongodb-ef4deb02f61e">Postgres Containment Operators : Part 2 — Performance... | Medium</a></li>
<li><a href="https://www.postgresql.org/docs/current/functions-json.html">PostgreSQL : Documentation: 18: 9.16. JSON Functions and Operators</a></li>
<li><a href="https://www.postgresql.org/docs/current/indexes-types.html">PostgreSQL : Documentation: 18: 11.2. Index Types</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#JSONB`, `#GIN`, `#performance`, `#schema design`

---

<a id="item-13"></a>
## [覆盖索引：PostgreSQL 17 写入开销增加 28%，读取加快 1.26 倍](https://postgr.es/p/9st) ⭐️ 7.0/10

Alexander Ioffe 发布了在 PostgreSQL 17 上对覆盖索引的基准测试结果，在 200 万行数据下，写入开销具体表现为 INSERT 增加 28%、UPDATE 增加 25%。读取速度提升 1.26 倍，当每次分析型读取对应的写入次数低于约 4300 次时，覆盖索引占优。 这为数据库工程师提供了一个具体、可测量的数字，而这一取舍以往往往只被模糊地讨论，有助于判断何时覆盖索引值得其写入开销。该临界点为 PostgreSQL 工作负载调优和索引设计提供了可操作的指导。 基准测试在 PostgreSQL 17 上使用 200 万行数据运行，临界点出现在每次分析型读取对应约 4300 次写入时。结果依赖于具体工作负载，实际百分比可能随表大小、数据类型和查询模式而变化。

rss · Planet PostgreSQL · 8月17日 00:00

**背景**: 覆盖索引包含查询所需的所有列，使数据库可以直接从索引返回结果，而无需额外回表查询，这称为索引-only 扫描（index-only scan）。然而，每次 INSERT、UPDATE 或 DELETE 也必须维护索引结构，且更宽的索引会增加存储和内存压力，导致写放大。这篇文章为 PostgreSQL 17 上这一固有取舍提供了具体数值。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dev.to/arnavsharma2711/your-index-only-scan-is-lying-covering-indexes-and-the-visibility-map-43nd">Your Index Only Scan Is Lying: Covering Indexes ... - DEV Community</a></li>
<li><a href="https://www.geeksforgeeks.org/dbms/indexing-in-databases-set-1/">Indexing in Databases - GeeksforGeeks</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#Indexing`, `#Database Performance`, `#Benchmark`

---

<a id="item-14"></a>
## [Flyway validate 检查的是文件完整性，而非数据库结构](https://postgr.es/p/9sr) ⭐️ 7.0/10

一篇技术博客文章澄清了 Flyway 的 validate 命令的作用：它重新计算本地迁移文件的校验和，并与 flyway_schema_history 表中记录的值进行比较，而不是检查实际数据库结构。文章明确否定了“validate 通过就代表数据库与迁移一致”这一常见误解。 团队常常依赖 validate 作为结构漂移检测手段，但这种虚假的安全感可能让未经授权的数据库结构更改被忽略。理解 validate 的真实范围有助于团队采用正确的漂移检测工具，例如付费版中的 Flyway check -drift，或其他结构比对工具。 validate 只读取 schema history 表，从不检查表、列、索引或约束；因此手工执行的 ALTER TABLE 语句会静默通过验证。文章还指出 flyway repair 只是更新历史记录，不会修复数据库结构，而 Flyway 的漂移检测功能（check -drift）位于免费核心工作流之外。

rss · Planet PostgreSQL · 8月17日 00:00

**背景**: Flyway 是一款流行的开源数据库迁移工具，它将带版本号的 SQL 迁移文件应用到数据库。当迁移执行时，Flyway 会计算文件校验和，并将其连同版本和执行元数据一起存储在 flyway_schema_history 表中。validate 命令将本地文件校验和与该历史记录进行比较，以检测已执行迁移是否被修改，但不会将历史记录与实际的数据库结构进行比对。对于在 CI/CD 流水线中依赖迁移验证来保证结构一致性的团队来说，理解这一区别非常重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://documentation.red-gate.com/flyway/reference/commands/validate">Validate - Redgate Flyway - Product Documentation</a></li>
<li><a href="https://documentation.red-gate.com/flyway/flyway-concepts/migrations/flyway-schema-history-table">Flyway schema history table - Redgate Flyway - Product...</a></li>
<li><a href="https://stackoverflow.com/questions/78454582/does-flyway-validate-table-schema-against-entity-in-spring-boot">Does flyway validate table schema against entity in... - Stack Overflow</a></li>

</ul>
</details>

**标签**: `#flyway`, `#postgresql`, `#database-migrations`, `#validation`, `#devops`

---