---
layout: default
title: "Horizon 日报：2026-07-17 (ZH)"
date: 2026-07-17
lang: zh
---

> 从 45 条内容中筛选出 18 条重要资讯。

---

1. [Firefox 通过 WebAssembly 在另一个浏览器中运行](#item-1) ⭐️ 10.0/10
2. [Kimi K3：开放前沿级 AI 模型](#item-2) ⭐️ 9.0/10
3. [LM Studio Bionic：面向开源模型的 AI 智能体](#item-3) ⭐️ 8.0/10
4. [从 Rust 到 Zig 重写编译器的进展报告](#item-4) ⭐️ 8.0/10
5. [pgEdge Spock 6 测试版：自定义 WAL 资源管理器与共享内存跟踪](#item-5) ⭐️ 8.0/10
6. [Postgres 19 默认压缩切换为 LZ4](#item-6) ⭐️ 8.0/10
7. [基于证据的 LLM 方法用于遗留 Java 现代化](#item-7) ⭐️ 8.0/10
8. [Inkling：Thinking Machines Lab 发布 975B 开放权重多模态 MoE 模型](#item-8) ⭐️ 8.0/10
9. [Linus Torvalds 捍卫 Linux 开发中使用 AI](#item-9) ⭐️ 8.0/10
10. [Claude web_fetch 漏洞导致数据泄露](#item-10) ⭐️ 8.0/10
11. [微软 Comic Chat 以开源形式发布](#item-11) ⭐️ 7.0/10
12. [诱饵字体：欺骗 AI 的字型](#item-12) ⭐️ 7.0/10
13. [DataGrip 2026.2：AI 智能体技能、MCP 工具及 CLI 命令](#item-13) ⭐️ 7.0/10
14. [exit_on_error 配置：快速失败的破坏性真相](#item-14) ⭐️ 7.0/10
15. [pg_hardstorage: 新的开源 PostgreSQL 备份工具](#item-15) ⭐️ 7.0/10
16. [小心监听：NOTIFY 如何让你的数据库翻车](#item-16) ⭐️ 7.0/10
17. [GPT-5.6 Codex 漏洞可删除 $HOME 目录](#item-17) ⭐️ 7.0/10
18. [通过 WASM 将 Mermaid 图表渲染为 Unicode 盒式艺术](#item-18) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Firefox 通过 WebAssembly 在另一个浏览器中运行](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 10.0/10

Puter 已将完整的 Firefox 浏览器编译为 WebAssembly，使其能够在另一个浏览器（如 Chrome）中完全运行。该演示加载了一个 233MB 的 gecko.wasm 文件，并通过基于 WebSocket 的 Wisp 协议代理网络流量。 这展示了在浏览器中运行完整复杂原生应用的前所未有的能力，突破了 WebAssembly 和 Web 平台的边界。它可能为遗留软件兼容性、沙盒执行和远程桌面替代方案带来新的可能性。 团队使用了价值约 25,000 美元的 Claude Opus 和 Fable 令牌（通过订阅计划降低了实际成本）来辅助编译。选择 Firefox/Gecko 是因为其强大的单进程支持，所有网络流量均通过使用 Wisp 协议的 Puter 服务器代理，该协议支持端到端加密。

rss · Simon Willison · 7月16日 23:34

**背景**: WebAssembly（WASM）是一种低级二进制指令格式，能在现代浏览器中以接近原生的速度运行，传统上用于游戏或图像处理等计算密集型任务。编译像 Firefox 这样的完整浏览器因其体积和系统依赖性而复杂得多。Wisp 协议是一种低开销标准，用于通过单个 WebSocket 连接代理多个 TCP 和 UDP 套接字，从而为在沙盒浏览器环境中运行的代码提供网络访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/ wisp - protocol : Wisp is a low-overhead...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Wire_protocol">Wire protocol</a></li>

</ul>
</details>

**社区讨论**: 在 Hacker News 上，该项目引发了极大的兴奋，用户对这项技术成就感到惊叹。团队提到他们不得不扩展服务器以应对讨论带来的流量激增。一些人质疑其实用性，而另一些人则称赞其创造性地使用 AI 辅助编程（Claude）来完成移植。

**标签**: `#WebAssembly`, `#Firefox`, `#browser engineering`, `#innovation`, `#web platform`

---

<a id="item-2"></a>
## [Kimi K3：开放前沿级 AI 模型](https://www.kimi.com/blog/kimi-k3) ⭐️ 9.0/10

Moonshot AI 发布了 Kimi K3，这是一个开放权重的模型，具有 2.8 万亿参数、前沿级性能、1M token 上下文窗口，以及每百万 token 3/15 美元的竞争性定价。 Kimi K3 以开放权重和激进定价挑战美国前沿模型，可能加速 AI 智能的 commoditization，并加剧中美 AI 实验室之间的竞争。 该模型在基准测试上超越 Opus 4.8，使用 1M 上下文，定价与 Anthropic 的 Sonnet 系列一致，并提供缓存折扣。其开放权重特性允许社区检查和微调。

hackernews · vincent_s · 7月16日 14:46 · [社区讨论](https://news.ycombinator.com/item?id=48935342)

**背景**: 开放权重 AI 模型是指其训练参数公开发布，使开发者能够运行、研究和修改的模型。大上下文窗口（1M tokens）允许模型处理海量输入，如整本书或长代码库。前沿模型通常指来自顶尖实验室（如 OpenAI、Google、Anthropic）的最强模型。

**社区讨论**: 社区评论指出推理 token 的高成本、中国实验室 commoditization 的战略意义，以及与其他前沿模型的比较。有人质疑如此大规模投资的回报，而其他人则赞赏其性能与定价的平衡。

**标签**: `#AI`, `#Large Language Models`, `#Open-Source`, `#Pricing`, `#Chinese AI`

---

<a id="item-3"></a>
## [LM Studio Bionic：面向开源模型的 AI 智能体](https://lmstudio.ai/blog/introducing-lm-studio-bionic) ⭐️ 8.0/10

LM Studio 发布了 Bionic，这是一个 AI 智能体框架，能让本地运行的开源模型自主行动，并且提供了类似 Codex 等工具的熟悉界面。 此次发布将智能体能力引入了本地 LLM 生态，使得企业和个人无需依赖云 API 即可使用强大的开源模型完成复杂任务。 Bionic 支持'Code'和'Work'两种项目类型，并在 Work 项目中提供自动检查点保存；它可以指向现有的 LM Studio 模型库，运行如 Qwen3.6 35B 等模型。

hackernews · minimaxir · 7月16日 20:18 · [社区讨论](https://news.ycombinator.com/item?id=48939662)

**背景**: LM Studio 是一款对初学者友好的桌面应用，用于发现、下载和运行本地大语言模型（LLM），无需命令行技能。像 Bionic 这样的 AI 智能体框架为 LLM 提供了执行多步骤任务、与工具交互以及自主运作的能力，超越了简单的聊天功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/LM_Studio">LM Studio</a></li>
<li><a href="https://lmstudio.ai/download">Download LM Studio - Mac, Linux, Windows</a></li>

</ul>
</details>

**社区讨论**: 早期用户反馈 Bionic 运行良好，对 Codex 用户很熟悉，但仍有粗糙之处。有人担心 LM Studio 的业务模式可能向企业云服务转变，但创始人积极互动，提供了免费试用点数。

**标签**: `#LM Studio`, `#AI agent`, `#open models`, `#local LLM`, `#agentic framework`

---

<a id="item-4"></a>
## [从 Rust 到 Zig 重写编译器的进展报告](https://rtfeldman.com/rust-to-zig) ⭐️ 8.0/10

一篇由 Richard Feldman 撰写的详细博客文章报告了将 Roc 编译器从 Rust 重写到 Zig 的进展，讨论了内存安全性权衡以及 Zig 增量构建的优势。 这篇文章为系统编程中的 Rust 与 Zig 对比提供了现实而细致的比较，特别是在编译器开发中，构建速度和内存控制至关重要。它指出 Zig 的增量构建是一个引人注目的特性，可能影响新编译器项目的语言选择。 这次重写从 Rust 转向 Zig 的部分原因是 Zig 的增量编译速度更快，这是开发迭代的一个“杀手级功能”。然而，这篇文章承认 Rust 的安全性保证对大多数编译器任务都很强，而 Zig 的运行时安全性检查（如检测释放后使用）受到了社区的质疑。

hackernews · jorangreef · 7月16日 11:39 · [社区讨论](https://news.ycombinator.com/item?id=48933149)

**背景**: Rust 和 Zig 是现代系统编程语言。Rust 以其无垃圾收集器的内存安全性而闻名，而 Zig 则定位为更好的 C 语言，具有手动内存管理和编译时特性。编译器通常需要针对机器代码生成等任务执行不安全的操作，这使得安全性与控制之间的权衡成为关键考虑因素。这篇博客文章在一个真实的编译器重写中探讨了这一权衡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://ziglang.org/">Home ⚡ Zig Programming Language</a></li>

</ul>
</details>

**社区讨论**: 社区成员如 steveklabnik 认为，不安全代码对于大多数编译器任务并非必要，仅用于热补丁。landr0id 质疑 Zig 声称能捕获释放后使用错误的能力。arthurbrown 好奇既然 OCaml 如此灵活，为何未被选为实现语言。onlyrealcuzzo 称赞 Zig 的增量构建，但对安全性表示担忧，希望有一种语言能结合 Rust 的安全性、Zig 的特性和 Go 的无 GC 运行时。

**标签**: `#Rust`, `#Zig`, `#compiler`, `#memory safety`, `#systems programming`

---

<a id="item-5"></a>
## [pgEdge Spock 6 测试版：自定义 WAL 资源管理器与共享内存跟踪](https://postgr.es/p/9pV) ⭐️ 8.0/10

该版本显著提升了 PostgreSQL 多主复制的性能、可扩展性和可靠性，减少了 I/O 争用并消除了目录膨胀。对于需要高可用性和多区域部署的 Active-Active 数据库集群用户来说，该版本非常重要。 自定义 WAL 资源管理器在关闭时将进度快照写入 WAL，允许使用 pg_waldump 等标准工具进行检查。共享内存进度跟踪消除了热路径上的目录写入，磁盘溢出支持多 GB 的异常事务而无需内存压力。

rss · Planet PostgreSQL · 7月16日 20:16

**背景**: Spock 6 是 PostgreSQL 的多主复制扩展，允许多个数据库节点接受写入并同步更改。以前的版本在目录表中跟踪复制进度，在高负载下会导致争用和膨胀。自定义 WAL 资源管理器使扩展能够直接集成 PostgreSQL 的预写日志，共享内存跟踪通过避免每次事务的磁盘写入来提高性能。此版本还通过改进的恢复机制解决了节点故障后的静默漂移问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/custom-rmgr.html">PostgreSQL: Documentation: 18: 64.2. Custom WAL Resource Managers</a></li>
<li><a href="https://wiki.postgresql.org/wiki/CustomWALResourceManagers">CustomWALResourceManagers - PostgreSQL wiki</a></li>
<li><a href="https://www.postgresql.org/docs/current/replication-origins.html">PostgreSQL: Documentation: 18: Chapter 48. Replication Progress Tracking</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#replication`, `#Spock`, `#database`, `#multi-master`

---

<a id="item-6"></a>
## [Postgres 19 默认压缩切换为 LZ4](https://postgr.es/p/9pU) ⭐️ 8.0/10

PostgreSQL 19 计划将默认的 TOAST 压缩算法从 pglz 改为 LZ4，从而提升压缩速度和存储效率。 这一变化将惠及所有 PostgreSQL 用户，降低 CPU 开销并可能提高吞吐量，尤其对写入密集型工作负载和大文本或二进制数据。 LZ4 在 PostgreSQL 14 中作为可选压缩方法引入；Postgres 19 将使其成为默认，而 pglz 仍然可用。每列或通过 default_toast_compression 参数可覆盖默认设置。

rss · Planet PostgreSQL · 7月16日 12:00

**背景**: PostgreSQL 使用 TOAST（超大属性存储技术）机制处理大字段值。对于 TEXT 和 BYTEA 等可变长度类型，自动应用压缩。pglz 算法在 Postgres 7.1 中引入，优先考虑速度而非压缩比，但效率低于 LZ4。LZ4 提供更快的压缩和解压速度，且压缩比相当，使其成为现代工作负载的更好默认选择。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/storage-toast.html">PostgreSQL: Documentation: 18: 66.2. TOAST</a></li>
<li><a href="https://www.tigerdata.com/blog/optimizing-postgresql-performance-compression-pglz-vs-lz4">PostgreSQL Compression: pglz vs. LZ4 | Tiger Data</a></li>
<li><a href="https://postgresqlco.nf/doc/en/param/default_toast_compression/">PostgreSQL Documentation: default_toast_compression parameter</a></li>

</ul>
</details>

**标签**: `#postgresql`, `#compression`, `#LZ4`, `#TOAST`, `#database performance`

---

<a id="item-7"></a>
## [基于证据的 LLM 方法用于遗留 Java 现代化](https://martinfowler.com/articles/archaeologist-copilot.html) ⭐️ 8.0/10

Nik Malykhin 在 Martin Fowler 的网站上发表了一篇文章，详细描述了一种使用 LLM（大型语言模型）现代化遗留 Java 1.5 代码库的方法，该方法以证据为约束，结合基于 Docker 的验证和测试保护的重构。 这种实用方法解决了行业常见挑战——现代化古老代码库——展示了当 AI 基于经验证据和严格测试时如何被可靠地使用。 该过程涉及使用 LLM 进行分析和建议，同时在稳定的 Docker 环境中验证更改，并通过自动化测试保护逐步重构；关键见解是，当 LLM 的输出受实际代码库可验证证据约束时，它们最为有用。

rss · Martin Fowler · 7月16日 13:25

**背景**: 遗留代码现代化是指更新旧软件系统以在现代硬件和平台上运行。LLM（大型语言模型）是可以生成代码的 AI 模型，但其输出对于与典型训练数据不一致的遗留代码库可能不可靠。所提出的方法使用 Docker 提供可重现环境，并使用自动化测试确保更改不会破坏现有功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://martinfowler.com/articles/archaeologist-copilot.html">The Archaeologist ’s Copilot</a></li>
<li><a href="https://arxiv.org/pdf/2411.14971">Leveraging LLMs for Legacy Code Modernization:</a></li>

</ul>
</details>

**标签**: `#legacy modernization`, `#LLM`, `#AI-assisted refactoring`, `#software engineering`, `#Java`

---

<a id="item-8"></a>
## [Inkling：Thinking Machines Lab 发布 975B 开放权重多模态 MoE 模型](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 8.0/10

Mira Murati 领导的 Thinking Machines Lab 发布了 Inkling，这是一个开放权重的 975B 参数（41B 活跃）多模态专家混合模型，采用 Apache-2.0 许可，在 45 万亿 token 的文本、图像、音频和视频数据上训练。他们还宣布了 Inkling-Small（总参数 276B，活跃 12B），但尚未发布其权重。 此次发布增强了美国开放权重 AI 生态系统，提供了中国开放模型的竞争性替代品，尽管它不是前沿模型。Apache-2.0 许可和通过 Tinker 平台进行微调的定位使其成为有价值的定制基础。 Inkling 被明确定位为用于微调的强大基础模型，而非顶尖前沿模型。其模型卡和训练数据文档非常简略，提供的技术细节有限。

rss · Simon Willison · 7月16日 15:35

**背景**: 专家混合（MoE）是一种神经网络架构，包含多个专家子网络和一个门控机制，每次输入仅激活部分专家，从而提高效率和容量。开放权重模型公开训练好的模型参数，但可能不包含完整训练代码或数据，这与完全开源的 AI 系统有所区别。Inkling 是一个多模态模型，能够处理文本、图像、音频和视频。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/mixture-of-experts-transformer-architecture">Mixture - of - Experts Transformer Architecture</a></li>
<li><a href="https://kilo.ai/open-source-vs-open-weight-models">Kilo - Open Source vs Open Weight AI Models Explained</a></li>

</ul>
</details>

**标签**: `#open-weights`, `#multimodal`, `#Mixture-of-Experts`, `#AI model`, `#Thinking Machines Lab`

---

<a id="item-9"></a>
## [Linus Torvalds 捍卫 Linux 开发中使用 AI](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 8.0/10

Linux 创始人兼最高维护者 Linus Torvalds 公开表示，Linux 不是一个反 AI 的项目，并且 AI 是一种明显有用的工具，他告诉不同意的人可以去创建分支或者离开。 来自最高维护者的强烈认可表明了 Linux 内核在 AI 集成方面的明确立场，可能解决长期的争议，并鼓励在开源开发中更广泛地采用 AI 工具。 Torvalds 在 Linux 媒体邮件列表中发表声明，强调虽然关于 AI 的经济性仍有问题，但其实用性已毋庸置疑。他指出，任何怀疑的人显然没有使用过它。

rss · Simon Willison · 7月16日 13:26

**背景**: Linux 是一个广泛使用的开源操作系统内核，Torvalds 是其终身仁慈独裁者（BDFL）。Linux 内核社区一直在讨论在开发工作流中使用 AI 工具（如大型语言模型）的问题。Torvalds 的声明直接回应了这一争议。

**标签**: `#Linux`, `#AI`, `#Linus Torvalds`, `#open source`

---

<a id="item-10"></a>
## [Claude web_fetch 漏洞导致数据泄露](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 8.0/10

安全研究员 Ayush Paul 发现了一个 Anthropic Claude 的 web_fetch 工具绕过漏洞，攻击者可通过恶意网站上的链接链诱使 AI 泄露用户记忆数据。 该漏洞破坏了 Anthropic 为 Claude 设计的数据泄露防护核心，凸显了 AI 代理中“致命三重奏”持续存在的风险。它影响所有依赖记忆功能和网页访问的 Claude 用户，可能导致敏感个人信息泄露。 攻击之所以成功，是因为 web_fetch 可以跟随获取页面中的嵌入链接，而不仅仅是用户提供的 URL。研究者的蜜罐网站展示了一个虚假的 Cloudflare 认证提示，指示模型按字母顺序访问 URL 以逐字母提取用户数据，成功获取了姓名、城市和雇主信息。

rss · Simon Willison · 7月15日 14:21

**背景**: Claude 的 web_fetch 工具旨在帮助 AI 检索网页内容，但其设计只允许获取用户明确提供的 URL 或来自其配套 web_search 工具的 URL。“致命三重奏”是指 AI 代理同时具备访问私有数据、处理不可信内容和拥有外部通信能力时的危险组合，这使得提示注入攻击尤其有效。Anthropic 的限制旨在防止通过 URL 操纵进行数据泄露，但该漏洞允许通过获取的网页进行链式导航。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.claude.com/en/docs/agents-and-tools/tool-use/web-fetch-tool">Web fetch tool - Claude Docs</a></li>
<li><a href="https://www.osohq.com/learn/lethal-trifecta-ai-agent-security">Understanding the Lethal Trifecta of AI Agents</a></li>
<li><a href="https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/">The lethal trifecta for AI agents: private data, untrusted content, and external communication</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#security`, `#Claude`, `#data exfiltration`, `#prompt injection`

---

<a id="item-11"></a>
## [微软 Comic Chat 以开源形式发布](https://opensource.microsoft.com/blog/2026/07/16/microsoft-comic-chat-is-now-open-source/) ⭐️ 7.0/10

2026 年 7 月 16 日，微软将 Comic Chat（后更名为 Microsoft Chat）开源，这款图形化 IRC 客户端最早于 1996 年发布，其源代码现已托管在 GitHub 上。 此次发布保留了一段怀旧的互联网历史，使社区能够研究、修改并在现代系统上运行该软件，凸显了微软对开源日益增长的承诺。 Comic Chat 通过自定义消息扩展了 IRC 协议，用于表示角色外观和情感，这在 IRC 社区中被一些人批评为非标准。开源版本包含原始的微软研究院项目和一个 Windows 98 时代的版本。

hackernews · jervant · 7月16日 16:06 · [社区讨论](https://news.ycombinator.com/item?id=48936426)

**背景**: IRC（互联网中继聊天）是一种基于文本的聊天协议，在 1990 年代和 2000 年代初期流行。微软 Comic Chat 由 David Kurlander 开发，是一款图形化 IRC 客户端，将对话渲染为带有可定制头像的漫画条，随 Internet Explorer 3.0 和后来的 Windows 98 捆绑发布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Microsoft_Comic_Chat">Microsoft Comic Chat</a></li>
<li><a href="https://en.wikipedia.org/wiki/IRC">IRC - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论总体积极，对这次发布背后的故事和怀旧情怀表示赞赏。促成本次开源的 Robert Standefer 分享了他的兴奋之情。一些用户回忆说，Comic Chat 因以非标准方式扩展 IRC 协议而受到批评，而其他人则珍视其实验精神。

**标签**: `#open-source`, `#microsoft`, `#comic-chat`, `#irc`, `#nostalgia`

---

<a id="item-12"></a>
## [诱饵字体：欺骗 AI 的字型](https://www.mixfont.com/experiments/decoy-font) ⭐️ 7.0/10

Decoy Font 是一种 TrueType 字体，每个字母都包含一个诱饵字母，导致 AI 模型读取与人类感知不同的文本。对 GPT、Claude 和 Gemini 等 LLM 的实验表明，它们常常输出诱饵信息而非人类可读的文本。 这种字体揭示了 LLM 处理视觉文本时的漏洞，可能影响 AI 安全和数据隐私。它可用于向 AI 爬虫隐藏信息，或作为一种对抗性工具，凸显了多模态理解需要更鲁棒。 该字体基于 DejaVu Sans Mono，每个字形都设计有模糊形状来欺骗 AI。当字体图像被缩放或以不同尺寸观看时，模型可能会在读取目标文本和诱饵文本之间切换；例如，Gemma E4B 在图像缩小到 150×150 像素之前读取更清晰的文本。

hackernews · ray__ · 7月16日 16:18 · [社区讨论](https://news.ycombinator.com/item?id=48936584)

**背景**: 字体通常是将字符代码映射到字形形状。Decoy Font 利用了人类和 AI 在感知边缘锐度、对比度等低级视觉特征上的差异。人类通常可以通过眯眼或模糊来读取目标文本，而 AI 模型则关注更清晰的诱饵轮廓。这一概念类似于光学错觉和欺骗神经网络的对抗性样本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.mixfont.com/experiments/decoy-font">Decoy Font: A TTF font that hides what you type</a></li>
<li><a href="https://typedrawers.com/discussion/5640/i-made-an-anti-ai-typeface-where-every-letter-contains-a-decoy-letter">I made an anti-AI typeface where every letter contains a decoy letter — TypeDrawers</a></li>
<li><a href="https://www.creativebloq.com/design/fonts-typography/this-optical-illusion-font-was-created-to-baffle-ai-and-it-actually-works-for-now">This optical illusion font was created to baffle AI, and it actually works (for now) | Creative Bloq</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：有人认为这种字体很酷且有趣，可用于实验；也有人质疑其实用性或阻止 AI 的真实效果。用户进行的测试表明，GPT-5.6 在提示下能部分解码隐藏文本，而 Claude 则完全不能。还有建议使用替换密码字体进行实际混淆。

**标签**: `#font`, `#AI`, `#obfuscation`, `#LLM`, `#UX`

---

<a id="item-13"></a>
## [DataGrip 2026.2：AI 智能体技能、MCP 工具及 CLI 命令](https://blog.jetbrains.com/datagrip/2026/07/16/datagrip-2026-2-ai-agent-skills-mcp-tools-and-cli-commands-for-data-source-management-bundled-jdbc-drivers-and-improved-session-control/) ⭐️ 7.0/10

DataGrip 2026.2 引入了三项新的 AI 智能体技能（database-tools、database-connection-management、database-text-to-sql）、MCP 工具、用于数据源管理的 CLI 命令、捆绑的 JDBC 驱动程序以及改进的会话控制。 此更新通过将 AI 驱动的自动化和现代工具直接集成到 IDE 中，简化了数据库工作流程，显著提高了 DataGrip 用户的开发效率。 AI 智能体技能使智能体能够探索模式、管理连接并将自然语言转换为 SQL。MCP 工具允许与外部 AI 助手集成，而捆绑的 JDBC 驱动程序消除了常见数据库的手动设置。

rss · JetBrains DataGrip · 7月16日 14:51

**背景**: DataGrip 是 JetBrains 出品的数据库管理和 SQL 开发 IDE。AI 智能体技能是可重用的能力，让 AI 助手执行诸如查询数据库等特定任务。模型上下文协议（MCP）是一种开放标准，用于将 AI 模型连接到外部工具和数据源。JDBC（Java 数据库连接）驱动程序是 Java 应用程序连接数据库所必需的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.jetbrains.com/datagrip/">DataGrip | JetBrains for Data</a></li>
<li><a href="https://www.jetbrains.com/datagrip/features/ai/">AI Assistant in DataGrip</a></li>

</ul>
</details>

**标签**: `#DataGrip`, `#AI`, `#database`, `#JetBrains`, `#IDE`

---

<a id="item-14"></a>
## [exit_on_error 配置：快速失败的破坏性真相](https://postgr.es/p/9pW) ⭐️ 7.0/10

Christophe Pettus 发表了对 PostgreSQL 的 exit_on_error 配置的深度批评，指出其快速失败方法可能具有破坏性，因为它会在任何错误时终止整个会话。 理解这一细微差别对数据库从业者至关重要，因为错误配置 exit_on_error 可能导致意外的会话终止和数据完整性风险，凸显了谨慎错误处理的必要性。 当 exit_on_error 参数设置为 on 时，每个错误都会升级为会话终止事件，但这可能中止原本可以恢复的事务，掩盖了更微妙的潜在问题。

rss · Planet PostgreSQL · 7月17日 01:00

**背景**: PostgreSQL 使用名为 GUC（Grand Unified Configuration）的集中式配置系统来在不同层次控制其行为。exit_on_error 参数是一个布尔型 GUC，决定任何错误是否终止当前会话；默认情况下，它是关闭的，允许优雅地处理错误。理解 GUC 对于数据库调优和故障排除至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pgpedia.info/g/guc.html">GUC - Grand Unified Configuration - pgPedia - a PostgreSQL ...</a></li>
<li><a href="https://www-postgresql-org.nproxy.org/docs/current/runtime-config-error-handling.html">PostgreSQL : Documentation: 18: 19.14. Error Handling</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#error handling`, `#GUC`, `#database configuration`, `#fail-fast`

---

<a id="item-15"></a>
## [pg_hardstorage: 新的开源 PostgreSQL 备份工具](https://postgr.es/p/9pS) ⭐️ 7.0/10

CYBERTEC 在经过六个月的开发和超过一年的实际客户部署后，以 Apache 2.0 许可证开源了新的 PostgreSQL 备份工具 pg_hardstorage。 pg_hardstorage 为 PostgreSQL 备份生态系统提供了一个可信的替代方案，特别适用于云原生部署和 Patroni 集群，为运维人员提供了选择和迁移路径。 它使用 PostgreSQL 的复制协议进行备份，不需要 archive_command，具有内容寻址去重功能，并且感知 Patroni，能自动处理故障切换。

rss · Planet PostgreSQL · 7月16日 04:00

**背景**: PostgreSQL 备份工具如 pgBackRest、Barman 和 WAL-G 一直是数据库恢复的主要选择。pg_hardstorage 通过原生使用流复制来区分自己，使其与托管 PostgreSQL 服务兼容。内容寻址存储允许每个备份独立于之前的备份进行恢复。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.pghardstorage.org/">pg _ hardstorage — PostgreSQL backup , done right.</a></li>
<li><a href="https://www.cybertec-postgresql.com/en/products/pg-hardstorage/">pg _ hardstorage – Open-Source PostgreSQL Backup | CYBERTEC</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#backup`, `#open source`, `#pg_hardstorage`, `#database tools`

---

<a id="item-16"></a>
## [小心监听：NOTIFY 如何让你的数据库翻车](https://postgr.es/p/9pH) ⭐️ 7.0/10

Jimmy Angelakos 在 POSETTE 2026 和 PG DATA 2026 上发表演讲，揭示了 PostgreSQL 的 LISTEN/NOTIFY 如何导致严重的性能瓶颈和生产宕机。 这场演讲对任何依赖 LISTEN/NOTIFY 进行异步通信的 PostgreSQL 用户都至关重要，因为它揭示了一个隐藏的锁升级问题，可能使高吞吐量数据库瘫痪。 该演讲解释了 NOTIFY 的内部序列化如何触发 pg_database 上的 AccessExclusive 锁级联，并提出了使用未记录队列表、pg_try_advisory_xact_lock 和批处理等修复方案。

rss · Planet PostgreSQL · 7月15日 12:37

**背景**: PostgreSQL 的 LISTEN/NOTIFY 允许数据库会话之间进行异步通知，常用于轻量级事件驱动架构。但在高并发下，NOTIFY 可能获取重型锁，阻塞其他操作，导致级联争用。该演讲基于一个真实的生产事故，其中这种行为导致数据库逐渐停止响应。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@atarax/demystifying-postgresqls-listen-notify-12fe9c2a3907">Demystifying PostgreSQL ’s LISTEN / NOTIFY | by Abhinav... | Medium</a></li>
<li><a href="https://www.compilenrun.com/docs/database/postgresql/postgresql-advanced-features/postgresql-listen-notify/">PostgreSQL LISTEN / NOTIFY - Real-time... | Compile N Run</a></li>
<li><a href="https://www.cybertec-postgresql.com/en/listen-notify-automatic-client-notification-in-postgresql/">LISTEN / NOTIFY : Automatic client notification in PostgreSQL</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#LISTEN/NOTIFY`, `#database`, `#talk`

---

<a id="item-17"></a>
## [GPT-5.6 Codex 漏洞可删除 $HOME 目录](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 7.0/10

GPT-5.6 Codex 存在一个漏洞：当启用完整访问模式时，模型可能将 $HOME 误认为是临时目录并将其删除，从而导致用户文件被意外删除。 该漏洞凸显了编码代理中关键的 AI 安全风险，可能导致不可逆的数据丢失，并削弱用户对 AI 辅助开发工作流的信任。 该漏洞发生在启用完整访问模式且未开启沙箱保护或自动审查时，模型尝试覆盖 $HOME 以定义临时目录，却错误地删除了 $HOME 本身。

rss · Simon Willison · 7月16日 17:45

**背景**: 完整访问模式赋予 AI 编码代理无限制的文件系统访问权限，绕过了通常用于隔离代理操作的沙箱保护。没有沙箱保护，一个错误的命令就可能导致灾难性的数据丢失。自动审查功能要求代理在执行潜在危险操作前获得用户批准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://explainx.ai/blog/openai-codex-gpt-5-6-home-deletion-full-access-july-2026">Codex GPT - 5 . 6 $HOME Deletion — Full Access | explainx.ai</a></li>
<li><a href="https://github.com/openai/codex/issues/33575">gpt - 5 . 6 -sol loses all MCP tools after runtime metadata changes to...</a></li>

</ul>
</details>

**标签**: `#codex`, `#coding-agents`, `#generative-ai`, `#ai-safety`, `#bug`

---

<a id="item-18"></a>
## [通过 WASM 将 Mermaid 图表渲染为 Unicode 盒式艺术](https://simonwillison.net/2026/Jul/16/grok-mermaid/#atom-everything) ⭐️ 7.0/10

Simon Willison 制作了一个浏览器工具，通过将开源 Grok CLI 中的 Rust 终端渲染器编译为 WebAssembly，将 Mermaid 图表转换为 Unicode 盒式艺术。 这展示了将终端级图表渲染带入浏览器的实用方法，无需服务器端处理，可用于聊天、代码审查或静态站点。 该工具基于 Grok CLI 代码库中的自包含 Mermaid 终端渲染器，通过 Claude Code for web (Fable 5) 使用 WebAssembly 移植到网页。

rss · Simon Willison · 7月16日 00:33

**背景**: Mermaid 是一种流行的开源工具，可以从类似 Markdown 的语法生成图表、流程图等。Unicode 盒式绘图字符是文本界面中用于绘制简单形状和框架的标准字符。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mermaid.ai/open-source/">Mermaid | Diagramming and charting tool</a></li>
<li><a href="https://en.wikipedia.org/wiki/Box-drawing_characters">Box-drawing characters - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Mermaid`, `#Unicode`, `#WebAssembly`, `#Rust`, `#Terminal Rendering`

---