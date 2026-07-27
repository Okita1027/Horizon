---
layout: default
title: "Horizon 日报：2026-07-27 (ZH)"
date: 2026-07-27
lang: zh
---

> 从 33 条内容中筛选出 8 条重要资讯。

---

1. [PGSimCity：PostgreSQL 内部机制的 3D 可视化](#item-1) ⭐️ 8.0/10
2. [美国公民因 GrapheneOS 手机在边境自动擦除数据被起诉](#item-2) ⭐️ 8.0/10
3. [Mike Acton 的数据导向设计介绍](#item-3) ⭐️ 8.0/10
4. [折扣 AI 代币的隐藏市场曝光](#item-4) ⭐️ 8.0/10
5. [欧盟提议通过浏览器隐私设置消灭 Cookie 横幅](#item-5) ⭐️ 8.0/10
6. [Ruff v0.16.0 默认规则从 59 条扩展到 413 条](#item-6) ⭐️ 8.0/10
7. [PostgreSQL 的 gin_fuzzy_search_limit 可能静默返回随机行](#item-7) ⭐️ 7.0/10
8. [开创性 Postgres 特性应始于分支](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [PGSimCity：PostgreSQL 内部机制的 3D 可视化](https://nikolays.github.io/PGSimCity/) ⭐️ 8.0/10

PGSimCity 是一个交互式 3D 模拟，将 PostgreSQL 的内部调度和进程可视化，把复杂的数据库架构变成一座可探索的城市。 该工具使 PostgreSQL 出了名复杂的内部机制更加易于开发者和学习者理解，有可能降低数据库系统的学习门槛。 该模拟是开源的，可在 GitHub 上获取，目前侧重于调度和进程生命周期，社区反馈建议增加查询流程可视化。

hackernews · jonbaer · 7月27日 00:19 · [社区讨论](https://news.ycombinator.com/item?id=49063754)

**背景**: PostgreSQL 采用多进程架构，调度器管理连接、查询和后台工作进程。PGSimCity 将每个进程表示为 3D 城市中的建筑，通过动画和颜色变化展示活动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nikolays.github.io/PGSimCity/">PGSimCity · How PostgreSQL Works, in 3D</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞其创意方法，但提出了用户体验改进建议：减少视觉杂乱、改为交互式而非自动播放、添加查询追踪。有人猜测它可能是 LLM 生成的，但肯定了其教育价值。

**标签**: `#PostgreSQL`, `#visualization`, `#databases`, `#open-source`, `#education`

---

<a id="item-2"></a>
## [美国公民因 GrapheneOS 手机在边境自动擦除数据被起诉](https://www.techspot.com/news/113236-us-prosecutors-charge-atlanta-man-after-grapheneos-phone.html) ⭐️ 8.0/10

一名美国公民在机场边境检查时，他的 GrapheneOS 手机输入胁迫 PIN 后自动擦除数据，因此被检方起诉。指控涉及该设备安全功能相关的妨碍或销毁证据。 此案开创先例，表明在美国边境使用胁迫 PIN 或自动擦除功能可能被视为故意妨碍，给注重隐私的操作系统用户带来法律风险。它凸显了安全措施与跨境法律义务之间的紧张关系。 该手机运行 GrapheneOS，这是一种基于 Android 的开源操作系统，具有增强的安全功能。胁迫 PIN 功能旨在受到胁迫时擦除设备，但检方认为用户故意销毁证据。该用户可能面临与妨碍司法相关的指控。

hackernews · eecc · 7月26日 22:21 · [社区讨论](https://news.ycombinator.com/item?id=49063022)

**背景**: GrapheneOS 是一款注重安全的移动操作系统，适用于 Google Pixel 设备，以其强化的隐私功能和减少攻击面著称。胁迫 PIN 是一个辅助 PIN，在受到胁迫时输入会触发设备擦除或无声警报，而非解锁——这是某些安全软件和操作系统的功能。在美国边境，法律先例允许官员搜查设备，但销毁数据可能被解释为妨碍，并带来严重的法律后果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GrapheneOS">GrapheneOS</a></li>
<li><a href="https://en.wikipedia.org/wiki/Duress_PIN">Duress PIN</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了法律权衡：有人认为用户必须接受在边境使用胁迫 PIN 的后果，而另一些人建议携带空白手机并在过境后恢复备份。少数人推荐类似 VeraCrypt 隐藏卷的诱饵操作系统功能，作为比擦除更安全的替代方案。

**标签**: `#privacy`, `#security`, `#grapheneos`, `#borde search`, `#legal`

---

<a id="item-3"></a>
## [Mike Acton 的数据导向设计介绍](https://www.gamedevs.org/uploads/introduction-to-data-oriented-design.pdf) ⭐️ 8.0/10

Mike Acton 的经典演示《数据导向设计介绍》被强调为高价值资源，强调以数据为先的算法设计以优化缓存性能。 该演示代表了从面向对象到数据导向思维的根本性转变，对于游戏开发等性能敏感领域至关重要。 该演示专注于缓存友好的数据结构如并行数组，并提倡在代码结构之前分析数据流。它引发了关于其实用性的实质性争论。

hackernews · tosh · 7月26日 18:11 · [社区讨论](https://news.ycombinator.com/item?id=49060724)

**背景**: 数据导向设计（DOD）是一种通过优化数据布局和访问模式来提高 CPU 缓存效率的软件优化方法。它常用于游戏开发，与面向对象设计不同，采用结构体数组而非数组结构体。该方法由 Mike Acton 等人推广。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Data-oriented_design">Data-oriented design</a></li>
<li><a href="https://www.baeldung.com/cs/cache-friendly-code">Cache-Friendly Code | Baeldung on Computer Science</a></li>

</ul>
</details>

**社区讨论**: 评论指出，当需求频繁变化时，DOD 可能不切实际，如重写项目中所示。一些人质疑 DOD 是否仅仅是缓存感知编程，而另一些人则强调其围绕数据流设计算法的核心原则。

**标签**: `#data-oriented-design`, `#game-development`, `#performance`, `#algorithms`, `#cache-optimization`

---

<a id="item-4"></a>
## [折扣 AI 代币的隐藏市场曝光](https://vectoral.com/blog/token-relay-market) ⭐️ 8.0/10

Matt Lenhard 的一项调查揭示了一个蓬勃发展的中继市场，AI 代币以深度折扣转售，这些代币通常通过欺诈手段获取，如盗取账户、滥用免费信用额度以及盗窃金融工具。 这种欺诈行为破坏了 OpenAI 和 Anthropic 等 AI 提供商的定价模式，为转售者创造不公平的竞争优势，并与历史上的广告欺诈和云信用滥用相提并论，威胁到 AI 生态系统的完整性。 中继市场通过汇集来自不同来源的 API 密钥、利用 AWS 和 Azure 等提供商的免费云信用额度，以及使用被盗或受损账户来生成折扣代币进行转售。

hackernews · mlenhard · 7月26日 15:17 · [社区讨论](https://news.ycombinator.com/item?id=49058993)

**背景**: AI 代币是大型语言模型处理的基本文本单位；AI 公司按代币数量收费。云提供商为吸引初创公司提供免费信用额度，这可能被滥用。这种欺诈类似于票务倒卖，当价格低于市场清算水平时就会出现套利机会。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blogs.nvidia.com/blog/ai-tokens-explained/">What Are AI Tokens? The Language and Currency Powering Modern AI | NVIDIA Blog</a></li>
<li><a href="https://simonwillison.net/2026/Jul/26/relay-market/">An Inside Look at the Relay Market Powering Token Resellers and...</a></li>
<li><a href="https://www.linkedin.com/posts/matthew-lenhard-0babb037_excited-to-share-what-ive-been-working-on-activity-7485727708698562560-cuID">Excited to share what I've been working on. It’s Vectoral Fraud has...</a></li>

</ul>
</details>

**社区讨论**: 社区评论将此比作广告欺诈和票务倒卖，指出类似转售市场存在于以往的互联网巨头中。一条评论强调了对免费云信用额度的滥用，另一条则批评订阅模式创造了套利机会。还有评论提到 WorkOS Radar 是检测此类欺诈的解决方案。

**标签**: `#AI tokens`, `#fraud`, `#token reselling`, `#cloud credits abuse`, `#subscription models`

---

<a id="item-5"></a>
## [欧盟提议通过浏览器隐私设置消灭 Cookie 横幅](https://killthecookiebanner.eu/) ⭐️ 8.0/10

欧盟委员会提出一项方案，通过允许用户在浏览器层面设置隐私偏好，并自动传达给网站，从而消灭 Cookie 横幅。 这可以显著改善网络用户体验，减轻同意疲劳，同时为全球隐私控制（Global Privacy Control）等具有法律约束力的隐私信号开创先例。 该提案利用了类似于全球隐私控制（GPC）的浏览器级机制，该机制在部分隐私法律下已具有法律效力。但批评者指出，欧盟委员会自己的网站仍在使用 Cookie 横幅，凸显了潜在的虚伪做法。

hackernews · rapnie · 7月26日 11:53 · [社区讨论](https://news.ycombinator.com/item?id=49057175)

**背景**: Cookie 横幅是根据欧盟《电子隐私指令》和 GDPR 引入的，用于获取用户对非必要 Cookie 的同意。然而，它们被广泛批评为侵入性强且效果不佳，许多用户在不了解同意内容的情况下就点击关闭。全球隐私控制（GPC）是一种技术标准，允许用户向网站发送“不出售个人数据”的信号，已在加州和欧盟等地获得法律认可。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Global_Privacy_Control">Global Privacy Control</a></li>
<li><a href="https://privacybadger.org/">Privacy Badger | Electronic Frontier Foundation</a></li>

</ul>
</details>

**社区讨论**: 社区讨论反映了多元观点。一些评论者认为 Cookie 横幅无法构成“知情同意”，建议在法律上将其定义为不足。另一些人指出欧盟委员会自己网站上的 Cookie 横幅是虚伪的。有用户提出真正解决方案是彻底停止监视用户，而另一位用户则欢迎这种生活质量提升，但希望提供按站点自定义的选项。

**标签**: `#Privacy`, `#Cookie Banners`, `#EU Regulation`, `#Web Browsing`, `#User Experience`

---

<a id="item-6"></a>
## [Ruff v0.16.0 默认规则从 59 条扩展到 413 条](https://simonwillison.net/2026/Jul/25/ruff/#atom-everything) ⭐️ 8.0/10

2026 年 7 月 23 日，Astral 发布了 Ruff v0.16.0，该版本将默认规则集从 59 条大幅增加到 413 条。这一变化导致许多 CI 流水线因新的 lint 错误而失败。 这一重大扩展会破坏许多现有 Python 项目的 CI 工作流，但同时也让 Ruff 能够在无需配置的情况下捕获语法错误和运行时错误等严重问题。它默认情况下显著提升了代码质量。 自 Ruff v0.1.0 以来，规则总数从 708 条增加到 968 条。在测试中，sqlite-utils 出现了 1618 个错误，其中 1538 个通过 `--fix --unsafe-fixes` 自动修复。剩余的问题包括像 DTZ005 这样缺少时区参数的检查。

rss · Simon Willison · 7月25日 22:44

**背景**: Ruff 是用 Rust 编写的高性能 Python 代码检查器和格式化工具，其速度比 Flake8 和 Black 等传统工具快 10–100 倍。它由 Astral 公司开发，该公司近期被 OpenAI 收购。Ruff 可以用一个快速的可执行文件替代多个 Python 代码检查和格式化依赖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.astral.sh/ruff/">An extremely fast Python linter and code formatter, written in Rust.</a></li>
<li><a href="https://astral.sh/ruff">Ruff , an extremely fast Python linter | Astral</a></li>

</ul>
</details>

**标签**: `#Python`, `#linting`, `#Ruff`, `#developer tools`

---

<a id="item-7"></a>
## [PostgreSQL 的 gin_fuzzy_search_limit 可能静默返回随机行](https://postgr.es/p/9qw) ⭐️ 7.0/10

PostgreSQL 的 `gin_fuzzy_search_limit` 参数可能导致使用 GIN 索引的查询静默返回随机子集的结果，而非全部匹配行，这是以牺牲正确性换取速度的行为。 这是一个危险的权衡，因为依赖 GIN 索引进行全文搜索或 JSONB 查询的开发人员可能无意中获得不完整的结果，导致数据完整性问题或应用程序行为错误。 该参数旨在作为一种性能优化，限制模糊搜索期间考虑的条目数，但其行为是静默的，且子集是随机的，并非一致的前 N 个结果。

rss · Planet PostgreSQL · 7月27日 01:00

**背景**: GIN（通用倒排索引）是 PostgreSQL 的一种索引类型，用于索引数组、JSONB 和全文搜索向量等复合类型。`gin_fuzzy_search_limit` 是一个配置参数，用于设置模糊搜索期间 GIN 索引扫描返回的条目数上限；当超过该限制时，索引停止进一步查找，仅返回已找到的内容，这可能是一个任意子集。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reddit.com/r/PostgreSQL/comments/1isdq7r/fulltext_results_way_off_when_using_gin_fuzzy/">Fulltext results way off when using gin_fuzzy_search_limit and tsquery ...</a></li>
<li><a href="https://www.postgresql.org/docs/current/gin.html">PostgreSQL: Documentation: 18: 65.4. GIN Indexes</a></li>
<li><a href="https://pganalyze.com/blog/gin-index">Understanding Postgres GIN Indexes: The Good and the Bad</a></li>

</ul>
</details>

**社区讨论**: 来自 Reddit 的用户报告称，对于单词查询，该限制效果良好，误差在 5-10% 左右，但对于多词查询，结果可能偏差很大。一些评论者指出了危险性，并建议除非应用能容忍不完整结果，否则应避免使用此参数。

**标签**: `#PostgreSQL`, `#GIN indexes`, `#database performance`, `#query correctness`

---

<a id="item-8"></a>
## [开创性 Postgres 特性应始于分支](https://postgr.es/p/9qt) ⭐️ 7.0/10

这篇文章认为，Postgres 的广泛采用源于其“足够好”的简洁性和开源灵活性，并建议开创性特性应先在分支中验证，再考虑纳入核心。 这一观点对希望为 Postgres 做贡献的开发者和公司至关重要，因为它解释了核心纳入的高门槛，并通过分支提供了实用路径，从而在保持稳定性的同时加速创新。 作者以临时表上的并行查询为例，该特性跨分支经历了三次尝试，最终在 Postgres Professional 的分支中验证概念后成功。

rss · Planet PostgreSQL · 7月26日 08:58

**背景**: Postgres 核心对新特性有非常高的门槛，优先考虑安全性、无回归和已证实的用户需求，而非新颖性。历史上，2000 年至 2015 年间特性发布更大胆，但现在社区更加谨慎。分支允许开发者在真实负载和边缘情况下测试代码，为提交核心提供证据。

**标签**: `#PostgreSQL`, `#database design`, `#open source`, `#engineering culture`

---