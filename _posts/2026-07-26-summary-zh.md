---
layout: default
title: "Horizon 日报：2026-07-26 (ZH)"
date: 2026-07-26
lang: zh
---

> 从 24 条内容中筛选出 8 条重要资讯。

---

1. [Anthropic 为 Claude 5 发布新的上下文工程规则](#item-1) ⭐️ 8.0/10
2. [fly.io 转向 AI 沙箱并更换 CEO，面临用户批评](#item-2) ⭐️ 8.0/10
3. [开源权重 AI 正经历它的 Kubernetes 时刻](#item-3) ⭐️ 8.0/10
4. [安卓可能限制设备端 ADB](#item-4) ⭐️ 8.0/10
5. [Ruff v0.16.0 将默认规则扩展至 413 条](#item-5) ⭐️ 8.0/10
6. [Claude Opus 5 发布：经济实惠的边界 AI 模型](#item-6) ⭐️ 8.0/10
7. [通用汽车支持钠离子电池用于电网储能](#item-7) ⭐️ 7.0/10
8. [深入解析 PostgreSQL 的 full_page_writes 与崩溃风险](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Anthropic 为 Claude 5 发布新的上下文工程规则](https://claude.com/blog/the-new-rules-of-context-engineering-for-claude-5-generation-models) ⭐️ 8.0/10

Anthropic 发布了专门针对 Claude 5 模型的新上下文工程指南，超越了传统的提示工程，专注于如何构建和管理整个对话上下文以实现最佳性能。 从提示工程到上下文工程的转变代表了开发者和企业与大语言模型交互方式的重要演变，有可能带来更可靠、可扩展和可控的 AI 应用。社区的不同反应凸显了对供应商锁定和 Claude 自动记忆功能有效性的担忧，使这些指南成为 AI 从业者争论的焦点。 该指南强调结构化上下文管理，包括有效使用系统提示、记忆访问和长上下文处理，但一些用户报告称 Claude 5 仍然存在意外删除和因任务失败导致令牌使用量增加的问题。批评者认为，新规则可能是推动用户使用 Anthropic 特定工具、增加平台依赖性的尝试。

hackernews · mellosouls · 7月25日 20:42 · [社区讨论](https://news.ycombinator.com/item?id=49051361)

**背景**: 与提示工程相比，上下文工程是一种较新的方法；提示工程侧重于设计单个提示，而上下文工程管理整个上下文窗口，包括过去的交互、系统指令和外部数据，以实现一致的行为。Claude 5 是 Anthropic 最新一代模型，包括 Sonnet 5、Fable 5 和 Mythos 5 等变体，在安全性和代理能力方面比之前版本有所改进，但也引入了上下文处理的新挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-sonnet-5">Introducing Claude Sonnet 5 \ Anthropic</a></li>
<li><a href="https://medium.com/data-science-in-your-pocket/context-engineering-vs-prompt-engineering-379e9622e19d">Context Engineering vs Prompt Engineering | by Mehul... | Medium</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些用户认为这些指南是常识，而另一些用户则持怀疑态度，认为这些规则旨在增加供应商锁定。几位用户报告了 Claude 5 自动记忆和任务执行的实际问题，指出该模型经常出错或需要重试，导致令牌使用量增加。

**标签**: `#claude-5`, `#context-engineering`, `#prompt-engineering`, `#anthropic`, `#AI-models`

---

<a id="item-2"></a>
## [fly.io 转向 AI 沙箱并更换 CEO，面临用户批评](https://fly.io/blog/kurt-scott-money-sprites/) ⭐️ 8.0/10

fly.io 宣布战略转型，专注于 AI 沙箱，推出新一代 Sprites 产品，创始人 Kurt Scott 卸任 CEO，由 Scott Johnston 接替。 这一转型标志着这家曾深受 Elixir 社区喜爱的公司发生了重大转变，但针对过去可靠性问题和 AI 沙箱市场激烈竞争的严厉批评，让其前景充满疑问。 fly.io 的计算抽象层 Sprites 一直存在数据丢失和僵尸状态等错误，而 AI 沙箱领域已趋于商品化，这给新任 CEO 带来了巨大挑战。

hackernews · subarctic · 7月25日 20:43 · [社区讨论](https://news.ycombinator.com/item?id=49051369)

**背景**: fly.io 是一个提供边缘计算和多区域部署的云平台，深受使用 Elixir 等语言的开发者欢迎。Sprites 是他们用于运行应用的轻量级计算抽象层。AI 沙箱是一种隔离环境，用于安全执行由大型语言模型（LLM）和 AI 代理生成的代码，这是一个快速增长但竞争激烈的市场。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://fly.io/">Computers for agents · Fly</a></li>
<li><a href="https://northflank.com/blog/what-is-an-ai-sandbox">What is an AI sandbox? | Blog — Northflank</a></li>

</ul>
</details>

**社区讨论**: 社区评论大多负面，用户报告了严重可靠性问题，如数据丢失和 Sprite 无响应。一些人对转向拥挤的 AI 沙箱领域表示怀疑，少数人指出如果执行得到改进，重新关注 Sprites 可能是积极的。

**标签**: `#fly.io`, `#pivot`, `#AI sandboxes`, `#cloud infrastructure`, `#CEO change`

---

<a id="item-3"></a>
## [开源权重 AI 正经历它的 Kubernetes 时刻](https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/) ⭐️ 8.0/10

文章指出，开权重 AI 模型正遵循与 Kubernetes 相同的轨迹，成为企业在其上构建而非竞争的基础层。 这一转变可能稳定 AI 定价、促进协作模型开发并加速创新，类似于 Kubernetes 如何改变云基础设施。 开权重模型发布训练好的参数（权重）以支持定制和自托管，但通常不包括训练数据，因此并非完全开源。

hackernews · tknaup · 7月25日 14:49 · [社区讨论](https://news.ycombinator.com/item?id=49048034)

**背景**: Kubernetes 是一个开源容器编排平台，已成为部署应用的标准，使公司能在此基础上构建平台而非竞争。类似地，开权重 AI 模型提供了推理成本和控制的基准，可能导致类似的协作开发和商品化生态系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/models">Comparison of AI Models across Intelligence, Performance, and Price</a></li>
<li><a href="https://openai.com/index/introducing-gpt-oss/">Introducing gpt-oss | OpenAI</a></li>
<li><a href="https://www.linkedin.com/pulse/open-weight-ai-what-we-finally-opened-bonnet-nicolas-pistorio-n3ulf">Open - weight AI : what if we finally opened the bonnet ?</a></li>

</ul>
</details>

**社区讨论**: 评论讨论了按产地禁止模型的不可能性（因为权重只是数字）、AI API 定价的波动性（代币经济学），以及希望有前沿开权重模型以便创业公司构建的需求。一些人将其与 Linux 和 Kubernetes 类比，倡导协作式模型开发。

**标签**: `#open-weight`, `#AI`, `#Kubernetes`, `#open-source`, `#community`

---

<a id="item-4"></a>
## [安卓可能限制设备端 ADB](https://kitsumed.github.io/blog/posts/android-may-soon-restrict-on-device-adb/) ⭐️ 8.0/10

谷歌正在考虑一项功能请求，限制设备端 ADB 访问，可能要求认证或限制连接以降低安全风险。 这可能严重影响安卓开发工作流，尤其是依赖无线 ADB 进行调试的开发者，并引发对谷歌日益增强的设备控制权的担忧。 该提案针对设备端 ADB（在设备本身上通过 TCP/IP 的 ADB），建议限制只对授权接口或 IP 地址的访问；批评者认为攻击面极小，因为用户必须已启用开发者选项和远程 ADB。

hackernews · shscs911 · 7月25日 06:57 · [社区讨论](https://news.ycombinator.com/item?id=49045159)

**背景**: ADB（安卓调试桥）是一个命令行工具，供开发者与安卓设备通信，用于调试、安装应用和运行 shell 命令。设备端 ADB 指直接在设备上使用 ADB，无需电脑。谷歌的提案源于一个功能请求，旨在通过限制设备端 ADB 访问来增强安全性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Android_Debug_Bridge">Android Debug Bridge - Wikipedia</a></li>
<li><a href="https://developer.android.com/tools/adb">Android Debug Bridge (adb) | Android Studio | Android Developers</a></li>

</ul>
</details>

**社区讨论**: 社区意见分歧：一些人认为在现有保护措施下安全收益极小，而另一些人则认为这是进一步锁定的步骤。评论者表达了对谷歌长期意图的担忧，将其与之前对侧载的限制相比较，并建议技术变通无法解决用户自主权丧失的根本问题。

**标签**: `#Android`, `#ADB`, `#Developer Tools`, `#Security`, `#Google`

---

<a id="item-5"></a>
## [Ruff v0.16.0 将默认规则扩展至 413 条](https://simonwillison.net/2026/Jul/25/ruff/#atom-everything) ⭐️ 8.0/10

Ruff v0.16.0 于 2026 年 7 月 23 日发布，将默认 lint 规则从 59 条增加到 413 条，无需任何配置即可捕获语法错误和运行时问题。 这一重大扩展意味着现有项目可能会在 CI 中看到数百条新警告，可能导致构建失败，但同时能通过早期捕获严重问题来提高代码质量。这反映了 Ruff 作为 Python linter 日益全面的特性。 自 v0.1.0 以来，Ruff 的规则总数从 708 条增长到 968 条，新的默认规则集包括诸如 `load-before-global-declaration` 和 `yield-in-init` 等规则。此更新可能需要运行 `ruff check --fix` 来自动解决许多问题。

rss · Simon Willison · 7月25日 22:44

**背景**: Ruff 是一个用 Rust 编写的快速 Python linter 和代码格式化工具，拥有超过 900 条内置规则，可替代 Flake8 和 Black 等工具。它由 Astral 开发，该公司最近被 OpenAI 收购。此前 Ruff 默认只启用 Flake8 规则的一个子集。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.astral.sh/ruff/">Ruff</a></li>
<li><a href="https://github.com/astral-sh/ruff">GitHub - astral-sh/ruff: An extremely fast Python linter and code formatter, written in Rust. · GitHub</a></li>
<li><a href="https://docs.astral.sh/ruff/rules/">Rules | Ruff - Astral</a></li>

</ul>
</details>

**标签**: `#Python`, `#Ruff`, `#linting`, `#static analysis`, `#release`

---

<a id="item-6"></a>
## [Claude Opus 5 发布：经济实惠的边界 AI 模型](https://simonwillison.net/2026/Jul/24/introducing-claude-opus-5/#atom-everything) ⭐️ 8.0/10

Anthropic 于 2026 年 7 月 24 日发布了 Claude Opus 5，该模型以 Fable 5 一半的价格提供接近边界智能的性能，目前位居 Artificial Analysis 排行榜首位。 此次发布使高端 AI 能力对开发者与企业更加可负担，可能改变竞争格局。其主动行为与强大的网络安全漏洞检测能力进一步提升了实用性。 Claude Opus 5 定价为每百万输入令牌 5 美元、每百万输出令牌 25 美元，快速模式价格翻倍但速度更快。它拥有 100 万令牌的上下文窗口，最多可输出 128,000 令牌。

rss · Simon Willison · 7月24日 23:48

**背景**: Claude 是 Anthropic 开发的一系列 AI 模型，以安全性和实用性著称。边界智能指 AI 模型的最尖端能力。Artificial Analysis 排行榜比较各 LLM 在多个基准上的表现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openrouter.ai/anthropic/claude-opus-5-fast">Claude Opus 5 ( Fast ) - API Pricing & Providers | OpenRouter</a></li>
<li><a href="https://apidog.com/blog/claude-opus-5-pricing/">Claude Opus 5 Pricing: The Full Cost Breakdown (2026)</a></li>
<li><a href="https://artificialanalysis.ai/leaderboards/models">LLM Leaderboard - Comparison of AI models from OpenAI, Anthropic...</a></li>

</ul>
</details>

**社区讨论**: Boris Cherny 指出 Opus 5 是目前最难以被提示注入的模型，对安全性来说是个令人兴奋的进步。整体反响积极，对其主动能力与性价比感到兴奋。

**标签**: `#AI`, `#Anthropic`, `#Claude`, `#model release`, `#frontier intelligence`

---

<a id="item-7"></a>
## [通用汽车支持钠离子电池用于电网储能](https://spectrum.ieee.org/sodium-ion-battery-peak-energy) ⭐️ 7.0/10

通用汽车宣布支持钠离子电池技术用于美国电网储能，标志着其战略上从锂离子电池主导地位的转变。 这一背书可能加速钠离子电池的采用，该技术具有更低的材料成本和更强的供应链安全性，有望改变电网储能市场，减少对锂进口的依赖。 钠离子电池的往返效率高达 96%，与锂离子电池相当，但使用丰富的钠替代稀缺的锂。然而，目前其能量密度较低，更适合固定式储能而非电动汽车。

hackernews · rbanffy · 7月25日 21:48 · [社区讨论](https://news.ycombinator.com/item?id=49051947)

**背景**: 电网储能对于平衡太阳能和风能等间歇性可再生能源至关重要。钠离子电池因其原材料丰富、成本更低且更安全，正逐渐成为锂离子电池的替代方案。通用汽车的参与表明工业界对在美国能源基础设施中规模化应用该技术的信心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://batterycouncil.org/wp-content/uploads/2026/04/Sodium-Ion-Batteries-Technology_-Market-Outlook-SBIG-Workstreams.pdf">Sodium - Ion Batteries</a></li>
<li><a href="https://www.linkedin.com/pulse/battery-runs-salt-why-sodium-ion-could-reshape-worlds-wptue">The Battery that runs on Salt: Why sodium - ion could reshape the...</a></li>

</ul>
</details>

**社区讨论**: 评论者指出 96%的往返效率对于电网储能非常出色。一些人对依赖中国制造表示怀疑，并惋惜一家有前景的美国钠离子初创公司倒闭。其他人则提到，如果成本与磷酸铁锂相当，仅暖通空调的节能就足以支持切换。

**标签**: `#sodium-ion batteries`, `#grid storage`, `#energy`, `#battery technology`, `#GM`

---

<a id="item-8"></a>
## [深入解析 PostgreSQL 的 full_page_writes 与崩溃风险](https://postgr.es/p/9qq) ⭐️ 7.0/10

Christophe Pettus 发文解释了 PostgreSQL 在崩溃后将整个页面写入 WAL 的原因，并警示关闭 full_page_writes 参数的危险性。 这很重要，因为 full_page_writes 是防止撕裂写入导致数据损坏的关键保护；误解它可能导致静默数据丢失，因此该文章帮助 PostgreSQL 用户做出明智的配置决策。 Full_page_writes 默认开启，在检查点后首次修改时将整个 8KB 页面记录到 WAL 中以防止撕裂写入；关闭它可提升 I/O 性能，但如果在部分写入期间发生崩溃，则存在无法恢复的数据损坏风险。

rss · Planet PostgreSQL · 7月25日 01:00

**背景**: PostgreSQL 的 WAL（预写日志）记录变更以实现崩溃恢复。“撕裂写入”是指在写入页面时系统崩溃，导致页面只更新了一部分。Full_page_writes 确保在检查点后的第一次修改中记录完整页面，从而可以从 WAL 重建页面。GUC（Grand Unified Configuration）系统管理所有 PostgreSQL 配置参数。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wiki.postgresql.org/wiki/Full_page_writes">Full page writes - PostgreSQL wiki</a></li>
<li><a href="https://postgresqlco.nf/doc/en/param/full_page_writes/">PostgreSQL Documentation: full_page_writes parameter</a></li>
<li><a href="https://pgpedia.info/g/guc.html">GUC - Grand Unified Configuration - pgPedia - a PostgreSQL Encyclopedia</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database reliability`, `#crash recovery`, `#WAL`

---