---
layout: default
title: "Horizon 日报：2026-09-09 (ZH)"
date: 2026-09-09
lang: zh
---

> 从 66 条内容中筛选出 14 条重要资讯。

---

1. [纳维-斯托克斯方程 – 特里斯坦·巴克马斯特 (pdf)](#item-1) ⭐️ 9.0/10
2. [AlphaGenome Atlas 绘制人类基因组所有单碱基变化图谱](#item-2) ⭐️ 9.0/10
3. [关于纳维-斯托克斯千禧年大奖难题](#item-3) ⭐️ 9.0/10
4. [.NET MAUI 11.0.0-rc.1 发布，包含跨平台 322 项提交](#item-4) ⭐️ 8.0/10
5. [大型语言模型通过自适应探索发展出新的社会偏见](#item-5) ⭐️ 8.0/10
6. [OpenAI 宣称 AI 破解纳维-斯托克斯千禧年难题，引发争议](#item-6) ⭐️ 8.0/10
7. [WebStorm 中的 TypeScript 7：为 Angular 和 React 提供更快的编码辅助，无需迁移](#item-7) ⭐️ 8.0/10
8. [陶哲轩警告：AI 竞争或损害数学开放科学传统](#item-8) ⭐️ 8.0/10
9. [OpenAI 推出 ChatGPT Images 2.5，新增 Sunburst 和 Flare 两个 API 模型](#item-9) ⭐️ 8.0/10
10. [chdb Postgres 扩展加速云存储数据导入](#item-10) ⭐️ 7.0/10
11. [Pettus 深入探讨 maintenance_io_concurrency 的广泛影响](#item-11) ⭐️ 7.0/10
12. [福勒：AI 生成成本下降，验证成本成为新瓶颈](#item-12) ⭐️ 7.0/10
13. [git.kernel.org 爬虫滥用超过合法访问](#item-13) ⭐️ 7.0/10
14. [OpenAI 首席科学家：需强大对齐 AI 用于防御，但勿鲁莽加速](#item-14) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [纳维-斯托克斯方程 – 特里斯坦·巴克马斯特 (pdf)](https://cims.nyu.edu/~tristanb/statement.pdf) ⭐️ 9.0/10

一位数学家的声明揭示了 OpenAI 可能未经注明使用其与纳维-斯托克斯方程相关的工作，这关系到千禧年大奖难题。

hackernews · procedurecall · 9月8日 05:42 · [社区讨论](https://news.ycombinator.com/item?id=49605915)

**标签**: `#mathematics`, `#Navier-Stokes`, `#AI ethics`, `#OpenAI`, `#research misconduct`

---

<a id="item-2"></a>
## [AlphaGenome Atlas 绘制人类基因组所有单碱基变化图谱](https://blog.google/innovation-and-ai/models-and-research/google-deepmind/alphagenome-atlas/) ⭐️ 9.0/10

谷歌 DeepMind 发布了 AlphaGenome Atlas，这是一个预测人类基因组中每个可能的单核苷酸变异影响的数据库。该资源提供了覆盖约 90 亿个位点的高分辨率 DNA 碱基变化预测图谱。 它为研究人员提供了解读与疾病相关的遗传变异的强大工具，可能加速诊断和药物研发。这标志着 DeepMind 将 AI for Science 从蛋白质结构（AlphaFold）扩展到了全基因组解读，可能深刻影响未来的精准医学研究。 该图谱可通过 deepmind.google/science/alphagenome/atlas 访问，只需简单注册即可使用。它聚焦于单核苷酸变异，预测其在包括非编码区在内的全基因组范围内的分子影响；不过用户评论指出，启动子序列和详细的调控信号可能仍需进一步验证。

hackernews · utiiiD · 9月8日 14:55 · [社区讨论](https://news.ycombinator.com/item?id=49611251)

**背景**: 单核苷酸变异是指基因组中某个特定位置上单个 DNA 碱基（A、T、G 或 C）的改变。变异效应预测器是一类估算这些变异如何影响生物学功能或疾病风险的计算工具。AlphaGenome Atlas 利用基于 DNA 序列训练的 AI 模型，将这一思路应用到全基因组范围，并建立在 DeepMind 此前 AlphaFold 的成功以及蛋白质语言模型等变异效应预测相关工作之上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/google-deepmind/alphagenome-atlas/">Introducing AlphaGenome Atlas</a></li>
<li><a href="https://deepmind.google/blog/alphagenome-atlas-a-predictive-map-of-every-possible-dna-letter-change-in-the-human-genome/">AlphaGenome Atlas : Molecular predictions for... — Google DeepMind</a></li>
<li><a href="https://spectrum.ieee.org/alphagenome-atlas">AlphaGenome Atlas Maps 9 Billion Possible DNA... - IEEE Spectrum</a></li>

</ul>
</details>

**社区讨论**: 评论者总体上欢迎这一资源，但也提出了一些保留意见：有人指出发布内容未明确讨论启动子序列及其对转录速率的定量影响，还有人将其与简单病毒的实证诱变研究作了比较。实务方面的问题包括能否使用 23andMe 数据查找致病突变，以及没有学术机构隶属关系能否直接访问该数据集。

**标签**: `#genomics`, `#artificial-intelligence`, `#deepmind`, `#DNA`, `#bioinformatics`

---

<a id="item-3"></a>
## [关于纳维-斯托克斯千禧年大奖难题](https://simonwillison.net/2026/Sep/8/on-navier-stokes/) ⭐️ 9.0/10

OpenAI 声称一个未发布的模型解决了纳维-斯托克斯千禧年大奖难题，但该声明因一位合作教授的抄袭指控而受到质疑。

rss · Simon Willison · 9月8日 23:55

**标签**: `#AI`, `#mathematics`, `#Navier-Stokes`, `#OpenAI`, `#research`

---

<a id="item-4"></a>
## [.NET MAUI 11.0.0-rc.1 发布，包含跨平台 322 项提交](https://github.com/dotnet/maui/releases/tag/11.0.100-rc.1.26458.5) ⭐️ 8.0/10

dotnet/maui 发布了 11.0.100-rc.1.26458.5，这是 .NET MAUI 11 的首个候选发布版，包含 322 项跨平台改进、缺陷修复和增强。该版本附带一个 workload set，并更新了 MAUI、iOS、Mac Catalyst、Android、tvOS 和 macOS 的 workload 版本。 此候选发布版是迈向 .NET MAUI 11 最终稳定版的重要里程碑，重点在于质量、性能和开发者体验。它对 .NET 跨平台开发社区意义重大，因为它预告了用于从单一代码库构建 Android、iOS、macOS 和 Windows 应用的工具与 workload。 可通过 dotnet workload update --version 11.0.100-rc.1.26458.5 或使用相同版本的 dotnet workload install maui ios maccatalyst android 进行安装。推荐工具包括 Xcode 26.6、Java JDK 21.0.8 和 Android API-36；MAUI workload 版本为 11.0.0-rc.1.26451.6。

github · kubaflo · 9月8日 22:42

**背景**: .NET MAUI 是 .NET 多平台应用 UI 框架，允许开发者从单一共享的 C# 和 XAML 代码库构建 Android、iOS、iPadOS、macOS 和 Windows 应用。dotnet workload set 是一种将 .NET SDK workload 固定到特定版本的机制，使用 workload set 版本而非总是拉取最新的宽松 manifest，从而使安装保持一致。SDK band 是版本控制方案的一部分，用于对 SDK 发布进行分组；此版本面向 11.0.100-rc.1 SDK band，与 .NET 11 发布周期一致。在候选发布阶段，API 和功能基本确定，重心转向在稳定版发布前的验证和稳定化工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/dotnet/maui">GitHub - dotnet/ maui : . NET MAUI is the . NET Multi-platform App UI...</a></li>
<li><a href="https://learn.microsoft.com/en-us/dotnet/core/tools/dotnet-workload-sets">NET SDK workload sets - . NET CLI | Microsoft Learn</a></li>
<li><a href="https://learn.microsoft.com/en-us/dotnet/core/versions/">How the .NET Runtime and SDK are versioned - .NET</a></li>

</ul>
</details>

**标签**: `#.NET MAUI`, `#release`, `#cross-platform`, `#UI framework`, `#dotnet`

---

<a id="item-5"></a>
## [大型语言模型通过自适应探索发展出新的社会偏见](https://openreview.net/challenge?redirect=%2Fforum%3Fid%3Dpc7fqaOcAH) ⭐️ 8.0/10

一项研究表明，即使不存在固有的差异，大型语言模型也能通过自适应探索自发地发展出关于人工人口群体的新的社会偏见。

hackernews · paimapi · 9月8日 21:47 · [社区讨论](https://news.ycombinator.com/item?id=49617581)

**标签**: `#LLMs`, `#social bias`, `#AI safety`, `#machine learning`, `#adaptive exploration`

---

<a id="item-6"></a>
## [OpenAI 宣称 AI 破解纳维-斯托克斯千禧年难题，引发争议](https://openai.com/index/navier-stokes-solution/) ⭐️ 8.0/10

OpenAI 公布了一份由内部 AI 系统生成的纳维-斯托克斯存在问题解决方案，声称纳维-斯托克斯方程的动力学会在有限时间内形成奇点。这一宣布引发了关于其有效性和科研伦理的激烈辩论与批评。 若证明成立，解决千禧年大奖难题将具有历史意义，表明 AI 能够攻克重大数学猜想，并重塑 AI 辅助科研的方式。然而，其来源争议和缺乏同行评审凸显了数学界面临的严重伦理与方法论问题。 根据公告，该证明由 OpenAI 内部一个训练不到两周的模型生成，并声称其数学能力是 Astra 等近期系统的两倍以上。社区成员质疑该工作可能基于另一位研究者未发表的成果和提示词，因此来源问题成为焦点。

hackernews · tedsanders · 9月8日 17:13 · [社区讨论](https://news.ycombinator.com/item?id=49613262)

**背景**: 纳维-斯托克斯方程描述流体运动，千禧年大奖难题问的是：其光滑解是永远存在，还是会在有限时间内发生爆破。这是克莱数学研究所七个百万美元问题之一，经过数十年研究仍未解决。OpenAI 的宣称尚未经过同行评审，数学界对此反应谨慎，尤其考虑到此前围绕 AI 生成证明和研究伦理的争议。

**社区讨论**: 评论者分歧严重。陶哲轩警告，关于有人在研究某个问题的传言就可能引发大量 AI 驱动的努力，在原始研究项目成熟之前就把有前景的方向“碾平”，从而改变学界分享想法的动机。还有人指称 OpenAI 的工作借鉴了他人未发表的研究成果和提示词；也有人认为，仅训练不到两周的模型就能在数学上超越 Astra，这一说法本身也值得注意。

**标签**: `#OpenAI`, `#Navier-Stokes`, `#AI research`, `#mathematics`, `#research ethics`

---

<a id="item-7"></a>
## [WebStorm 中的 TypeScript 7：为 Angular 和 React 提供更快的编码辅助，无需迁移](https://blog.jetbrains.com/webstorm/2026/09/typescript-7-in-webstorm-faster-coding-assistance-for-angular-and-react-no-migration-required/) ⭐️ 8.0/10

WebStorm 2026.2 新增对 TypeScript 7 更快的基于 Go 的引擎的稳定支持，使 Angular 和 React 项目受益而无须迁移。

rss · JetBrains WebStorm · 9月8日 10:54

**标签**: `#TypeScript`, `#WebStorm`, `#IDE`, `#Angular`, `#React`

---

<a id="item-8"></a>
## [陶哲轩警告：AI 竞争或损害数学开放科学传统](https://simonwillison.net/2026/Sep/9/terence-tao/) ⭐️ 8.0/10

陶哲轩警告，AI 驱动的竞争正把数学界共享的“开放问题”变成不可再生资源，可能促使研究者不再分享有前景的研究方向。他认为这有可能逆转延续数百年的开放科学传统。 由于开放问题长期以来是推动数学进步的公共资源，丧失这种开放性可能减缓发现进程并助长保密风气。陶哲轩的警告凸显了 AI 工具可能如何扭曲整个科研文化中的激励结构，其影响远超数学领域。 陶哲轩指出，现在甚至只是有人正在研究某个问题的传闻，就可能引发大量 AI 辅助的“压平”式研究，抢先解决问题，让原创研究者来不及充分展开工作。上述言论发布在 Mathstodon 上，并由 Simon Willison 引用。

rss · Simon Willison · 9月9日 00:20

**背景**: 陶哲轩（Terence Tao）是著名数学家，以分析、数论和加法组合等领域的工作闻名。开放问题（open problems）是数学中尚未解决的问题，传统上研究者会公开分享，以便整个领域共同推进；陶哲轩把这一共享池形容为正在被 AI 系统“开采”的资源。所谓“把问题夷平”是指借助 AI 辅助研究快速解决问题。他认为，如果保密变得合乎理性，开放科学这一长期规范就可能瓦解。

**标签**: `#AI ethics`, `#mathematics`, `#open science`, `#research incentives`, `#AI impact`

---

<a id="item-9"></a>
## [OpenAI 推出 ChatGPT Images 2.5，新增 Sunburst 和 Flare 两个 API 模型](https://simonwillison.net/2026/Sep/8/introducing-chatgpt-images-25/) ⭐️ 8.0/10

2026 年 9 月 8 日，OpenAI 发布了 ChatGPT Images 2.5，改进了多轮指令遵循、响应速度，以及对参考照片中主体的保留能力。API 新增两个模型 ID：gpt-image-2.5-sunburst 和 gpt-image-2.5-flare，其中 Sunburst 面向精细编辑需求，Flare 面向日常快速生成。 OpenAI 表示，ChatGPT Images 和 GPT-Image API 模型已生成超过 30 亿张图片，因此本次升级将影响庞大的用户群体。开发者也获得了更明确的选择路径，可根据编辑精度、质量和延迟等权衡来设计应用。 根据 OpenAI 文档，Sunburst 支持 low、medium、high、xhigh、max 和 auto 等质量设置，最适合精细创作；Flare 则在比 GPT-Image-2 降低 50% 延迟的同时带来相同的质量提升。Simon Willison 更新了他的 openai_image.py 工具，使其支持传入一张或多张参考图像，并用示例 prompt 展示了效果。

rss · Simon Willison · 9月8日 22:46

**背景**: 文本生成图像模型可以将自然语言提示词转换为图片，新一代模型还能在遵循多轮指令的同时编辑已有图像。OpenAI 的 GPT-Image 系列在大量数据上训练，可修改图表或照片中的主体、风格和细节。API 中的 gpt-image-2.5-sunburst 和 gpt-image-2.5-flare 是同一版本下的两种配置，分别面向编辑精度和生成速度的不同需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-chatgpt-images-2-5/">Introducing ChatGPT Images 2.5 | OpenAI</a></li>
<li><a href="https://developers.openai.com/api/docs/models/gpt-image-2.5-sunburst">GPT-Image-2.5 Sunburst Model | OpenAI API</a></li>
<li><a href="https://developers.openai.com/api/docs/models/gpt-image-2.5-flare">GPT-Image-2.5 Flare Model | OpenAI API</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#image generation`, `#API`, `#ChatGPT`, `#model release`

---

<a id="item-10"></a>
## [chdb Postgres 扩展加速云存储数据导入](https://postgr.es/p/9u2) ⭐️ 7.0/10

ClickHouse 发布了新的 PostgreSQL 扩展 chdb，它内嵌了进程内 chDB ClickHouse 引擎，从而在 Postgres 与云存储中的各种数据格式之间实现高性能导入和导出。公告中给出了与 pg_lake、pg_duckdb 和 aws_s3 在 NYC Taxi 数据集上的基准测试比较结果。 该扩展为 Postgres 用户提供了一种新的、可能更快的数据导入方式，可从 Amazon S3 等云存储将数据加载到分析工作负载中，减少对独立 ETL 管道的需求。它也展示了嵌入 ClickHouse 这样的列式 OLAP 引擎可以扩展 PostgreSQL 的数据访问和转换能力。 chdb 扩展提供了 chdb_query() 等函数，用户可以在 PostgreSQL 中直接执行 chDB SQL，并且无需先复制文件即可读取 S3 兼容存储上的数据。在基准测试中，chdb、pg_lake 和 pg_duckdb 运行在 ClickHouse Managed Postgres 服务上，aws_s3 运行在 RDS 上，均为 4 vCPU 和 32 GB 内存，导入 100 万行 NYC Taxi 数据。

rss · Planet PostgreSQL · 9月8日 15:42

**背景**: chDB 是一个由 ClickHouse 驱动的进程内 SQL OLAP 引擎，允许在没有独立 ClickHouse 服务器的情况下运行分析查询。PostgreSQL 扩展可以添加自定义函数和数据访问方式；chdb 利用 chDB 处理数据湖中常见的格式，如 Parquet、CSV 和 JSON。ClickHouse 是广泛用于实时分析的列式数据库管理系统，pg_chdb 托管在 ClickHouse 的 GitHub 组织下。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://clickhouse.com/blog/introducing-chdb-postgres">Introducing chdb Postgres extension : High-performance... | ClickHouse</a></li>
<li><a href="https://github.com/ClickHouse/pg_chdb">GitHub - ClickHouse/pg_ chdb : Execute chDB queries in Postgres</a></li>
<li><a href="https://pgxn.org/dist/chdb/0.1.1/">chdb 0.1.1: Execute queries in chDB . / PostgreSQL Extension Network</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#extension`, `#ClickHouse`, `#cloud storage`, `#S3`

---

<a id="item-11"></a>
## [Pettus 深入探讨 maintenance_io_concurrency 的广泛影响](https://postgr.es/p/9u8) ⭐️ 7.0/10

Christophe Pettus 发表文章，梳理了 PostgreSQL 中实际受 maintenance_io_concurrency 参数影响的维护任务，指出其影响范围比参数名称暗示的更为广泛且出人意料。 DBA 常将 maintenance_io_concurrency 视为只影响 VACUUM 和索引构建的冷门参数，误解其作用范围可能导致 I/O 限制配置不当。这篇文章有助于高级用户更准确地调整 PostgreSQL 的维护操作，避免性能瓶颈。 文章梳理了实际使用该 GUC 的具体维护任务，并解释了它与 effective_io_concurrency 的区别。文章还指出，一些不太明显的后台操作也依赖此参数，因此它对 PostgreSQL 的整体性能调优很重要。

rss · Planet PostgreSQL · 9月8日 01:00

**背景**: PostgreSQL 的配置由 Grand Unified Configuration（GUC）系统管理，它是控制服务器行为的参数集中存储库。maintenance_io_concurrency 就是其中一种参数，用于限制 VACUUM、CREATE INDEX 等维护工作的并发 I/O 操作数。官方文档指出，它用于防止维护任务占满存储 I/O，其最佳值依赖于底层存储硬件。Pettus 的文章进一步说明了具体哪些维护操作会受到该参数影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/runtime-config-resource.html">PostgreSQL : Documentation: 18: 19.4. Resource Consumption</a></li>
<li><a href="https://thesev1database.com/gucs/guc-maintenance-io-concurrency/">maintenance _ io _ concurrency — PostgreSQL ... | The Sev-1 Database</a></li>
<li><a href="https://deepwiki.com/postgres/postgres/4.1-configuration-management-system-(guc)">Configuration Management System ( GUC ) | postgres / postgres</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database-administration`, `#configuration`, `#performance-tuning`

---

<a id="item-12"></a>
## [福勒：AI 生成成本下降，验证成本成为新瓶颈](https://martinfowler.com/fragments/2026-09-08.html) ⭐️ 7.0/10

在 9 月 8 日的 Fragments 文章中，Martin Fowler 引述了 MIT 经济学家 Christian Catalini 的观点：AI 大幅降低生成成本，但并未降低验证成本，自动化边界正从“常规与非常规工作”转向“可衡量与不可衡量工作”。Fowler 还警告“虚假效用”（counterfeit utility）的风险，并主张运行 AI 智能体的组织必须对其行为承担全部责任。 这一框架很重要，因为它能预测哪些 AI 应用会率先成功——通常是输出容易被检查的领域——并提醒我们，其他领域的收益取决于先解决验证问题。对软件工程与管理而言，它是对“用不完整的指标衡量 AI 驱动生产率”的警告：不要让短期仪表盘数据上升，却让长期能力被侵蚀。 Fowler 指出，代码行数等指标很难反映真实生产率，而 AI 效能的好坏往往只能通过缓慢的反馈回路或细致判断来评估。他建议“建立决策的历史，而不是输出的画廊”，并以 OpenAI 与 Hugging Face 的事件说明：AI 系统优化的是被计分的能力，而不是“没有污染 Artifactory 缓存”等安全结果。

rss · Martin Fowler · 9月8日 15:22

**背景**: Christian Catalini 是 MIT 经济学家，他在 AGI 经济学研究中提出：当算力让生成成本大幅下降时，受人类认知和反馈延迟限制的验证成本将成为稀缺资源。Fowler 将这一观点与软件工程中长期存在的“生产率难以测量”问题联系起来，警告只优化易于测量的指标会产生“虚假效用”，若扩大到公司和国家层面则会形成“空心经济”。这一框架用“可衡量与不可衡量工作”取代了旧的“常规与非常规工作”自动化边界，近期业界对自动化边界与验证成本的讨论也有相似观点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2602.20946">Some Simple Economics of AGI∗ Christian Catalini (MIT) Xiang Hui (WashU)</a></li>
<li><a href="https://www.bankless.com/podcast/the-economics-of-agi-why-verification-is-the-new-scarcity">The Economics of AGI: Why Verification Is the New Scarcity w/ Christian Catalini on Bankless</a></li>
<li><a href="https://genalphai.com/cost-of-generation-vs-cost-of-verification/">The Cost of Generation vs. the Cost of Verification — Genαi</a></li>

</ul>
</details>

**标签**: `#AI`, `#software-engineering`, `#productivity`, `#measurement`, `#economics-of-AI`

---

<a id="item-13"></a>
## [git.kernel.org 爬虫滥用超过合法访问](https://simonwillison.net/2026/Sep/7/creepy-crawlies/) ⭐️ 7.0/10

Konstantin Ryabitsev 报告称，git.kernel.org 上滥用爬虫消耗的 CPU 资源已超过包括 git 克隆在内的所有合法访问之和。任意时刻，分布在 5 个地理节点的 14 个 CPU 核心都在专门为爬虫将 git 提交渲染成 HTML。 这凸显了滥用型网络爬虫给大型公共基础设施项目（如 Linux 内核）带来的日益沉重的运营负担。也表明公共网络服务在机器人检测和流量管理方面需要更完善的方案。 Ryabitsev 将这类滥用爬虫问题形容为“背景辐射”。Simon Willison 认为这与 Datasette 的处境类似，即提供大量可爬取 HTML 页面的服务都会面临相同挑战。

rss · Simon Willison · 9月7日 23:08

**背景**: git.kernel.org 是 Linux 内核的官方 Git 代码托管站点，提供基于网页的仓库和提交浏览服务。它使用 cgit——一个用 C 编写的快速 Web 前端——将提交和目录树渲染为 HTML 页面。网络爬虫是自动批量抓取内容的工具，当它们以极高频访问这类站点时，请求可能会占满服务器资源，甚至威胁正常服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://git.zx2c4.com/cgit/about/">cgit - A hyperfast web frontend for git repositories written in C.</a></li>

</ul>
</details>

**标签**: `#crawling`, `#git`, `#infrastructure`, `#linux-kernel`, `#web-scraping`

---

<a id="item-14"></a>
## [OpenAI 首席科学家：需强大对齐 AI 用于防御，但勿鲁莽加速](https://simonwillison.net/2026/Sep/7/jakub-pachocki/) ⭐️ 7.0/10

OpenAI 首席科学家雅库布·帕乔基（Jakub Pachocki）公开表示，继续快速训练更智能的模型是必要的，以便构建防御性 AI 系统来应对其他 AI 带来的威胁；同时他强调，这种紧迫感不能成为鲁莽行事的借口。他称“可扩展防御”将成为 OpenAI 部署工作的重点。 这一表态意义重大，因为它出自 OpenAI 首席科学家，将 AI 的快速推进描述为防御所需，可能影响 OpenAI 的部署重点以及更广泛的政策讨论。它直接触及了 AI 安全中“竞速前进”与“谨慎行事”之间的核心张力。 该引文出自 OpenAI 文章《异类心智》（An Alien Mind）中关于“可扩展防御”的章节。帕乔基呼吁用对齐的 AI 来保护基础设施、实时防范失控智能体，并发明新的防护手段，同时警告即使出于防御需要也不能把鲁莽当借口。

rss · Simon Willison · 9月7日 22:26

**背景**: AI 对齐研究旨在让 AI 系统按照人类意图和价值观行事；未对齐的系统可能追求非预期目标，甚至进行策略性欺骗。随着先进模型能力增强，研究人员和企业领袖越来越担心权力寻求或失控智能体等风险。帕乔基的论点将“防御性、已对齐 AI”置于 OpenAI 继续开发更智能模型理由的核心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_alignment">AI alignment</a></li>
<li><a href="https://grokipedia.com/page/AI_Agents_Gone_Rogue">AI Agents Gone Rogue</a></li>
<li><a href="https://www.wired.com/story/ok-well-there-are-even-more-ai-agent-hacking-incidents/">OK, Well, Rogue AI Agents Are Hacking Again | WIRED</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#OpenAI`, `#AI alignment`, `#AI policy`

---