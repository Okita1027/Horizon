---
layout: default
title: "Horizon 日报：2026-08-26 (ZH)"
date: 2026-08-26
lang: zh
---

> 从 48 条内容中筛选出 12 条重要资讯。

---

1. [苹果发布 M6 与 M5 Ultra，性能和 AI 算力大幅跃升](#item-1) ⭐️ 9.0/10
2. [OpenAI Jalapeño 芯片据称超越英伟达 Blackwell](#item-2) ⭐️ 9.0/10
3. [FDA 批准首款可监测酮体和血糖水平的可穿戴设备](#item-3) ⭐️ 8.0/10
4. [苹果发布搭载 M5 Max 和 M5 Ultra 的新款 Mac Studio](#item-4) ⭐️ 8.0/10
5. [Nitter 收到停止函后关停，隐私访问 X 受阻](#item-5) ⭐️ 8.0/10
6. [PostgreSQL 19 新增 WAIT FOR 命令，实现读写一致性](#item-6) ⭐️ 8.0/10
7. [EVE Online 启动从 Stackless Python 2.7 到 Python 3 的期待已久的迁移](#item-7) ⭐️ 8.0/10
8. [depesz 探索 PostgreSQL 正则表达式新扩展 pg_tre 和 pg_re2](#item-8) ⭐️ 7.0/10
9. [无法建索引时的 PostgreSQL 查询优化](#item-9) ⭐️ 7.0/10
10. [PostgreSQL 场景树测试：用保存点在提交前共享分支历史](#item-10) ⭐️ 7.0/10
11. [碎片：8 月 24 日](#item-11) ⭐️ 7.0/10
12. [SQLite 数据库可直接作为 Linux 可执行文件](#item-12) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [苹果发布 M6 与 M5 Ultra，性能和 AI 算力大幅跃升](https://www.apple.com/newsroom/2026/08/apple-introduces-m6-and-m5-ultra-for-a-big-leap-in-performance-and-ai-compute/) ⭐️ 9.0/10

苹果于 2026 年 8 月 25 日发布了 M6 和 M5 Ultra 芯片。M6 是苹果首款 2nm 芯片，采用 12 核 CPU、12 核 GPU 和双 16 核神经引擎；M5 Ultra 则首次采用四芯片（quad-die）架构，是苹果迄今最强大的芯片。 这一发布标志着苹果在将 AI 计算带到消费级硬件方面迈出一大步，M5 Ultra 宣称峰值 AI 性能较 M3 Ultra 提升最高 4.3 倍。这可能对高通、AMD 等竞争对手形成压力，并影响未来 Mac 产品线规划；有报道称苹果可能集中资源开发以 AI 为核心的 M7 芯片。 M6 将首发于新款 Mac mini，M5 Ultra 则驱动更新的 Mac Studio，最高配备 36 核 CPU、80 核 GPU、1.2TB/s 统一内存带宽、32 核神经引擎，视频编解码模块数量为 M5 Max 的两倍。高端机型价格上涨明显，据称顶配 Mac Studio 售价约达 24,699 美元。

hackernews · interpol_p · 8月25日 13:01 · [社区讨论](https://news.ycombinator.com/item?id=49433292)

**背景**: 苹果 M 系列芯片是 ARM 架构的片上系统（SoC），自 2020 年起逐步取代 Mac 中的 Intel 处理器。神经引擎（Neural Engine）是苹果为机器学习设计的专用 AI 加速器，于 2017 年首次推出，可处理卷积、矩阵乘法等神经网络运算。M6 标志着苹果采用台积电 2nm 制程，而 M5 Ultra 通过四芯片（quad-die）设计，将多个芯片封装在一起以扩展性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.apple.com/newsroom/2026/08/apple-introduces-m6-and-m5-ultra-for-a-big-leap-in-performance-and-ai-compute/">Apple introduces M6 and M5 Ultra for a big leap in performance and AI compute - Apple</a></li>
<li><a href="https://www.macrumors.com/2026/08/25/apple-debuts-m5-ultra/">Apple Debuts M5 Ultra as Most Powerful Chip Ever - MacRumors</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_M6">Apple M 6 - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论区对性能跃升与价格上涨反应不一：有人认为按通胀调整后，价格已回到早期 Mac SE/30 的水平，却能毫不费力地通过图灵测试；也有多位用户提到彭博社报道称苹果可能跳过 M6 Pro、Max 和 Ultra 版本，集中精力打造专注 AI 的 M7。还有用户计算出顶配 M5 Ultra Mac Studio 售价可能达到 24,699 美元。

**标签**: `#Apple`, `#M6`, `#M5 Ultra`, `#AI compute`, `#hardware`

---

<a id="item-2"></a>
## [OpenAI Jalapeño 芯片据称超越英伟达 Blackwell](https://newsletter.semianalysis.com/p/openai-jalapeno-better-than-nvidia) ⭐️ 9.0/10

据报道，OpenAI 与博通（Broadcom）合作推出了首款自研 AI 推理芯片 Jalapeño，并声称其在测试中优于英伟达 Blackwell 处理器。该芯片以整片掩模版大小的 ASIC 形式在短短九个月内完成开发。 如果这一说法属实，可能会打破英伟达在 AI 硬件领域的主导地位，并标志着行业向定制化、专用推理芯片的重大转变。这还表明 OpenAI 正通过垂直整合基础设施来降低成本并提升 ChatGPT 等模型的推理性能。 Jalapeño 是与博通合作打造的 LLM 推理 ASIC，与 OpenAI 到 2029 年 10GW 基础设施承诺相关。评论者指出，其芯片尺寸与英伟达 Rubin 大致相当，但 NVFP4 PFLOPS 约为后者三分之一，而 FP4 等低精度也体现了速度与精度之间的权衡。

hackernews · bmulholland · 8月25日 14:06 · [社区讨论](https://news.ycombinator.com/item?id=49434378)

**背景**: 英伟达 Blackwell 架构是用于数据中心 AI 加速器的 GPU 微架构，采用定制 TSMC 4NP 工艺制造，包含 2080 亿个晶体管。OpenAI 此举反映了大型 AI 实验室更广泛的趋势：为推理任务开发定制芯片（ASIC），而非依赖通用 GPU，以在大规模运行中降低成本并减少延迟。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.stork.ai/blog/jalapeo-openais-nvidia-killer">OpenAI 's Jalapeño Chip : A Custom ASIC to Challenge... | Stork.AI</a></li>
<li><a href="https://www.spheron.network/blog/openai-jalapeno-chip-gpu-cloud-inference-2026/">OpenAI Jalapeño Chip Explained: What OpenAI 's First Custom ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Blackwell_(microarchitecture)">Blackwell (microarchitecture) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者将早期推理芯片市场比作 3dfx、Riva 和 PowerVR 时代，并讨论专用芯片能否长期胜出。有人指出，按每 token 能耗计算，人类大脑仍比 AI 高效 22 倍；也有人认为硬件快速进步将使 token 价格继续大幅下降。

**标签**: `#AI hardware`, `#OpenAI`, `#Nvidia`, `#semiconductors`, `#inference`

---

<a id="item-3"></a>
## [FDA 批准首款可监测酮体和血糖水平的可穿戴设备](https://www.fda.gov/news-events/press-announcements/fda-authorizes-first-wearable-device-continuously-monitors-both-ketone-levels-and-blood-sugar) ⭐️ 8.0/10

FDA 批准了首款可连续监测酮体和血糖水平的可穿戴设备，标志着糖尿病管理技术的重大进步。

hackernews · sunnynagra · 8月25日 19:07 · [社区讨论](https://news.ycombinator.com/item?id=49439017)

**标签**: `#FDA`, `#wearables`, `#health technology`, `#diabetes`, `#glucose monitoring`

---

<a id="item-4"></a>
## [苹果发布搭载 M5 Max 和 M5 Ultra 的新款 Mac Studio](https://www.apple.com/newsroom/2026/08/apple-introduces-new-mac-studio-with-m5-max-and-m5-ultra/) ⭐️ 8.0/10

2026 年 8 月 25 日，苹果发布了搭载 M5 Max 和 M5 Ultra 芯片的新款 Mac Studio，最高支持 1.2TB/s 内存带宽，并将本地 AI 性能作为重点。 这款产品让专业人士可以在桌面端获得高带宽统一内存和强大的 AI 算力，可能让他们直接在本地运行大型语言模型，而无需依赖云端服务。这也巩固了苹果在本地 AI 硬件竞赛中的地位。 M5 Ultra 由两颗 M5 Max 芯片通过 4.4TB/s 的芯片间互联组成，峰值 AI 性能最高达 M3 Ultra 的 4.3 倍，图形性能提升 1.8 倍。新款 Mac Studio 首发最高提供 256GB 统一内存，512GB 版本预计稍后推出。

hackernews · interpol_p · 8月25日 13:03 · [社区讨论](https://news.ycombinator.com/item?id=49433316)

**背景**: Mac Studio 是苹果面向专业人士的高端台式电脑，主打 CPU、GPU 和内存性能。其统一内存架构让 CPU 和 GPU 共享同一块高带宽内存池，这对于需要几十甚至上百 GB 容量的大型 AI 模型尤为关键。苹果一直将 M 系列芯片定位为可在本地运行 AI 模型的平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.macrumors.com/2026/08/25/apple-debuts-m5-ultra/">Apple Debuts M 5 Ultra as Most Powerful Chip Ever - MacRumors</a></li>
<li><a href="https://www.apple.com/newsroom/2026/08/apple-introduces-m6-and-m5-ultra-for-a-big-leap-in-performance-and-ai-compute/">Apple introduces M6 and M 5 Ultra for a big leap in performance and...</a></li>
<li><a href="https://support.apple.com/en-us/126318">MacBook Pro (14-inch, M 5 Pro or M 5 Max ) - Tech... - Apple Support</a></li>

</ul>
</details>

**社区讨论**: 不少评论者对价格表示不满，认为 256GB 配置价格高昂，并指出新闻稿中频繁使用“最高可达”（up to）这一表述。也有用户对本地 AI 前景感到乐观，一位用户估算，在 M5 Ultra 上运行未量化的千亿参数模型，预填充速度可达每秒 1000+ tokens，生成速度约每秒 50+ tokens，接近云端水平。

**标签**: `#Apple`, `#Mac Studio`, `#M5 chip`, `#local AI`, `#hardware`

---

<a id="item-5"></a>
## [Nitter 收到停止函后关停，隐私访问 X 受阻](https://github.com/zedeus/nitter/issues/1442) ⭐️ 8.0/10

Nitter 项目宣布收到停止函（cease-and-desist），目前正在等待法律意见，所有 Nitter 实例预计将在可预见的未来保持下线。开发工作也已暂时停止。 此事破坏了一种被广泛使用的、无需登录、无追踪、无广告浏览 X/Twitter 的隐私保护方式，影响记者、研究人员和受限制环境中的用户。它还引发了对开源和隐私工具面临法律压力的更广泛担忧，以及对公共对话平台访问权的讨论。 最初的公告只提供了很少细节，仅表示已收到停止函，并将在获得法律意见前让所有实例保持下线。Nitter 仅支持浏览，不能用于登录、发帖或与社区互动，同时它还为 Twitter 个人资料提供 RSS 订阅源。

hackernews · Banditoz · 8月25日 17:08 · [社区讨论](https://news.ycombinator.com/item?id=49437283)

**背景**: Nitter 是一个免费开源的 Twitter（现为 X）替代前端，让用户无需登录、不被追踪、不看广告就能查看个人资料、推文、回复、媒体和搜索结果。许多用户依赖公开的 Nitter 实例，因为 X 对未登录用户和第三方客户端的访问限制越来越严格。该项目关停之前，X 已在持续收紧对其内容查看和使用方式的控制，包括对 AI 公司的限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Nitter">Nitter</a></li>
<li><a href="https://grokipedia.com/page/Nitter">Nitter</a></li>
<li><a href="https://nitter.net/">nitter.net</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，包括地方议会在内的许多组织仍将 X 作为主要沟通渠道，这使得一些用户无法再关注它们。有人建议中等强国应为这类项目提供法律保护，并提及美国科技产业的影响力；也有人质疑 X 是否仍具重要性，并猜测这次停止函的动机可能是 AI 公司利用 Nitter 和 xcancel 抓取推文内容。

**标签**: `#privacy`, `#open-source`, `#legal`, `#twitter`, `#nitter`

---

<a id="item-6"></a>
## [PostgreSQL 19 新增 WAIT FOR 命令，实现读写一致性](https://postgr.es/p/9ta) ⭐️ 8.0/10

PostgreSQL 19 引入了新的 SQL 命令 WAIT FOR，该命令会阻塞会话，直到写入前日志（WAL）达到指定的 LSN（日志序列号）。这允许在异步副本上实现写后读一致性，而无需承担同步复制的开销。 该特性为需要在副本上立即看到自身写入的应用程序提供了一种实用的同步复制替代方案。它降低了与同步复制相关的延迟和稳定性问题，同时仍为写后读场景提供了更强的一致性保证。 WAIT FOR 命令接受目标 LSN 和可选参数，如 MODE、TIMEOUT 和 NO_THROW（例如：WAIT FOR LSN 'lsn' WITH (MODE 'mode', TIMEOUT 'timeout', NO_THROW)）。它允许会话等待 WAL 重放到特定点，并可配置处理超时或错误的行为。

rss · Planet PostgreSQL · 8月25日 00:00

**背景**: 在 PostgreSQL 中，写入前日志（WAL）是确保数据完整性的标准方法；所有更改都在应用到数据文件之前记录到日志中。LSN（日志序列号）是一个 64 位整数，表示 WAL 流中的字节位置；同步复制要求主库等待备库确认收到 WAL，这会增加延迟。异步复制则不等待，因此副本可能落后于主库，破坏写后读一致性。新的 WAIT FOR 命令允许会话显式等待，直到 WAL 在副本上重放到所需的 LSN，从而在不强制使用同步复制的情况下提供这种一致性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/wal-intro.html">PostgreSQL: Documentation: 18: 28.3. Write-Ahead Logging (WAL)</a></li>
<li><a href="https://postgrespro.com/docs/postgresql/9.6/datatype-pg-lsn">PostgreSQL : Documentation: 9.6: 8.19. pg_ lsn Type</a></li>
<li><a href="https://www.geeksforgeeks.org/system-design/read-your-writes-consistency-in-system-design/">Read - your - Writes Consistency in System Design - GeeksforGeeks</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#WAL`, `#replication`, `#read-your-writes`, `#SQL`

---

<a id="item-7"></a>
## [EVE Online 启动从 Stackless Python 2.7 到 Python 3 的期待已久的迁移](https://simonwillison.net/2026/Aug/25/eve-online-move-to-python-3/) ⭐️ 8.0/10

EVE Online 宣布已开始将其 240 万行服务器代码从 Stackless Python 2.7 迁移到 Python 3，首先使用自动化脚本 futurize。随后团队将手动审查约 2 万个 Python 2 与 Python 3 行为差异之处。 这是生产环境中规模最大、运行时间最长的 Python 代码库之一的标志性迁移，为脱离 Python 2 提供了真实可参考的方案。它也凸显了整个行业放弃 Python 2 的压力，以及替换 Stackless 等自定义运行时的挑战。 公告未说明 EVE Online 将如何替代 Stackless Python，但去年团队介绍了在 EVE Frontier 中使用开源的 carbonengine/scheduler 库替换 Stackless 的经验。行为差异的例子包括整数除法：在 Python 2 中 1 / 2 返回 0，而在 Python 3 中返回 0.5。

rss · Simon Willison · 8月25日 22:59

**背景**: Stackless Python 是 Python 解释器的一个分支，增加了称为 tasklet 的微线程，使程序无需操作系统线程即可实现大规模并发。EVE Online 自 2003 年起使用它，上一次重大升级是在 2010 年升级到 Stackless Python 2.7。futurize 工具基于 Python 自带的 2to3 重写机制，可自动将过时的 Python 2 写法重写为对 Python 2 和 Python 3 都兼容的形式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.eveonline.com/news/view/the-move-to-python-3-begins">The Move to Python 3 Begins! | EVE Online</a></li>
<li><a href="https://en.wikipedia.org/wiki/Stackless_Python">Stackless Python - Wikipedia</a></li>
<li><a href="https://wiki.python.org/moin/StacklessPython">StacklessPython</a></li>

</ul>
</details>

**标签**: `#Python`, `#migration`, `#Stackless`, `#EVE Online`, `#software engineering`

---

<a id="item-8"></a>
## [depesz 探索 PostgreSQL 正则表达式新扩展 pg_tre 和 pg_re2](https://postgr.es/p/9tb) ⭐️ 7.0/10

Hubert 'depesz' Lubaczewski 发表了一篇博客文章，使用 explain.depesz.com 的真实查询计划数据来测试 PostgreSQL 新的正则表达式扩展 pg_tre 和 pg_re2。他指出这些扩展其实几个月前就有了，只是他现在才抽空研究。 这些扩展为 PostgreSQL 带来了替代的正则表达式引擎（TRE 和 RE2），相比内置的 Henry Spencer 实现，可能提供更快或功能不同的模式匹配。这位知名 PostgreSQL 专家的实用评测有助于开发者决定是否在文本密集型工作负载中采用它们。 文章使用从 explain.depesz.com 数据库提取并创建的 all_plans 侧表作为测试数据。虽然 pg_tre 和 pg_re2 并非全新，但它们仍是相对较新的扩展，需要安装，并且与核心正则表达式功能相比可能存在一些限制。

rss · Planet PostgreSQL · 8月25日 18:41

**背景**: PostgreSQL 的默认正则表达式支持由 Henry Spencer 的 regex 库实现。像 pg_tre 和 pg_re2 这样的扩展将其他著名正则表达式引擎（TRE 和 Google 的 RE2）集成到数据库中，它们各自具有不同的性能特点和功能集。这篇博客文章使用真实数据进行了动手探索，展示了这些扩展在实际中的表现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://production-marketing-website.vercel.app/blog/introducing-pg_re2-regex-in-postgres">Introducing pg _ re 2 , fast, RE 2 -powered regular expressions in...</a></li>
<li><a href="https://www.postgresql.org/docs/current/functions-matching.html">PostgreSQL : Documentation: 18: 9.7. Pattern Matching</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#regular expressions`, `#pg_re2`, `#pg_tre`, `#extensions`

---

<a id="item-9"></a>
## [无法建索引时的 PostgreSQL 查询优化](https://postgr.es/p/9t9) ⭐️ 7.0/10

Henrietta Dombrovskaya 在 Postgres 上发文，讲述如何优化 PostgreSQL 13.6 生产环境中的一条查询，该查询扫描 750GB、160 亿行的表。由于创建 GIST 索引需超过 24 小时，且现有索引都不匹配该查询，她提出在 start_date 上增加额外约束条件。 这很重要，因为数据库从业者经常面临无法实际建索引的现实约束，尤其是在超大表上。文章提供了一种基于数据分布和基于成本的规划器的实用优化思路，无需修改表结构。 目标查询同时过滤 a、b、c 三个列，并用 start_date 和 end_date 判断某个日期是否落在区间内；选择性最高的 end_date 没有以它开头的索引，而现有的(a, start_date, end_date)索引又因 a 选择性低而效果不佳。文章提出的方案是下推一个“实际 start_date 不会太早”的附加谓词，不过原文在展示完整结果前被截断。

rss · Planet PostgreSQL · 8月25日 11:50

**背景**: PostgreSQL 使用基于成本的查询规划器，它会估算不同执行计划的成本并选择最优者，对高选择性的过滤条件通常会优先选择索引扫描。GIST 索引支持通用搜索结构，可以索引 daterange 等范围类型，但在数十亿行上构建这种索引耗时很长且会锁表。即使 CREATE INDEX CONCURRENTLY 可以减少阻塞，如此巨大的表规模仍使建索引不现实，因此基于查询重写的优化方法很有价值。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/runtime-config-query.html">PostgreSQL: Documentation: 18: 19.7. Query Planning</a></li>
<li><a href="https://pganalyze.com/docs/explain/basics-of-postgres-query-planning">The Basics of Postgres Query Planning · pganalyze</a></li>
<li><a href="https://www.postgresql.org/docs/current/sql-createindex.html">PostgreSQL : Documentation: 18: CREATE INDEX</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#query-optimization`, `#performance`, `#databases`

---

<a id="item-10"></a>
## [PostgreSQL 场景树测试：用保存点在提交前共享分支历史](https://postgr.es/p/9t8) ⭐️ 7.0/10

这篇文章提出了一种 PostgreSQL 场景树测试方法：把业务逻辑的分支场景表示成目录树，并用保存点遍历，使每个分支继承共享的初始状态。测试在未提交的部署事务中运行，只有所有预设场景通过时才提交部署。 该方法消除了数据库测试中重复的初始化工作，让每个场景都能基于其真实父状态运行，而无需重建状态。对于生命周期复杂、有状态的数据库应用尤其有价值，同时还能与事务性 DDL 自然结合，让迁移测试更安全、更高效。 该遍历会让每个预设场景从它实际依赖的父状态开始运行，同时各分支之间互不可见。由于 PostgreSQL 的大部分 DDL 是可事务的，整个遍历可以在一个尚未提交的部署事务中执行；若有场景失败，则丢弃所有测试状态。

rss · Planet PostgreSQL · 8月25日 00:00

**背景**: PostgreSQL 中的保存点允许事务部分回滚到某个标记点，从而让多个测试分支共享初始化工作。场景测试用贴近现实的故事式场景来验证复杂行为，而基于树形的遍历则是覆盖层级逻辑路径的常见方法。作者将这些思想结合起来：人工编写的分支、通过保存点共享历史，以及在单个事务内全部通过后再提交。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/sql-savepoint.html">PostgreSQL : Documentation: 18: SAVEPOINT</a></li>
<li><a href="https://en.wikipedia.org/wiki/Scenario_testing">Scenario testing - Wikipedia</a></li>
<li><a href="https://andyatkinson.com/blog/2024/07/22/postgresql-savepoints">You make a good point! — PostgreSQL Savepoints</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#testing`, `#database`, `#savepoints`, `#scenario-tree`

---

<a id="item-11"></a>
## [碎片：8 月 24 日](https://martinfowler.com/fragments/2026-08-24.html) ⭐️ 7.0/10

Martin Fowler 反思了 AI 代理在内部协调时无需人工检查的现象，并引用了 Ezra Klein 与 Helen Toner 关于 OpenAI 黑客事件的讨论。

rss · Martin Fowler · 8月24日 15:29

**标签**: `#AI safety`, `#AI agents`, `#OpenAI`, `#alignment`, `#cybersecurity`

---

<a id="item-12"></a>
## [SQLite 数据库可直接作为 Linux 可执行文件](https://simonwillison.net/2026/Aug/24/your-executable-is-a-sqlite-database/) ⭐️ 7.0/10

Farid Zakaria 展示了一种技术，通过在文件偏移 68 处将 SQLite 的 application ID 设为 'SELF'，并把 ELF 组件存储到多个 SQLite 表中，使 SQLite 数据库文件可以直接作为 Linux 可执行文件运行。配合 'self-exec' 解释器和 binfmt_misc 内核注册机制，该数据库即可作为程序执行。 该技术巧妙地将 SQLite 文件格式与 ELF 可执行格式结合在一起，为在数据库文件中嵌入可执行代码带来了新颖且有创意的应用场景。虽然算不上重大变革，但它展现了两种格式的灵活性，并可能激发更多关于多格式（polyglot）文件的实验。 SQLite 文件偏移 68 字节处的 4 字节 application ID 被设置为 'SELF'（Structured Executable & Linkable Format）。ELF 组件按提供的 schema 存放在多个 SQLite 表中，self-exec C 解释器负责提取并执行它们；在非 NixOS 系统上，可通过向 /proc/sys/fs/binfmt_misc/register 写入如上命令行来注册 binfmt_misc。

rss · Simon Willison · 8月24日 11:38

**背景**: ELF（Executable and Linkable Format）是 Linux 上可执行文件和共享库的标准二进制格式。SQLite 是一种广泛使用的嵌入式数据库，其文件格式包含一个 application_id 字段，用于标识拥有该数据库文件的应用程序。binfmt_misc 是 Linux 内核的一项功能，允许用户注册自定义二进制格式（通过魔数识别）并交给用户空间解释器处理。这个技巧将三者结合，让内核把 SQLite 数据库当作可执行文件来运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Binfmt_misc">binfmt _ misc - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Executable_and_Linkable_Format">Executable and Linkable Format - Wikipedia</a></li>
<li><a href="https://sqlite.org/forum/info/6a768e7dca11a7b2">SQLite User Forum: Usage of application_id and magic.txt</a></li>

</ul>
</details>

**标签**: `#SQLite`, `#Linux`, `#ELF`, `#binfmt_misc`, `#hack`

---