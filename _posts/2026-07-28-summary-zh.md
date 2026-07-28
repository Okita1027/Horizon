---
layout: default
title: "Horizon 日报：2026-07-28 (ZH)"
date: 2026-07-28
lang: zh
---

> 从 33 条内容中筛选出 11 条重要资讯。

---

1. [Anthropic：开放权重模型需强制安全测试](#item-1) ⭐️ 8.0/10
2. [Python-Build-Standalone：Astral 接管的便携式 Python 发行版](#item-2) ⭐️ 8.0/10
3. [漏掉下划线导致无辜者含冤入狱 18 个月](#item-3) ⭐️ 8.0/10
4. [沃尔沃/埃彻车队平台严重漏洞可完全控制车辆](#item-4) ⭐️ 8.0/10
5. [《Paged Out》第 9 期发布](#item-5) ⭐️ 8.0/10
6. [PostgreSQL 的 MVCC 并不糟糕，它是设计权衡](#item-6) ⭐️ 8.0/10
7. [Moonshot AI 发布 2.8 万亿参数 Kimi K3 权重](#item-7) ⭐️ 8.0/10
8. [LLM 代币转售欺诈内幕曝光](#item-8) ⭐️ 8.0/10
9. [PostgreSQL 的 gin_fuzzy_search_limit 返回随机子集](#item-9) ⭐️ 7.0/10
10. [Postgres 先锋特性应从分支起步](#item-10) ⭐️ 7.0/10
11. [AI 工具指南从聊天转向代理系统](#item-11) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Anthropic：开放权重模型需强制安全测试](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 8.0/10

Anthropic 正式表明立场，不主张禁止开放权重的 AI 模型，但认为所有足够强大的模型，无论是开源还是闭源，都应在发布前接受强制安全测试。 这一立场意义重大，因为它介入了开源 AI 开发与安全监管之间的持续辩论，可能影响未来的 AI 政策以及创新与风险缓解之间的平衡。 Anthropic CEO Dario Amodei 的文章还支持限制向中国销售芯片等措施，一些评论者认为这与反对禁止开放权重模型的立场相矛盾。

hackernews · surprisetalk · 7月27日 22:03 · [社区讨论](https://news.ycombinator.com/item?id=49076057)

**背景**: 开放权重 AI 模型指的是将训练好的参数（权重）公开发布，允许其他人进行微调、分发和在此基础上构建。这与完全开源模型不同，后者还包括训练代码和数据。争论的焦点在于，开放强大 AI 模型的访问是否会带来安全风险——可能被恶意行为者滥用——以及透明度和民主化的好处。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@aruna.kolluru/exploring-the-world-of-open-source-and-open-weights-ai-aa09707b69fc">Exploring the World of Open Source and Open Weights AI | Medium</a></li>
<li><a href="https://www.ai21.com/glossary/foundational-llm/open-weights-model/">What is an Open - Weights Model ? | AI 21</a></li>

</ul>
</details>

**社区讨论**: 社区评论大多批评 Anthropic 的立场，认为强制安全测试可能通过施加昂贵的要求而实际上禁止开放权重模型。一些人指出 Anthropic 支持硬件出口限制而反对软件禁令的矛盾。还有人指责 Anthropic 通过倡导可能阻碍开源竞争对手的监管来保护其商业利益。

**标签**: `#AI safety`, `#open-weights`, `#AI policy`, `#Anthropic`, `#open-source`

---

<a id="item-2"></a>
## [Python-Build-Standalone：Astral 接管的便携式 Python 发行版](https://gregoryszorc.com/docs/python-build-standalone/main/) ⭐️ 8.0/10

python-build-standalone 项目生成自包含、高度便携的 Python 二进制文件，无需额外依赖即可在任何机器上运行，现由 uv 包管理器背后的公司 Astral 积极维护。 这些发行版被 uv、pipx、Hatch、Poetry 等主流 Python 工具使用，消除了 Python 版本管理的痛点，使跨平台的 Python 部署更简单、更可靠。 Astral 已维护该项目约一年半，工程时间分配在跟进上游 CPython、改进交叉编译以及向上游贡献代码等方面。

hackernews · jcbhmr · 7月27日 18:43 · [社区讨论](https://news.ycombinator.com/item?id=49073942)

**背景**: 标准 Python 安装通常需要特定的系统库或预装的 Python 解释器，导致将 Python 捆绑到应用程序中很困难。Python-build-standalone 通过提供预编译、可重定位且包含所有必要组件的二进制文件解决了此问题。像 uv 这样的工具利用这些二进制文件，使用户只需一条命令即可安装 Python，无需手动管理多个 Python 版本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/astral-sh/python-build-standalone">GitHub - astral-sh/python-build-standalone: Produce redistributable builds of Python · GitHub</a></li>
<li><a href="https://astral.sh/blog/python-build-standalone">A new home for python-build-standalone</a></li>
<li><a href="https://github.com/astral-sh/uv">GitHub - astral-sh/uv: An extremely fast Python package and project manager, written in Rust. · GitHub</a></li>

</ul>
</details>

**社区讨论**: uv 的创建者 charliermarsh 确认 uv 使用这些发行版，并且 Astral 的工程时间分配在上游维护、交叉编译改进和贡献代码上。simonw 称赞这些发行版非常适合将 Python 捆绑到桌面应用中。rsyring 向读者介绍了 PyOxy 姊妹项目，用于生成单文件可执行文件；zie 则提到了 APE/Cosmopolitan 跨平台二进制文件，可在多个操作系统上原生运行 Python。

**标签**: `#Python`, `#distribution`, `#packaging`, `#portable`, `#uv`

---

<a id="item-3"></a>
## [漏掉下划线导致无辜者含冤入狱 18 个月](https://arstechnica.com/tech-policy/2026/07/police-missed-one-underscore-and-sent-the-wrong-man-to-prison/) ⭐️ 8.0/10

据 Ars Technica 报道，一个用户名中缺失的下划线导致无辜者 Klayme 被错误定罪，并因此含冤入狱 18 个月。 此案揭示了数字证据中微小软件错误可能导致的严重后果，暴露了司法体系在未经过严格验证即采信此类证据时的系统性缺陷，并强调了改进法证标准和法律保障的必要性。 关键错误是一个用户名中缺失的下划线，导致执法部门错误地将 Klayme 认定为罪犯。尽管没有私密影像、没有相关期间使用 Kik 的证据，也没有其他关联，他仍被定罪并服刑 18 个月。

hackernews · quantified · 7月27日 22:10 · [社区讨论](https://news.ycombinator.com/item?id=49076116)

**背景**: 数字证据（如用户名和 IP 地址）常用于刑事调查。像下划线这样的小差异可以区分不同用户。正如本案所示，法证证据中的字符串比较错误可能导致身份误认。司法系统通常缺乏审查此类证据的技术专业知识，从而使冤假错案成为可能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nij.ojp.gov/topics/articles/impact-false-or-misleading-forensic-evidence-wrongful-convictions">The Impact of False or Misleading Forensic Evidence on Wrongful Convictions | National Institute of Justice</a></li>
<li><a href="https://www.forensicchem.com/posts/empirical-validation-in-forensic-text-comparison-requirements-methods-and-future-directions">Empirical Validation in Forensic Text Comparison</a></li>

</ul>
</details>

**社区讨论**: 评论者对司法失误表示愤怒，质疑辩护方为何没有有效质疑证据。一些人想知道被错误定罪者是否获得了赔偿。其他人则引用了经典故事《计算机不争论》，将其与过度依赖计算机输出的危险相提并论。

**标签**: `#digital-evidence`, `#wrongful-conviction`, `#software-errors`, `#legal-tech`, `#cybersecurity`

---

<a id="item-4"></a>
## [沃尔沃/埃彻车队平台严重漏洞可完全控制车辆](https://eaton-works.com/2026/07/27/my-eicher-hack/) ⭐️ 8.0/10

一名安全研究员披露了沃尔沃/埃彻的“My Eicher”车队管理平台存在严重漏洞，攻击者可未经授权控制所有用户和车辆。该披露于 2026 年 7 月 27 日发布，此前供应商数周未回应，最终修复了主要问题但未公开确认。 该漏洞可能允许恶意行为者远程监控和控制商用车辆，对驾驶员安全、货物安全和运营完整性构成风险。它凸显了依赖云的汽车系统中的系统性安全弱点，可能影响数千辆车辆。 研究员于 2025 年 11 月 3 日报告漏洞，但直到 11 月 20 日才收到回应，当时主要 API 被修复，但未进行协调。完整披露在八个多月后发布，表明供应商未解决所有相关问题或发布安全公告。

hackernews · EatonZ · 7月27日 15:08 · [社区讨论](https://news.ycombinator.com/item?id=49070756)

**背景**: “My Eicher”平台是一个基于云的车队管理和 GPS 追踪系统，用于商用车辆所有者和运营商。它依赖支持远程信息处理的车辆和内部 API 提供预测性正常运行时间和燃油管理等功能。此类系统的漏洞可能允许未经授权访问车辆控制功能，类似于 CAN 总线攻击向量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://eaton-works.com/2026/07/27/my-eicher-hack/">Exploiting Volvo/Eicher's fleet management platform to gain ...</a></li>
<li><a href="https://apps.apple.com/us/app/my-eicher/id1554986853">MY EICHER App - App Store</a></li>
<li><a href="https://www.sealingtech.com/2024/03/05/can-bus-vulnerabilities-raise-threats-for-cars-and-tanks/">CAN Bus Vulnerabilities Raise Threats for Cars and Tanks</a></li>

</ul>
</details>

**社区讨论**: 评论者指出研究员的宽限时间——给供应商一年多时间修复漏洞才披露，并表达了对现代汽车依赖云端软件的担忧，引用了因缺乏连接导致车辆无法启动的案例。一名用户分享了 FSF 的维修权视频链接，反映了对汽车安全表演的广泛不满。

**标签**: `#security`, `#vulnerability`, `#automotive`, `#IoT`, `#fleet management`

---

<a id="item-5"></a>
## [《Paged Out》第 9 期发布](https://pagedout.institute/download/PagedOut_009.pdf) ⭐️ 8.0/10

免费黑客杂志《Paged Out》第 9 期已以 PDF 形式发布，内容涵盖低层次技术文章，如 C 语言编程和次像素渲染。 《Paged Out》在黑客和复古计算社区中备受尊敬，第 9 期延续了深度技术内容的传统，被视为经典杂志 2600 和 Phrack 的现代等同物。 该期包含《C 语言入门》（Baby Steps in C）和《次像素动物园》（The Subpixel Zoo）等文章，可免费下载 PDF，并可购买印刷版。

hackernews · laurensr · 7月27日 14:22 · [社区讨论](https://news.ycombinator.com/item?id=49070138)

**背景**: 《Paged Out》是一本免费的社区驱动杂志，专注于黑客、复古计算和低层次编程。它以高质量的技术内容和精美设计而闻名，常被比作历史上的黑客杂志 2600 和 Phrack。

**社区讨论**: 社区评论表现出热情，有用户觉得《C 语言入门》很有趣，另一用户欣赏《次像素动物园》。评论者将其比作现代版的 2600 或 Phrack，并对购买印刷版表现出兴趣。

**标签**: `#hacker magazine`, `#retro computing`, `#low-level programming`, `#technical articles`, `#PDF zine`

---

<a id="item-6"></a>
## [PostgreSQL 的 MVCC 并不糟糕，它是设计权衡](https://postgr.es/p/9qy) ⭐️ 8.0/10

Radim Marek 发表了一篇详细的反驳文章，认为 PostgreSQL 的 MVCC 并非本质上存在缺陷；相反，每种 MVCC 实现都面临不同的权衡，PostgreSQL 的设计选择是合理的。 这一观点挑战了常见的批评（即 PostgreSQL 的 MVCC 尤其糟糕），鼓励在数据库系统间进行更细致的比较，并指出没有任何方法是没有开销的。 文章分解了四个基本设计问题——旧版本存放位置、链方向、索引指针和清理责任——并展示了替代方案（如 MySQL 的 undo log 或 Oracle 的回滚段）如何将成本转移到其他地方。

rss · Planet PostgreSQL · 7月27日 14:00

**背景**: 多版本并发控制（MVCC）是一种标准技术，通过保留行的多个版本来确保读取者不阻塞写入者。PostgreSQL 将旧版本存储在主表（堆）中，使用物理行标识符，并依赖后台 VACUUM 进程清理死元组。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Multiversion_concurrency_control">Multiversion concurrency control - Wikipedia</a></li>
<li><a href="https://www.postgresql.org/docs/current/sql-vacuum.html">PostgreSQL: Documentation: 18: VACUUM</a></li>
<li><a href="https://www.postgresql.org/docs/current/routine-vacuuming.html">PostgreSQL: Documentation: 18: 24.1. Routine Vacuuming</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#MVCC`, `#Database Design`, `#Performance`

---

<a id="item-7"></a>
## [Moonshot AI 发布 2.8 万亿参数 Kimi K3 权重](https://simonwillison.net/2026/Jul/27/kimi-k3/#atom-everything) ⭐️ 8.0/10

Moonshot AI 于 2026 年 7 月 27 日在 Hugging Face 上发布了 Kimi K3 的开放权重，这是一个 2.8 万亿参数的大语言模型。该模型采用非开源许可证，要求大规模商业使用时需另行签订协议。 此次发布延续了 Moonshot 推动开放权重模型前沿的趋势，使研究人员和开发者能够获得最先进的模型。2.8 万亿参数规模和原生视觉能力可能推动多模态理解和长上下文处理的 AI 研究。 Kimi K3 具有 100 万 token 的上下文窗口、Kimi Delta Attention 和原生视觉支持，权重总计 1.56 TB。其许可证设置了收入和用户阈值，可能限制大型 API 提供商的使用，这与早期 K2 的修改版 MIT 许可证有所不同。

rss · Simon Willison · 7月27日 23:39

**背景**: 像 Kimi K3 这样的开放权重模型会发布训练好的参数，允许推理和微调，但通常不包含完整的训练代码和数据。相比之下，开源模型提供完整的复现能力。Moonshot AI 始终使用“开放权重”而非“开源”来描述其发布，强调这一区别。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/moonshotai/Kimi-K3">moonshotai/ Kimi - K 3 · Hugging Face</a></li>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://www.linkedin.com/pulse/open-weights-vs-source-llms-why-difference-matters-more-kapil-uthra-6kanf">Open Weights vs . Open Source in LLMs: Why the Difference Matters...</a></li>

</ul>
</details>

**标签**: `#Kimi K3`, `#LLM`, `#open weights`, `#Moonshot AI`, `#Hugging Face`

---

<a id="item-8"></a>
## [LLM 代币转售欺诈内幕曝光](https://simonwillison.net/2026/Jul/26/relay-market/#atom-everything) ⭐️ 8.0/10

Matt Lenhard 的调查揭示了中国存在一个市场，转售者通过滥用免费试用、窃取凭证以及使用 one-api 和 new-api 等开源代理软件来汇集 API Key，从而提供折扣 LLM 代币。 这凸显了 LLM API 提供商和用户面临的重大安全风险，因为整个生态系统都在利用未受保护的端点牟利。这强调了迫切需要更严格的 API Key 使用上限和欺诈检测机制。 这些代理基于合法的开源项目（one-api 和 new-api）构建，可在汇集的凭证之间进行负载均衡。买家包括寻求廉价代币、绕过地理限制或收集数据进行模型蒸馏的人。

rss · Simon Willison · 7月26日 19:30

**背景**: LLM API 代币是允许访问如 OpenAI 的 GPT 等大语言模型服务的凭证。通常，开发者按使用的代币付费。这个市场的转售者汇集多个 API Key（通常通过欺诈手段获得），并通过代理服务器以折扣价出售。这些代理软件原本用于合法的多 Key 管理，现被滥用于此。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/songquanpeng/one-api">GitHub - songquanpeng/one-api: LLM API 管理 & 分发系统，支持 Open... Songquanpeng - One Api - StackBlitz one-api command - github.com/songquanpeng/one-api - Go Packages songquanpeng/one-api | GitHub | Ecosyste.ms: Repos Components available for installation — Intel® oneAPI CI ... Intel Samples Catalog - oneapi-src.github.io</a></li>
<li><a href="https://ossinsight.io/analyze/QuantumNous/new-api">Analyze QuantumNous/ new - api | OSSInsight</a></li>

</ul>
</details>

**标签**: `#LLM`, `#API security`, `#fraud`, `#token reselling`, `#proxy`

---

<a id="item-9"></a>
## [PostgreSQL 的 gin_fuzzy_search_limit 返回随机子集](https://postgr.es/p/9qw) ⭐️ 7.0/10

PostgreSQL 的 gin_fuzzy_search_limit 参数在启用时会静默返回匹配行的随机子集而非全部结果，以正确性换取速度。 这对依赖 GIN 索引进行精确搜索的用户来说很危险，他们可能不知不觉中得到不完整的结果，可能导致数据丢失或应用程序行为错误。 默认值为 0（禁用），但当设置为正整数时，索引最多返回该数量的随机匹配行，且不保证省略了哪些行。

rss · Planet PostgreSQL · 7月27日 01:00

**背景**: GIN（通用倒排索引）专为数组、JSONB 和全文搜索等复合值索引设计。使用 GIN 索引的查询可能产生大量结果集，尤其是常见词。gin_fuzzy_search_limit 旨在限制返回的行数，但采用随机子集而非完全遵循搜索条件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/gin.html">PostgreSQL: Documentation: 18: 65.4. GIN Indexes</a></li>
<li><a href="https://pgpedia.info/g/gin_fuzzy_search_limit.html">gin _ fuzzy _ search _ limit - pgPedia - a PostgreSQL Encyclopedia</a></li>
<li><a href="https://postgresqlco.nf/doc/en/param/gin_fuzzy_search_limit/">PostgreSQL Documentation: gin _ fuzzy _ search _ limit parameter</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#GIN`, `#fuzzy search`, `#performance`, `#correctness`

---

<a id="item-10"></a>
## [Postgres 先锋特性应从分支起步](https://postgr.es/p/9qt) ⭐️ 7.0/10

Andrei Lepikhov 主张，新的 PostgreSQL 先锋特性应在分支中开发，以保持核心的稳定性和简洁性，这基于社区偏好“足够好”而非快速创新的理念。他以临时表的并行查询为例，该特性在分支中经过三次尝试后才考虑进入核心。 这一观点挑战了所有优秀特性都应进入核心的常见假设，提供了一条在不牺牲 PostgreSQL 可靠性前提下的创新实践路径。它突显了快速创新与稳定性之间的权衡，这对数据库的治理和长期健康至关重要。 文章描述了临时表并行扫描的第一个尝试是在 Postgres Professional 分支中实现的，通过刷新脏页并允许后台工作进程扫描。经过另外两次迭代，该特性最终被接受进入核心。

rss · Planet PostgreSQL · 7月26日 08:58

**背景**: PostgreSQL 以其对稳定性和鲁棒性的高度重视而闻名，特别是对于关键任务数据。新特性面临很高的门槛：在合并到核心之前，必须证明安全性、避免回归，并展示真实用户需求。分支允许开发者在真实条件下测试先锋想法，而不危及主代码库。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/runtime-config-query.html">PostgreSQL: Documentation: 18: 19.7. Query Planning</a></li>
<li><a href="https://www.postgresql.org/docs/current/planner-optimizer.html">PostgreSQL: Documentation: 18: 51.5. Planner/Optimizer</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#open-source development`, `#database forks`, `#software engineering`

---

<a id="item-11"></a>
## [AI 工具指南从聊天转向代理系统](https://simonwillison.net/2026/Jul/27/an-opinionated-guide-to-which-ai-to-use-to-do-stuff/#atom-everything) ⭐️ 7.0/10

Ethan Mollick 更新的 AI 工具选择指南现在强调代理系统（如 ChatGPT Work 和 Claude Cowork），而非以聊天为中心的方法。值得注意的模型包括 o3、Claude 4 Opus 和 Gemini 2.5 Pro，以及 Deep Research 作为替代模式。 这一转变反映了行业从简单聊天机器人向能够执行数小时人类工作的自主代理的广泛趋势，帮助用户驾驭复杂的 AI 工具环境以实现最高生产力。 Gemini 因 Google 在 Codex/ChatGPT Work/Cowork 类别中缺乏成熟产品而被排除。AI 模式的命名令人困惑——ChatGPT Work 和 Codex 与 Claude 的 Cowork 和 Code 不同，桌面版提供完整的计算机访问权限。

rss · Simon Willison · 7月27日 21:55

**背景**: 代理型 AI 指能够在有限监督下感知、推理并采取行动以实现目标的半自主或全自主系统。Deep Research 是一种独立进行多步骤网络研究的功能。该指南比较了 o3（OpenAI）、Claude 4 Opus（Anthropic）和 Gemini 2.5 Pro（Google）等模型在不同用例中的表现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>
<li><a href="https://mitsloan.mit.edu/ideas-made-to-matter/agentic-ai-explained">Agentic AI, explained | MIT Sloan</a></li>
<li><a href="https://www.ibm.com/think/topics/agentic-ai">What is Agentic AI? | IBM</a></li>
<li><a href="https://openai.com/index/introducing-deep-research/">Introducing deep research - OpenAI</a></li>
<li><a href="https://help.openai.com/en/articles/20001275-chatgpt-work-and-codex">ChatGPT Work and Codex - OpenAI Help Center</a></li>

</ul>
</details>

**标签**: `#AI tools`, `#agentic AI`, `#commentary`, `#Ethan Mollick`, `#Simon Willison`

---