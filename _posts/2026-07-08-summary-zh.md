---
layout: default
title: "Horizon 日报：2026-07-08 (ZH)"
date: 2026-07-08
lang: zh
---

> 从 54 条内容中筛选出 18 条重要资讯。

---

1. [欧盟聊天控制：对加密和隐私的威胁](#item-1) ⭐️ 9.0/10
2. [微软裁掉 id Software 的 idTech 引擎团队](#item-2) ⭐️ 9.0/10
3. [Kokoro：CPU 友好、高质量文本转语音模型](#item-3) ⭐️ 8.0/10
4. [AI 工具发现 Cloudflare Circl 库漏洞](#item-4) ⭐️ 8.0/10
5. [Rider 中 Natvis 调试器可视化现已支持 Linux 和 macOS](#item-5) ⭐️ 8.0/10
6. [Postgres 14-16 复制死锁缺陷](#item-6) ⭐️ 8.0/10
7. [本地 LLM 用于编程的可行性分析](#item-7) ⭐️ 8.0/10
8. [sqlite-utils 4.0 新增数据库迁移、嵌套事务和复合外键支持](#item-8) ⭐️ 8.0/10
9. [腾讯发布 Hy3：295B MoE 模型，激活参数 21B](#item-9) ⭐️ 8.0/10
10. [Telerik 停用永久许可，转向纯订阅模式](#item-10) ⭐️ 8.0/10
11. [不要为了 AI 代理重写你的 CLI](#item-11) ⭐️ 7.0/10
12. [模型升级可能降低智能体任务性能](#item-12) ⭐️ 7.0/10
13. [pgBackRest TLS 传输用于 PostgreSQL 灾难恢复](#item-13) ⭐️ 7.0/10
14. [数据库中的不诚实基准测试](#item-14) ⭐️ 7.0/10
15. [PostgreSQL 20 添加强后端锁统计功能](#item-15) ⭐️ 7.0/10
16. [CloudNativePG 1.30 新增声明式角色和无密码 TLS](#item-16) ⭐️ 7.0/10
17. [解读 PostgreSQL WAL 的.ready 和.done 文件](#item-17) ⭐️ 7.0/10
18. [sqlite-utils 4.0rc3 增加复合外键支持](#item-18) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [欧盟聊天控制：对加密和隐私的威胁](https://fightchatcontrol.eu/chat-control-overview) ⭐️ 9.0/10

欧盟的聊天控制提案（1.0 和 2.0）旨在以打击儿童性虐待为名，强制大规模扫描私人信息（包括加密信息），威胁端到端加密。 如果获得通过，这些提案将破坏数百万欧盟公民的数字隐私和安全，为政府监控树立危险先例。这些提案引发了隐私倡导者和科技界的广泛反对。 聊天控制 1.0 允许自愿扫描私人信息，而聊天控制 2.0 将强制扫描，包括破坏端到端加密。关键机制包括客户端扫描，即在加密前扫描内容。

hackernews · gasull · 7月7日 14:23 · [社区讨论](https://news.ycombinator.com/item?id=48818311)

**背景**: 聊天控制是指欧盟一系列立法提案，旨在通过扫描私人通信来打击儿童性虐待材料（CSAM）。端到端加密（E2EE）确保只有发送者和接收者能读取消息；客户端扫描则会在用户设备上在加密前扫描消息，从而绕过 E2EE 保护。这些提案颇具争议，欧洲议会最近否决了最侵入性的措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Regulation_to_Prevent_and_Combat_Child_Sexual_Abuse">Chat Control - Wikipedia</a></li>
<li><a href="https://www.eff.org/deeplinks/2026/04/eu-parliament-blocks-mass-scanning-our-chats-whats-next">EU Parliament Blocks Mass-Scanning of Our Chats—What's Next? | Electronic Frontier Foundation</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了强烈反对，用户 mikaeluman 称其为‘授予我独裁权力’的玩法，arjie 指出对普通照片的隐私担忧。其他人则注意到欧盟声称保护隐私却推动监控的讽刺（Zufriedenheit），delichon 指出相关尝试禁止反对聊天控制的政党。

**标签**: `#privacy`, `#encryption`, `#surveillance`, `#EU policy`, `#chat control`

---

<a id="item-2"></a>
## [微软裁掉 id Software 的 idTech 引擎团队](https://gamefromscratch.com/microsoft-fire-idtech-team-at-id-software/) ⭐️ 9.0/10

微软裁掉了 id Software 整个 idTech 引擎开发团队，该团队是 idTech 游戏引擎系列的创造者。 此举可能加速行业对 Unreal Engine 的依赖，减少引擎多样性和创新。这也意味着游戏行业最具影响力的工作室之一失去了数十年的内部引擎专业知识。 裁员专门针对引擎团队，而非整个 id Software。idTech 曾为《毁灭战士》、《雷神之锤》和《德军总部》等标志性游戏提供动力，以其尖端图形技术闻名。

hackernews · bauc · 7月7日 15:33 · [社区讨论](https://news.ycombinator.com/item?id=48819244)

**背景**: idTech 是 id Software 开发的专有游戏引擎，最早可追溯到 1990 年代的 Quake 引擎。它经历了多个版本，包括 id Tech 5、6 和 7。微软于 2021 年收购了 id Software 的母公司 Zenimax Media，将 id Software 纳入 Xbox Game Studios 旗下。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Id_tech_5_engine">Id tech 5 engine</a></li>
<li><a href="https://en.wikipedia.org/wiki/Id_Tech">id Tech - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区表达了深深的失望，许多人称这是一个重大的企业失误，优先考虑短期成本节约而忽视长期创新。一些人指出，这种趋势可能导致游戏引擎的同质化和独特技术文化的丧失，而另一些人则指出，依赖 Unreal Engine 更容易雇佣廉价的承包商。

**标签**: `#game engines`, `#Microsoft`, `#idTech`, `#game development`, `#corporate strategy`

---

<a id="item-3"></a>
## [Kokoro：CPU 友好、高质量文本转语音模型](https://ariya.io/2026/03/local-cpu-friendly-high-quality-tts-text-to-speech-with-kokoro/) ⭐️ 8.0/10

Kokoro 是一个仅有 8200 万参数的开权重 TTS 模型，可在 CPU 上高效运行，无需 GPU 即可实现高质量语音合成。 这使得没有专用 GPU 的用户也能使用先进的 TTS，降低了无障碍工具、内容消费和注重隐私的本地处理的门槛。 Kokoro 支持手动 IPA 发音覆盖以处理同形异义词，但在孤立单词上可能表现不佳。该模型可在 GitHub 和 Hugging Face 上获取。

hackernews · speckx · 7月7日 18:24 · [社区讨论](https://news.ycombinator.com/item?id=48821576)

**背景**: 文本转语音（TTS）模型将书面文本转换为语音音频。许多高质量 TTS 模型需要强大的 GPU，限制了其使用。Kokoro 体积小且兼容 CPU，使其适用于更广泛的硬件，包括笔记本电脑和边缘设备。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://kokorottsai.com/">Kokoro TTS: Advanced AI Text-to-Speech Model with 82M parameters</a></li>
<li><a href="https://github.com/hexgrad/kokoro">GitHub - hexgrad/kokoro: https://hf.co/hexgrad/Kokoro-82M · GitHub</a></li>
<li><a href="https://huggingface.co/hexgrad/Kokoro-82M">hexgrad/Kokoro-82M · Hugging Face</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的用户反馈积极，尤其是在无障碍产品方面。他们赞赏其 CPU 效率和 IPA 支持，但也指出了对极短语的限制。一些人基于 Kokoro 构建了 Chrome 扩展或播客流水线。

**标签**: `#TTS`, `#AI`, `#open source`, `#accessibility`, `#CPU`

---

<a id="item-4"></a>
## [AI 工具发现 Cloudflare Circl 库漏洞](https://blog.zksecurity.xyz/posts/circl-bugs/) ⭐️ 8.0/10

研究人员利用大型语言模型（LLM）在 Cloudflare 的 Circl 加密库中发现了七个漏洞，展示了 AI 在安全审计中的实际应用。 这项工作表明，AI 可以帮助发现现实世界中的加密漏洞，从而可能降低安全审计的成本并提高效率。它可能鼓励在关键安全库中更广泛地采用 AI 辅助代码审查。 AI 生成的候选发现数量众多，但需要人工在环路中进行验证，才能产生关于七个真正漏洞的可信报告。这些漏洞包括 CP-ABE 中的访问控制破坏以及加密算法中意外使用浮点运算。

hackernews · duha · 7月7日 18:36 · [社区讨论](https://news.ycombinator.com/item?id=48821749)

**背景**: Cloudflare Circl 是一个用 Go 编写的开源加密库，旨在用于后量子密码学和椭圆曲线密码学的实验性部署。传统上，加密库中的漏洞发现依赖于人工代码审查和静态分析，这可能耗时且可能遗漏细微缺陷。将 LLM 用于此类任务是一种新兴方法，利用模型理解代码和检测异常的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/cloudflare/circl">GitHub - cloudflare/circl: CIRCL: Cloudflare Interoperable Reusable Cryptographic Library · GitHub</a></li>
<li><a href="https://blog.cloudflare.com/introducing-circl/">Introducing CIRCL: An Advanced Cryptographic Library</a></li>
<li><a href="https://pkg.go.dev/github.com/cloudflare/circl">circl package - github.com/cloudflare/circl - Go Packages</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞这项工作避免了花哨的营销名称，并要求更深入的技术见解，例如 AI 候选报告与真正漏洞的比例。一位评论者对在加密算法中使用浮点运算表示惊讶，并提到了历史上使用 FPU 进行奇怪整数操作的先例。

**标签**: `#AI`, `#cryptography`, `#vulnerability discovery`, `#Cloudflare`, `#LLM`

---

<a id="item-5"></a>
## [Rider 中 Natvis 调试器可视化现已支持 Linux 和 macOS](https://blog.jetbrains.com/dotnet/2026/07/06/natvis-comes-to-linux-and-macos-in-rider-2026-2-debugger/) ⭐️ 8.0/10

JetBrains 宣布 Rider 2026.2 将 Natvis 自定义可视化功能引入 Linux 和 macOS，使开发者能够使用之前仅在 Windows 上 MSVC 工具链中可用的 .natvis 文件。 此举消除了在 Linux 和 macOS 上编写手动数据格式化程序的需要，跨平台节省了大量开发时间并降低了复杂性。 与 Windows 上 MSVC 配合使用的相同 .natvis XML 文件，现在在 Linux 和 macOS 上使用 Rider 调试时无需修改即可工作。该功能是 Rider 2026.2 EAP 的一部分，并在这两个平台上使用 LLDB 调试器。

rss · JetBrains .NET Tools (Rider/ReSharper) · 7月6日 11:13

**背景**: Natvis 是一个框架，允许开发者在调试器变量窗口中定义原生 C++ 类型的自定义可视化。此前，Natvis 仅适用于 Windows 上的 MSVC 工具链，导致 Linux 和 macOS 用户依赖复杂的手写数据格式化程序来获得可读的调试输出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.jetbrains.com/dotnet/2026/07/06/natvis-comes-to-linux-and-macos-in-rider-2026-2-debugger/">Natvis Comes to Linux and macOS: Visualize Your C++ Types Without Writing a Single Data Formatter - The JetBrains Blog</a></li>
<li><a href="https://code.visualstudio.com/docs/cpp/natvis">Natvis: Custom views for native objects</a></li>

</ul>
</details>

**标签**: `#C++`, `#debugging`, `#JetBrains Rider`, `#Natvis`, `#cross-platform`

---

<a id="item-6"></a>
## [Postgres 14-16 复制死锁缺陷](https://postgr.es/p/9os) ⭐️ 8.0/10

PostgreSQL 14.23、15.18 和 16.14 次要版本引入了一个回归缺陷，导致在 WAL 重放期间出现 MultiXactOffsetSLRU 死锁，影响流复制和基于时间点恢复。 该缺陷至关重要，因为它会导致备用服务器或 PITR 实例挂起，而且推荐的更新流程（先更新备用节点）增加了遇到该问题的可能性，可能对补丁更新滞后的组织的数据库操作造成中断。 当备用节点（运行最新次要版本）重放由较旧主节点（例如 14.20/15.15/16.11）生成的 WAL 时会发生死锁。启动进程挂起，等待事件为 LWLock/MultiXactOffsetSLRU。受影响的版本为 14-16；版本 17、18 及更早版本不受影响。

rss · Planet PostgreSQL · 7月6日 15:30

**背景**: PostgreSQL 使用预写日志 (WAL) 进行复制和崩溃恢复。MultiXactOffsetSLRU 是用于管理多事务偏移量的共享内存结构；此处的死锁会阻塞 WAL 重放。次要版本是包含缺陷修复和安全补丁的点版本；版本 14-16 的最新版本于 2025 年 5 月 14 日发布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://stackoverflow.com/questions/76149827/what-could-cause-postgresql-to-suddenly-report-waiting-for-multixactoffsetslru-a">performance - What could cause Postgresql to suddenly report waiting for MultiXactOffsetSLRU and MultiXactOffsetBuffer for almost all active queries? - Stack Overflow</a></li>
<li><a href="https://www.postgresql.org/message-id/CAFiTN-vzDvNz=ExGXz6gdyjtzGixKSqs0mKHMmaQ8sOSEFZ33A@mail.gmail.com">PostgreSQL: SLRU optimization - configurable buffer pool and partitioning the SLRU lock</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database`, `#bug`, `#replication`, `#deadlock`

---

<a id="item-7"></a>
## [本地 LLM 用于编程的可行性分析](https://martinfowler.com/articles/exploring-gen-ai/local-models-for-coding-factors.html) ⭐️ 8.0/10

Birgitta Böckeler 在 Martin Fowler 的网站上发布了一份备忘录，详细说明了影响本地大型语言模型在编程任务中可行性的关键因素。 这项分析帮助软件工程师评估何时使用本地 LLM 而非云 API，考虑到隐私、成本、延迟和控制权等权衡因素，随着本地模型的改进，这一点日益重要。 讨论的因素包括模型大小、硬件限制（GPU 内存、带宽）、推理速度、代码准确性以及对多种编程语言的支持，这些都影响实际可用性。

rss · Martin Fowler · 7月7日 12:34

**背景**: 大型语言模型（LLM）可以在用户硬件上本地运行，或通过云 API 访问。本地部署提供隐私和离线能力，但通常需要强大的 GPU 且推理速度较慢；云 API 则提供更快的响应，但有成本且数据离开用户控制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://apxml.com/courses/getting-started-local-llms/chapter-1-introduction-large-language-models/local-vs-cloud-llms">Local vs. Cloud-Based LLMs</a></li>
<li><a href="https://dasroot.net/posts/2026/01/local-llm-for-code-generation-best/">Local LLM for Code Generation: Best Practices and Limitations · Technical news about AI, coding and all</a></li>
<li><a href="https://inventivehq.com/blog/local-llm-performance-what-to-expect">Local LLM Performance: What Tokens-Per-Second to Expect From Your Hardware</a></li>

</ul>
</details>

**标签**: `#local LLMs`, `#coding`, `#AI-assisted programming`, `#software engineering`

---

<a id="item-8"></a>
## [sqlite-utils 4.0 新增数据库迁移、嵌套事务和复合外键支持](https://simonwillison.net/2026/Jul/7/sqlite-utils-4/#atom-everything) ⭐️ 8.0/10

sqlite-utils 4.0 发布了三大新特性：使用 Python 迁移文件进行数据库模式迁移、通过新的 db.atomic() 方法实现嵌套事务、以及对复合外键的支持。此版本还包含破坏性变更和升级指南。 这是自 2020 年以来的首次主版本升级，为一个广受欢迎的 Python SQLite 工具带来了关键的数据库管理功能，使开发者能够直接在 Python 中处理模式演进和高级事务。这简化了使用 SQLite 数据库的数据工程师和 Python 开发者的工作流程。 迁移通过 Migrations 类定义，并利用 table.transform() 方法，该方法实现了 SQLite 推荐的创建新表、复制数据并重命名的模式。嵌套事务使用 SQLite 保存点，允许内部事务独立回滚。复合外键支持引用复合主键。

rss · Simon Willison · 7月7日 19:32

**背景**: SQLite 是一个轻量级嵌入式数据库，但其 ALTER TABLE 命令功能有限——无法轻松删除列或更改列类型。推荐的解决方案是创建具有所需模式的新表、复制数据并重命名。sqlite-utils 自动化了这一模式。SQLite 通过保存点支持嵌套事务，允许一个事务包含可独立回滚的子事务。复合外键允许外键引用父表复合主键的多个列。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sqlite.org/foreignkeys.html">SQLite Foreign Key Support</a></li>
<li><a href="https://learn.microsoft.com/en-us/dotnet/standard/data/sqlite/transactions">Transactions - Microsoft.Data.Sqlite | Microsoft Learn</a></li>

</ul>
</details>

**标签**: `#sqlite`, `#python`, `#database`, `#migrations`, `#open-source`

---

<a id="item-9"></a>
## [腾讯发布 Hy3：295B MoE 模型，激活参数 21B](https://simonwillison.net/2026/Jul/6/hy3/#atom-everything) ⭐️ 8.0/10

腾讯发布了 Hy3，这是一个 2950 亿参数的混合专家（MoE）模型，激活参数为 210 亿，采用 Apache 2.0 许可证。该模型性能优于同类尺寸模型，并可媲美参数规模大 2-5 倍的旗舰模型。 此次发布以宽松许可提供了极具竞争力的模型，强化了开源 AI 生态，使更多用户能获得最先进的能力。这也突显了腾讯在全球大语言模型领域日益增长的影响力，以及 MoE 架构在平衡性能与效率方面的有效性。 完整模型权重在 Hugging Face 上为 598 GB，FP8 量化版本为 300 GB，上下文长度为 256K tokens。在 OpenRouter 上可免费使用至 2026 年 7 月 21 日。

rss · Simon Willison · 7月6日 23:57

**背景**: Hy3 采用混合专家（MoE）架构，每个 token 仅使用部分（激活）参数，从而以较低计算成本实现高总容量。它还引入了多 token 预测（MTP）技术，即模型同时预测多个未来 token，以加速推理。FP8 量化通过将权重存储为 8 位浮点格式来减少内存占用，从而能在更少 GPU 上部署且精度损失极小。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.nvidia.com/nemo/megatron-bridge/latest/training/multi-token-prediction.html">Multi-Token Prediction (MTP) — Megatron Bridge</a></li>
<li><a href="https://www.spheron.network/blog/fp8-quantization-inference-performance-hardware-explained/">What is FP8 Quantization? AI Inference Performance, Accuracy, and Hardware Support Explained (2026) | Spheron Blog</a></li>
<li><a href="https://www.f22labs.com/blogs/active-vs-total-parameters-whats-the-difference/">Active vs Total Parameters: What’s the Difference?</a></li>

</ul>
</details>

**标签**: `#AI`, `#machine learning`, `#open-source`, `#large language model`, `#MoE`

---

<a id="item-10"></a>
## [Telerik 停用永久许可，转向纯订阅模式](https://www.reddit.com/r/dotnet/comments/1uq5vq9/telerik_discontinued_perpetual_licensing/) ⭐️ 8.0/10

Telerik 已停止提供永久许可选项，所有新购买将改为纯订阅模式。 这一转变影响了许多依赖 Telerik UI 组件的 .NET 开发者，可能增加长期成本并改变购买决策。 现有永久许可持有者不受影响，但未来升级和新客户必须使用订阅模式。

reddit · r/dotnet · /u/MrZander · 7月7日 19:47

**背景**: 永久许可允许客户一次性付费并无限期使用软件，而订阅模式需要定期付款。Telerik 是 .NET UI 组件库的主要提供商，这一变化顺应了行业向订阅制定价的趋势。

**标签**: `#.NET`, `#Telerik`, `#licensing`, `#software-as-a-service`, `#component libraries`

---

<a id="item-11"></a>
## [不要为了 AI 代理重写你的 CLI](https://devblogs.microsoft.com/blog/dont-rewrite-your-cli-for-agents) ⭐️ 7.0/10

微软开发者博客反对当前流行的建议——将 CLI 的平展参数替换为单一的--json 负载以适配 AI 代理，文章指出了其中的权衡并提出了更好的方法，如结构化输出和幂等命令。 这很重要，因为许多开发者被敦促重新设计他们的 CLI 以适应 AI 代理，但这可能破坏现有工作流并增加复杂性而收益不明确；该文章提供了细致的视角，帮助开发者做出明智决策。 文章认为，采用如重复标志等约定的平展参数实际上能很好地适用于代理，而将其替换为 JSON blob 会丧失可发现性和 shell 兼容性；它建议保留标准 CLI 模式，同时增加结构化输出（如--json 输出）和幂等命令。

rss · Microsoft for Developers · 7月7日 13:52

**背景**: CLI（命令行界面）传统上使用平展参数（如--name value），便于人类和脚本解析。然而，AI 代理通常更擅长处理结构化数据（如 JSON）。一些人主张改用单一的--json 参数来简化代理工具的使用。这篇文章质疑了该建议，指出了其权衡，例如丢失 shell 自动补全和增加解析复杂性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dev.to/uenyioha/writing-cli-tools-that-ai-agents-actually-want-to-use-39no">Writing CLI Tools That AI Agents Actually Want to Use - DEV Community</a></li>
<li><a href="https://joelclaw.com/cli-design-for-ai-agents">CLI Design for AI Agents — JoelClaw</a></li>
<li><a href="https://www.firecrawl.dev/blog/best-cli-tools">Best CLI Tools for Your AI Agents in 2026</a></li>

</ul>
</details>

**标签**: `#CLI`, `#AI Agents`, `#JSON`, `#Developer Tools`, `#Microsoft`

---

<a id="item-12"></a>
## [模型升级可能降低智能体任务性能](https://devblogs.microsoft.com/blog/not-all-model-upgrades-are-upgrades) ⭐️ 7.0/10

微软在 15 个场景下对 Claude Sonnet 4.6 和 Sonnet 5 进行了 150 项智能体任务测试，发现 Sonnet 5 的 token 消耗最高增加了 12 倍，同时输出质量下降，与其更好的基准测试结果相矛盾。 这一发现挑战了“基准分数更高的新模型总是更适合实际智能体工作流”的假设。开发者在升级时可能面临意外的成本增加和质量下降，凸显了针对具体任务进行评估的必要性。 Sonnet 5 使用了新的分词器，相同文本的 token 数量是 Sonnet 4.6 的 1.0 到 1.35 倍，其更高的“努力”参数会在推理上消耗更多 token，导致成本增加且输出质量不稳定。

rss · Microsoft for Developers · 7月6日 07:49

**背景**: LLM 基准测试通常评估单轮任务的准确性（如问答或摘要），但智能体任务需要多步推理、工具调用和计划执行。模型更新可能以不可预见的方式改变分词、行为或输出格式，从而降低这些复杂工作流的性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://emergent.sh/learn/claude-sonnet-4-6-vs-sonnet-5">Sonnet 4.6 vs Sonnet 5: Should You Upgrade?</a></li>
<li><a href="https://www.reddit.com/r/ClaudeAI/comments/1uloomx/claude_sonnet_5_vs_46_on_arenaai/">r/ClaudeAI on Reddit: Claude Sonnet 5 vs 4.6 on arena.ai</a></li>
<li><a href="https://www.labellerr.com/blog/claude-sonnet-5-vs-sonnet-4-6/">Claude Sonnet 5 vs Sonnet 4.6: Performance, Cost & Features</a></li>

</ul>
</details>

**社区讨论**: 在 Reddit 上，用户指出尽管 Anthropic 宣传 Sonnet 5 的每 token 价格相同，但 token 数量的增加使其每次查询的实际成本高出 35%。还有人指出，更高的“努力”参数可能导致模型循环或产生冗长、不必要的步骤。

**标签**: `#AI models`, `#LLM evaluation`, `#agent performance`, `#model selection`, `#Microsoft`

---

<a id="item-13"></a>
## [pgBackRest TLS 传输用于 PostgreSQL 灾难恢复](https://postgr.es/p/9oD) ⭐️ 7.0/10

这篇博客文章解释了 pgBackRest 的原生 TLS 传输模式如何为 PostgreSQL 灾难恢复提供证书认证的恢复和严格的安全隔离，为大规模部署提供了一个比 SSH 更简洁的替代方案。 这一点很重要，因为随着 PostgreSQL 部署规模扩大，管理 SSH 密钥变得复杂，并且如果 DR 服务器被攻破，存在横向移动的安全风险。使用 TLS 通过消除 shell 访问并集中管理证书来减少攻击面。 pgBackRest 的 TLS 模式使用由证书颁发机构签名的 X.509 证书，DR 服务器只需持有一个证书，该证书向监听 8432 端口的专用 TLS 守护进程进行身份验证，该守护进程仅理解 pgBackRest 协议。即使 DR 服务器完全被攻破，也能防止 shell 访问。

rss · Planet PostgreSQL · 7月7日 15:41

**背景**: pgBackRest 是 PostgreSQL 流行的备份和恢复工具。在典型设置中，它使用 SSH 在备份节点和 DR 服务器之间进行通信，需要无密码的 SSH 密钥对。随着服务器数量增加，管理 SSH 密钥变得繁琐且不安全，因为存在横向移动的风险。

**标签**: `#PostgreSQL`, `#pgBackRest`, `#disaster recovery`, `#TLS`, `#security`

---

<a id="item-14"></a>
## [数据库中的不诚实基准测试](https://postgr.es/p/9p0) ⭐️ 7.0/10

Mayur B. 发表了一篇文章，详细介绍了 Wisconsin Benchmark 和 DeWitt 条款的历史，并警告说现代数据库供应商使用不诚实的基准测试策略，使其产品看起来比竞争对手快得多。 这很重要，因为误导性的基准测试可能欺骗从业者选择劣质的数据库解决方案，从而破坏对整个数据库生态系统的信任。文章呼吁回归公开的基准测试批评，而不是法律压制。 常见的不诚实策略包括对自己的数据库进行过度调优而将对比数据库保持在默认设置、选择有利于供应商架构的工作负载，以及忽略成本、尾部延迟和操作复杂性等因素。

rss · Planet PostgreSQL · 7月7日 07:21

**背景**: Wisconsin Benchmark 是 20 世纪 80 年代初由威斯康星大学的 David DeWitt 创建的一项开创性数据库性能测试。Oracle 的 Larry Ellison 因糟糕的基准测试结果而愤怒，据称他要求解雇 DeWitt，这导致了 DeWitt 条款——一项限制未经供应商批准发布基准测试结果的许可证条款。随着时间的推移，类似的条款抑制了独立的基准测试，将斗争从公开的技术辩论转变为法律控制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeWitt_Clause">DeWitt Clause</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#benchmarking`, `#database`, `#performance`, `#ethics`

---

<a id="item-15"></a>
## [PostgreSQL 20 添加强后端锁统计功能](https://postgr.es/p/9ow) ⭐️ 7.0/10

PostgreSQL 20 引入了一项新功能，提供每个后端的锁统计信息，包括锁等待次数、等待时间和快速路径超限计数。 此功能大大增强了数据库管理员和系统工程师的性能监控和调试能力，使他们能够在后端级别细粒度地观察锁争用情况。 该补丁于 2026 年 6 月 30 日由 Michael Paquier 提交，提供了与 pg_stat_lock 相同的信息，但基于每个后端。

rss · Planet PostgreSQL · 7月6日 17:30

**背景**: PostgreSQL 使用锁来管理对数据的并发访问。以前，锁统计信息是全局聚合的；此更新允许按后端跟踪，这对于诊断性能瓶颈非常有价值。

**标签**: `#PostgreSQL`, `#database`, `#lock statistics`, `#backend`, `#performance`

---

<a id="item-16"></a>
## [CloudNativePG 1.30 新增声明式角色和无密码 TLS](https://postgr.es/p/9op) ⭐️ 7.0/10

CloudNativePG 1.30 引入了 DatabaseRole 自定义资源定义（CRD）和内置 TLS 客户端证书颁发，使得在 Kubernetes 上的 PostgreSQL 能够实现声明式角色管理和无密码连接。 此更新简化了应用团队的数据库凭证管理，允许他们以声明方式拥有 PostgreSQL 角色而无需处理密码，增强了 Kubernetes 原生环境中的安全性和运维效率。 DatabaseRole CRD 允许直接在 Kubernetes 清单中定义角色及其权限，而内置的 TLS 证书颁发则自动生成客户端证书以实现无密码认证。

rss · Planet PostgreSQL · 7月6日 08:56

**背景**: CloudNativePG 是一个用于 PostgreSQL 的 Kubernetes 运算符，在 CNCF 旗下开发。它管理 Kubernetes 上的 PostgreSQL 集群，此版本将其声明式方法扩展到角色管理和 TLS 安全。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cloud_Native_Computing_Foundation">Cloud Native Computing Foundation</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#CloudNativePG`, `#Kubernetes`, `#TLS`, `#database`

---

<a id="item-17"></a>
## [解读 PostgreSQL WAL 的.ready 和.done 文件](https://postgr.es/p/9ox) ⭐️ 7.0/10

本文提供了关于 PostgreSQL WAL 归档中.ready 和.done 标记文件的实用指南，解释了它们指示 WAL 段归档状态的含义以及段可能积累的原因。 这很重要，因为对.ready 文件的误解可能导致对复制健康状况的不必要警报；理解这些标记有助于 DBA 正确诊断归档问题并管理磁盘使用。 文章详细说明.ready 文件标记待归档的 WAL 段，.done 文件标记成功归档的段。它解释了 archive_command 过程，包括 Postgres 在非零退出码时重试。

rss · Planet PostgreSQL · 7月6日 08:00

**背景**: 在 PostgreSQL 中，WAL（预写日志）段被归档以确保时间点恢复和复制。archive_command 被配置为复制已完成的段。pg_wal/archive_status/目录包含.ready 和.done 文件以跟踪归档状态。.ready 表示段已准备好被归档，.done 表示已成功归档。

**标签**: `#PostgreSQL`, `#WAL`, `#database administration`, `#archiving`, `#replication`

---

<a id="item-18"></a>
## [sqlite-utils 4.0rc3 增加复合外键支持](https://simonwillison.net/2026/Jul/6/sqlite-utils/#atom-everything) ⭐️ 7.0/10

sqlite-utils 4.0rc3 引入了对复合外键的检查和创建支持，并遵循 SQLite 对不区分大小写列名的约定。自 rc2 以来，作者在处理问题和 PR 的过程中，变更日志显著增加。 复合外键是长期请求的功能，可以在 SQLite 数据库中实现更复杂的关系完整性约束，使使用 sqlite-utils 进行数据转换和模式管理的开发者受益。此版本还使 sqlite-utils 与 SQLite 不区分大小写的列匹配行为保持一致，减少了潜在的不一致性。 新的复合外键支持涉及对 table.foreign_keys 属性的细微破坏性变更，因此必须引入 4.0 稳定版。不区分大小写的列匹配更新同时影响了代码库的多个部分。

rss · Simon Willison · 7月6日 05:40

**背景**: sqlite-utils 是由 Simon Willison 创建的 Python 命令行工具和库，用于简化 SQLite 数据库操作。它允许用户轻松地在 SQLite 数据库中插入、查询和转换数据。复合外键允许一个外键约束跨越多个列，这对于规范化数据库模式至关重要。不区分大小写的列匹配确保 SQL 查询不区分列名大小写，以匹配 SQLite 的默认行为。

**标签**: `#sqlite-utils`, `#sqlite`, `#release-candidate`, `#databases`

---