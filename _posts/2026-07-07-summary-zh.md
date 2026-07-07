---
layout: default
title: "Horizon 日报：2026-07-07 (ZH)"
date: 2026-07-07
lang: zh
---

> 从 39 条内容中筛选出 15 条重要资讯。

---

1. [Anthropic 揭示语言模型中的全局工作空间](#item-1) ⭐️ 9.0/10
2. [OpenWrt One 开源硬件路由器发布](#item-2) ⭐️ 8.0/10
3. [GLM 5.2 预示 AI 利润率崩溃](#item-3) ⭐️ 8.0/10
4. [微软 Xbox 重置凸显利润困境](#item-4) ⭐️ 8.0/10
5. [学习编程在 AI 时代仍具价值](#item-5) ⭐️ 8.0/10
6. [新模型在实际任务中表现更差](#item-6) ⭐️ 8.0/10
7. [Natvis 调试可视化功能登陆 Rider 的 Linux 和 macOS 版本](#item-7) ⭐️ 8.0/10
8. [PostgreSQL 20 增加后端级锁统计](#item-8) ⭐️ 8.0/10
9. [PostgreSQL 14-16 最新小版本中的复制死锁漏洞](#item-9) ⭐️ 8.0/10
10. [PostgreSQL VACUUM 页级字节分析](#item-10) ⭐️ 8.0/10
11. [腾讯发布 Hy3 MoE 模型，参数达 2950 亿](#item-11) ⭐️ 8.0/10
12. [VS Code 与 OpenAI 通过 GPT-5.5 提示调优减少 Token 消耗](#item-12) ⭐️ 7.0/10
13. [CloudNativePG 1.30：声明式角色与免密 TLS](#item-13) ⭐️ 7.0/10
14. [PostgreSQL 中 .ready 和 .done 文件实用指南](#item-14) ⭐️ 7.0/10
15. [PostgreSQL 分区裁剪的两阶段执行](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Anthropic 揭示语言模型中的全局工作空间](https://www.anthropic.com/research/global-workspace) ⭐️ 9.0/10

Anthropic 发表了一项研究，在语言模型中识别出一个“全局工作空间”（J-space），这是一小部分激活，使得逻辑推理和抽象思维成为可能。 这一发现是 AI 可解释性和安全性的重要一步，有望让研究人员隔离和控制推理回路，从而提高模型可靠性并减少幻觉。 J-space 对于流畅的文本生成或事实回忆并非必需，但对高阶认知功能至关重要；它容量有限且在机制上具有特权地位，众多电路从中读取和写入。

hackernews · in-silico · 7月6日 17:44 · [社区讨论](https://news.ycombinator.com/item?id=48808002)

**背景**: 全局工作空间理论最初来自认知科学，认为存在一个中央枢纽整合信息以实现意识。Anthropic 的工作在大型语言模型中找到了类似物：一个激活子空间充当推理瓶颈，尽管这不一定暗示意识。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/research/global-workspace">A global workspace in language models \ Anthropic</a></li>
<li><a href="https://transformer-circuits.pub/2026/workspace/index.html">Verbalizable Representations Form a Global Workspace in Language Models</a></li>

</ul>
</details>

**社区讨论**: 评论者指出了与其他实验的联系，例如复制与数学相关的层以提高性能。一些人批评了与意识的类比，倾向于更直接的术语。还分享了 Neel Nanda 独立评论的链接。

**标签**: `#language models`, `#AI research`, `#interpretability`, `#global workspace`, `#Anthropic`

---

<a id="item-2"></a>
## [OpenWrt One 开源硬件路由器发布](https://openwrt.org/toh/openwrt/one) ⭐️ 8.0/10

OpenWrt 宣布推出 OpenWrt One，这是一款完全开源的参考设计路由器，含外壳和天线售价约 106 美元。 这是 OpenWrt 首个官方开源硬件参考设计，让社区能够自行构建和定制路由器，同时延长设备寿命并减少电子垃圾。 OpenWrt One 含外壳和天线的售价约为 106 美元，不含则为 84 美元，但仅配备 1GB 内存。未来支持 WiFi 7 的 OpenWrt Two 型号已在开发中。

hackernews · peter_d_sherman · 7月6日 18:23 · [社区讨论](https://news.ycombinator.com/item?id=48808482)

**背景**: OpenWrt 是一款基于 Linux 的开源嵌入式操作系统，主要用于无线路由器。它提供完全可写的文件系统和包管理功能，使用户能够自定义和扩展路由器功能，超越原厂固件。OpenWrt One 是一款完全开放硬件原理图和设计文件的参考设计，让爱好者能够自行构建路由器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenWrt">OpenWrt</a></li>
<li><a href="https://github.com/openwrt/openwrt">GitHub - openwrt/openwrt: This repository is a mirror of ...</a></li>

</ul>
</details>

**社区讨论**: 社区反响热烈，称赞开源硬件倡议和具有竞争力的定价。部分用户讨论了未来 OpenWrt Two 对 WiFi 7 的支持，并将 OpenWrt 与 OPNSense 等替代方案进行比较，还有一些用户指出了 1GB 内存等小限制。

**标签**: `#openwrt`, `#open hardware`, `#router`, `#networking`, `#embedded systems`

---

<a id="item-3"></a>
## [GLM 5.2 预示 AI 利润率崩溃](https://martinalderson.com/posts/the-upcoming-ai-margin-collapse-part-1-glm-5-2/) ⭐️ 8.0/10

文章认为，Z.AI 发布的具有竞争力的开源权重模型 GLM 5.2 将加剧价格竞争，导致 AI 模型市场利润率崩溃。 这可能通过降低用户成本重塑 AI 行业，但也威胁到 OpenAI 和 Anthropic 等专有模型提供商的盈利能力，可能导致市场商品化。 GLM 5.2 是一个开源权重模型，拥有 744B 总参数、40B 活跃参数和 1M 上下文窗口，在编码、推理和智能体任务上表现卓越，且定价远低于专有替代方案。

hackernews · martinald · 7月6日 20:14 · [社区讨论](https://news.ycombinator.com/item?id=48809877)

**背景**: AI 模型需要大量资金进行训练和推理，市场一直由 OpenAI 等公司的专有模型主导。开源权重模型允许任何人低成本部署，加剧了竞争。文章认为，随着 GLM 5.2 等模型以更低成本达到或超越专有模型性能，整个行业的利润率将被压缩。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.z.ai/guides/llm/glm-5.2">GLM-5.2 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-is-glm-5-2-open-weight-model">What Is GLM 5.2? The Open-Weight Model Beating GPT 5.5 on Design Benchmarks | MindStudio</a></li>
<li><a href="https://unsloth.ai/docs/models/glm-5.2">GLM-5.2 - How to Run Locally | Unsloth Documentation</a></li>

</ul>
</details>

**社区讨论**: 评论者争论单纯的成本下降是否会导致利润率侵蚀，并举出云计算和办公套件等例子，说明尽管有更便宜的替代品，现有企业仍保持高利润率。一些人指出中国的竞争阻止了合谋，而另一些人则强调持续的训练成本是固定支出，可能使利润率保持微薄。

**标签**: `#AI`, `#GLM`, `#margin collapse`, `#LLM economics`, `#market competition`

---

<a id="item-4"></a>
## [微软 Xbox 重置凸显利润困境](https://news.xbox.com/en-us/2026/07/06/resetting-xbox/) ⭐️ 8.0/10

微软游戏部门正在进行战略“重置”，以解决利润率偏低的问题，尽管其季度营收达 50 亿美元，利润约为 1.5-1.6 亿美元。 此次重置反映了游戏行业更广泛的挑战：公司正从硬件销售转向 Game Pass 等订阅服务，这对开发者、消费者和投资者都将产生影响。 利润率被描述为“微薄且无增长”；微软正在精简业务以恢复增长。批评者指出其收购管理和 Game Pass 策略存在失误。

hackernews · dijksterhuis · 7月6日 14:18 · [社区讨论](https://news.ycombinator.com/item?id=48804993)

**背景**: Xbox 是微软的游戏品牌，与索尼的 PlayStation 和任天堂竞争。虽然 Xbox 营收很高，但利润率落后于竞争对手。Game Pass 订阅服务和重大收购（如动视暴雪）是其战略核心，但因成本不可持续而受到质疑。

**社区讨论**: 评论者表达了怀疑：有人指出微软规模庞大但利润率微薄；另一些人则归咎于企业文化和经营不善。评论还对比了任天堂在简单游戏上的成功以及索尼的“慢速死亡螺旋”。裁员和工作室关闭令人惋惜。

**标签**: `#Xbox`, `#Microsoft`, `#gaming`, `#business strategy`, `#industry analysis`

---

<a id="item-5"></a>
## [学习编程在 AI 时代仍具价值](https://stevekrouse.com/learn-to-code) ⭐️ 8.0/10

作者认为，尽管像大语言模型这样的 AI 工具不断进步，学习编程仍然是一项有价值的创造性和实用技能。 这场争论影响着有志于成为开发者的人和教育工作者，他们正在权衡是否要投入时间学习编程技能，因为担心 AI 会自动化编程工作。 社区评论指出，AI 目前能处理应用和仪表盘等外层开发，但深层的架构知识对于保证质量仍然至关重要。

hackernews · stevekrouse · 7月6日 20:59 · [社区讨论](https://news.ycombinator.com/item?id=48810439)

**背景**: 人们越来越担心 AI 语言模型能够生成代码，可能会减少对初级程序员的需求。然而，许多人认为理解基础知识仍然是引导 AI 和生成可靠软件所必需的。

**社区讨论**: 评论者表达了不同的观点；一些人将编程比作 AI 无法取代的创造性艺术，而另一些人则警告入门级编程岗位正在减少。一个反复出现的观点是，扎实的架构理解仍然至关重要，AI 常常被用来增强而不是取代熟练的开发者。

**标签**: `#AI`, `#coding`, `#career`, `#education`

---

<a id="item-6"></a>
## [新模型在实际任务中表现更差](https://devblogs.microsoft.com/blog/not-all-model-upgrades-are-upgrades) ⭐️ 8.0/10

微软在 150 个代理任务、15 个场景中测试了 Claude Sonnet 4.6 和 5，发现 Sonnet 5 虽然每 token 定价更低、基准得分更高，但实际使用了 12 倍的 token，输出质量反而更差。 这挑战了普遍认为新模型版本总是有益的假设。研究结果强调了在实际任务中评估模型的重要性，而非仅依赖基准测试，尤其对于成本敏感的 AI 部署而言。 该比较使用 GitHub Copilot 在 15 个场景的 150 个代理任务上进行。尽管 Sonnet 5 的每 token 价格更低，但 12 倍的 token 消耗导致总体成本更高且输出质量下降。

rss · Microsoft for Developers · 7月6日 07:49

**背景**: Claude Sonnet 是由 Anthropic 开发的大型语言模型系列，常用于 AI 辅助编程和代理任务。模型升级通常声称在标准基准测试上有所改进，但实际性能可能因 token 效率和输出相关性等因素而有所不同。微软的这项研究提供了此类差异的具体证据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-sonnet-4-6">Introducing Claude Sonnet 4.6 - Anthropic</a></li>
<li><a href="https://www.anthropic.com/news/claude-sonnet-5">Introducing Claude Sonnet 5 \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI models`, `#model evaluation`, `#cost efficiency`, `#AI agents`, `#practical AI`

---

<a id="item-7"></a>
## [Natvis 调试可视化功能登陆 Rider 的 Linux 和 macOS 版本](https://blog.jetbrains.com/dotnet/2026/07/06/natvis-comes-to-linux-and-macos-in-rider-2026-2-debugger/) ⭐️ 8.0/10

JetBrains Rider 2026.2 现在在 Linux 和 macOS 上支持 Natvis，允许开发者在调试器中可视化 C++ 类型，而无需编写自定义数据格式化程序。 这消除了在 Linux 或 macOS 上进行调试的 C++ 开发者的一个主要痛点，他们之前必须编写复杂的自定义格式化程序才能看到容器、字符串等类型的有用调试信息。 Natvis 是一个最初来自 Visual Studio 的框架，使用基于 XML 的架构来定义自定义视图；它在 Rider 中的支持现在扩展到非 Windows 平台，利用与 Windows 上相同的 .natvis 文件。

rss · JetBrains .NET Tools (Rider/ReSharper) · 7月6日 11:13

**背景**: Natvis 是一个调试器可视化框架，允许开发者在调试器变量窗口中创建原生类型的自定义表示。它以前仅通过 Visual Studio 在 Windows 上可用，但通过此次更新，JetBrains Rider 通过集成 GDB 和 LLDB 调试器，将其带到了 Linux 和 macOS 上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://code.visualstudio.com/docs/cpp/natvis">Natvis: Custom views for native objects - Visual Studio Code</a></li>
<li><a href="https://learn.microsoft.com/en-us/windows/apps/develop/cpp-winrt/natvis">Visual Studio native debug visualization (natvis) for C++/WinRT</a></li>

</ul>
</details>

**标签**: `#C++`, `#debugging`, `#Natvis`, `#Rider`, `#cross-platform`

---

<a id="item-8"></a>
## [PostgreSQL 20 增加后端级锁统计](https://postgr.es/p/9ow) ⭐️ 8.0/10

2026 年 6 月 30 日提交的一个补丁为 PostgreSQL 20 增加了后端级锁统计，提供与 pg_stat_lock 相同的信息（锁等待次数、等待时间和快速路径超限计数），且按后端划分。 这一增强使数据库管理员能够将锁争用定位到单个后端，从而实现更精确的性能诊断和并发工作负载调优，而此前只能在集群级别进行。 新统计信息可通过类似于现有后端级 IO 和 WAL 统计的函数获取。该补丁还包含快速路径超限计数，指示快速路径锁槽何时耗尽。

rss · Planet PostgreSQL · 7月6日 17:30

**背景**: PostgreSQL 使用锁来管理并发访问。pg_stat_lock 视图提供集群范围的锁统计信息，但缺少后端级粒度。快速路径锁定是一种降低轻量级锁开销的优化；当槽位耗尽时，系统会回退到重量级锁，从而增加争用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.depesz.com/2026/07/06/waiting-for-postgresql-20-add-backend-level-lock-statistics/">Waiting for PostgreSQL 20 – Add backend-level lock statistics</a></li>
<li><a href="https://www.postgresql.org/message-id/aiAzEY+cMQb/W8yu@bdtpg">PostgreSQL: Add per-backend lock statistics</a></li>
<li><a href="https://www.postgresql.org/docs/19/monitoring-stats.html">PostgreSQL: Documentation: 19: 27.2. The Cumulative Statistics ...</a></li>

</ul>
</details>

**社区讨论**: 社区成员指出，后端级统计允许测量单个后端在特定操作中的锁行为、比较会话前后的差异，并观察不同后端类型的锁特征。该补丁受到欢迎，因为它填补了监控能力的空白。

**标签**: `#PostgreSQL`, `#database`, `#monitoring`, `#locks`, `#performance`

---

<a id="item-9"></a>
## [PostgreSQL 14-16 最新小版本中的复制死锁漏洞](https://postgr.es/p/9os) ⭐️ 8.0/10

PostgreSQL 14.23、15.18 和 16.14 小版本引入了一个严重的复制死锁漏洞，在备用服务器或 PITR 实例进行 WAL 回放时会导致 MultiXactOffsetSLRU 死锁。 该漏洞可能导致流复制完全挂起，影响数据库可用性和复制稳定性，尤其对遵循先升级备库建议顺序的许多组织造成影响。 死锁仅在主库运行 2025 年 Q4 或更早小版本且备库运行最新小版本（14.23/15.18/16.14）时发生。临时解决方案包括回滚备库、应用 5 月 27 日的官方补丁，或等待计划于 8 月 13 日发布的下一小版本。

rss · Planet PostgreSQL · 7月6日 15:30

**背景**: PostgreSQL 使用预写式日志（WAL）进行崩溃恢复和复制。备库回放来自主库的 WAL 记录。MultiXactOffsetSLRU 是一个共享内存结构，用于跟踪行级锁中的多个事务 ID。该漏洞在特定版本组合下，当备库在回放期间尝试访问该结构时引入了自死锁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://stackoverflow.com/questions/76149827/what-could-cause-postgresql-to-suddenly-report-waiting-for-multixactoffsetslru-a">performance - What could cause Postgresql to suddenly report waiting for MultiXactOffsetSLRU and MultiXactOffsetBuffer for almost all active queries? - Stack Overflow</a></li>
<li><a href="https://www.postgresql.org/docs/current/wal-intro.html">PostgreSQL: Documentation: 18: 28.3. Write-Ahead Logging (WAL)</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#bug`, `#replication`, `#deadlock`, `#database`

---

<a id="item-10"></a>
## [PostgreSQL VACUUM 页级字节分析](https://postgr.es/p/9ol) ⭐️ 8.0/10

Radim Marek 发表了一篇关于 PostgreSQL VACUUM 页级操作的详细分析，使用 pageinspect、pg_visibility 和 pg_freespacemap 跟踪每个 VACUUM 阶段前后的字节级变化。 这篇对 VACUUM 内部机制的深入分析帮助数据库工程师理解精确的页级转换，从而更好地进行性能调优和排查 PostgreSQL 中死元组清理的问题。 该分析涵盖了页头、行指针、元组头、空闲空间映射和可见性映射的变化，展示了 VACUUM 与仅 HOT 修剪的区别，以及索引如何影响其行为。

rss · Planet PostgreSQL · 7月5日 14:31

**背景**: PostgreSQL 使用 MVCC，需要通过 VACUUM 删除死元组。HOT 更新可以在无需 VACUUM 的情况下回收空间，但仅适用于同一页面上非索引列的更新。完整 VACUUM 处理所有情况，包括索引清理和可见性映射更新。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/storage-hot.html">PostgreSQL: Documentation: 18: 66.7. Heap-Only Tuples (HOT)</a></li>
<li><a href="https://www.postgresql.org/docs/current/storage-page-layout.html">PostgreSQL : Documentation: 18: 66.6. Database Page Layout</a></li>
<li><a href="https://www.postgresql.org/docs/current/storage-vm.html">PostgreSQL: Documentation: 18: 66.4. Visibility Map</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database internals`, `#VACUUM`, `#page-level operations`, `#performance tuning`

---

<a id="item-11"></a>
## [腾讯发布 Hy3 MoE 模型，参数达 2950 亿](https://simonwillison.net/2026/Jul/6/hy3/#atom-everything) ⭐️ 8.0/10

腾讯发布了 Hy3，这是一个 2950 亿参数的混合专家（MoE）模型，活跃参数为 210 亿，采用 Apache 2.0 许可证。该模型性能优于同尺寸模型，并与参数规模大 2-5 倍的开源模型相竞争。 Hy3 展示了高效的 MoE 架构能够与更大的密集模型竞争，可能降低高质量 AI 部署的门槛。其 Apache 2.0 许可证以及在 OpenRouter 上截至 7 月 21 日的免费访问，使其广泛可及于开发者和研究人员。 完整模型在 Hugging Face 上为 598GB，FP8 量化版本为 300GB，支持 256K 上下文长度。该模型由腾讯 Hy 团队开发，并在后训练阶段整合了超过 50 个产品的反馈。

rss · Simon Willison · 7月6日 23:57

**背景**: 混合专家（MoE）是一种神经网络架构，每次输入只激活部分参数，从而减少计算量同时保持高容量。FP8 量化通过使用 8 位浮点数减小模型大小和内存需求，使得在有限硬件上的部署成为可能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/day-14-glam-googles-mixture-of-experts-model-efficient-durai-siujc">Day 14: GLaM – Google's Mixture - of - Experts Model for Efficient...</a></li>
<li><a href="https://arxiv.org/abs/2208.09225">[2208.09225] FP8 Quantization: The Power of the Exponent</a></li>
<li><a href="https://rcrtech.com/semiconductor-news/llms-quantization-fp8-fp4-int8/">LLMs and quantization: FP8, FP4, and INT8 explained</a></li>

</ul>
</details>

**标签**: `#AI/ML`, `#open-source`, `#large language model`, `#Mixture-of-Experts`, `#Tencent`

---

<a id="item-12"></a>
## [VS Code 与 OpenAI 通过 GPT-5.5 提示调优减少 Token 消耗](https://code.visualstudio.com/blogs/2026/07/06/optimizing-vscode-coding-harness-model-providers) ⭐️ 7.0/10

在为期两周的实验中，VS Code 与 OpenAI 优化了 GPT-5.5 的系统提示，减少了工具调用和尾端 token 消耗，从而加快了编辑响应速度。 这表明提示调优可以显著提升 AI 编程助手的效率，可能为在 IDE 中使用大型语言模型的开发者降低成本和延迟。 实验重点减少'尾端 token 消耗'，即响应末尾常不必要生成的 token，从而降低 API 成本并提升速度。

rss · Visual Studio Code · 7月6日 00:00

**背景**: 提示调优是一种参数高效的技术，通过调整输入提示使大型预训练模型适应新任务，而无需修改模型数十亿的参数。VS Code 的编程助手使用 GPT-5.5 帮助开发者编写和编辑代码。尾端 token 是模型输出末尾生成的 token，可能价值不大但会增加成本和延迟。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/artificial-intelligence/prompt-tuning/">What is Prompt Tuning? - GeeksforGeeks</a></li>
<li><a href="https://research.ibm.com/blog/what-is-ai-prompt-tuning">What is prompt-tuning? - IBM Research</a></li>
<li><a href="https://www.statsig.com/perspectives/sure-please-provide-the-title-or-main-topic-of-the-blog">Max tokens: Output length optimization</a></li>

</ul>
</details>

**标签**: `#prompt engineering`, `#GPT-5.5`, `#VS Code`, `#AI coding assistant`, `#performance optimization`

---

<a id="item-13"></a>
## [CloudNativePG 1.30：声明式角色与免密 TLS](https://postgr.es/p/9op) ⭐️ 7.0/10

CloudNativePG 1.30 引入了 DatabaseRole 自定义资源定义（CRD），用于声明式管理 PostgreSQL 角色。它还内置了 TLS 客户端证书签发功能，从而实现免密码连接。 这简化了在 Kubernetes 上运行 PostgreSQL 的应用团队的凭据管理，无需处理密码，并支持 GitOps 友好的工作流程。通过转向基于证书的身份验证，增强了安全性。 DatabaseRole CRD 与 Cluster 规范中现有的内联角色字段并行工作，并具有防止冲突的保护措施。TLS 证书签发利用操作员现有的证书基础设施自动生成客户端证书。

rss · Planet PostgreSQL · 7月6日 08:56

**背景**: CloudNativePG 是一个用于管理 PostgreSQL 集群的 Kubernetes 操作员。自定义资源定义（CRD）扩展了 Kubernetes，使其能够管理像 DatabaseRole 这样的自定义资源。PostgreSQL 中的免密码 TLS 身份验证使用 X.509 客户端证书：服务器通过受信任的 CA 验证客户端证书，而不是要求提供密码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/about/news/cloudnativepg-1300-released-3337/">CloudNativePG 1.30.0 Released! - PostgreSQL</a></li>
<li><a href="https://github.com/cloudnative-pg/cloudnative-pg/issues/5341">[Feature]: Declarative role management (`DatabaseRole` CRD ...</a></li>

</ul>
</details>

**标签**: `#CloudNativePG`, `#PostgreSQL`, `#Kubernetes`, `#TLS`, `#declarative`

---

<a id="item-14"></a>
## [PostgreSQL 中 .ready 和 .done 文件实用指南](https://postgr.es/p/9ox) ⭐️ 7.0/10

本文清晰解释了 PostgreSQL 的 .ready 和 .done 归档状态文件，阐明了它们在 WAL 归档中的作用以及关于复制问题的常见误解。 理解 .ready 和 .done 文件可以帮助数据库管理员和运维人员诊断 WAL 积累和存储问题，这是 PostgreSQL 环境中常见的运维挑战。 .ready 文件表示 WAL 段等待归档，而 .done 表示归档成功。WAL 段通常为 16 MB，归档在段完成时进行，而非按事务进行。

rss · Planet PostgreSQL · 7月6日 08:00

**背景**: PostgreSQL 使用预写日志（WAL）进行崩溃恢复和复制。archive_command 设置将完成的 WAL 段复制到远程位置。在 pg_wal/archive_status/ 目录中，标记文件跟踪每个段的归档状态。如果 archive_command 失败，.ready 文件会积累，导致磁盘增长。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/continuous-archiving.html">PostgreSQL: Documentation: 18: 25.3. Continuous Archiving and Point-in-Time Recovery (PITR)</a></li>
<li><a href="https://www.percona.com/blog/speed-up-of-the-wal-archiving-in-postgresql-15/">Speed Up of the WAL Archiving in PostgreSQL 15 - Percona</a></li>
<li><a href="https://www.opsdash.com/blog/postgresql-wal-archiving-backup.html">PostgreSQL WAL Archiving - OpsDash</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#WAL archiving`, `#database administration`, `#replication`

---

<a id="item-15"></a>
## [PostgreSQL 分区裁剪的两阶段执行](https://postgr.es/p/9on) ⭐️ 7.0/10

Christophe Pettus 解释了 PostgreSQL 的分区裁剪发生在两个阶段：计划时和执行时，并重点介绍了控制此行为的 enable_partition_pruning GUC 参数。 理解两阶段分区裁剪有助于数据库管理员和开发人员优化分区表上的查询性能，减少不必要的分区扫描，提高效率。 enable_partition_pruning 参数在 PostgreSQL 11 中引入，默认启用，控制计划时和执行时的裁剪；该文章提供了如何验证和调整此行为的实用见解。

rss · Planet PostgreSQL · 7月6日 01:00

**背景**: 分区裁剪是一种基于查询过滤器消除不必要分区扫描的优化。PostgreSQL 使用 Grand Unified Configuration (GUC) 系统管理数百个配置参数，包括 enable_partition_pruning。计划时裁剪在查询规划期间移除分区，而执行时裁剪在运行时参数（如绑定参数）已知时进一步消除分区。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/ddl-partitioning.html">PostgreSQL: Documentation: 18: 5.12. Table Partitioning</a></li>
<li><a href="https://www.enterprisedb.com/postgres-tutorials/partition-pruning-during-executionpartition-pruning-during-execution">Partition Pruning During ExecutionPartition Pruning During Execution | EDB</a></li>
<li><a href="https://postgresqlco.nf/doc/en/param/enable_partition_pruning/">PostgreSQL Documentation: enable_partition_pruning parameter</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#partition pruning`, `#database optimization`, `#query planning`

---