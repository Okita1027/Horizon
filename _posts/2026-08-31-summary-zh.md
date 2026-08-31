---
layout: default
title: "Horizon 日报：2026-08-31 (ZH)"
date: 2026-08-31
lang: zh
---

> 从 27 条内容中筛选出 8 条重要资讯。

---

1. [内核开发者讨论对付爬虫机器人的 Anubis 与 iocaine 方案](#item-1) ⭐️ 8.0/10
2. [QubesOS QSB-118：qvm-copy-to-vm 致 Dom0 任意代码执行](#item-2) ⭐️ 8.0/10
3. [Omarchy 漏洞：任意用户进程均可提权至 root](#item-3) ⭐️ 8.0/10
4. [欧盟委员会在 ProtectEU 战略中重新推动加密后门](#item-4) ⭐️ 8.0/10
5. [ChatGPT Work 解析：云端与本地桌面版](#item-5) ⭐️ 8.0/10
6. [1980 年 Spacelab 计算机磁芯内存模块剖析](#item-6) ⭐️ 7.0/10
7. [PostgreSQL 日志：善用 log_line_prefix 与 log_timezone 提升可观测性](#item-7) ⭐️ 7.0/10
8. [腾讯发布 770B 参数开放权重大模型 Hy4 Preview，支持百万级上下文](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [内核开发者讨论对付爬虫机器人的 Anubis 与 iocaine 方案](https://people.kernel.org/monsieuricon/creepy-crawlies) ⭐️ 8.0/10

一位 kernel.org 贡献者撰文分析了 git.kernel.org 面临的爬虫机器人负担，并评估了 Anubis 的工作量证明挑战和 iocaine 的粘滞陷阱（tarpit）等反机器人方案。这篇文章引发了广泛讨论，获得了 944 分和 452 条评论。 此事意义重大，因为 git.kernel.org 等大型开源代码托管平台正日益成为 AI 爬虫和无差别抓取工具的目标，维护者需要切实可行的缓解方案。这场讨论揭示了工作量证明、粘滞陷阱技术与用户体验之间的现实权衡，影响整个 Web 生态。 Anubis 使用 SHA-256 工作量证明挑战，但评论者指出，难度较高时移动设备可能需要约 180 秒才能完成。iocaine 则通过构造无尽的虚拟页面迷宫来困住爬虫；有评论者将其以 Elixir 中间件的形式低成本地集成到自己的应用中。

hackernews · zdw · 8月29日 17:49 · [社区讨论](https://news.ycombinator.com/item?id=49491791)

**背景**: git.kernel.org 是为 Linux 内核及相关项目提供公开 Git 托管服务的重要平台，cgit 会生成海量参数与哈希组合的链接，因此成为无差别爬虫的重点目标。Anubis 是一款开源的反 AI 爬虫工具，通过工作量证明挑战来限制抓取；iocaine 则是一个用 Rust 实现的粘滞陷阱工具，向爬虫投喂无穷无尽的虚假内容。两者代表了两种不同的思路：让机器人消耗算力，或主动欺骗并困住它们。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anubis_(software)">Anubis (software) - Wikipedia</a></li>
<li><a href="https://xeiaso.net/blog/2025/anubis/">Block AI scrapers with Anubis - Xe Iaso</a></li>
<li><a href="https://pablomurad.com/iocaine-poisoning-ais/">iocaine: poisoning AI's - pablomurad.com</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认同爬虫问题确实存在，但对最佳解决方案看法不一。有人批评 Anubis 在常见难度下对移动设备不友好，也有人称赞 iocaine 这类粘滞陷阱防御方案服务器开销低且富有创意；还有人提议让工作量证明的算力直接为网站所有者创造价值。

**标签**: `#bots`, `#web-scraping`, `#proof-of-work`, `#security`, `#kernel.org`

---

<a id="item-2"></a>
## [QubesOS QSB-118：qvm-copy-to-vm 致 Dom0 任意代码执行](https://www.qubes-os.org/news/2026/08/29/qsb-118/) ⭐️ 8.0/10

2026 年 8 月 29 日，Qubes OS 发布安全公告 QSB-118，披露了 qvm-copy-to-vm（Dom0 版）中的任意代码执行漏洞。当用户从 Dom0 向一台被攻破的 qube 复制文件时，该 qube 可在 Dom0 中注入并执行任意命令。 由于 Dom0 是拥有整个 Qubes OS 完全控制权的特权管理域，在其中实现任意代码执行意味着攻击者可完全攻陷系统并绕过其隔离保障。这对于所有依赖 Qubes 保护敏感工作负载的安全意识强的用户都有着重要影响。 该漏洞位于 Dom0 版 qvm-copy-to-vm 所用的错误报告路径中，该路径调用了 system() 函数。VM 端的 qvm-copy-to-vm 变体不受影响，因为它不使用 system()；利用该漏洞需要用户明确执行从 Dom0 向被攻破 qube 的复制操作。

hackernews · vntok · 8月30日 08:51 · [社区讨论](https://news.ycombinator.com/item?id=49496918)

**背景**: Qubes OS 是一款注重安全的桌面操作系统，借助 Xen 虚拟化技术将应用隔离到称为 qube 的独立虚拟机中。Dom0 是首个也是权限最高的域，负责管理系统；运行在 Dom0 中的软件可以完全控制整台机器。qvm-copy-to-vm 命令是在 qube 与 Dom0 之间安全复制文件的标准工具。这一背景解释了为什么错误报告函数中的缺陷会演变为完全的系统沦陷。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.qubes-os.org/news/2026/08/29/qsb-118/">QSB-118: Dom0 arbitrary code execution in qvm-copy-to-vm error reporting | Qubes OS</a></li>
<li><a href="https://en.wikipedia.org/wiki/Qubes_OS">Qubes OS - Wikipedia</a></li>
<li><a href="https://doc.qubes-os.org/en/latest/user/advanced-topics/how-to-install-software-in-dom0.html">How to install software in dom0 — Qubes OS Documentation</a></li>

</ul>
</details>

**社区讨论**: 评论者承认该漏洞的严重性，但也指出攻击面有限，因为利用需要用户主动从 Dom0 复制文件，而 Dom0 本就不应用于日常操作。还有人提及 Theo de Raadt 长期以来对单一系统设计的批评，质疑为何 Qubes 优于 BSD Jails 等替代方案，并指出相关代码是 Joanna Rutkowska 离开之后提交的。少数评论者还讨论了 Qubes 缺乏硬件加速等更广泛的问题。

**标签**: `#security`, `#qubesos`, `#vulnerability`, `#arbitrary-code-execution`, `#operating-systems`

---

<a id="item-3"></a>
## [Omarchy 漏洞：任意用户进程均可提权至 root](https://0xcc.io/posts/omarchy-root-creds/) ⭐️ 8.0/10

Omarchy 默认 Docker 配置中存在一个严重的权限提升漏洞，任何用户进程都可以在无需密码、无需 sudo 或任何授权提示的情况下获取 root 权限。该问题已在 Omarchy 4.0.1 中修复，官方敦促用户立即更新。 这一漏洞意义重大，因为它在一个备受关注的 Linux 发行版上彻底消除了用户进程与 root 之间的安全边界，任何恶意或被攻破的程序都可以完全控制系统。它也引发了对那些被热捧、匆忙开发的发行版安全性以及 Linux 桌面安全现状的更广泛担忧。 该漏洞源于 Omarchy 默认的 Docker 配置，该配置向用户桌面会话中运行的每个进程暴露了等同于 root 的权限。最重要的应对措施是尽快更新到 4.0.1 版本。

hackernews · trap0xcc · 8月30日 15:59 · [社区讨论](https://news.ycombinator.com/item?id=49499854)

**背景**: Omarchy 是由 David Heinemeier Hansson（DHH）创建的开源 Linux 发行版，它基于 Arch Linux，并围绕 Hyprland 平铺式 Wayland 合成器和 Quickshell 桌面 shell 构建。权限提升是一类安全漏洞，低权限用户或进程可利用错误配置获得更高权限，通常是 root 权限。Docker 容器与宿主机共享内核，配置不当的容器环境常常是本地权限提升漏洞的来源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://0xcc.io/posts/omarchy-root-creds/">Omarchy : Any User Process Can Escalate to Root</a></li>
<li><a href="https://en.wikipedia.org/wiki/Omarchy">Omarchy</a></li>
<li><a href="https://github.com/basecamp/omarchy">GitHub - basecamp/ omarchy : Beautiful, Modern & Opinionated Linux</a></li>

</ul>
</details>

**社区讨论**: 评论者态度尖锐，有人指出 Omarchy 此前曾将 USB 描述符直接送入 shell，并警告不要使用这类“vibecoded”（随意拼凑/由 AI 生成的）发行版。还有人认为 Ubuntu 已经够用，并提醒不要盲目追捧 CachyOS、Omarchy 这类被媒体热炒的发行版。也有观点认为 Linux 缺少真正的桌面沙箱架构，因此这类可修复的漏洞只是“安全剧场”的一部分，而 sudo 本身就让恶意软件在任何主流发行版上都能轻易提权到 root。

**标签**: `#security`, `#vulnerability`, `#linux`, `#privilege-escalation`, `#omarchy`

---

<a id="item-4"></a>
## [欧盟委员会在 ProtectEU 战略中重新推动加密后门](https://reclaimthenet.org/eu-protecteu-strategy-encryption-backdoor-law-enforcement) ⭐️ 8.0/10

2025 年 4 月 1 日，欧盟委员会推出了新的五年期内部安全战略“ProtectEU”，据报道该战略重新推动执法部门获取加密通信，实际上就是呼吁设立加密后门。此举重新引发了关于安全与隐私之间长期存在的争论。 此事意义重大，因为它可能重塑整个欧盟的加密政策，并为其他民主国家树立先例，影响数百万用户和在欧洲运营的科技公司。如果付诸实施，它将削弱端到端加密服务的安全承诺，并可能被恶意行为者利用。 ProtectEU 战略是面向 2025–2030 年的计划，旨在支持成员国应对内部安全威胁。包括数字权利组织在内的批评者警告说，后门本身就不安全，会损害加密为所有人——而不仅仅是罪犯——提供的保护。

hackernews · nickslaughter02 · 8月30日 15:12 · [社区讨论](https://news.ycombinator.com/item?id=49499394)

**背景**: 加密后门是故意隐藏的漏洞或特殊的访问机制，允许政府或执法部门绕过加密读取数据。安全专家普遍认为，任何为“好人”设置的后门也可能被黑客和敌对势力利用，从而破坏所有人的加密安全。ProtectEU 是欧盟委员会于 2025 年 4 月 1 日公布的五年期内部安全战略，已遭到数字权利组织的批评。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ec.europa.eu/commission/presscorner/detail/en/ip_25_920">Commission unveils ProtectEU – a new European Internal Security Strategy</a></li>
<li><a href="https://home-affairs.ec.europa.eu/news/commission-presents-protecteu-internal-security-strategy-2025-04-01_en">Commission presents ProtectEU Internal Security Strategy - Migration and Home Affairs</a></li>
<li><a href="https://edri.org/our-work/protecteu-security-strategy-a-step-further-towards-a-digital-dystopian-future/">‘ProtectEU’ security strategy - European Digital Rights (EDRi)</a></li>

</ul>
</details>

**社区讨论**: 评论者压倒性地反对该计划，一些人认为欧盟委员会权力过大且对公民不负责。还有人警告，此类政策可能助长未来威权领导人，而且鉴于 AI 代理已能破解脆弱系统，故意留下漏洞是鲁莽之举。少数人提出讽刺性建议，比如在支持者的银行系统中公开后门，看他们是否很快就会改变立场。

**标签**: `#encryption`, `#privacy`, `#EU-policy`, `#security`, `#surveillance`

---

<a id="item-5"></a>
## [ChatGPT Work 解析：云端与本地桌面版](https://simonwillison.net/2026/Aug/30/understanding-chatgpt-work/) ⭐️ 8.0/10

西蒙·威利森（Simon Willison）发表了一篇关于 OpenAI ChatGPT Work 的深度分析，将其拆解为两个不同版本：Work Cloud 和 Work Local。他详细介绍了模型选择、可访问互联网的代码执行环境、无头 Chrome 浏览器、持久文件系统、ChatGPT Sites 和子代理等专属功能。 由于 ChatGPT Work 是一个快速演变且令人困惑的产品，这篇分析为开发者和 AI 从业者提供了实用的指引，帮助他们了解何时应使用 Work 而非 Chat，以及 Work 具有哪些独特能力。同时它也展现了 OpenAI 如何从传统聊天扩展到自动化、子代理、代码执行等智能体功能。 威利森指出，Work Cloud 可通过 chatgpt.com 和移动应用访问，而 Work Local 则通过原先名为 Codex 的桌面应用提供，使非开发人员更易上手。Work Cloud 提供 GPT-5.6 Sol/Luna/Terra（推理级别最高至 Ultra），并包含无头 Chrome、持久共享文件系统、ChatGPT Sites 发布和子代理会话；Chat 与 Work 在模型可用性上也有所不同，例如 5.6 Pro 仅限 Chat 使用。

rss · Simon Willison · 8月30日 23:59

**背景**: ChatGPT 是 OpenAI 广泛使用的对话式 AI 助手，而 ChatGPT Work 是 2026 年 7 月推出的智能体模式，用于完成分析、演示文稿、工作流或文件等有明确结果的较长任务。Codex 是 OpenAI 的 AI 编程代理，可在终端、桌面和 IDE 中运行；其桌面应用被重新定名为 Work Local 的基础。该文章将 OpenAI 的官方指南（“用 Chat 获取答案，用 Work 获取成品输出”）与通过实验观察到的实际功能差异进行了对比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/chatgpt-work/">ChatGPT Work for every team | OpenAI</a></li>
<li><a href="https://learn.chatgpt.com/docs/get-started-with-work">Get started with ChatGPT Work</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(AI_agent)">OpenAI Codex (AI agent) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI`, `#ChatGPT`, `#OpenAI`, `#product analysis`, `#developer tools`

---

<a id="item-6"></a>
## [1980 年 Spacelab 计算机磁芯内存模块剖析](https://www.righto.com/2026/08/spacelab-core-memory.html) ⭐️ 7.0/10

Ken Shirriff 发布了对 1980 年 Spacelab 计算机（法国制造的 Mitra 125 MS）磁芯内存模块的详细拆解与逆向工程分析，重点探讨了其省略抑制线的独特设计，并解释了这种架构的工作原理及权衡取舍。 这很重要，因为它提供了对前微处理器时代航天级计算硬件的罕见而详细观察，展示了设计者如何通过精细的物理与逻辑设计实现可靠性。对复古计算爱好者、硬件工程师和太空历史爱好者而言，这是高价值内容。 该磁芯内存模块将铁氧体磁芯排列在一个平面上，带有 X/Y 选择线和读出线，但没有抑制线——这一选择减少了读出放大器的数量并简化了电路板布局。正如更广泛的逆向工程系列所指出的，Spacelab 计算机的 16 位 CPU 完全由分立逻辑芯片构建，而非微处理器。

hackernews · pwg · 8月30日 20:00 · [社区讨论](https://news.ycombinator.com/item?id=49502214)

**背景**: 磁芯存储器在 1950 年代至 1970 年代是随机存取存储器的主要形式，每个位以穿线微型铁氧体磁环的磁化方向来存储。在典型的磁芯存储器中，抑制线在写周期内防止半选磁芯被覆写；省略它则改变了写入策略并可能减少元件数量。Spacelab 在 1980 年前后搭载了法国制造的 Mitra 125 MS 小型计算机，Ken Shirriff 的博客系列对其电路进行逆向工程，该计算机完全没有使用微处理器，颇具特色。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Magnetic-core_memory">Magnetic-core memory - Wikipedia</a></li>
<li><a href="https://www.computerhistory.org/revolution/memory-storage/8/253">Magnetic Core Memory - CHM Revolution</a></li>
<li><a href="https://hackaday.com/2026/05/24/spacelabs-mitra-125-ms/">Spacelab ’s Mitra 125 MS | Hackaday</a></li>

</ul>
</details>

**社区讨论**: 评论者询问省略抑制线是否使内存更快，还是主要为了减少读出放大器数量并简化电路板布局，作者 Ken Shirriff 参与回答相关问题。还有人感叹磁芯存储器在太空中的可靠性及其相比现代 RAM 的重量，一位评论者则将太空计算机的 N 模冗余与提议的基于多个 LLM 编写实现的 N 模冗余进行了类比。

**标签**: `#core-memory`, `#retrocomputing`, `#space-hardware`, `#hardware`, `#history`

---

<a id="item-7"></a>
## [PostgreSQL 日志：善用 log_line_prefix 与 log_timezone 提升可观测性](https://postgr.es/p/9tx) ⭐️ 7.0/10

PostgreSQL 专家 Christophe Pettus 解释了如何使用 log_line_prefix 和 log_timezone 配置参数，让 PostgreSQL 日志在跨会话和外部系统关联条目时更有用。文章将日志前缀视为把日志行与其上下文来源连接起来的关键。 对于在生产环境运行 PostgreSQL 的数据库管理员而言，结构良好的日志对故障排查、审计和可观测性至关重要。正确设置 log_line_prefix 和 log_timezone 有助于团队在分布式系统中关联事件，并避免因时间戳不一致而产生混淆。 log_line_prefix 只能在 postgresql.conf 中设置，默认值为'%m [%p] '（时间戳加进程 ID）。log_timezone 是集群级设置，默认是 GMT，但通常会被覆盖为 localtime 或指定的时区；两者都是 PostgreSQL 的 GUC 参数。

rss · Planet PostgreSQL · 8月30日 01:00

**背景**: PostgreSQL 使用名为 GUC（Grand Unified Configuration）的集中式配置系统来管理数百个参数。log_line_prefix 参数控制每条日志条目的前缀，管理员可以在其中加入时间戳、进程 ID、用户名、数据库名等占位符。log_timezone 确保所有会话以同一时区写入日志时间戳，这在聚合多台服务器的日志时至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://postgresqlco.nf/doc/en/param/log_line_prefix/">PostgreSQL Documentation: log_line_prefix parameter</a></li>
<li><a href="https://postgresqlco.nf/doc/en/param/log_timezone/">PostgreSQL Documentation: log_timezone parameter PostgreSQL: Documentation: 18: 19.8. Error Reporting and Logging log_timezone - pgPedia - a PostgreSQL Encyclopedia A Guide to PostgreSQL log_timezone: Avoiding Timestamp Mismatches postgresql - postgres default timezone - Stack Overflow PostgreSQL: Documentation: 18: 8.5. Date/Time Types postgresql - Setting postgres logfile's timestamp to same as ...</a></li>
<li><a href="https://www.enterprisedb.com/postgres-tutorials/how-tune-postgresql-guc-parameters">How to Tune PostgreSQL GUC Parameters | EDB</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#logging`, `#database administration`, `#observability`

---

<a id="item-8"></a>
## [腾讯发布 770B 参数开放权重大模型 Hy4 Preview，支持百万级上下文](https://simonwillison.net/2026/Aug/29/hy4/) ⭐️ 7.0/10

腾讯发布了 Hy4 Preview，这是一款开放权重的纯文本大语言模型，总参数量 770B，激活参数量 49B，上下文窗口达 100 万 token，Hugging Face 上文件大小 1.56TB。相比之前的 Hy3（295B 总参数、256K 上下文），规模大幅提升。 此次发布标志着中国头部公司推出的开放权重大模型中规模最大的之一，大幅扩展了本地和 API 实验可用的模型能力。100 万 token 的上下文窗口也使 Hy4 能够与领先的长上下文模型竞争，可能影响依赖开放权重替代品进行研究和生产的开发者。 该模型仅支持文本输入，不支持视觉，采用混合专家（MoE）架构，770B 参数中只有 49B 处于激活状态。其聊天模板暴露了 reasoning_effort 参数，只有'high'（默认）和'no_think'两个取值，早期测试显示其隐藏推理链使用简化、节省 token 的英文。

rss · Simon Willison · 8月29日 23:53

**背景**: Hy4 采用了混合专家（MoE）架构，这种设计保持很大的总参数量，但每个 token 只激活一部分参数，从而降低计算成本并保留模型容量。Hugging Face 模型使用 Jinja2 聊天模板将对话消息格式化为模型专属的 token 序列，而推理大模型中常见的 reasoning_effort 参数，通常控制模型在作答前进行多少内部思考。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@mindscope-academy.online/the-power-of-mixture-experts-in-llms-cf913f3253c4">The Power of Mixture of Experts in LLMs | by Mindscope... | Medium</a></li>
<li><a href="https://deepwiki.com/huggingface/alignment-handbook/6.3-chat-templates-and-message-formatting">Chat Templates and Message Formatting - deepwiki.com</a></li>
<li><a href="https://community.openai.com/t/o1s-reasoning-effort-parameter/1062308">O1's ' reasoning effort ' parameter - API - OpenAI Developer Commun...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#Tencent`, `#open-weights`, `#AI`, `#model-release`

---