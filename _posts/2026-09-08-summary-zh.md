---
layout: default
title: "Horizon 日报：2026-09-08 (ZH)"
date: 2026-09-08
lang: zh
---

> 从 30 条内容中筛选出 9 条重要资讯。

---

1. [GitHub 上发布 Stuxnet 重建源码，供安全研究与教学使用](#item-1) ⭐️ 8.0/10
2. [博通撤下 VDDK 下载，迁移离开 VMware 更难](#item-2) ⭐️ 8.0/10
3. [LG 智能电视被曝隐秘录音并窥探网络](#item-3) ⭐️ 8.0/10
4. [数据流模型再探](#item-4) ⭐️ 8.0/10
5. [滥用爬虫在 git.kernel.org 上的负载超过全部合法访问](#item-5) ⭐️ 8.0/10
6. [研究加速：OpenAI 内部视角](#item-6) ⭐️ 8.0/10
7. [Knowledge Fabric 项目让 PostgreSQL 借助 HNSW 和 RRF 扩展至 5000 万向量](#item-7) ⭐️ 8.0/10
8. [DNS 滥用危机：多达 20%的新 gTLD 域名被用于诈骗](#item-8) ⭐️ 7.0/10
9. [从头重写代码很少能成功——Simon Willison 的经验之谈](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [GitHub 上发布 Stuxnet 重建源码，供安全研究与教学使用](https://github.com/Sadpainy/Stuxnet) ⭐️ 8.0/10

Hacker News 用户 Sadpainy 发布了一个重建 Stuxnet 恶意软件源代码的项目，并将其定位为教育与研究资源。代码托管在 github.com/Sadpainy/Stuxnet，评论区有人估计其约有一万五千行。 Stuxnet 至今仍是最复杂的网络武器之一，因此重建源码对恶意软件分析人员和防御方研究人员来说是宝贵的实战研究对象。研究它有助于安全团队理解 SCADA 与 PLC 环境如何被攻击，并加强对关键基础设施的保护。 Stuxnet 专门针对西门子 Step7 软件和 PLC，被认为曾破坏伊朗纳坦兹核浓缩设施，据称摧毁了其中约五分之一离心机。它通过感染 U 盘跨越物理隔离网络传播，并利用了四个零日漏洞；不过这段重建代码只应在安全、受控的研究或教学环境中使用。

hackernews · CMDDestory · 9月7日 22:12 · [社区讨论](https://news.ycombinator.com/item?id=49603546)

**背景**: Stuxnet 是一种恶意计算机蠕虫，2010 年首次被发现，此前已悄悄开发多年；外界普遍认为它是美国与以色列针对伊朗核计划的联合网络武器。它通过在 PLC 上植入 rootkit，同时向操作员显示正常的运行数值来破坏工业控制系统，最终让高速旋转的离心机撕裂损毁。该恶意软件感染了超过 20 万台计算机，成为针对关键基础设施的网络物理攻击早期标志性事件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Stuxnet_(malware)">Stuxnet (malware)</a></li>
<li><a href="https://www.trellix.com/security-awareness/ransomware/what-is-stuxnet/">What Is Stuxnet ? | Trellix</a></li>
<li><a href="https://www.kaspersky.co.in/resource-center/definitions/what-is-stuxnet">Stuxnet Definition & Explanation</a></li>

</ul>
</details>

**社区讨论**: 评论区整体以赞赏和好奇为主：有用户表示这份重建代码约有 1.5 万行，并说自己因 PLC 相关工作经历而改变了看待工业基础设施的方式；也有用户推荐《Countdown to Zero Day》这本书。还有人质疑 U 盘传播是否意味硬件已在经销商环节被感染，另外有用户调侃道“g_dwCentrifugeDestroyed++;”。批评主要集中在项目缺少文档，这会让读者较难浏览和理解代码。

**标签**: `#cybersecurity`, `#malware-analysis`, `#stuxnet`, `#reverse-engineering`, `#critical-infrastructure`

---

<a id="item-2"></a>
## [博通撤下 VDDK 下载，迁移离开 VMware 更难](https://www.virtualizationhowto.com/2026/09/leaving-vmware-just-got-harder-after-broadcom-pulled-vddk-downloads/) ⭐️ 8.0/10

博通移除了 VMware 虚拟磁盘开发套件（VDDK）的公开下载，包括 8.0.3 版本。这一举措切断了第三方备份、容灾及迁移工具读取和传输 VMware 虚拟磁盘所依赖的主要 API。 几乎所有虚拟机迁移产品都依赖 VDDK，因此移除它将直接妨碍用户把工作负载从 vSphere 迁移到 Hyper-V、Proxmox 等其它虚拟化平台。这会加深博通收购 VMware 后生态访问受限带来的“被锁定”忧虑。 下载限制不仅影响迁移，还影响多家主要厂商的备份与容灾产品，因为它们依赖 VDDK 访问磁盘数据。社区成员指出可用 qemu-img 等工具直接处理 .vmdk 作为部分变通方案，但对大规模企业迁移而言并不能完全替代 VDDK。

hackernews · josephcsible · 9月7日 20:32 · [社区讨论](https://news.ycombinator.com/item?id=49602699)

**背景**: VDDK 是一组 C 语言库和实用程序（如 VixDiskLib），允许应用程序访问和操作由 vSphere、Workstation 与 Fusion 创建的虚拟磁盘。VMware 备份和迁移软件历史上一直通过 VDDK 与 vSphere 存储 API 作为移动或保护虚拟机的基础机制。博通此前已因收购后的 VMware 产品组合调整限制了 VDDK 的分发，而这次移除公开下载被视为该策略的又一步。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://platform9.com/blog/vddk-no-longer-available/">Broadcom Cut Public Access of Virtual Disk Development Kit (VDDK) Overnight • Platform9</a></li>
<li><a href="https://www.rackwareinc.com/post/the-impact-and-importance-of-vmware-s-restriction-on-vddk">The Impact and Importance of VMware's Restriction on VDDK</a></li>
<li><a href="https://techdocs.broadcom.com/us/en/vmware-cis/vsphere/vsphere-sdks-tools/8-0/an-introduction-getting-started-with-vsphere-apis-and-sdks-8-0/example-use-cases-for-vsphere-apis/virtual-disk-api-use-cases.html">Virtual Disk Development Kit</a></li>

</ul>
</details>

**社区讨论**: 前 VMware 工程师对博通所谓的“受控坠落”以及重获利轻创新的取向表示难过。一位曾主导 Hyper-V 到 VMware、VMware 到 Hyper-V 迁移的工程师认为 VMware 更优秀，而 Hyper-V 像是拼凑出来的产品；一名家庭实验室用户则表示 VMware 到 Proxmox 的迁移在小规模下出奇顺利。还有评论者质疑仅用 qemu-img 转换镜像并手工配置虚拟硬件是否足够离开 VMware。

**标签**: `#VMware`, `#Broadcom`, `#virtualization`, `#migration`, `#infrastructure`

---

<a id="item-3"></a>
## [LG 智能电视被曝隐秘录音并窥探网络](https://www.youtube.com/watch?v=6IFVTcM28KA) ⭐️ 8.0/10

Gamers Nexus 的调查发现，LG 智能电视即使在屏幕关闭时也会记录麦克风音频，并扫描本地网络以映射附近设备。这一行为影响多达 2.16 亿台 LG 智能电视。 这表明消费级 IoT 设备即使处于非活跃状态也能进行隐蔽监控，削弱了用户对‘智能’家居产品的信任。它影响了全行业的智能电视用户，并引发了关于常开麦克风和不透明数据处理的法律、伦理和安全担忧。 LG 的 webOS 会以纯文本记录语音提示，并可在离线时缓存音频，待电视重新联网后上传。这些电视还存在安全漏洞，可能被利用转化为隐蔽窃听设备；LG 条款还要求用户告知并征得任何声音可能被捕获者的同意。

hackernews · treve · 9月7日 00:22 · [社区讨论](https://news.ycombinator.com/item?id=49592375)

**背景**: 智能电视是指运行操作系统（如 LG 的 webOS）的联网电视，通常会收集观看习惯和语音命令数据以用于个性化广告。此前已有多次研究对消费设备中的常开麦克风提出了隐私担忧。Gamers Nexus 的调查提供了具体技术证据，证明 LG 电视会扫描网络以盘点手机等设备，甚至在“关机”时也会记录音频。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.notebookcheck.net/LG-smart-TVs-caught-logging-audio-with-screen-off-and-snooping-on-local-devices.1391214.0.html">LG smart TVs caught logging audio with screen off and snooping on...</a></li>
<li><a href="https://cybersecuritynews.com/lg-smart-tvs-caught-scanning-networks/">LG Smart TVs Caught Scanning Networks and Logging Audio in...</a></li>

</ul>
</details>

**社区讨论**: 评论者大多表示震惊和愤怒，有人称 LG 的合同条款“很糟糕”，因为它要求用户获得周围所有人的同意。多位用户表示已禁用网络功能或物理移除 WiFi 芯片，还有人认为这种行为应违反窃听法律。

**标签**: `#privacy`, `#smart-tv`, `#surveillance`, `#security`, `#lg`

---

<a id="item-4"></a>
## [数据流模型再探](https://www.vldb.org/pvldb/volumes/19/paper/The%20Dataflow%20Model%20Revisited) ⭐️ 8.0/10

这是一场专家讨论，围绕 VLDB 论文重新审视数据流模型，反思从以流为中心的编程向以表/SQL 为中心的分析转变。

hackernews · scott_s · 9月6日 18:10 · [社区讨论](https://news.ycombinator.com/item?id=49589190)

**标签**: `#dataflow`, `#stream processing`, `#databases`, `#apache beam`, `#research`

---

<a id="item-5"></a>
## [滥用爬虫在 git.kernel.org 上的负载超过全部合法访问](https://simonwillison.net/2026/Sep/7/creepy-crawlies/) ⭐️ 8.0/10

康斯坦丁·里亚比采夫（Konstantin Ryabitsev）报告称，在 git.kernel.org 上，滥用型爬虫消耗的 CPU 周期已超过包括 git 克隆在内的所有合法访问总和。在该服务的 5 个地理分布式节点上，随时约有 14 个 CPU 核心只用于为抓取工具把 Git 提交渲染成 HTML。 这表明滥用爬虫的代价已不再只是带宽问题：基础设施运营者正把稀缺的计算资源和维护精力花在毫无价值的自动化请求上。这也凸显了所有发布大量可抓取 HTML 页面的项目所面临的日益严重的担忧，尤其是依赖捐赠或志愿者资源的自由及开源基础设施。 该报告由内核基础设施关键人物康斯坦丁·里亚比采夫发布，西蒙·威利森（Simon Willison）转发并表达了对 Datasette 项目的担忧——该项目会提供大量可抓取的网页。CPU 负载分布在 5 个地理分布式节点上，说明问题影响的是整个服务，而不是单点瓶颈。

rss · Simon Willison · 9月7日 23:08

**背景**: Linux 内核在 git.kernel.org 托管的 Git 仓库中开发，该站点除了提供 git clone 访问外，还提供用于浏览提交和代码的网页。这类 HTML 页面通常由 cgit 之类的 Git Web 前端即时生成，因此每次页面访问都会消耗服务器 CPU 周期。搜索引擎和其他自动化爬虫会不断抓取这些页面；当爬虫属于滥用或不受欢迎的类型时，项目方最终要为此投入计算成本，却得不到任何收益。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://git.zx2c4.com/cgit/about/">cgit - A hyperfast web frontend for git repositories written in C.</a></li>

</ul>
</details>

**标签**: `#crawling`, `#git`, `#web-scraping`, `#server-operations`, `#open-source`

---

<a id="item-6"></a>
## [研究加速：OpenAI 内部视角](https://simonwillison.net/2026/Sep/6/research-acceleration-the-view-inside-openai/) ⭐️ 8.0/10

Simon Willison 强调了 OpenAI 针对 RSI 的新沟通策略，并揭示编码代理如今已成为 OpenAI 内部研究流程的核心，附有使用图表作支持。

rss · Simon Willison · 9月6日 23:57

**标签**: `#OpenAI`, `#RSI`, `#coding agents`, `#AI research`, `#AGI`

---

<a id="item-7"></a>
## [Knowledge Fabric 项目让 PostgreSQL 借助 HNSW 和 RRF 扩展至 5000 万向量](https://www.reddit.com/r/PostgreSQL/comments/1w8ute5/pushing_postgresql_to_50m_vectors_hybrid_rrf_hnsw/) ⭐️ 8.0/10

开源项目 Knowledge Fabric 证明了 PostgreSQL 16+ 可以处理多达 5000 万个向量的生产级 RAG 工作负载，其实现采用 pgvector HNSW 索引、词法/向量混合搜索以及行级安全。在数百万向量的规模上，查询时间保持在 10 毫秒以内。 这挑战了 AI 社区中普遍认为 PostgreSQL 不适合向量搜索、必须使用专用向量数据库的观点。通过将向量与关系元数据保留在同一个支持 ACID 的数据库中，团队可以降低运维复杂度，并在多租户 RAG 应用中保持事务一致性。 该项目的混合搜索在单个 SQL 查询中同时执行 tsvector 全文搜索和 pgvector 稠密向量搜索，并通过 RRF（score = 1/(60+rank_lexical) + 1/(60+rank_vector)）合并结果。它还提供可选的行级安全策略：若未设置 tenant_id，查询将返回零行；并通过按 tenant_id 的 LIST 分区实现分区裁剪和局部 HNSW 扫描。

reddit · r/PostgreSQL · /u/Asleep-History9366 · 9月6日 12:25

**背景**: pgvector 是 PostgreSQL 的一个扩展，用于存储向量并执行近似最近邻搜索，其 HNSW（层次可导航小世界）索引可实现快速近似查询，但构建时间更长、内存占用更高。混合搜索通常将 BM25 等词法检索方法与稠密向量检索结合，而 RRF 通过对各排序列表的排名取倒数并求和来合并为一个结果列表。PostgreSQL 的行级安全根据策略限制查询可访问的行，为多租户 RAG 系统提供了第二层隔离边界。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepwiki.com/pgvector/pgvector/5.1-hnsw-index">HNSW Index | pgvector/pgvector | DeepWiki</a></li>
<li><a href="https://learn.microsoft.com/en-us/azure/search/hybrid-search-ranking">Hybrid Search Scoring (RRF) - Azure AI Search | Microsoft Learn</a></li>

</ul>
</details>

**标签**: `#postgresql`, `#vector-search`, `#pgvector`, `#HNSW`, `#hybrid-search`

---

<a id="item-8"></a>
## [DNS 滥用危机：多达 20%的新 gTLD 域名被用于诈骗](https://simonwillison.net/2026/Sep/6/the-purpose-of-dns-is-to-spread-scams/) ⭐️ 7.0/10

Terence Eden 援引 Interisle 报告指出，2025 年 8,500 万个新 gTLD 注册中，到 5 月已有 850 万个被列入黑名单，实际滥用率估计为 10%至 20%，意味着每五个新注册的通用顶级域中可能就有一个用于诈骗。 这些数据将 DNS 滥用重新定义为一个系统性危机，而非个别案例，影响 ICANN 治理、注册局、品牌安全和普通网民。如果 10%至 20%的新 gTLD 域名都是恶意的，那么现有的缓解措施和政策显然在规模化应对上失效了。 这些数据针对的是新 gTLD 注册而非传统顶级域，并以是否被列入黑名单来定义滥用。据报道，ICANN 多年来一直在讨论这一问题却未解决，凸显了治理上的迟缓。

rss · Simon Willison · 9月6日 14:40

**背景**: 域名系统（DNS）将人类可读的域名转换为 IP 地址，相当于互联网的电话簿。通用顶级域（gTLD）是域后缀的类别，如.com，以及通过 ICANN 新 gTLD 项目引入的众多新后缀。DNS 滥用指利用域名或 DNS 基础设施进行恶意活动，如钓鱼、投放恶意软件和诈骗。ICANN 是负责协调 DNS 的非营利组织，设有 DNS 滥用缓解项目，但在定义与责任分配等问题上仍存持续争议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Generic_top-level_domain">Generic top-level domain - Wikipedia</a></li>
<li><a href="https://haveibeensquatted.com/learn/dns-security/dns-abuse">What is DNS abuse? Definition, types & why it's contentious - Learn ...</a></li>
<li><a href="https://www.icann.org/dnsabuse">DNS Abuse Mitigation Program - ICANN</a></li>

</ul>
</details>

**标签**: `#DNS`, `#security`, `#scams`, `#ICANN`, `#domain abuse`

---

<a id="item-9"></a>
## [从头重写代码很少能成功——Simon Willison 的经验之谈](https://simonwillison.net/2026/Sep/6/theres-no-limit-to-how-bad-code-can-get/) ⭐️ 7.0/10

Simon Willison 在 Lobste.rs 的一条评论中指出，为了摆脱技术债务而彻底重写代码库的做法很少能成功。他建议用自动化测试加固现有系统，并进行针对性的重构，而不是追求绿地式重写。 这一观点挑战了常见的“从头重写”诱惑，为技术债务、团队激励和系统复杂性提供了现实的视角。它对于决定如何处理老代码库的工程领导者以及可能被绿地乐观情绪误导的团队都很重要。 Willison 观察到，遗留系统因为支撑着核心业务而不断变化，同时开发者缺乏改进它的动力，导致债务持续积累。他引用 Will Larson 的文章《Migrations: the sole scalable fix to tech debt》作为最佳指南，并认为自动化测试加上针对性重构通常更有可能成功。

rss · Simon Willison · 9月6日 09:08

**背景**: 技术债务指的是在代码中走捷径所带来的长期成本，它会让未来的修改变得更慢、更有风险。“绿地”项目指从零开始、没有遗留约束的项目，但替换一个复杂的现有系统往往失败，因为旧系统的完整行为常常没有文档且仍在变化。“扼杀者无花果树”式（strangler fig）的渐进迁移法，通常被视为比“大爆炸”式重写更安全的选择。

**标签**: `#technical-debt`, `#software-engineering`, `#code-quality`, `#refactoring`, `#rewrites`

---