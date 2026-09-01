---
layout: default
title: "Horizon 日报：2026-09-01 (ZH)"
date: 2026-09-01
lang: zh
---

> 从 26 条内容中筛选出 8 条重要资讯。

---

1. [Dan Ariely 著名拖延研究被曝数据造假证据](#item-1) ⭐️ 9.0/10
2. [谷歌从 Chrome 网上应用店移除 Manifest V2 扩展，包括 uBlock Origin](#item-2) ⭐️ 8.0/10
3. [NAT：互联网中心化的原罪](#item-3) ⭐️ 8.0/10
4. [把安防摄像头变成自动鸟类识别系统](#item-4) ⭐️ 7.0/10
5. [陶哲轩通俗讲解数学的六个基本概念](#item-5) ⭐️ 7.0/10
6. [PostgreSQL 19 新增 WAIT FOR LSN 以实现读写一致性](#item-6) ⭐️ 7.0/10
7. [pg-catalog-almanac：追踪 PostgreSQL 19 破纪录的 pg_catalog 变更](#item-7) ⭐️ 7.0/10
8. [Wrapture：用于猴子补丁、测试与追踪的 Python 新库](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Dan Ariely 著名拖延研究被曝数据造假证据](https://datacolada.org/138) ⭐️ 9.0/10

DataColada 第 138 号分析指出，由 Dan Ariely 合著的一项有影响力的拖延症研究存在数据伪造证据。报告数据中的统计模式不合理，表明数据是捏造的，而非单纯失误。 这很重要，因为该研究被广泛引用以支持关于截止日期和自我控制的论断，影响了学术理论和实践建议。它凸显了科学出版中的系统性问题，使得伪造数据能够通过同行评审并在多年内得不到纠正。 DataColada 团队在数据集中发现了特定的统计异常，例如不同实验条件下数值重叠的模式，这些模式在自然情况下极不可能出现。这并非 Ariely 的研究第一次面临数据完整性问题，但他仍与杜克大学保持关联。

hackernews · Anon84 · 8月31日 23:45 · [社区讨论](https://news.ycombinator.com/item?id=49516199)

**背景**: 可重复性危机（replication crisis）指的是大量已发表的科学研究结果无法被重复验证，从而削弱了理论的可信度并挑战科学知识体系。心理学一直是重复验证工作的重点领域。Dan Ariely 是著名行为科学家和多本畅销书作者，他的公众知名度使得这一案例在关于研究诚信的更广泛讨论中尤为显眼。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Replication_crisis">Replication crisis</a></li>
<li><a href="https://www.ipr.northwestern.edu/news/2024/an-existential-crisis-for-science.html">‘An Existential Crisis’ for Science: Institute for Policy Research - Northwestern University</a></li>

</ul>
</details>

**社区讨论**: 评论者感到沮丧，认为伪造研究可能在多年内不被发现，有人主张任何论文在被独立复制之前都不应被引用。还有人建议改变学术激励机制以鼓励复制研究，例如让本科生参与复制随机论文，并对杜克大学为何继续与 Ariely 保持关系提出质疑。

**标签**: `#research-fraud`, `#replication-crisis`, `#scientific-integrity`, `#procrastination`, `#Dan-Ariely`

---

<a id="item-2"></a>
## [谷歌从 Chrome 网上应用店移除 Manifest V2 扩展，包括 uBlock Origin](https://webiterate.dev/google-removed-extensions-ublock-origin-108/) ⭐️ 8.0/10

谷歌已正式从 Chrome 网上应用店移除 Manifest V2（MV2）扩展，包括广受欢迎的广告拦截工具 uBlock Origin。这一强制阶段结束了 Chrome 全面过渡到 Manifest V3 时代后对旧版扩展的支持。 这一变化让数百万用户失去了他们偏好的广告拦截和隐私工具，使他们更容易受到侵入性和恶意广告的影响。社区讨论强调了对谷歌单方面控制浏览器生态系统的担忧，并指出 Firefox 是主要替代方案。 uBlock Origin 依赖 webRequest API 实时拦截网络请求，而这一能力在 Manifest V3 中受到严格限制。Chrome 版 uBlock Origin 拥有超过 2900 万活跃用户，Firefox 版拥有超过 1060 万，是 Firefox 上最受欢迎的扩展。

hackernews · twapi · 8月31日 21:10 · [社区讨论](https://news.ycombinator.com/item?id=49514878)

**背景**: 浏览器扩展是向浏览器添加功能（如广告拦截）的小型软件程序。Manifest V2 和 Manifest V3 是 Chromium 内核浏览器的扩展规范；谷歌开始逐步淘汰 MV2，转而采用更安全、性能更好的 MV3，但 MV3 也限制了 webRequest 等强大 API。uBlock Origin 是一款免费开源的内容过滤器，高度依赖这些受限 API，因此在 MV3 下无法完全发挥作用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/UBlock_Origin">UBlock Origin</a></li>
<li><a href="https://ublockorigin.com/">uBlock Origin - Free, open-source ad blocker extension</a></li>
<li><a href="https://grokipedia.com/page/UBlock_Origin">uBlock Origin</a></li>

</ul>
</details>

**社区讨论**: 评论者绝大多数建议改用 Firefox，并有人指出 uBlock Origin 在该浏览器上一直表现最佳。用户将广告拦截视为安全问题，尤其是对不太懂技术的家人而言，并批评谷歌对网络拥有单方面控制权。有人表达了对 Firefox 的忠诚，称即使支持减少也会继续使用它或其分支。

**标签**: `#Chrome`, `#Extensions`, `#Manifest V2`, `#Ad-blocking`, `#Privacy`

---

<a id="item-3"></a>
## [NAT：互联网中心化的原罪](https://dreamstation.systems/personal/ntppost.html) ⭐️ 8.0/10

一篇评论文章指出，网络地址转换（NAT）通过削弱公共端点模型、使客户端-服务器不对称变得常态，成为互联网中心化的早期关键推手。该文章引发了社区广泛讨论，包括 Linux 中现行 NAT 系统的实现者 Rusty Russell 的评论。 这一观点将 NAT 不仅仅视为 IPv4 地址枯竭的临时解决方案，而是将其视为塑造当今中心化、以云为核心的互联网的基础力量。它的意义在于说明日常技术选择如何对开放性和用户自主权产生长期的结构性影响。 文章强调，NAT 天然地阻止来自不同地址的入站流量，取消了曾经让任何人都能托管服务器的公共端点。文章还指出，客户端-服务器模式之所以被视为理所当然，其实源于地址稀缺这一历史产物。

hackernews · robinpie · 8月31日 02:23 · [社区讨论](https://news.ycombinator.com/item?id=49504905)

**背景**: 互联网最初采用公共端点模型，每台设备拥有唯一 IP 地址，既能发起连接，也能接收连接。NAT 于 1990 年代引入，用于应对 IPv4 地址枯竭，它让多台设备共享一个公共 IP，但破坏了支持对等应用的双向对称通信。久而久之，家庭用户在未配置端口转发的情况下无法运行服务器，这促使服务向数据中心和大型云提供商迁移，加速了中心化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Client–server_model">Client–server model - Wikipedia</a></li>
<li><a href="https://link.springer.com/chapter/10.1007/978-3-642-11623-0_5">Typing Asymmetric Client-Server Interaction | SpringerLink</a></li>

</ul>
</details>

**社区讨论**: 评论者观点各异。RustyRussell 承认自己实现了 NAT 系统并同意它削弱了公共端点模型；solatic 赞同该文章，称其为开放互联网的挽歌。然而，elric 认为常规 NAT 在可控情况下可以接受，且保护了许多不安全设备，真正有害的是运营商级 NAT（CGNAT）。miki123211 补充了更广泛的批评，指出互联网设计者错误地将现实世界规范套用到网络空间。

**标签**: `#NAT`, `#internet architecture`, `#networking`, `#centralization`, `#IPv4`

---

<a id="item-4"></a>
## [把安防摄像头变成自动鸟类识别系统](https://jasontucker.blog/how-i-turned-my-security-cameras-into-an-automatic-bird-identification-system-with-birdnet-go/) ⭐️ 7.0/10

开发者 Jason Tucker 发布了一篇博客文章，介绍了他如何用 BirdNET-Go 把现有的安防摄像头改造成自动鸟类识别系统。这篇文章在 Hacker News 上引发了热烈讨论，获得了 371 分和 97 条评论。 这个项目表明，价格实惠且可自托管的 AI 可以把日常硬件重新用于野生动物监测，让鸟类识别对爱好者变得触手可及。它也体现了将消费级物联网设备与本地机器学习相结合、用于实时环境感知的流行趋势。 BirdNET-Go 通过摄像头的 RTSP 音频流进行监听，并在本地运行多模型分类，在快速的网页界面中展示识别结果。该系统需要 48kHz 的音频采样率，但有些摄像头（如 Aqara）仅支持 16kHz，因此一位评论者通过在树莓派上外接更好的麦克风解决了这个问题。

hackernews · speckx · 8月31日 16:47 · [社区讨论](https://news.ycombinator.com/item?id=49511856)

**背景**: BirdNET 是康奈尔大学开发的基于 AI 的鸟类声音识别工具。BirdNET-Go 是一个可自托管的实时声景分析器，可运行在树莓派上，接收声卡输入或网络音频流，全天候对鸟类、野生动物和蝙蝠进行分类。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/tphakala/birdnet-go">GitHub - tphakala/ birdnet-go : Self-hosted realtime soundscape ...</a></li>
<li><a href="https://birdnet.cornell.edu/">BirdNET – AI-Powered Sound ID</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了他们自己的 BirdNET-Go 配置，比如配合 Unifi 门铃摄像头或 Aqara 摄像头使用。有人提出了技术问题，包括音频采样率限制、内置麦克风的风噪，以及 Markdown 卡片中一个 ASCII 块的渲染问题，还提到康奈尔的 Merlin 应用是一个易用的替代方案。

**标签**: `#birdnet-go`, `#bird-identification`, `#security-cameras`, `#diy`, `#machine-learning`

---

<a id="item-5"></a>
## [陶哲轩通俗讲解数学的六个基本概念](https://www.youtube.com/watch?v=OOMx2BHHWtE) ⭐️ 7.0/10

在一段新视频中，数学家陶哲轩（Terence Tao）深入浅出地讲解了六个基本数学概念：数、代数、几何、概率、分析和动力系统。 陶哲轩是世界上最顶尖的数学家之一，他的讲解能让深奥的数学思维变得平易近人，激发大众对数学的兴趣。该视频也体现了他眼中数学的核心支柱，引发人们关于数学学科结构的讨论。 该视频采用讲座式风格，面向普通观众，并非技术性讲解。评论区中，观众对概念的选择提出不同看法：有人建议用拓扑学替代几何学，也有人对陶哲轩关于“猴子打出《哈姆雷特》”与暴力搜索的类比提出质疑。

hackernews · matthewsinclair · 8月30日 22:37 · [社区讨论](https://news.ycombinator.com/item?id=49503521)

**背景**: 陶哲轩是加州大学洛杉矶分校的著名数学家，研究领域涵盖调和分析、偏微分方程和数论，并于 2006 年获得菲尔兹奖。数学通常被划分为代数、几何、分析、概率等相互交叉的分支，各有独特但彼此关联的思维方式。公开讲解这些“支柱”有助于非专业人士理解数学各分支如何构成一个整体。

**社区讨论**: 评论区反响热烈，观众盛赞陶哲轩的清晰讲解，并对他强调动力系统表示认可。有人提出替代或补充的概念：如用拓扑学替换几何学，或加入逻辑和类型理论；也有观众希望多谈谈数学推理的过程本身。还有人反驳陶哲轩关于“猴子与《哈姆雷特》”的类比，认为它过于简化了这种暴力演化所需的时间。

**标签**: `#mathematics`, `#education`, `#Terence Tao`, `#video`, `#concepts`

---

<a id="item-6"></a>
## [PostgreSQL 19 新增 WAIT FOR LSN 以实现读写一致性](https://postgr.es/p/9tB) ⭐️ 7.0/10

PostgreSQL 19 引入了 WAIT FOR LSN 命令，允许备库阻塞直到重放到指定的 WAL 位置。这使应用程序在从副本读取时能够保证读写一致性。 现代前端应用常从 PostgreSQL 副本读取数据，可能因复制延迟导致用户更改暂时消失。WAIT FOR LSN 提供了一种标准机制，避免将读固定到主库、添加睡眠延迟或使用 Redis 标志等临时做法。 该命令必须是顶层语句而非函数，以防止自死锁；其源自 2016 年的提案。副本延迟包含多个部分——write_lag、flush_lag 和 replay_lag，其中 replay_lag 是主要瓶颈，因为恢复是单个进程顺序应用 WAL 记录。

rss · Planet PostgreSQL · 8月31日 23:00

**背景**: PostgreSQL 中的复制延迟是指主服务器上的更改尚未在副本服务器上反映出来。读写一致性确保写入后的后续读取能看到该写入，但复制延迟可能破坏这一保证。WAIT FOR LSN 命令让客户端指定一个 LSN，备库会暂停直到重放到该位置，为应用提供了一种与副本状态精确同步的方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/system-design/read-your-writes-consistency-in-system-design/">Read-your-Writes Consistency in System Design - GeeksforGeeks</a></li>
<li><a href="https://arpitbhayani.me/blogs/read-your-write-consistency/">Read-Your-Writes Consistency</a></li>
<li><a href="https://www.pgedge.com/blog/understanding-and-reducing-postgresql-replication-lag">Understanding and Reducing PostgreSQL Replication Lag</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#replication`, `#consistency`, `#application design`

---

<a id="item-7"></a>
## [pg-catalog-almanac：追踪 PostgreSQL 19 破纪录的 pg_catalog 变更](https://postgr.es/p/9tA) ⭐️ 7.0/10

Richard Yen 的 pg-catalog-almanac 提供了跨版本浏览 PostgreSQL pg_catalog 关系历史的功能。该工具显示，PostgreSQL 19 beta 3 新增了 12 个目录/视图和 43 个列，这是自 9.6 以来单个版本中新增关系数量最多的一次。 这使开发人员和 DBA 能更轻松地追踪跨版本新增的目录列和视图。PostgreSQL 19 中异常多的变更（包括新的 SQL 属性图目录）标志着 PostgreSQL 的元数据和查询能力的一次重大演进。 该年鉴目前涵盖从 PostgreSQL 9.6 到即将发布的 PostgreSQL 19 的全部 143 个已记录关系。新增目录中有 5 个支持 SQL 属性图，包括 pg_propgraph_element、pg_propgraph_element_label、pg_propgraph_label 和 pg_propgraph_label_property。

rss · Planet PostgreSQL · 8月31日 08:00

**背景**: pg_catalog 是一个系统模式，存储有关表、列、索引、约束、类型和依赖关系的元数据，以及实时服务器活动视图。PostgreSQL 的系统目录是普通表，保存模式元数据和内部记账信息，如官方文档所述。跨版本追踪目录条目变更通常需要比较多个文档版本和发布说明，非常繁琐。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/catalogs.html">PostgreSQL: Documentation: 18: Chapter 52. System Catalogs</a></li>
<li><a href="https://www.postgresql.org/docs/current/catalogs-overview.html">PostgreSQL: Documentation: 18: 52.1. Overview</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#pg_catalog`, `#PG19`, `#database internals`

---

<a id="item-8"></a>
## [Wrapture：用于猴子补丁、测试与追踪的 Python 新库](https://simonwillison.net/2026/Aug/31/introducing-wrapture/) ⭐️ 7.0/10

Graham Dumpleton 发布了新 Python 库 Wrapture，将 wrapt 风格的猴子补丁扩展到测试与追踪领域。它允许开发者包装函数和方法，以观察或覆盖其行为，可作为 unittest.mock 的替代品及追踪机制。 它的重要性在于为 Python 开发者提供了一个同时支持 mock 和追踪的统一工具，可能简化调试与可观测性工作。由于它出自 wrapt 和 mod_wsgi 的作者之手，很可能在 Python 生态中受到关注。 Wrapture 包含 OpenTelemetry 支持，并提供基于配置（TOML）的机制，将追踪添加到现有项目中。该项目仅发布数周，值得一提的是，其全部代码和文档均由 AI 助手在 Graham Dumpleton 的指导下编写。

rss · Simon Willison · 8月31日 23:59

**背景**: 猴子补丁（monkey patching）指在运行时动态修改代码，常用于 Python 测试中以替换或桩替行为。wrapt 是一个用于装饰器、包装器和猴子补丁的 Python 模块，提供透明对象代理。Wrapture 基于这些概念，将观察与覆盖功能结合到一个库中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pypi.org/project/wrapt/">wrapt · PyPI</a></li>
<li><a href="https://wrapt.readthedocs.io/">wrapt — wrapt 2.3.0 documentation</a></li>
<li><a href="https://stackoverflow.com/questions/5626193/what-is-monkey-patching">python - What is monkey patching? - Stack Overflow</a></li>

</ul>
</details>

**标签**: `#Python`, `#Testing`, `#Tracing`, `#Monkeypatching`, `#Open Source`

---