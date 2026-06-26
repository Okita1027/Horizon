---
layout: default
title: "Horizon 日报：2026-06-26 (ZH)"
date: 2026-06-26
lang: zh
---

> 从 46 条内容中筛选出 9 条重要资讯。

---

1. [首次利用 AI 完整阅读赫库兰尼姆卷轴](#item-1) ⭐️ 10.0/10
2. [Zig 重定义 bitCast 语义并改进 LLVM 后端](#item-2) ⭐️ 8.0/10
3. [德国裁定：谷歌对 AI 概览错误承担责任](#item-3) ⭐️ 8.0/10
4. [用 Rust 重写的 PostgreSQL 备份工具 WAL-G：WAL-RUS](#item-4) ⭐️ 8.0/10
5. [科技博客先驱 Om Malik 去世，享年 60 岁](#item-5) ⭐️ 7.0/10
6. [强制在线身份验证威胁隐私](#item-6) ⭐️ 7.0/10
7. [PostgreSQL 19 中使用 SQL/PGQ 进行异构图查询](#item-7) ⭐️ 7.0/10
8. [AI 代理架构：规划、工具与反思](#item-8) ⭐️ 7.0/10
9. [LLM 生成的求职申请侵蚀真实性](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [首次利用 AI 完整阅读赫库兰尼姆卷轴](https://scrollprize.org/firstscroll) ⭐️ 10.0/10

研究人员首次利用 AI 和先进的 3D 成像技术，在不展开的情况下完整阅读了赫库兰尼姆卷轴 PHerc. 1667 的文本。 这一突破表明，AI 可以从碳化卷轴中解锁失传的古代文本，有望从唯一完整保存的古代图书馆中恢复数百部作品。 该卷轴通过显微 CT 扫描和机器学习模型进行数字展开，模型经过训练可检测碳化纸莎草上的墨水；完整的幸存文本（约 22 列）已由纸莎草学家审阅。

hackernews · verditelabs · 6月25日 15:48 · [社区讨论](https://news.ycombinator.com/item?id=48675179)

**背景**: 赫库兰尼姆卷轴是公元 79 年维苏威火山喷发掩埋的 1800 多卷碳化纸莎草卷轴，主要包含希腊哲学文本，尤其是伊壁鸠鲁学派作品。2023 年发起的“维苏威挑战赛”以奖金悬赏，鼓励使用非破坏性 AI 技术阅读这些卷轴。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://scrollprize.org/firstscroll">An entire Herculaneum scroll has been read for the first time</a></li>
<li><a href="https://en.wikipedia.org/wiki/Herculaneum_scrolls">Herculaneum scrolls</a></li>
<li><a href="https://scrollprize.org/">Vesuvius Challenge</a></li>

</ul>
</details>

**社区讨论**: 社区成员对这一成就表示惊叹，一位维苏威挑战赛团队成员主动回答问题，另一人指出该遗址仅发掘了 20%，暗示还有更多卷轴等待发现。总体情绪极为积极，强调该项目与科技商业化形成鲜明对比，具有鼓舞人心的意义。

**标签**: `#AI`, `#archaeology`, `#herculaneum`, `#machine learning`, `#historical preservation`

---

<a id="item-2"></a>
## [Zig 重定义 bitCast 语义并改进 LLVM 后端](https://ziglang.org/devlog/2026/#2026-06-25) ⭐️ 8.0/10

Zig 为其 @bitCast 内置函数引入了新的端序无关语义，使得该操作在所有目标上行为一致，不受端序影响。此外，LLVM 后端也进行了优化，以提高底层代码的性能。 这一变化简化了编写可移植底层代码的工作，例如处理二进制文件格式或网络协议，无需手动处理端序问题。同时它也增强了 Zig 在系统编程领域的吸引力，因为性能和可移植性至关重要。 在新语义下，例如将 [2]u8 位转换为 u16，在大端和小端目标上都会产生相同的逻辑结果。该更改还与现有的 packed struct 逻辑集成，改进了对位打包二进制头部的处理。

hackernews · kouosi · 6月25日 14:19 · [社区讨论](https://news.ycombinator.com/item?id=48673825)

**背景**: 端序是指多字节数据类型在内存中存储的字节顺序。许多语言中传统的 bitCast 操作依赖于目标的端序，导致代码不可移植。Zig 的新语义重新解释逻辑位而不考虑字节顺序，使代码在各平台上保持一致。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ziglang.org/devlog/2026/">Devlog ⚡ Zig Programming Language</a></li>
<li><a href="https://news.ycombinator.com/item?id=48673825">Zig's New BitCast Semantics and LLVM Back End Improvements | Hacker News</a></li>
<li><a href="https://github.com/ziglang/zig/issues/19755">Proposal: initial `@bitCast` semantics (packed + vector + array) · Issue #19755 · ziglang/zig</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了强烈赞同，用户指出这一更改加上现有的 packed struct 逻辑将简化处理位打包二进制头部的工作。但也有部分用户质疑任意宽度整数的复杂性，认为为了清晰起见更倾向于手动打包。

**标签**: `#Zig`, `#bitcasting`, `#compiler`, `#endianness`, `#systems programming`

---

<a id="item-3"></a>
## [德国裁定：谷歌对 AI 概览错误承担责任](https://simonwillison.net/2026/Jun/25/ai-and-liability/#atom-everything) ⭐️ 8.0/10

德国法院裁定，谷歌需对其 AI 概览中的虚假信息承担责任，将 AI 生成的摘要视为谷歌自身的表述。Bruce Schneier 认为，法律上应将 AI 代理视为其部署者的代理，以防止公司利用 AI 逃避责任。 这一里程碑式的裁决为 AI 责任设立了先例，确保公司不能通过归咎于 AI 错误来逃避责任。它对各行业 AI 的部署方式具有广泛影响，可能塑造未来的法规和企业激励结构。 德国裁决明确指出，AI 概览是谷歌自身的表述，因此公司需直接承担责任。Schneier 警告称，允许公司以 AI 出错为由逃避责任，将催生灾难性激励，例如用更廉价、无需担责的 AI 系统替代人类员工。

rss · Simon Willison · 6月25日 22:28

**背景**: AI 概览是谷歌搜索的一项功能，可根据搜索结果生成 AI 编写的摘要，但因不准确和传播错误信息而饱受批评。德国裁决回应了当 AI 产生错误输出时谁应承担法律责任的问题——随着 AI 代理变得更加自主并在商业领域广泛使用，这是一个关键问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Google_AI_overviews">Google AI overviews</a></li>
<li><a href="https://agentliability.co/">Agent Liability . Global Desk on AI Agent Law and Operator Duty</a></li>

</ul>
</details>

**标签**: `#AI liability`, `#legal`, `#AI ethics`, `#Google`, `#Bruce Schneier`

---

<a id="item-4"></a>
## [用 Rust 重写的 PostgreSQL 备份工具 WAL-G：WAL-RUS](https://www.reddit.com/r/PostgreSQL/comments/1ufjlbo/why_we_rewrote_walg_for_postgres_backups_in_rust/) ⭐️ 8.0/10

作者介绍了 WAL-RUS，这是用 Rust 编程语言完全重写的 WAL-G PostgreSQL 备份工具，旨在提升性能和内存安全性。 这次重写通过利用 Rust 的安全性保障和效率，可能为数据库备份工具树立新标准，并影响其他关键基础设施工具的构建方式。 WAL-RUS 保留了 WAL-G 的核心功能，包括加密和压缩的全量及增量备份，并支持远程存储后端。重写专注于减少资源消耗并消除基于 C 语言的工具中常见的内存安全漏洞。

reddit · r/PostgreSQL · /u/Admirable_Morning874 · 6月25日 19:14

**背景**: WAL-G 是一个广泛使用的 PostgreSQL（及其他数据库）归档与恢复工具，基于 Go 语言构建。它依赖于预写式日志（WAL），这是一种通过在应用更改之前记录更改来确保数据完整性的标准方法。该工具用于生产环境中的备份和按时间点恢复。用 Rust 重写旨在兼顾性能与内存安全性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/wal-g/wal-g">GitHub - wal-g/wal-g: Archival and Restoration for databases in the Cloud · GitHub</a></li>
<li><a href="https://www.postgresql.org/docs/current/wal-intro.html">PostgreSQL: Documentation: 18: 28.3. Write-Ahead Logging (WAL)</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#Rust`, `#WAL-G`, `#backups`, `#database-tools`

---

<a id="item-5"></a>
## [科技博客先驱 Om Malik 去世，享年 60 岁](https://om.co/2026/06/24/1966-2026/) ⭐️ 7.0/10

GigaOm 创始人、科技博客先驱 Om Malik 于 2026 年 6 月 24 日去世，享年 60 岁。他的个人博客 om.co 发布了这一消息。 Om Malik 是科技新闻和博客领域的奠基人之一，以其对硅谷诚实而深刻的报道而闻名。他的去世是科技界的重大损失，他曾指导过许多人，并塑造了早期科技博客的形态。 Malik 享年 60 岁。他创立了知名科技新闻网站 GigaOm，此前曾为 Fast Company、Red Herring 和 Light Reading 撰稿，并著有《Broadbandits》一书。

hackernews · minimaxir · 6月25日 20:33 · [社区讨论](https://news.ycombinator.com/item?id=48678852)

**背景**: Om Malik 是早期最具影响力的科技博主之一，始于 20 世纪 90 年代末。他凭借 GigaOm 声名鹊起，该网站成为硅谷内部人士的必读内容。他的文章以诚实和深度著称，并且是业内许多人的导师。

**社区讨论**: 社区评论表达了震惊和悲痛，强调了 Malik 的善良、指导以及深远影响。许多评论者分享了他给予支持和坦诚反馈的个人回忆，并指出他是早期科技博客的教父。

**标签**: `#tech blogging`, `#obituary`, `#Om Malik`, `#community`, `#Silicon Valley`

---

<a id="item-6"></a>
## [强制在线身份验证威胁隐私](https://expression.fire.org/p/the-papers-please-era-of-the-internet) ⭐️ 7.0/10

文章指出，强制身份验证以访问年龄限制内容导致了一个'出示证件'的互联网，侵蚀了隐私，社区评论强调匿名凭证是潜在的技术解决方案。 随着政府推动年龄验证法律，这场辩论影响着所有互联网用户的基本隐私权，其结果可能塑造在线身份的未来架构。 匿名凭证允许选择性披露属性（例如证明年龄超过 18 岁而不透露确切出生日期），并能防止跨验证请求的关联。然而，采用需要政府支持的证书颁发机构和广泛的协议共识。

hackernews · bilsbie · 6月25日 21:44 · [社区讨论](https://news.ycombinator.com/item?id=48679608)

**背景**: 匿名凭证最早由 David Chaum 提出，是一种加密工具，允许用户证明属性（如年龄）而不泄露身份。它们支持选择性披露和不可链接性，即验证者无法将多次请求关联到同一用户。这项技术是隐私保护身份验证的核心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anonymous_credential">Anonymous credential</a></li>
<li><a href="https://blog.cryptographyengineering.com/2026/03/02/anonymous-credentials-an-illustrated-primer/">Anonymous credentials: an illustrated primer – A Few Thoughts on Cryptographic Engineering</a></li>

</ul>
</details>

**社区讨论**: 评论者大多认同隐私威胁，一些人倡导使用匿名凭证作为解决方案，另一些人质疑儿童是否确实需要持续上网。还有观点认为这个问题终于获得了应有的公众关注。

**标签**: `#privacy`, `#age verification`, `#identity`, `#internet governance`, `#anonymous credentials`

---

<a id="item-7"></a>
## [PostgreSQL 19 中使用 SQL/PGQ 进行异构图查询](https://postgr.es/p/9nk) ⭐️ 7.0/10

Hans-Juergen Schoenig 演示了如何在 PostgreSQL 19 中使用 SQL/PGQ 建模和查询异构属性图，通过添加人员-公司关系图（人员既互相认识又在公司工作）扩展了之前的示例。 SQL/PGQ 将基于标准的图查询直接引入 PostgreSQL，无需单独的图数据库即可执行复杂的关系查询。该功能对于需要遍历多种实体和关系类型的应用（如社交网络、推荐系统和欺诈检测）非常有价值。 属性图定义包括两个顶点标签（person 和 company）和两个边标签（knows 和 works_at），每个标签都有自己的属性。博客提供了六个人员、三个公司以及表示友谊和雇佣关系的边的示例数据。

rss · Planet PostgreSQL · 6月25日 05:00

**背景**: SQL/PGQ（属性图查询）是一个 SQL 标准扩展，允许使用图模式匹配语法查询属性图。PostgreSQL 19 是第一个实现该标准的版本。属性图将顶点（实体）和边（关系）与属性相结合，使得在 SQL 查询内部进行复杂的图遍历成为可能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/19/ddl-property-graphs.html">PostgreSQL: Documentation: 19: 5.15. Property Graphs</a></li>
<li><a href="https://www.postgresql.org/docs/19/queries-graph.html">PostgreSQL: Documentation: 19: 7.9. Graph Queries</a></li>
<li><a href="https://www.cybertec-postgresql.com/en/handling-graphs-with-sql-pgq-in-postgresql/">Handling graphs with SQL/PGQ in PostgreSQL</a></li>

</ul>
</details>

**标签**: `#postgresql`, `#sql-pgq`, `#graph`, `#database`

---

<a id="item-8"></a>
## [AI 代理架构：规划、工具与反思](https://postgr.es/p/9ni) ⭐️ 7.0/10

Vibhor Kumar 的博文指出，企业 AI 代理除了记忆外，还需要三种核心能力：规划、工具使用和反思，并通过 PostgreSQL 示例说明安全、可审计的代理行为。 这为构建能够可靠参与业务流程的企业代理提供了实用框架，使其从简单的问答转向具有问责制的实际行动。 该文章强调将执行计划视为可持久化、版本化和暂停以供审批的工件；警告不要让模型执行任意 SQL；并规定反思标准必须预先定义。

rss · Planet PostgreSQL · 6月24日 16:30

**背景**: AI 代理将基础模型与推理、记忆和工具使用相结合，以执行实际任务。规划涉及将目标分解为步骤，工具使用将模型与外部系统连接，反思则使代理能够自我评估和纠错。最新的调查和指南强调这些是可靠的企业代理架构所必需的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/ai-agent-planning">What is AI Agent Planning? | IBM</a></li>
<li><a href="https://www.langchain.com/blog/reflection-agents">Reflection Agents - langchain.com</a></li>
<li><a href="https://arxiv.org/html/2601.01743v1">AI Agent Systems: Architectures, Applications, and Evaluation</a></li>

</ul>
</details>

**标签**: `#AI Agents`, `#Enterprise Systems`, `#Architecture`, `#Planning`, `#Reflection`

---

<a id="item-9"></a>
## [LLM 生成的求职申请侵蚀真实性](https://simonwillison.net/2026/Jun/24/tom-macwright/#atom-everything) ⭐️ 7.0/10

Tom MacWright 观察到，由 LLM 共同编写的求职申请，包括 LLM 生成的作品集和 GitHub 项目，使候选人变得千篇一律且缺乏个性，无法揭示任何关于个人的信息。 随着 LLM 在求职申请中的广泛使用，真实性和个人品牌可能受到损害，使得雇主更难评估真正的匹配度，并可能贬低创意和技术岗位中的人类努力。 MacWright 指出，完善、生成后的简历千篇一律且缺乏个性，除了表明候选人使用了某些特定工具外，无法提供任何关于该候选人的信息。

rss · Simon Willison · 6月24日 18:13

**背景**: Tom MacWright 是一位知名的软件开发者和作家。他的博文《意外的匿名性》讨论了求职申请中 LLM 生成的内容如何导致个人身份的丧失，因为候选人依赖 AI 制作申请的所有要素。

**标签**: `#careers`, `#ai`, `#authenticity`, `#hiring`, `#llm`

---