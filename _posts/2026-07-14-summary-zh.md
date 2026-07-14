---
layout: default
title: "Horizon 日报：2026-07-14 (ZH)"
date: 2026-07-14
lang: zh
---

> 从 38 条内容中筛选出 9 条重要资讯。

---

1. [苹果 SpeechAnalyzer API 与 Whisper 及前代对比测试](#item-1) ⭐️ 8.0/10
2. [Telegram 的 t.me 域名被暂停](#item-2) ⭐️ 8.0/10
3. [前 NOAA 员工推出 Climate.us 以保护公共气候数据](#item-3) ⭐️ 8.0/10
4. [Samsung 健康：退出 AI 训练则删除数据](#item-4) ⭐️ 8.0/10
5. [RegreSQL 2.0：测试查询计划，而不仅仅是数据行](#item-5) ⭐️ 8.0/10
6. [首个纯.NET 的 F5-TTS 语音克隆运行器](#item-6) ⭐️ 8.0/10
7. [JetBrains 为 VS Code 和 Cursor 的 ReSharper 扩展添加调试功能](#item-7) ⭐️ 7.0/10
8. [Datasette 代码频率图展示 AI 编码影响](#item-8) ⭐️ 7.0/10
9. [Simon Willison 认为 LLM 代理不应成为直接责任人](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [苹果 SpeechAnalyzer API 与 Whisper 及前代对比测试](https://get-inscribe.com/blog/apple-speech-api-benchmark.html) ⭐️ 8.0/10

苹果在 iOS 26 和 macOS 26 中推出了 SpeechAnalyzer 和 SpeechTranscriber API，取代了旧的 SFSpeechRecognizer。第三方基准测试将 SpeechAnalyzer 与 OpenAI 的 Whisper 进行了比较，结果显示其在速度和准确性上具有竞争力。 这一进展可能改变语音识别格局，为苹果开发者提供一个原生、可能更高效的设备端转录选项。同时，它也对基于 Whisper 的第三方服务构成挑战，可能使部分付费封装应用过时。 基准测试显示，SpeechAnalyzer 缺少其前代产品中的自定义词汇功能，这可能影响对专业术语的准确性。此外，社区评论指出 Whisper 已不再是顶尖模型，像 Voxtral 和 Parakeet 等模型取得了更低的错误率。

hackernews · get-inscribe · 7月13日 16:06 · [社区讨论](https://news.ycombinator.com/item?id=48894752)

**背景**: 语音识别（ASR）将音频转换为文本。OpenAI 于 2022 年发布的 Whisper 是一个广泛使用的开源模型，基于 68 万小时数据训练。苹果之前的 API SFSpeechRecognizer 在 iOS 10 中推出。新的 SpeechAnalyzer 是苹果推动设备端 AI 处理的一部分，旨在提升隐私和降低延迟。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer-mdn.apple.com/videos/play/wwdc2025/277/">Bring advanced speech -to-text to your app with... - Apple Developer</a></li>
<li><a href="https://get-inscribe.com/blog/apple-speech-api-benchmark.html">Apple 's New Speech API vs Whisper: The First Real Benchmark</a></li>
<li><a href="https://en.wikipedia.org/wiki/Whisper_(speech_recognition_system)">Whisper ( speech recognition system) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者认为苹果的原生 API 可能使付费的 Whisper 封装应用过时，并指出 Whisper 并非最佳基准；Mistral 的 Voxtral 和 Nvidia 的 Parakeet 等模型更准确。一名用户发现 SpeechAnalyzer 在数学讲座中比 Whisper 更快但略逊准确性，另一名用户则称赞 Voxtral 在技术会议中具有极低的缩略词错误率。

**标签**: `#speech recognition`, `#Apple`, `#benchmarking`, `#ASR`, `#Whisper`

---

<a id="item-2"></a>
## [Telegram 的 t.me 域名被暂停](https://www.whois.com/whois/t.me) ⭐️ 8.0/10

Telegram 的短链接域名 t.me 已被暂停，Whois 数据显示多个 ICANN EPP 状态码。 这一中断影响了数百万依赖 t.me 链接访问 Telegram 频道和内容的用户，并凸显了注册商和域名治理在平台运营中的权力。 该域名的状态包括 clientRenewProhibited 和 serverDeleteProhibited，这些通常在法律纠纷期间或待删除时应用，注册商是 GoDaddy，以其不透明著称。

hackernews · Tiberium · 7月13日 19:52 · [社区讨论](https://news.ycombinator.com/item?id=48897878)

**背景**: 域名暂停发生在注册商或注册管理机构因法律、监管或政策违规而锁定域名时。ICANN 设定了标准化的 EPP 状态代码，指示域名的状态，例如禁止续费或删除。Telegram 在俄罗斯、法国和印度受到法律审查，这可能导致该暂停。

**社区讨论**: 用户表达了不满，有人指出他们使用重定向来避免直接使用 t.me 链接，并批评 Telegram 依赖 GoDaddy 作为注册商。其他人则认为这是将社区从 Telegram 转移到 Zulip 等替代方案的理由。

**标签**: `#Telegram`, `#domain suspension`, `#ICANN`, `#GoDaddy`, `#legal investigations`

---

<a id="item-3"></a>
## [前 NOAA 员工推出 Climate.us 以保护公共气候数据](https://19thnews.org/2026/07/noaa-climate-data-website/) ⭐️ 8.0/10

前 NOAA 员工推出了非营利网站 Climate.us，以在 NOAA 的 Climate.gov 于 2025 年 6 月关闭后保存并继续提供公共气候数据。 这确保了在数据完整性面临政治威胁时，公众仍能继续获取联邦资助的气候信息，并凸显了公民科技在保护开放数据方面的作用。 Climate.us 由创建 Climate.gov 的团队构建，依靠捐赠维持运营，填补了 NOAA 气候平台全职员工被解雇后留下的空白。

hackernews · benwerd · 7月13日 19:57 · [社区讨论](https://news.ycombinator.com/item?id=48897945)

**背景**: NOAA 的 Climate.gov 近 15 年来一直是美国政府面向公众的首要气候信息平台，但其全职员工在 2025 年初被解雇，网站于 2025 年 6 月停运。这引发了对公共资助气候数据保存的担忧，促使前员工创建了独立的替代站点 Climate.us。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.climate.us/about">About Climate.us</a></li>
<li><a href="https://multiplier.org/project/climate-us/">Climate.us - Multiplier</a></li>

</ul>
</details>

**社区讨论**: 评论者对数据保护工作表示支持，但也对资金可持续性和实时数据更新的必要性表示担忧。有人建议对政府内容使用 IPFS 等去中心化存档，另一些人则提到了类似的先例，如澳大利亚的气候委员会。

**标签**: `#climate data`, `#data preservation`, `#open data`, `#government data`, `#NOAA`

---

<a id="item-4"></a>
## [Samsung 健康：退出 AI 训练则删除数据](https://neow.in/cWsyMTV3) ⭐️ 8.0/10

Samsung Health 更新了政策，要求用户同意将其健康数据用于 AI 训练；选择退出者的数据将被从服务中删除。 这项政策强迫用户在失去健康数据或允许将其用于 AI 训练之间做出胁迫性选择，引发了关于健康科技领域隐私、同意和数据所有权的严重担忧。 涉及的数据类别包括睡眠、用药、医疗记录和周期追踪详情。该政策影响 Samsung Health 应用用户，可能波及 Galaxy Watch 及其他三星设备用户。

hackernews · bundie · 7月13日 20:01 · [社区讨论](https://news.ycombinator.com/item?id=48897991)

**背景**: 许多健康应用收集敏感数据，但通常允许用户在不删除数据的情况下退出。三星的做法异常胁迫，将数据保留与 AI 训练同意挂钩。GDPR 等隐私法规要求明确同意，可能对此类做法提出挑战。

**社区讨论**: 评论者表达了不满，有人指出拒绝同意反而导致数据被删除的讽刺性。其他人称赞 Sparky Fitness 等本地替代方案能保护数据隐私。还有人质疑这种胁迫性政策的道德性。

**标签**: `#privacy`, `#AI training`, `#health data`, `#Samsung`, `#data ethics`

---

<a id="item-5"></a>
## [RegreSQL 2.0：测试查询计划，而不仅仅是数据行](https://postgr.es/p/9pn) ⭐️ 8.0/10

RegreSQL 2.0 通过将查询执行计划与生产统计信息进行比较，增强了回归测试能力，能够捕获基于行的测试无法发现的性能退化。 这解决了 PostgreSQL 中一个常见而微妙的性能退化问题：查询返回正确结果但使用了低效的执行计划，可能导致生产环境故障。 该工具比较来自生产统计信息的缓冲区使用量和成本估算，标记诸如从索引扫描变为顺序扫描等变化。

rss · Planet PostgreSQL · 7月12日 18:16

**背景**: PostgreSQL 使用查询计划器根据数据库统计信息决定如何执行 SQL 查询。RegreSQL 1.0 测试查询结果是否与预期行匹配，但未检测计划变化。2.0 版本引入了基于计划的回归测试，利用生产统计信息及早捕获低效的执行计划。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://boringsql.com/products/regresql/">RegreSQL - SQL Query Regression Testing for PostgreSQL | boringSQL</a></li>
<li><a href="https://github.com/dimitri/regresql">GitHub - dimitri/ regresql : Regression Testing your SQL queries · GitHub</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#testing`, `#query planning`, `#database performance`, `#regression testing`

---

<a id="item-6"></a>
## [首个纯.NET 的 F5-TTS 语音克隆运行器](https://www.reddit.com/r/dotnet/comments/1uvhv3p/i_built_the_first_purenet_runner_for_f5tts_voice/) ⭐️ 8.0/10

一个名为 Horus.F5Tts.Onnx 的全新开源库，允许.NET 开发者完全在.NET 环境中通过 ONNX Runtime 运行 F5-TTS 语音克隆，无需再依赖 Python。 这消除了.NET 开发者在原生应用中使用先进语音克隆技术的主要集成障碍，并展示了 ONNX Runtime 如何弥合以 Python 为中心的机器学习模型与.NET 生态系统之间的鸿沟。 该库打包了三个 ONNX 计算图（预处理、变换器、解码），包含字符级分词器和 WAV 辅助工具。支持 CPU、DirectML 和 CUDA 执行提供程序，作者还修复了 ONNX 导出器中一个导致非英语检查点输出乱码的 bug。

reddit · r/dotnet · /u/nibor1896 · 7月13日 17:19

**背景**: F5-TTS 是一款以高质量输出著称的开源文本转语音和语音克隆模型，但其原生运行环境是 Python 与 PyTorch。ONNX Runtime 是微软提供的跨平台机器学习推理引擎，允许模型脱离原始框架运行。该库利用 ONNX Runtime 的.NET 绑定将 F5-TTS 引入.NET 应用程序。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/spaces/mrfakename/E2-F5-TTS">F5-TTS - a Hugging Face Space by mrfakename</a></li>
<li><a href="https://github.com/microsoft/onnxruntime">GitHub - microsoft/onnxruntime: ONNX Runtime: cross-platform, high ...</a></li>
<li><a href="https://onnxruntime.ai/docs/execution-providers/DirectML-ExecutionProvider.html">Instructions to execute ONNX Runtime with the DirectML execution ...</a></li>

</ul>
</details>

**标签**: `#.NET`, `#TTS`, `#voice cloning`, `#ONNX`, `#open source`

---

<a id="item-7"></a>
## [JetBrains 为 VS Code 和 Cursor 的 ReSharper 扩展添加调试功能](https://blog.jetbrains.com/dotnet/2026/07/13/rs-vsc-debugging/) ⭐️ 7.0/10

JetBrains 在 2026.2 版本中为 Visual Studio Code 和 Cursor 的 ReSharper 扩展发布了首个调试支持版本，满足了社区最迫切的需求。 这满足了用户长期以来的需求，显著提升了在 VS Code 和 Cursor 等轻量级编辑器中的 .NET 开发体验，使其成为完整 IDE 的更可行替代方案。 该调试器基于与 JetBrains Rider 相同的核心引擎构建，初始版本专注于核心调试功能，未来更新将添加更多特性。

rss · JetBrains .NET Tools (Rider/ReSharper) · 7月13日 10:39

**背景**: ReSharper 是一款流行的 .NET 生产力扩展，适用于 Visual Studio，下载量超过 250 万次。JetBrains 后来将 ReSharper 扩展到 VS Code 和 Cursor，但调试功能一直缺失。Cursor 是一款以 AI 为先的代码编辑器，于 2026 年 6 月被 SpaceX 收购。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.jetbrains.com/resharper/">Many IDEs and code editors - one ReSharper - JetBrains</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cursor_(code_editor)">Cursor (code editor)</a></li>
<li><a href="https://marketplace.visualstudio.com/items?itemName=JetBrains.ReSharper">ReSharper - Visual Studio Marketplace</a></li>

</ul>
</details>

**标签**: `#.NET`, `#debugging`, `#VS Code`, `#ReSharper`, `#JetBrains`

---

<a id="item-8"></a>
## [Datasette 代码频率图展示 AI 编码影响](https://simonwillison.net/2026/Jul/13/datasette-code-frequency/#atom-everything) ⭐️ 7.0/10

Simon Willison 分享了他 Datasette 项目的 GitHub 代码频率图，显示 2026 年代码增减量出现巨大峰值，他将其归因于 AI 编码代理和 Opus 4.5 类模型。 这提供了具体的数据驱动证据，展示了 AI 辅助编码工具如何显著提升开源项目的开发者生产力，为这些技术的影响提供了真实世界的基准。 最大的一周峰值显示新增 37,022 行、删除 9,528 行，超过了自 2018 年以来的所有活动；该图表还提到了 Opus 4.8、GPT-5.5、Fable 5 和 GPT-5.6 Sol 等后续模型。

rss · Simon Willison · 7月13日 21:45

**背景**: AI 编码代理（如 Cursor 和 CodeGPT）是一种通过自主生成或编辑代码来辅助开发者的工具。Opus 4.5 是 Anthropic 于 2025 年末发布的先进语言模型，针对编码和代理任务进行了优化。Datasette 是 Simon Willison 开发的开源工具，用于将数据探索和发布为交互式网站。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zencoder.ai/">Zencoder | The AI Coding Agent</a></li>
<li><a href="https://c-ai.chat/model-guides/claude-opus-4-5/">Claude Opus 4 . 5 - c-ai.chat</a></li>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and publishing data</a></li>

</ul>
</details>

**标签**: `#AI-assisted coding`, `#open-source`, `#productivity`, `#datasette`

---

<a id="item-9"></a>
## [Simon Willison 认为 LLM 代理不应成为直接责任人](https://simonwillison.net/2026/Jul/12/directly-responsible-individuals/#atom-everything) ⭐️ 7.0/10

Simon Willison 提出，基于 LLM 的代理绝不应被视为直接责任人（DRI），因为它们无法为自己的行为承担责任，并引用了 IBM 1979 年的培训幻灯片，其中指出计算机永远不能承担责任。 这一论点引发了关于团队将 AI 代理整合到工作流程中的关键问责问题，强调人类必须对 AI 驱动的决策和结果承担最终责任。 DRI 概念起源于苹果公司，并在 GitLab 中用于指代为项目成功或失败最终负责的人。Willison 明确划清界限，认为机器不能承担这一角色。

rss · Simon Willison · 7月12日 23:57

**背景**: 直接责任人（DRI）是对特定项目或成果拥有最终所有权的人，常见于苹果和 GitLab 等公司。该概念确保问责清晰，但将其应用于 AI 代理会引发伦理和实践上的担忧。IBM 1979 年的培训幻灯片曾指出，计算机永远不应做出管理决策，因为它们无法被追究责任，Willison 认为这一原则同样适用于现代的 LLM 代理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://handbook.gitlab.com/handbook/people-group/directly-responsible-individuals/">Directly Responsible Individuals (DRI) | The GitLab Handbook</a></li>
<li><a href="https://ifunny.co/picture/ibm-slide-1979-a-computer-can-never-be-held-accountable-416RcHn7C">IBM slide , 1979 A COMPUTER CAN NEVER BE HELD ... - iFunny</a></li>

</ul>
</details>

**标签**: `#software engineering`, `#AI ethics`, `#accountability`, `#LLM agents`

---