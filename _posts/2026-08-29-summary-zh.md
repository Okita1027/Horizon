---
layout: default
title: "Horizon 日报：2026-08-29 (ZH)"
date: 2026-08-29
lang: zh
---

> 从 34 条内容中筛选出 9 条重要资讯。

---

1. [vphone-cli：用 Apple Virtualization.framework 本地启动虚拟 iPhone](#item-1) ⭐️ 8.0/10
2. [第九巡回法院在 Kalshi 博彩案中支持各州](#item-2) ⭐️ 8.0/10
3. [Htmx 4.0 发布：超媒体驱动 Web 应用的重大升级](#item-3) ⭐️ 8.0/10
4. [OpenAI 在 Cursor 被 SpaceX 收购后切断其模型访问](#item-4) ⭐️ 8.0/10
5. [美国制裁意大利隐私托管组织 Autistici/Inventati](#item-5) ⭐️ 8.0/10
6. [Martin Fowler：智能体 AI 需要扎实可信的数据基础](#item-6) ⭐️ 8.0/10
7. [研究员以 80%成功率绕过 Claude Code 自动模式](#item-7) ⭐️ 8.0/10
8. [乌迈尔·沙希德：你应该多快修补生产环境的 PostgreSQL？](#item-8) ⭐️ 7.0/10
9. [pg_dump 数据恢复因 search_path 被清空而导致触发器引用失败](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [vphone-cli：用 Apple Virtualization.framework 本地启动虚拟 iPhone](https://github.com/Lakr233/vphone-cli) ⭐️ 8.0/10

Lakr233 发布了 vphone-cli，这是一款开源命令行工具，可在 Apple Silicon Mac 上利用苹果官方的 Virtualization.framework 本地启动虚拟 iPhone，并支持 DFU 恢复、获取 SHSH 以及越狱固件变体。 这标志着开发者不再必须依赖 Corellium 等专有服务，而是可以通过本地的、可脚本化的 iOS 虚拟化方案来支撑 CI 流水线、自动化测试和安全研究，且无需第三方破解手段。 该工具会下载并合并 IPSW 固件文件，使用多种安全绕过变体（例如 --variant jb）修补引导链，并将所有产物存放在 ~/.vphone 目录下；它依赖 macOS 主机，并且官方提示在 iOS 设置中不要选择日本或欧盟地区，因为虚拟机无法满足这些地区的额外监管检查。

hackernews · hentrep · 8月28日 23:02 · [社区讨论](https://news.ycombinator.com/item?id=49485267)

**背景**: 苹果的 Virtualization.framework 让开发者可以在 Apple Silicon 上创建和运行虚拟机，但它此前只支持 macOS 和 Linux 来宾系统，并不支持 iOS。vphone-cli 的工作原理是下载官方 IPSW 固件、将其合并成可启动的镜像包、修补引导链，然后执行 DFU 恢复——这与真实设备的底层刷机流程相同。这种方案使本地 iOS 虚拟化成为可能，并直接与 Corellium 专有的虚拟硬件方案形成竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Lakr233/vphone-cli">GitHub - Lakr233/vphone-cli · GitHub</a></li>
<li><a href="https://grokipedia.com/page/vPhone">vPhone</a></li>
<li><a href="https://developer.apple.com/documentation/virtualization/virtualize-macos-on-a-mac">Virtualize macOS on a Mac | Apple Developer Documentation</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者反响积极但也有不少疑问：有人询问它与 iOS 模拟器有什么区别，有人关心是否包含虚拟基带、能否用于账号恢复，还有用户指出 macOS 主机依赖仍会限制其规模化部署。

**标签**: `#iOS`, `#Virtualization`, `#CI`, `#Apple`, `#Developer Tools`

---

<a id="item-2"></a>
## [第九巡回法院在 Kalshi 博彩案中支持各州](https://azmirror.com/2026/08/28/9th-circuit-sides-with-states-in-kalshi-gambling-fight-potentially-reviving-arizonas-prosecution/) ⭐️ 8.0/10

美国第九巡回上诉法院一致裁定，Kalshi 平台上的体育博彩合约不受《商品交易法》的联邦豁免保护，不能凌驾于各州赌博法之上。这项裁决可能会恢复亚利桑那州总检察长 Kris Mayes 对该公司提起的诉讼。 这对 Kalshi 及整个预测市场行业是一次重大法律挫折，该行业此前主张受联邦监管的事件合约优先于各州赌博禁令。该裁决可能迫使 Kalshi 及类似平台遵守各州五花八门的法律，或在某些州停售体育博彩产品。 该合议庭意见由法官 Ryan Nelson 撰写，驳回了《商品交易法》优先于各州体育博彩法规的主张，称国会并未用“大锤”摧毁联邦、州及部落积累数十年的博彩监管规则。该裁决推翻了下级法院此前阻止亚利桑那州起诉的决定。

hackernews · hungryhobbit · 8月28日 23:32 · [社区讨论](https://news.ycombinator.com/item?id=49485452)

**背景**: Kalshi 是一家受监管的预测市场和交易所，于 2021 年推出，用户可就选举、体育、加密货币和天气等事件结果交易合约；到 2025 年，体育博彩已占其网站活动的 90%以上。预测市场是参与者就未来事件结果交易合约的平台，价格相当于群体估计的概率。《商品交易法》监管期货交易，Kalshi 曾据此主张其产品是合法商品而非非法赌博。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kalshi">Kalshi - Wikipedia</a></li>
<li><a href="https://www.worldmonitor.app/blog/glossary/prediction-market/">Prediction Market Definition | World Monitor</a></li>

</ul>
</details>

**社区讨论**: 评论者提供了法律分析和反应：一位律师指出联邦体育博彩法律和《商品交易法》监管的复杂性，另一位则表示这一结果“显而易见”，并称赞法院终于得出这一结论。还有人以外行身份询问巡回法院的级别与体系，并猜测该裁决对各州损失追讨法的影响。

**标签**: `#legal`, `#regulation`, `#prediction markets`, `#sports betting`, `#Kalshi`

---

<a id="item-3"></a>
## [Htmx 4.0 发布：超媒体驱动 Web 应用的重大升级](https://four.htmx.org/announcements/2026-08-28-htmx-4.0.0-is-released) ⭐️ 8.0/10

Htmx 4.0.0 于 2026 年 8 月 28 日正式发布，带来了新特性和兼容性改进。值得关注的新增功能包括 hx-alpine-compat，它平滑了 htmx 与 Alpine.js 之间的兼容性问题。 作为最广泛使用的超媒体库之一的主要版本发布，Htmx 4.0 加强了服务器端渲染和更简化前端架构的趋势。对于希望在 HTML 中直接使用 AJAX、WebSockets 和 CSS 过渡而无需重型 JavaScript 框架的开发者来说，这具有重要意义。 该版本包含 hx-alpine-compat，用于平滑 htmx 与 Alpine.js 之间的兼容性。Htmx 依然保持小巧（压缩后约 14k）、无依赖且可扩展，延续其设计理念。

hackernews · rmsaksida · 8月28日 13:28 · [社区讨论](https://news.ycombinator.com/item?id=49478178)

**背景**: Htmx 是由 Carson Gross 创建的开源前端 JavaScript 库，作为 intercooler.js 的继任者，于 2020 年首次发布。它通过自定义属性扩展 HTML，使 AJAX、WebSockets、CSS Transitions 和 Server-Sent Events 可以直接在 HTML 中使用，从而无需编写 JavaScript 即可构建动态网页。该库采用超媒体驱动的方法，服务器响应（通常是 HTML 片段）会被插入页面指定位置，而无需刷新整个页面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Htmx">Htmx</a></li>
<li><a href="https://htmx.org/">htmx - high power tools for html</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hypermedia">Hypermedia</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一，但大多热情。支持者称赞 htmx 为 Web 开发带来了乐趣和简洁；一位 .NET/Angular 开发者则提出相反观点，认为 htmx 迫使人们回到服务器渲染 UI，将表现层与业务逻辑混在一起。另一位用户指出 alpine-ajax 更小且足够满足其需求，还有人欣赏 htmx 作为一种有机成长的非企业级替代方案，启发了 Datastar 等项目。

**标签**: `#htmx`, `#web development`, `#hypermedia`, `#release`

---

<a id="item-4"></a>
## [OpenAI 在 Cursor 被 SpaceX 收购后切断其模型访问](https://openai.com/index/our-decision-on-cursor-following-its-acquisition-by-spacex/) ⭐️ 8.0/10

OpenAI 已限制 Cursor 在其 AI 模型上的访问权限，此前 Cursor 被 SpaceX 收购。这一决定在 OpenAI 官网上公布，反映了前沿 AI 领域竞争紧张局势的升级。 此举表明，前沿模型供应商愿意切断被视为竞争威胁的下游工具的访问。依赖 Cursor 多模型集成的开发者可能需要改用其他代码编辑器或模型提供商。 此次限制发生在违反服务条款之后，马斯克据称承认对 OpenAI 模型进行了蒸馏。值得注意的是，Anthropic 今年早些时候已因类似原因封禁了 xAI。

hackernews · meetpateltech · 8月29日 01:47 · [社区讨论](https://news.ycombinator.com/item?id=49486172)

**背景**: Cursor 是一个基于 Visual Studio Code 构建、由 AI 驱动的代码编辑器，集成多个大型语言模型来协助编码、调试和重构。前沿 AI 模型是当前能力最强的通用 AI 系统，通常由 OpenAI、Anthropic 等公司提供。模型提供商通常禁止使用其 API 训练竞争模型，OpenAI 对 Cursor 的举措正反映了这种竞争动态。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cursor.com/features">Features | Cursor - The AI -first Code Editor</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/frontier-models/">What Are Frontier AI Models and How They Work | NVIDIA Glossary</a></li>
<li><a href="https://www.linkedin.com/pulse/why-cursor-ai-loved-developers-coding-editor-transforming-o0vjc">Why Cursor AI Is Loved by Developers: The AI Coding Editor ...</a></li>

</ul>
</details>

**社区讨论**: 评论者大多认为此举是违反服务条款的必然后果，并指出 Anthropic 此前已因类似行为封禁了 xAI。一些开发者表示这一变化让他们重新转向 Anthropic 的模型，而另一些在 Cursor 中使用 Grok 或 Composer 的用户受影响较小，并建议 Cursor 托管更多开源模型。此外，Cursor 创始人也在推特上回应了此事。

**标签**: `#AI`, `#OpenAI`, `#Cursor`, `#SpaceX`, `#Tech Industry`

---

<a id="item-5"></a>
## [美国制裁意大利隐私托管组织 Autistici/Inventati](https://www.inventati.org/) ⭐️ 8.0/10

2026 年 8 月下旬，美国国务院和财政部将意大利组织 Autistici/Inventati（Noblogs.org 博客平台的托管方）认定为“特别指定全球恐怖分子”实体。制裁措施禁止美国个人与该组织及其服务进行往来。 此举标志着将互联网基础设施和注重隐私的托管服务商视为恐怖组织的一次重大升级，也为其他去中心化工具开创了令人警惕的先例。这一认定可能让依赖 Noblogs.org 及类似隐私服务的独立媒体、活动人士和文化项目感到寒蝉效应。 Autistici/Inventati 于 2001 年由意大利自主反资本主义运动中的个人和集体创建，提供电子邮件、网页托管以及 Noblogs.org 平台，许多书展、广播节目和文化项目都依赖该平台。该组织与 Indymedia Italy 及 2001 年热那亚八国集团峰会抗议活动有历史关联，一些评论者认为这正是此次制裁的相关背景。

hackernews · exiguus · 8月28日 12:58 · [社区讨论](https://news.ycombinator.com/item?id=49477854)

**背景**: Autistici/Inventati 是一个为活动人士和草根运动提供安全通信工具与托管服务的集体，其旗下 Noblogs.org 是被广泛使用的免费博客平台。美国的此次认定是更广泛的制裁行动的一部分，同期被制裁的还有 Palestine Action 和 Masar Badil 等组织，这引发担忧：不仅仅是个人，连基础设施提供方也可能被贴上恐怖分子的标签。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.radiorebelde.cu/english/u-s-designates-palestine-action-masar-badil-and-autistici-inventati-as-terrorist-groups-26082026/">U.S. Designates Palestine Action, Masar Badil, and Autistici Inventati ...</a></li>
<li><a href="https://crimethinc.com/2026/08/27/us-government-designates-host-of-noblogsorg-a-global-terrorist">US Government Designates Host of NoBlogs . org a "Global Terrorist"</a></li>
<li><a href="https://www.autistici.org/">autistici.org - Welcome to Autistici / Inventati</a></li>

</ul>
</details>

**社区讨论**: 评论区普遍对这一先例感到震惊，一位用户认为将基础设施提供方列为“恐怖分子”是前所未有的，并质疑 I2P、Monero、Veilid、Tox 或 Signal 的用户和开发者是否会成为下一个目标。还有人补充了该组织源自热那亚八国集团峰会抗议和 Indymedia 的历史背景；也有少数人表示看不懂该组织到底做什么，或用伊拉克大规模杀伤性武器的说法进行讽刺。

**标签**: `#sanctions`, `#privacy`, `#internet infrastructure`, `#civil liberties`, `#hosting`

---

<a id="item-6"></a>
## [Martin Fowler：智能体 AI 需要扎实可信的数据基础](https://martinfowler.com/articles/making-data-ready-for-agentic-ai.html) ⭐️ 8.0/10

Martin Fowler 发布了由 Pramod Sadalage 和 Prem Chandrasekaran 撰写的文章，指出企业必须先建立准确、可信的数据基础，才能成功实施智能体 AI。文章为企业数据如何为自主 AI 系统做好准备提供了实用指导。 在企业争相采用智能体 AI 来实现自动化和降本增效之际，多数人却忽略了 AI 的可靠性取决于它所访问的数据。这篇文章聚焦数据质量与信任这一关键缺口，而这正是智能体 AI 在生产环境中安全有效运行的基础。 文章由两位数据工程实践者 Pramod Sadalage 和 Prem Chandrasekaran 撰写，发布在备受推崇的软件工程网站 Martin Fowler 上。文中强调，不可靠的数据基础——被形容为“不过是沙子”——无论模型多先进，都会拖垮 AI 项目。

rss · Martin Fowler · 8月27日 13:11

**背景**: 智能体 AI（Agentic AI）指的是能够设定目标、使用工具并在一定自主程度上采取行动的人工智能程序，其控制流通常由大语言模型驱动。与仅回答问题的传统聊天机器人不同，智能体系统需要执行多步骤任务并与外部环境交互，因此对准确、可信数据的依赖更为关键。对许多企业而言，现有数据管道在设计时从未考虑过支持这种自主决策。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agentic_AI">Agentic AI</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>

</ul>
</details>

**标签**: `#agentic-ai`, `#data-quality`, `#data-engineering`, `#ai-adoption`

---

<a id="item-7"></a>
## [研究员以 80%成功率绕过 Claude Code 自动模式](https://simonwillison.net/2026/Aug/27/breaking-claude-code-opus-5-auto-mode/) ⭐️ 8.0/10

安全研究员 Johann Rehberger 演示了一种提示注入攻击，可在大约 80%的情况下绕过 Claude Code 的自动模式。该攻击诱使编码代理下载并解压一个包含恶意 struct.py 的 zip 压缩包，当代理随后导入 base64 时，该恶意文件会被执行。 这很重要，因为自动模式现已成为 Pro、Max 和 Team 计划的默认设置，而 Anthropic 对其有效性曾作出大胆宣称。一种具有高成功率的实际绕过方式表明，基于分类器的防护措施不足以应对对抗性内容，也进一步证明了应在沙箱中运行编码代理。 该攻击的原理是让 Claude Code 获取一个 zip 文件并解压，然后运行导入 base64 的代码；由于 base64 本身会导入 struct，因此从压缩包中解压出的本地 struct.py 会遮蔽 Python 标准库模块。在某些运行中，自动模式甚至阻止了代理自身终止恶意进程的尝试，意味着安全机制本身成了故障的一部分。

rss · Simon Willison · 8月27日 22:50

**背景**: Claude Code 是 Anthropic 推出的 AI 编码代理，可执行较长时间的自主任务。自动模式现已成为许多计划的默认设置，它会将工具调用交给一个分类器处理，以拦截不可逆、破坏性或针对外部环境的命令。提示注入是一类攻击，利用隐藏在网页、文件或其他内容中的恶意指令，诱导大语言模型执行非预期操作。此次攻击还利用了 Python 的模块搜索顺序：当前目录下的文件（如 struct.py）可能替代 base64 内部所要导入的标准库模块而被加载。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/auto-mode-config">Configure auto mode - Claude Code Docs</a></li>
<li><a href="https://claude.com/blog/auto-mode-default-in-claude-code">Auto mode is now the default in Claude Code for Pro, Max, and Team plans | Claude by Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>

</ul>
</details>

**标签**: `#prompt injection`, `#AI security`, `#Claude Code`, `#LLM agents`, `#security research`

---

<a id="item-8"></a>
## [乌迈尔·沙希德：你应该多快修补生产环境的 PostgreSQL？](https://postgr.es/p/9ts) ⭐️ 7.0/10

该文章分析了 PostgreSQL 史上最大规模的安全更新（涉及 28 个 CVE），并督促生产用户着力缩短从发布到部署的补丁延迟。

rss · Planet PostgreSQL · 8月28日 11:41

**标签**: `#PostgreSQL`, `#Security`, `#Patching`, `#Production`, `#Database`

---

<a id="item-9"></a>
## [pg_dump 数据恢复因 search_path 被清空而导致触发器引用失败](https://postgr.es/p/9tt) ⭐️ 7.0/10

PostgreSQL 的 pg_dump 数据恢复可能失败，因为转储文件开头将 search_path 设置为空字符串，导致触发器函数中未加模式限定的表名无法解析。即使恢复到全新的空模式中，也会出现“relation book_audit does not exist”之类的错误。 这个微妙的问题会影响使用触发器执行数据恢复的数据库管理员和开发人员。如果不了解常见的解决方法，恢复可能会在某个表上悄然留下零行数据，同时序列却已前进，导致问题难以排查。 转储文件开头包含 `SELECT pg_catalog.set_config('search_path', '', false);`，将会话的搜索路径固定为空。触发器错误会中断并回滚整个 COPY 块，导致只有该表为空，而随后的 setval 调用仍会推进序列。

rss · Planet PostgreSQL · 8月28日 00:00

**背景**: 在 PostgreSQL 中，schema（模式）用于对表、视图等对象进行分组，而 search_path 设置决定了引用不加模式前缀的对象时 PostgreSQL 会搜索哪些模式。pg_dump 会在输出中显式将 search_path 设置为空字符串，以确保恢复出来的对象都使用完整限定名，不依赖会话的默认路径。但这也会影响触发器函数，因为函数内可能包含原本依赖默认 search_path 解析的未限定表名。文章建议使用 --disable-triggers、延迟约束或将会话的 session_replication_role 设置为 replica 等解决方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://stackoverflow.com/questions/42157311/is-there-a-way-for-pg-dump-not-to-use-search-path-for-schema">postgresql - Is there a way for pg_dump not to use search_path for schema - Stack Overflow</a></li>
<li><a href="https://www.crunchydata.com/blog/demystifying-schemas-search_path-through-examples">Demystifying Schemas & search_path through Examples | Crunchy Data Blog</a></li>
<li><a href="https://sqlpey.com/postgresql/postgresql-search-path-explained/">PostgreSQL Schema Search Path Explained: Configuration and</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#pg_dump`, `#search_path`, `#triggers`, `#database administration`

---