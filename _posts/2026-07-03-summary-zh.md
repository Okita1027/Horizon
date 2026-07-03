---
layout: default
title: "Horizon 日报：2026-07-03 (ZH)"
date: 2026-07-03
lang: zh
---

> 从 38 条内容中筛选出 13 条重要资讯。

---

1. [crustc：将整个 rustc 编译器翻译为 C 语言](#item-1) ⭐️ 9.0/10
2. [美国隐私紧急：Aaronson 呼吁行动](#item-2) ⭐️ 8.0/10
3. [Linux 6.9 LUKS 挂起未擦除加密密钥](#item-3) ⭐️ 8.0/10
4. [Podman v6.0.0 发布，带来网络增强和 Quadlet](#item-4) ⭐️ 8.0/10
5. [EFF 敦促 FTC 对 X 执行同意令，涉及 Grok AI 生成 CSAM](#item-5) ⭐️ 8.0/10
6. [VS Code 1.128 Insiders 预览版发布](#item-6) ⭐️ 8.0/10
7. [使用 PDU Dropscan 的极端 PostgreSQL 勒索软件恢复](#item-7) ⭐️ 8.0/10
8. [PostgreSQL 检查点进程无限重试循环 bug](#item-8) ⭐️ 8.0/10
9. [AI 基准测试无法反映编码代理真实表现](#item-9) ⭐️ 7.0/10
10. [enable_nestloop 调优：避免嵌套循环性能灾难](#item-10) ⭐️ 7.0/10
11. [pg-healthcheck：开源 PostgreSQL 健康诊断工具](#item-11) ⭐️ 7.0/10
12. [pgcopydb v0.18 发布：包含 88 次提交的重大更新](#item-12) ⭐️ 7.0/10
13. [理解才能参与：避免认知债务](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [crustc：将整个 rustc 编译器翻译为 C 语言](https://github.com/FractalFir/crustc) ⭐️ 9.0/10

名为 crustc 的项目成功将整个 rustc 编译器翻译为 C 语言，使其无需 LLVM 或 GCC，即可由任何 C 编译器编译。 这一突破解决了 Rust 的引导编译问题，使得没有 LLVM/GCC 支持的旧式或小众硬件只需使用 C 编译器即可运行 Rust。 该项目是已知的第 14 次将 Rust 编译为 C 的尝试，其主要目标是支持缺少 LLVM 或 GCC 后端的硬件目标。

hackernews · Philpax · 7月2日 22:57 · [社区讨论](https://news.ycombinator.com/item?id=48768464)

**背景**: 编译器引导编译是指使用编译器所编译语言的最小子集来构建编译器的过程。Rust 目前需要已有的 Rust 编译器或 LLVM 才能构建，这为新平台带来了鸡生蛋蛋生鸡的问题。将 rustc 翻译为 C 可以利用无处不在的 C 工具链来打破这种依赖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/FractalFir/crustc">crustc: entirety of `rustc`, translated to C - GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Compiler_bootstrapping">Compiler bootstrapping</a></li>
<li><a href="https://gab.ae/news/crustc-entirety-of-rustc-translated-to-c-2026">crustc: entirety of `rustc`, translated to C | GAB adventures</a></li>

</ul>
</details>

**社区讨论**: 评论者对该项目的奉献精神和原创性表示赞赏。有人建议使用多样性双重编译（DDC）来验证官方 rustc 二进制文件是否存在后门。另有人指出，转译为 C 并让 GCC 优化可能比使用 LLVM IR 更实用。

**标签**: `#rust`, `#compiler`, `#bootstrapping`, `#c`, `#transpilation`

---

<a id="item-2"></a>
## [美国隐私紧急：Aaronson 呼吁行动](https://scottaaronson.blog/?p=9902) ⭐️ 8.0/10

Scott Aaronson 发表了一篇题为《美国隐私紧急》的博文，认为当前的美国隐私实践构成紧急情况，并呼吁采取立法行动。 这篇文章意义重大，因为它出自一位受人尊敬的计算机科学家之手，可能影响关于隐私改革的公共讨论，从而推动立法者应对猖獗的数据收集和监控问题。 该帖子在 Hacker News 上获得了很高的社区参与度（138 分，37 条评论），表明强烈关注。评论提供了关于企业政策影响力的背景，并附有查找国会代表的直接链接。

hackernews · flowercalled · 7月3日 00:01 · [社区讨论](https://news.ycombinator.com/item?id=48768992)

**背景**: 美国的隐私由零散的部门法律管辖，缺乏像欧盟 GDPR 那样全面的联邦隐私立法。Aaronson 的论点强调了公众关注与实际保护之间的差距，并将其定性为紧急情况。

**社区讨论**: 评论表达了对企业游说阻碍诸如育儿假等受欢迎措施的不满，一位用户指出“资本管理国家”。另一位用户建议帖子缺乏直接行动号召链接，并提供了该链接。一些人对政治动机提出了疑问。

**标签**: `#privacy`, `#US politics`, `#technology policy`, `#civil liberties`

---

<a id="item-3"></a>
## [Linux 6.9 LUKS 挂起未擦除加密密钥](https://mathstodon.xyz/@iblech/116769502749142438) ⭐️ 8.0/10

自 Linux 内核版本 6.9 起，LUKS 挂起功能不再从内核内存中移除磁盘加密密钥，这是对先前行为的回归。社区测试和内核邮件列表讨论已确认此问题。 此回归降低了全盘加密系统的安全性，因为在挂起期间加密密钥仍留在内存中，可能允许冷启动攻击或取证恢复。它影响所有依赖 LUKS 保护静态数据的用户，尤其是那些挂起到 RAM 的用户。 该引入于 Linux 6.9 的 bug 已通过 cryptsetup 挂起机制确认，该机制通常使用内核的 dm-crypt 挂起调用。问题是密钥擦除步骤被无意移除或绕过，且在后续稳定版本中尚未修复。

hackernews · IngoBlechschmid · 7月2日 15:25 · [社区讨论](https://news.ycombinator.com/item?id=48763035)

**背景**: LUKS（Linux Unified Key Setup）是 Linux 磁盘加密的标准，它使用存储在内核内存中的主密钥来加密/解密数据。'cryptsetup luksSuspend' 命令旨在通过从内存中移除主密钥并阻塞 I/O 来安全挂起 LUKS 设备，恢复时需要重新输入密码短语。在内核 6.9 之前，这一功能正常工作；此回归意味着密钥仍留在内存中，使挂起的安全性目的失效。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/vianney/arch-luks-suspend">GitHub - vianney/arch-luks-suspend: Lock encrypted root volume on suspend in Arch Linux · GitHub</a></li>
<li><a href="https://eucloudservers.com/security-encryption/since-linux-6-9-luks-suspend-stopped-wiping-disk-encryption-keys-from-memory/">Since Linux 6.9, LUKS Suspend Stopped Wiping Disk- encryption ...</a></li>
<li><a href="https://blog.freesources.org/posts/2020/08/cryptsetup-suspend/">cryptsetup- suspend</a></li>

</ul>
</details>

**社区讨论**: 社区评论显示不同反应：一些用户淡化风险，指出挂起到 RAM 本身就将密钥留在内存中，而另一些人则认为在挂起期间显式擦除密钥对于抵御冷启动攻击至关重要。少数人指出该 bug 可能仅影响 Debian 对 luksSuspend 的扩展使用，但 Linux 内核回归仍然令人担忧。

**标签**: `#linux`, `#security`, `#encryption`, `#kernel`, `#bug`

---

<a id="item-4"></a>
## [Podman v6.0.0 发布，带来网络增强和 Quadlet](https://blog.podman.io/2026/07/introducing-podman-v6-0-0/) ⭐️ 8.0/10

Podman v6.0.0 引入了网络增强和 Quadlet 功能，Quadlet 允许将容器作为 systemd 服务进行管理。此版本由于有重大变更，要求同时升级到特定版本的 Buildah、Skopeo、Netavark 和 Aardvark。 此版本大幅提升了 Podman 的易用性和与 systemd 的集成，使其成为更强大的 Docker 替代方案，尤其适合需要无根容器和无守护进程运行的用户。 Podman v6.0.0 包含重大变更：放弃对 cgroups v1、iptables 和 CNI 网络的支持。用户必须同时升级到 Buildah v1.44.0、Skopeo v1.23 以及 Netavark/Aardvark v2.0.0。

hackernews · soheilpro · 7月2日 14:23 · [社区讨论](https://news.ycombinator.com/item?id=48762098)

**背景**: Podman 是一个无守护进程、支持无根运行的容器引擎，旨在成为 Docker 的即插即用替代品。Quadlet 是一个将容器配置转换为 systemd 服务单元的功能，便于管理和自动启动。新的网络改进增强了 IPv6 支持和网络性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.podman.io/en/latest/markdown/podman-quadlet.1.html">podman - quadlet — Podman documentation</a></li>
<li><a href="https://www.redhat.com/en/blog/multi-container-application-podman-quadlet">Deploying a multi-container application using Podman and Quadlet</a></li>
<li><a href="https://windowsforum.com/threads/podman-6-0-migration-guide-cgroups-v1-iptables-cni-removed-what-to-upgrade.430182/">Podman 6.0 Migration Guide: cgroups v1, iptables, CNI Removed—What ...</a></li>

</ul>
</details>

**社区讨论**: 社区反馈积极，用户称赞 Podman 从 Docker 切换的简便性以及新的 Quadlet 功能。有些用户批评缺少官方 Ubuntu 软件包，而其他用户则分享了成功的部署经验。

**标签**: `#podman`, `#containers`, `#docker-alternative`, `#devops`, `#open-source`

---

<a id="item-5"></a>
## [EFF 敦促 FTC 对 X 执行同意令，涉及 Grok AI 生成 CSAM](https://cdn.arstechnica.net/wp-content/uploads/2026/07/EFF-letter-to-FTC-on-X-consent-order-7-2-26.pdf) ⭐️ 8.0/10

电子前哨基金会（EFF）于 2026 年 7 月 2 日致信联邦贸易委员会（FTC），敦促其对 X（原 Twitter）执行同意令，原因是其 Grok AI 图像生成器产生了大量儿童性虐待材料（CSAM）和非自愿亲密图像。 此举意义重大，因为 EFF 传统上是数字权利和言论自由的坚定捍卫者，现在却呼吁对 AI 生成的有害内容进行监管执法，凸显了计算自由与 AI 安全监管之间日益紧张的矛盾。其结果可能为社交媒体平台如何对 AI 生成的非法内容承担责任开创先例。 这封信具体提到了 Grok Imagine，该工具直到最近仍能被操纵生成涉及哈莉·奎因等角色的露骨内容。社区成员注意到 X 此后已大幅限制亲密图像生成，但 EFF 认为仍需执行同意令以解决过去的违规行为并确保合规。

hackernews · Terretta · 7月2日 19:27 · [社区讨论](https://news.ycombinator.com/item?id=48766209)

**背景**: FTC 的同意令可能是基于此前对 X 内容审核惯例的调查结果。EFF 的介入值得注意，因为该组织历来反对政府对计算的限制，但此次优先考虑保护弱势群体免受 AI 生成的伤害。CSAM 指涉及未成年人的色情图像或视频，在大多数司法管辖区属于非法内容。这一争论反映了如何在不过度抑制创新或言论自由的前提下监管快速发展的生成式 AI 技术的更广泛张力。

**社区讨论**: 文章评论观点不一。一些用户指出 Grok 的图像生成已受到严格限制，质疑进一步执法的必要性。另一些人则担心 EFF 在主张减少计算自由，与其核心使命相悖。少数评论者指控政治影响，暗示马斯克 2024 年的竞选支出买通了监管宽松。

**标签**: `#AI safety`, `#CSAM`, `#regulation`, `#EFF`, `#social media`

---

<a id="item-6"></a>
## [VS Code 1.128 Insiders 预览版发布](https://code.visualstudio.com/updates/v1_128) ⭐️ 8.0/10

Visual Studio Code 1.128 内部预览版现已发布，包含了新的实验性功能和改进。 此版本为开发者提供了即将推出的功能和修复的早期访问权限，有助于影响稳定版的发布。这是 VS Code 快速发布周期的一部分。 作为内部预览版，它可能包含不稳定的功能，仅供测试使用。用户应预期频繁更新和潜在错误。

rss · Visual Studio Code · 7月1日 17:00

**背景**: Visual Studio Code Insiders 是编辑器的每日构建版本，包含最新的未发布功能。它允许用户在功能被纳入稳定版之前试用新功能。这种发布周期有助于微软及早收集反馈并修复问题。

**标签**: `#Visual Studio Code`, `#code editor`, `#release notes`, `#insiders`, `#developer tools`

---

<a id="item-7"></a>
## [使用 PDU Dropscan 的极端 PostgreSQL 勒索软件恢复](https://postgr.es/p/9n-) ⭐️ 8.0/10

张晨发布了一篇现场报告，详细介绍了如何通过改编 PDU dropscan 工具，利用已知的 DDL 结构，从勒索软件加密的文件中恢复核心 PostgreSQL 表并导出关键数据。 该报告为面临勒索软件攻击的 PostgreSQL 管理员提供了一种实用的创新取证恢复方法，表明即使在系统目录不可用的情况下也能挽救关键数据，这对灾难恢复极具价值。 恢复过程依赖测试环境的 DDL 将单个表文件与已知结构进行匹配，并使用 PDU dropscan（扫描原始磁盘块以查找已删除表的碎片）进行扫描。

rss · Planet PostgreSQL · 7月2日 00:00

**背景**: PostgreSQL 将每个表存储在磁盘上的单独文件中，其系统目录包含解释这些文件所需的元数据。勒索软件会加密所有数据库文件，导致正常查询无法进行。PDU（PostgreSQL Data Unloader）是一款专为损坏数据库设计的专业恢复工具，具有 dropscan 等高级功能，即使没有目录信息也能从原始块中恢复数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepwiki.com/wublabdubdub/PDU-PostgreSQLDataUnloader/4-user-guide">User Guide | wublabdubdub/PDU-PostgreSQLDataUnloader | DeepWiki</a></li>
<li><a href="https://pduzc.com/blog/dropscan_recovery">PDU - PostgreSQL Data Unloader</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#ransomware`, `#database recovery`, `#forensic analysis`, `#security`

---

<a id="item-8"></a>
## [PostgreSQL 检查点进程无限重试循环 bug](https://postgr.es/p/9nV) ⭐️ 8.0/10

一个生产环境的 PostgreSQL 16.8 数据库遇到“无效内存分配请求大小”错误，该错误由已知的检查点进程 bug 引起，导致进程陷入无限重试循环，最终不得不重启并重放 WAL。通过次要版本升级永久解决了此问题。 该 bug 可能导致 PostgreSQL 部署中出现意外停机和数据恢复延迟，凸显了检查点进程在确保数据库一致性中的关键作用。通过次要版本升级修复，强调了保持补丁更新到最新版本的重要性。 该错误发生在检查点进程的 fsync 请求队列变得过大时，导致内存分配失败，而实际内存并未耗尽。手动检查点无法打破循环，因为检查点进程一直重试同一个失败的操作。

rss · Planet PostgreSQL · 7月1日 13:17

**背景**: 在 PostgreSQL 中，检查点进程是一个后台进程，负责在检查点期间将共享内存中的脏缓冲区写入磁盘，确保数据持久性和高效的崩溃恢复。它维护一个 fsync 请求队列，用于跟踪需要同步的文件。所述的 bug 涉及当该队列中的内存分配失败时导致无限重试循环，后续的次要版本已修复此问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://stormatics.tech/blogs/postgresql-checkpointer-bug-causing-infinite-retry-loop">Inside a PostgreSQL Checkpointer Bug: A Production Postmortem</a></li>
<li><a href="https://pgpedia.info/c/checkpointer.html">Checkpointer - pgPedia - a PostgreSQL Encyclopedia</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database`, `#bug`, `#postmortem`, `#checkpointer`

---

<a id="item-9"></a>
## [AI 基准测试无法反映编码代理真实表现](https://devblogs.microsoft.com/blog/what-ai-benchmarks-are-not-telling-you) ⭐️ 7.0/10

微软 DevBlogs 的文章指出，当前的 AI 基准测试无法反映编码代理在实际开发中的有效性，强调需要引入代理体验（AX）指标。 随着 AI 编码代理日益普及，依赖有缺陷的基准测试可能导致工具选择错误和资源浪费。这一见解帮助开发者基于实际开发体验而非合成分数来评估代理。 该文章是“代理体验（AX）”系列的一部分，专注于让 AI 编码代理与用户技术正确协作。文章讨论了代理栈中可控与不可控的部分，以及如何衡量扩展是否真正有帮助。

rss · Microsoft for Developers · 7月1日 14:31

**背景**: 像 HumanEval 或 SWE-bench 这样的 AI 基准测试在孤立任务上测试编码代理，但实际开发涉及上下文、依赖关系和迭代工作。代理体验（AX）是一个新兴概念，评估代理与工具、API 和用户环境的交互质量。理解这些局限性有助于指导更好的开发实践。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://resend.com/blog/agent-experience">What is AX (Agent Experience) and how to improve it · Resend</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-are-ai-coding-agents">What Is an AI Coding Agent? How They Work and When to Use Them | MindStudio</a></li>

</ul>
</details>

**标签**: `#AI`, `#benchmarks`, `#agent experience`, `#software development`

---

<a id="item-10"></a>
## [enable_nestloop 调优：避免嵌套循环性能灾难](https://postgr.es/p/9n_) ⭐️ 7.0/10

Christophe Pettus 解释了 PostgreSQL 中嵌套循环连接导致性能问题的主要原因是行数估算错误，并提供了关于 enable_nestloop GUC 参数的调优建议。 这很重要，因为嵌套循环连接是查询性能低下的常见原因；理解何时禁用或调整 enable_nestloop 可以帮助 DBA 和开发人员优化 PostgreSQL 工作负载。 enable_nestloop 是一个布尔型 GUC 参数（默认开启），用于控制规划器是否考虑嵌套循环连接路径；将其设置为 off 会为嵌套循环路径添加 disable_cost，但如果不存在替代方案，则不会禁止使用。

rss · Planet PostgreSQL · 7月3日 01:00

**背景**: PostgreSQL 的查询规划器使用基于成本的优化在嵌套循环、哈希连接和合并连接中选择连接方法。当内部关系较小时，嵌套循环连接效率高，但当规划器低估行数时可能导致性能灾难。GUC 参数 enable_nestloop 允许用户阻止规划器使用嵌套循环。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thebuild.com/blog/all-your-gucs-in-a-row-enable_nestloop/">All Your GUCs in a Row: enable_nestloop — The Build</a></li>
<li><a href="https://runebook.dev/en/docs/postgresql/runtime-config-query/GUC-ENABLE-NESTLOOP">A Developer's Guide to PostgreSQL's enable_nestloop Setting</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#query optimization`, `#nested loop joins`, `#performance tuning`, `#enable_nestloop`

---

<a id="item-11"></a>
## [pg-healthcheck：开源 PostgreSQL 健康诊断工具](https://postgr.es/p/9nX) ⭐️ 7.0/10

Ahsan Hadi 发布了 pg-healthcheck，这是一个用 Go 语言编写的开源工具，可对 PostgreSQL 实例执行 180 多项健康检查，覆盖 14 个类别，并输出带颜色标记的终端报告或 JSON 格式数据以便集成到监控管道。 该工具针对 PostgreSQL 常见且严重的问题（如膨胀、复制槽延迟、事务 ID 回卷）提供检测，这些问题往往不易察觉，有助于 DBA 和运维团队主动维护数据库健康。 检查内容包括真空与膨胀分析、基于滚动基线的 WAL 增长率峰值检测、通过 amcheck 进行 TOAST 数据完整性验证，以及使用 pg_check_visible()和 pg_check_frozen()检测可见性图损坏。

rss · Planet PostgreSQL · 7月1日 14:18

**背景**: PostgreSQL 是一种流行的开源关系型数据库。随着数据库规模增长，表膨胀、复制延迟和事务 ID 回卷等问题可能导致性能下降或服务中断。传统监控工具往往缺乏深入的健康检查功能，因此专用的诊断工具很有价值。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://fluca1978.github.io/2021/02/08/PostgreSQLToastCorruption.html">PostgreSQL TOAST Data Corruption (ERROR: unexpected chunk number)</a></li>
<li><a href="https://www.pgedge.com/blog/multi-master-replication-using-pgedge-enterprise-postgres-with-spock-and-cloudnativepg">Multi-Master Postgres with Spock & CloudNativePG</a></li>
<li><a href="https://www.crunchydata.com/blog/managing-transaction-id-wraparound-in-postgresql">Managing Transaction ID Exhaustion (Wraparound) in PostgreSQL | Crunchy Data Blog</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#open-source`, `#database`, `#monitoring`, `#tool`

---

<a id="item-12"></a>
## [pgcopydb v0.18 发布：包含 88 次提交的重大更新](https://postgr.es/p/9nW) ⭐️ 7.0/10

pgcopydb v0.18 已发布，自 2024 年 8 月的 v0.17 以来包含 88 次提交，成为有史以来最大的版本。它增加了对 PostgreSQL 16、17 和 18 的兼容性，新的 pgoutput-default CDC 引擎，基于正则表达式的过滤，以及 Citus 到 Citus 迁移支持。 此版本显著提高了 PostgreSQL 数据库复制的可靠性和性能，使得以最小停机时间迁移数据库更加快捷。添加 Citus 到 Citus 支持将其实用性扩展到水平扩展的 PostgreSQL 部署。 新的 pgoutput-default CDC 引擎带来了显著的可靠性和性能提升。该版本还包含 24 个错误修复，并可通过本地 SQLite 目录实现重启能力。

rss · Planet PostgreSQL · 7月1日 14:05

**背景**: pgcopydb 是一个开源工具，在无法进行物理文件复制时，尽可能快地将 PostgreSQL 数据库复制到另一台服务器。它将 COPY 操作并行化到所有表，并在数据加载后并行构建索引。它支持通过逻辑复制实现变更数据捕获（CDC），以最小停机时间进行迁移，其状态记录在本地 SQLite 目录中，支持重启。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/dimitri/pgcopydb/releases">Releases · dimitri/pgcopydb - GitHub</a></li>
<li><a href="https://pgcopydb.readthedocs.io/en/latest/">Welcome to pgcopydb’s documentation! — pgcopydb 0.18~dev ...</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#pgcopydb`, `#database migration`, `#open source`

---

<a id="item-13"></a>
## [理解才能参与：避免认知债务](https://simonwillison.net/2026/Jul/2/understand-to-participate/#atom-everything) ⭐️ 7.0/10

Geoffrey Litt 在 AIE 会议上提出，开发者必须深入理解 AI 代理生成的代码，才能积极参与并避免认知债务。 这一观点揭示了 AI 辅助开发中的一个关键挑战：随着编码代理日益自主，如何保持人类的理解力和主动性，防止认知债务积累，从而避免软件质量下降。 Litt 在 2026 年 AI Engineer World's Fair 上发表演讲，该演讲与其他 300 多场演讲一起被录制，将在三周内陆续发布到 YouTube。他还在 Twitter 上发布了演讲的摘要串。

rss · Simon Willison · 7月2日 17:07

**背景**: 认知债务是指团队对代码的共同理解随时间逐渐消退，特别是在 AI 工具生成了开发者未能完全理解的代码时。技术债务存在于代码中，而认知债务存在于人的脑海中。2026 年，这个概念作为 AI 驱动软件开发中的隐藏风险开始受到关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2603.22106">From Technical Debt to Cognitive and Intent Debt: Rethinking ... Cognitive debt: The hidden risk in AI-driven software development How Generative and Agentic AI Shift Concern from Technical ... From Technical Debt to Cognitive and Intent Debt: - arXiv.org Understanding Cognitive Debt in Engineering Teams What Is Cognitive Debt? How AI Coding Tools Are Silently ...</a></li>
<li><a href="https://www.linkedin.com/pulse/cognitive-debt-software-engineering-oren-chapo-6qw7f/">Cognitive Debt in Software Engineering - LinkedIn</a></li>
<li><a href="https://getdx.com/blog/cognitive-debt-the-hidden-risk-in-ai-driven-software-development/">Cognitive debt: The hidden risk in AI-driven software development</a></li>

</ul>
</details>

**标签**: `#AI-assisted development`, `#coding agents`, `#cognitive debt`, `#software engineering`, `#human-AI collaboration`

---