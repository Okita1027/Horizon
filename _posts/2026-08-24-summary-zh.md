---
layout: default
title: "Horizon 日报：2026-08-24 (ZH)"
date: 2026-08-24
lang: zh
---

> 从 33 条内容中筛选出 7 条重要资讯。

---

1. [1998 年论文《复杂系统如何失效》引发实践者讨论](#item-1) ⭐️ 9.0/10
2. [黑客记录如何逆向固件实现对个人设备的完全掌控](#item-2) ⭐️ 8.0/10
3. [Anthropic 最好的 AI 模型难以吸引用户，而更便宜的替代品蓬勃发展](#item-3) ⭐️ 8.0/10
4. [17 万非营利组织数据全丢：微软该负责吗？](#item-4) ⭐️ 8.0/10
5. [现代关系查询语言愿望清单引发 SQL 替代品讨论](#item-5) ⭐️ 8.0/10
6. [Linus Torvalds 称赞坚持不懈的 AI 辅助内核调试会话](#item-6) ⭐️ 7.0/10
7. [不止于代码审查：精通 AI 编程代理](#item-7) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [1998 年论文《复杂系统如何失效》引发实践者讨论](https://how.complexsystems.fail/) ⭐️ 9.0/10

理查德·库克 1998 年的文章《复杂系统如何失效》正在 Hacker News 上被广泛分享，经验丰富的工程师们围绕其核心论点——对复杂系统做根本原因分析往往是徒劳的——展开讨论。这个获得 228 分和 61 条评论的讨论表明，该文章对现代可靠性实践仍具有持续的相关性。 这篇文章提供了一个基础性框架，挑战了简单的‘根本原因’叙事，影响了混沌工程和网站可靠性工程等学科。它之所以重要，是因为它改变了工程师思考复杂系统（如医疗、电网和分布式软件）中安全、失效与韧性的方式。 库克论证说，所有复杂系统本质上都存在风险，失效是正常且不可避免的，而安全是一种动态的、非线性的属性，无法通过静态规则实现。讨论中强调的‘准事故’概念解释了为什么事后审查常常错误地归因原因，而不是识别出系统性模式。

hackernews · shortcrct · 8月23日 15:13 · [社区讨论](https://news.ycombinator.com/item?id=49409473)

**背景**: 这篇文章由患者安全研究员理查德·库克撰写，是系统工程和安全科学领域的经典文献。它借鉴了复杂性理论和高可靠性组织的思想，解释为什么复杂系统中的事故不可避免，以及为什么传统的根本原因分析具有误导性。关键概念包括‘系统运行是动态的，组件以非线性方式相互作用’，以及冗余既可能有助于也可能阻碍安全。这场讨论将这些思想与混沌工程等现代实践联系起来，混沌工程通过故意注入故障来构建韧性。

**社区讨论**: 讨论非常正面且充满认同感：tptacek 称这篇文章‘重要’，并强调对复杂系统做根本原因分析是徒劳的；jedberg 指出‘无失效运行需要拥有失效的经验’，并认为它启发了混沌工程；anonymars 引用关于冗余和准事故的段落；feynman_r 推荐约翰·高尔的《系统学》；ChrisMarshallNY 则幽默地质疑第一句中的拼写问题。总体而言，评论者一致认可文章的持久价值，并分享了实践中的洞见。

**标签**: `#complex systems`, `#reliability`, `#chaos engineering`, `#systems thinking`, `#root cause analysis`

---

<a id="item-2"></a>
## [黑客记录如何逆向固件实现对个人设备的完全掌控](https://schlarp.com/posts/everything-i-own-owned/) ⭐️ 8.0/10

在一篇详细的博客文章中,黑客 schlarp 记录了对个人设备进行逆向工程以实现完全掌控的过程,首先从 ASUS ROG Swift PG42UQ 显示器入手,目标是永久移除烦人的“像素清洗”弹窗。文章还探讨了 WebUSB、WebHID 和 WebBluetooth 如何让用户一次点击权限提示的失误变成对设备的永久后门。 这件事之所以重要,是因为它揭示了消费者实际能控制的内容与硬件厂商允许的范围之间的差距,引发了对设备所有权和安全的重要讨论。WebUSB 的攻击面尤其值得关注:网页越来越有能力访问物理设备,因此一次权限授予就可能让设备被永久植入后门。 作者逆向分析了显示器的固件,试图禁用反复出现的像素清洗弹窗,但尚未冒险刷入修改后的固件,因为显示器价格昂贵且存在变砖风险。文章指出,WebUSB、WebHID 和 WebBluetooth 分别将浏览器攻击面扩展到了 USB、HID 和蓝牙设备,一旦用户接受权限提示就可能被利用。

hackernews · schlarpc · 8月23日 22:41 · [社区讨论](https://news.ycombinator.com/item?id=49413320)

**背景**: WebUSB 是一种 JavaScript API,允许网页应用直接从浏览器安全地访问 USB 设备,目前受基于 Chromium 的浏览器支持。硬件后门是嵌入设备固件或硬件中的恶意修改,难以检测,并且能抵御系统重装或磁盘擦除。这篇文章正是这两个概念的交汇点:远程网页代码获得对物理设备的底层控制,以及验证固件实际行为的困难。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebUSB">WebUSB - Wikipedia</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/WebUSB_API">WebUSB API - Web APIs | MDN</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hardware_backdoor">Hardware backdoor</a></li>

</ul>
</details>

**社区讨论**: 评论区反应热烈,有用户指出 LLM 让逆向工程变得容易得多:有人用 AI 代理在几小时内逆向出一种小众设备笔记文件格式;还有人感叹 LLM 带来了开源运动只敢梦想的“软硬件自由”。也有人表达现实顾虑,比如尝试给路由器打固件补丁时将其变砖。讨论中反复提到的一个关键警示是:一次 WebUSB 权限提示就可能让设备被永久植入后门。

**标签**: `#reverse-engineering`, `#firmware`, `#security`, `#hardware-hacking`, `#webusb`

---

<a id="item-3"></a>
## [Anthropic 最好的 AI 模型难以吸引用户，而更便宜的替代品蓬勃发展](https://www.ft.com/content/5ee49718-c258-4f01-aa32-7e5b76ae5245) ⭐️ 8.0/10

Anthropic 的前沿 AI 模型面临采用挑战，因为用户更倾向于更便宜的替代品，社区讨论指出了其变现失误、安全开销和企业功能缺口等问题。

hackernews · naves · 8月23日 18:16 · [社区讨论](https://news.ycombinator.com/item?id=49411102)

**标签**: `#Anthropic`, `#AI adoption`, `#pricing strategy`, `#enterprise AI`, `#LLM market`

---

<a id="item-4"></a>
## [17 万非营利组织数据全丢：微软该负责吗？](https://slate.com/technology/2026/08/microsoft-software-nonprofit-data-delete.html) ⭐️ 8.0/10

据 Slate 报道，超过 17 万个非营利组织丢失了全部数据，引发了对微软云数据保留做法及其责任的质疑。 这一事件凸显了依赖云提供商存储数据的风险，以及保留策略失效时可能产生的后果。它对技术资源有限、可能无法独立备份的非营利组织影响尤甚，并可能促使组织要求更强有力的供应商保障。 根据微软官方文档，许可证到期后数据应保留 90 天，但受影响的非营利组织报告称数据完全丢失。具体根本原因以及 90 天保留政策是否被违反尚不清楚。

hackernews · tchalla · 8月23日 18:55 · [社区讨论](https://news.ycombinator.com/item?id=49411395)

**背景**: 像 Microsoft 365 这样的云提供商通常会提供数据保留策略和服务水平协议（SLA），其中规定了备份频率、保留期和恢复目标。然而，在许多情况下，数据备份的最终责任在于客户，单纯依赖提供商侧的保留策略可能带来风险。非营利组织通常通过捐赠计划使用 Microsoft 365，因此对微软的基础设施和政策产生依赖。这一事件是研究独立备份重要性和了解 SLA 限制的典型案例。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/microsoft-365/content-management-solutions/data-retention">Data Retention: Content Governance Strategies | Microsoft 365</a></li>
<li><a href="https://www.filecloud.com/blog/data-retention-policy-best-practices/">Data Retention Policy: 10 Best Practices</a></li>
<li><a href="https://www.contractscounsel.com/t/us/cloud-service-level-agreement">What's a Cloud Service Level Agreement? (Sample)</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍对微软持批评态度，有人称该公司和整个行业“不靠谱”。还有评论者质疑，既然微软文档规定了 90 天保留期，为何仍会发生数据丢失。其他评论则分享了个人遭遇微软糟糕备份机制的体验，并警告云存储的长期脆弱性。

**标签**: `#data-loss`, `#microsoft`, `#cloud`, `#nonprofits`, `#reliability`

---

<a id="item-5"></a>
## [现代关系查询语言愿望清单引发 SQL 替代品讨论](https://sporks.space/2026/08/19/things-i-want-in-a-modern-relational-query-language/) ⭐️ 8.0/10

一篇题为《现代关系查询语言中我想要的东西》的文章列出了下一代查询语言的功能愿望清单，并批评了 SQL 的局限性。这篇文章引发了包含 79 条评论的活跃讨论。 这一点很重要，因为 SQL 是大多数数据系统的基础；如果 Datalog 或 EdgeQL 等替代方案获得更多关注，数据库工具链和开发者体验可能会发生显著变化。这场讨论反映了业界对更可组合、更具表现力且更易维护的查询语言的广泛兴趣。 这篇文章引发了活跃讨论，评论者引用了《Against SQL》等早期文章，并提到了 Mangle Datalog 和 GelData 的《We Can Do Better Than SQL》等具体替代方案。有评论者还指出这与早期的 Apache Spark 开发有相似之处，也有人抱怨没有语法高亮的代码块与长评论结合时难以阅读。

hackernews · zdw · 8月22日 18:38 · [社区讨论](https://news.ycombinator.com/item?id=49402491)

**背景**: 关系数据库以表格形式存储数据，通常使用 SQL 进行查询，SQL 已主导数十年。SQL 应用广泛，但因其组合性差、冗长以及递归支持薄弱而受到批评；Datalog 是一种基于 Horn 子句的声明式逻辑编程语言，被视为替代方案之一，EdgeQL 是另一个选择。这篇文章属于关于改进或替换 SQL 的长期讨论的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Datalog">Datalog</a></li>

</ul>
</details>

**社区讨论**: 评论者的讨论总体具有建设性：有人认为替代 SQL 是艰巨任务并推荐了相关文章，也有人建议尝试 Mangle 等 Datalog 实现，或指出这与早期 Spark 的相似之处。还有一条关于在缺少语法高亮时代码可读性的元评论，表明讨论者对讨论形式本身也很关注。

**标签**: `#SQL`, `#relational databases`, `#query languages`, `#datalog`, `#database systems`

---

<a id="item-6"></a>
## [Linus Torvalds 称赞坚持不懈的 AI 辅助内核调试会话](https://simonwillison.net/2026/Aug/22/linus-torvalds/) ⭐️ 7.0/10

Linus Torvalds 描述了他在 drm/xe 驱动上进行的一次 AI 辅助调试过程，指出 AI 最初称该问题不可能、无法解决，但在他坚持推动下，AI 持续添加调试代码并分析结果，最终提供了帮助。他称赞 AI 是不知疲倦的助手，甚至让 AI 撰写了提交信息。 这段引语难得地展现了顶级内核开发者对 AI 在软件调试中的实际局限与价值的真实看法。它说明在使用 AI 工具时，人的坚持和判断依然至关重要，并且即使 AI 起初放弃或过于悲观，它仍然可能提供有价值的帮助。 这次调试涉及 drm/xe 驱动，具体问题是 Intel Battlemage G21（16 GiB 显存）上把扁平 CCS 存储错误地当作可用 VRAM 分配出去。根本原因在于将内存上限向上取整后，有 2 KiB 的 CCS 压缩存储被并入分配器池中，而压缩硬件无需页表项、buffer object 或 GPU 提交，就能在用户空间存在之前覆盖这部分内存。

rss · Simon Willison · 8月22日 21:04

**背景**: drm/xe 驱动是 Intel 在 Linux 内核中较新的 Direct Rendering Manager（DRM）GPU 驱动。现代 GPU 使用压缩硬件来降低内存带宽压力，而压缩元数据（CCS）占用独立的内存区域，绝不能作为通用 VRAM 暴露给用户。Linus Torvalds 是 Linux 的创建者，也是以固执著称的维护者，这与他在调试中推动 AI 突破其自称极限的轶事十分契合。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/torvalds/linux/commit/818bebeb63dd6bf5f4e07e145f6cdbace520a34c">drm/xe: Don't hand out the flat CCS storage as usable VRAM · torvalds/linux@818bebe</a></li>
<li><a href="https://en.wikipedia.org/wiki/Direct_Rendering_Manager">Direct Rendering Manager - Wikipedia</a></li>
<li><a href="https://docs.kernel.org/gpu/xe/index.html">drm/xe Intel GFX Driver — The Linux Kernel documentation</a></li>

</ul>
</details>

**标签**: `#AI`, `#Linux`, `#debugging`, `#kernel`, `#Linus Torvalds`

---

<a id="item-7"></a>
## [不止于代码审查：精通 AI 编程代理](https://simonwillison.net/2026/Aug/22/more-than-just-code-review/) ⭐️ 7.0/10

Simon Willison 发表了一篇博客文章，指出高效使用编程代理的关键在于自信地指示修改并验证结果，而非总是逐行审查代码。他认为逐行审查并非始终最有效的验证方式。 这一观点很重要，因为它重新定义了开发者与 AI 编程代理协作的方式，将重心从繁琐的手工审查转向基于结果的验证。它可能影响团队采用 AI 辅助开发的模式，并塑造 agentic engineering（代理工程）的最佳实践。 文章明确指出，有时逐行审查是必要的，但也强调了其他验证策略的价值。Willison 的论点适用于生成式 AI 编程工具及更广泛的 agentic engineering（代理工程）领域。

rss · Simon Willison · 8月22日 15:56

**背景**: 编程代理（coding agents）是基于自然语言指令自主编写或修改代码的 AI 系统。Agentic engineering（代理工程）是一门新兴学科，将自主 AI 代理与人类高层指导及验证相结合，Grokipedia 的相关文章对此有详细阐述。传统代码审查仍是常见做法，但随着 AI 代理能力提升，开发者正在探索更高效的输出验证方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Agentic_Engineering">Agentic Engineering</a></li>
<li><a href="https://www.linkedin.com/pulse/agentic-engineering-from-code-workflows-regie-san-juan-sjyyc">Agentic Engineering : From Code to Workflows</a></li>

</ul>
</details>

**标签**: `#coding-agents`, `#code-review`, `#AI`, `#LLMs`, `#agentic-engineering`

---