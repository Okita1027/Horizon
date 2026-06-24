---
layout: default
title: "Horizon 日报：2026-06-24 (ZH)"
date: 2026-06-24
lang: zh
---

> 从 44 条内容中筛选出 12 条重要资讯。

---

1. [大型语言模型无法区分特权文本，优先考虑风格](#item-1) ⭐️ 9.0/10
2. [所见即所得的 TikZ 编辑器，同步代码与图形](#item-2) ⭐️ 8.0/10
3. [维生素 D 的益处被夸大但并非无用](#item-3) ⭐️ 8.0/10
4. [即将到来的循环：人工智能与人类代码清晰度的丧失](#item-4) ⭐️ 8.0/10
5. [百度无限 OCR 实现恒定内存长文档解析](#item-5) ⭐️ 8.0/10
6. [谷歌员工因开发非官方工作区 CLI 被解雇](#item-6) ⭐️ 8.0/10
7. [将 Moebius 0.2B 图像修复模型移植到浏览器 WebGPU 运行](#item-7) ⭐️ 8.0/10
8. [模型无偏好，唯有上下文影响回答](#item-8) ⭐️ 7.0/10
9. [Christophe Pettus 论使用 GUC 诊断索引扫描](#item-9) ⭐️ 7.0/10
10. [Tomas Vondra 更新关于 random_page_cost 的思考](#item-10) ⭐️ 7.0/10
11. [理解 PostgreSQL 的 pg_stats 与查询规划](#item-11) ⭐️ 7.0/10
12. [Datasette 1.0a35 新增创建/修改表的 JSON API](#item-12) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [大型语言模型无法区分特权文本，优先考虑风格](https://simonwillison.net/2026/Jun/22/prompt-injection-as-role-confusion/#atom-everything) ⭐️ 9.0/10

一篇研究论文揭示，大型语言模型（LLM）无法可靠区分自身的特权文本（如系统提示）与不可信的用户输入，反而优先考虑文本风格而非内容，从而导致危险的越狱攻击。 这一发现挑战了当前的 LLM 安全方法，表明除非模型实现真正的角色感知，否则提示注入防御从根本上受限，使得防御成为一场永无止境的打地鼠游戏。 该研究引入了“去风格化”——将文本重写以使其看起来不像角色标签格式——这使得数据集中平均攻击成功率从 61%骤降至 10%。研究人员将底层机制称为“角色混淆”，并认为除非实现真正的角色感知，否则注入防御将永远是“打地鼠游戏”。

rss · Simon Willison · 6月22日 23:59

**背景**: 提示注入是一种安全漏洞，恶意输入会导致 LLM 产生意外行为。LLM 通常依赖特殊标签（如<system>、<user>、<assistant>）来区分文本的不同角色，但研究表明，当不可信文本模仿特权角色标签的风格时，模型会变得混乱，从而覆盖安全训练。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>
<li><a href="https://genai.owasp.org/llmrisk/llm01-prompt-injection/">LLM 01:2025 Prompt Injection - OWASP Gen AI Security Project</a></li>
<li><a href="https://www.linkedin.com/pulse/prompt-injection-llm-applications-how-works-build-security-mazhar-qym5e">Prompt Injection in LLM Applications: How It Works and How to Build...</a></li>

</ul>
</details>

**标签**: `#prompt injection`, `#LLM security`, `#role confusion`, `#AI safety`

---

<a id="item-2"></a>
## [所见即所得的 TikZ 编辑器，同步代码与图形](https://tikz.dev/editor/) ⭐️ 8.0/10

一款开源的所见即所得 TikZ 编辑器已发布，用户可同步编辑源代码和渲染图形，并支持拖拽定位。该编辑器几乎完全由 AI 编程智能体 Codex 构建。 该工具极大简化了 LaTeX 中的图形创建，这是学术界常见的痛点。它也展示了 AI 如何构建人类难以完成的繁琐软件，为类似的复杂工具开辟了可能性。 编辑器解析 TikZ 代码以跟踪每个对象的精确源代码位置，从而可以直接操作坐标而不改变代码格式。它重新实现了 TikZ 的很大一部分，并包含从 SVG、PPTX 和 IPE 格式的转换器。

hackernews · DominikPeters · 6月23日 14:24 · [社区讨论](https://news.ycombinator.com/item?id=48645437)

**背景**: TikZ 是 LaTeX 中用于创建矢量图形的强大宏包，但需要手动编写 \draw 和 foreach 循环等命令，通常涉及繁琐的坐标调整。这款所见即所得编辑器提供了可视化界面，同时保持了与原始源代码的兼容性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PGF/TikZ">PGF/TikZ - Wikipedia</a></li>
<li><a href="https://www.overleaf.com/learn/latex/TikZ_package">TikZ package - Overleaf, Online LaTeX Editor</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞了其概念，但指出生成的代码使用绝对坐标，这在 TikZ 中不常见。一些人将其与现有的工具（如 Quiver）进行有利比较，并询问是否支持 Typst 的 cetz 包。

**标签**: `#TikZ`, `#LaTeX`, `#editor`, `#WYSIWYG`, `#open-source`

---

<a id="item-3"></a>
## [维生素 D 的益处被夸大但并非无用](https://dynomight.net/vitamin-d/) ⭐️ 8.0/10

一项详细分析指出，虽然维生素 D 并非完全无用，但其益处主要局限于严重缺乏的个体，这与许多流行的健康说法相矛盾。 这很重要，因为维生素 D 补充剂被广泛推广，该分析有助于澄清哪些人真正受益，可能影响公共卫生指南并减少不必要的补充。 文章引用的研究指出，当前推荐可能基于错误数学，且维生素 K2 等辅因子可能影响吸收，但许多试验未测量血液水平的变化。

hackernews · surprisetalk · 6月23日 16:30 · [社区讨论](https://news.ycombinator.com/item?id=48647486)

**背景**: 维生素 D 是一种脂溶性维生素，对骨骼健康、免疫功能和钙吸收至关重要。许多人基于广泛的健康益处声称而服用补充剂，但科学证据不一，一些近期研究质疑其对普通人群的有效性。

**社区讨论**: 评论者赞赏这种平衡的分析，指出强有力的证据仅针对严重缺乏者。他们还讨论了研究设计中的潜在问题，如指南中的错误数学以及需要与维生素 K2 共同补充以改善吸收。

**标签**: `#Health`, `#Nutrition`, `#Vitamin D`, `#Evidence-based medicine`, `#Public health`

---

<a id="item-4"></a>
## [即将到来的循环：人工智能与人类代码清晰度的丧失](https://lucumr.pocoo.org/2026/6/23/the-coming-loop/) ⭐️ 8.0/10

这篇文章强调了人类对 AI 日益增长的依赖，这可能会削弱软件工程中的人类专业知识，使代码库变得脆弱且维护依赖于 AI，同时引发对 AI 在创意和审美任务中局限性的担忧。 Ronacher 创造了术语“即将到来的循环”，用来描述人类越来越依赖 AI 进行总结、上下文化和生成代码的循环，从而导致在没有机器辅助下完全解释代码或进行推理的能力丧失。

hackernews · ingve · 6月23日 11:06 · [社区讨论](https://news.ycombinator.com/item?id=48643180)

**背景**: 这篇文章的背景是快速改进的大语言模型（LLMs）和能够快速生成大量代码的 AI 编程助手。Armin Ronacher 是知名的 Python 开发者，也是 Flask 和 Jinja2 等流行框架的创建者，这使得他对代码可维护性和人为因素的看法具有重要分量。

**社区讨论**: 评论者普遍同意文章的观点，指出通过迭代实现清晰度是一个 AI 无法加速的瓶颈。一些人强调在使用 AI 代理之前编写清晰规范的重要性，而另一些人则区分了 AI 擅长的目标驱动工作与人类品味至关重要的审美驱动工作。

**标签**: `#AI`, `#software engineering`, `#programming`, `#LLMs`, `#code maintenance`

---

<a id="item-5"></a>
## [百度无限 OCR 实现恒定内存长文档解析](https://github.com/baidu/Unlimited-OCR) ⭐️ 8.0/10

百度发布了 Unlimited OCR，该模型采用参考滑动窗口注意力（R-SWA）机制，一次性解析长文档而无需线性内存增长，克服了 KV 缓存瓶颈。 这使得在消费级 GPU 上处理长文档（例如 100 页 PDF）而不会出现内存溢出崩溃，为资源受限的用户普及了文档 AI。 该模型通过 R-SWA 扩展了 DeepSeek-OCR 架构，在处理文本时保持原始图像的全局参考，无论文档长度如何，内存均保持 O(1)恒定。

hackernews · ingve · 6月23日 11:35 · [社区讨论](https://news.ycombinator.com/item?id=48643426)

**背景**: 传统的基于 Transformer 的 OCR 模型存在 KV 缓存内存线性增长的问题，通常需要分割文档，从而丢失上下文。Unlimited OCR 的 R-SWA 将注意力分为全局参考路径（保留全图上下文）和局部滑动窗口（用于文本解码），避免了内存累积。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48643426">Unlimited OCR: One-shot long-horizon parsing - Hacker News</a></li>
<li><a href="https://github.com/baidu/Unlimited-OCR">Unlimited OCR Works: Welcome the Era of One-shot Long ... - GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区欣赏这一巧妙架构，并称赞其致谢 DeepSeek-OCR 是'高尚行为'。然而，有用户反映实际 OCR 质量欠佳，尽管技术本身很有趣。其名称'Unlimited OCR Works'来源于《命运之夜》的梗。

**标签**: `#OCR`, `#AI`, `#memory optimization`, `#document parsing`

---

<a id="item-6"></a>
## [谷歌员工因开发非官方工作区 CLI 被解雇](https://twitter.com/JPoehnelt/status/2069482265953087602) ⭐️ 8.0/10

谷歌员工贾斯汀·波内尔特（Justin Poehnelt）因未经内部批准创建并发布谷歌工作区（Google Workspace）的非官方命令行界面（CLI）而被解雇。 这一事件凸显了企业官僚主义与员工创新之间的紧张关系，引发了关于大型科技公司对副业项目和开源贡献政策的讨论。 该非官方 CLI 托管在 GitHub 上，集成了 Gmail、日历、Drive 等 Workspace 应用，但被一些人误认为是谷歌的官方产品。谷歌后来于 2026 年 3 月发布了其官方的 Workspace CLI。

hackernews · justinwp · 6月23日 18:13 · [社区讨论](https://news.ycombinator.com/item?id=48649011)

**背景**: 谷歌工作区是一套基于云的生产力工具，包括 Gmail、Drive 和日历。CLI（命令行界面）允许用户从终端与这些服务交互，通常是开发人员偏爱的自动化工具。谷歌内部要求员工对副业项目进行审批，尤其是那些可能被误认为是官方产品的项目。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/omriariav/workspace-cli">GitHub - omriariav/workspace-cli: Unofficial Google Workspace CLI · GitHub</a></li>
<li><a href="https://github.com/googleworkspace/cli">GitHub - googleworkspace/cli: Google Workspace CLI — one command-line tool for Drive, Gmail, Calendar, Sheets, Docs, Chat, Admin, and more. Dynamically built from Google Discovery Service. Includes AI agent skills.</a></li>
<li><a href="https://x.com/addyosmani/status/2029372736267805081">Addy Osmani on X: "Introducing the Google Workspace CLI: https://t.co/8yWtbxiVPp - built for humans and agents. Google Drive, Gmail, Calendar, and every Workspace API. 40+ agent skills included." / X</a></li>

</ul>
</details>

**社区讨论**: 评论者意见不一：一些人批评该员工判断力差，发布了可能被误认为是官方产品的项目；另一些人则认为解雇体现了官僚主义的过度干预，引用了普内尔的官僚铁律。一些前谷歌员工指出，这类副业项目在“20%时间”政策下曾受到鼓励，但现在面临更严格的审查。

**标签**: `#Google`, `#Open Source`, `#Corporate Policy`, `#Side Projects`, `#Employment`

---

<a id="item-7"></a>
## [将 Moebius 0.2B 图像修复模型移植到浏览器 WebGPU 运行](https://simonwillison.net/2026/Jun/22/porting-moebius/#atom-everything) ⭐️ 8.0/10

Simon Willison 成功将 Moebius 0.2B 图像修复模型移植到浏览器中运行，使用 ONNX Runtime Web 和 WebGPU 后端，并在 simonw.github.io/moebius-web/提供了可用的演示。他借助 Claude Code 作为智能编码助手完成了这一工作。 这表明小型而强大的 AI 模型可以直接在消费级硬件的浏览器中运行，无需昂贵的 GPU 或云服务器。同时，它也展示了像 Claude Code 这样的 AI 编码代理如何加速复杂的移植任务，使尖端 AI 对开发者和最终用户更加可及。 该模型只有 0.22 亿参数，但声称性能可与 60 倍大小的模型相媲美。首次运行需要从 Hugging Face 下载约 1.27GB 的权重，其中 UNet 部分就有 907MB。演示允许用户加载任意图像，绘制要移除的区域，并在本地运行修复。

rss · Simon Willison · 6月22日 23:43

**背景**: Moebius 是由华中科技大学和 VIVO AI Lab 开发的轻量级图像修复框架。图像修复是指真实地填充图像中缺失或移除区域的任务。原始的 Moebius 版本需要 PyTorch 和 NVIDIA CUDA，仅限于配备强大 GPU 的机器。WebGPU 是一种现代浏览器 API，能够在浏览器中直接进行高性能 GPU 计算，无需插件即可进行神经网络推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonw.github.io/moebius-web/">Moebius Inpainting — WebGPU</a></li>
<li><a href="https://www.mlhive.com/2026/06/why-moebius-0-2b-disrupts-generative-image-inpainting">Why Moebius 0.2B is Disrupting Generative Image Inpainting</a></li>
<li><a href="https://www.creativeainews.com/blog/moebius-inpainting-browser-webgpu-2026/">Moebius Inpainting Model Runs Free in Your Browser</a></li>

</ul>
</details>

**标签**: `#AI/ML`, `#WebGPU`, `#Image Inpainting`, `#Model Porting`, `#Browser ML`

---

<a id="item-8"></a>
## [模型无偏好，唯有上下文影响回答](https://devblogs.microsoft.com/blog/models-dont-have-preferences-they-have-context) ⭐️ 7.0/10

微软的一篇博文澄清，大型语言模型（LLM）并不具有内在偏好；它们的回答是由提示中的上下文和训练数据塑造的。 这一区分至关重要，因为将偏好归因于 AI 模型会导致对其能力和偏见的误解，影响用户设计提示和解读输出的方式。 文章警告不要将 LLM 拟人化，指出诸如持续推荐某特定技术的行为往往源于提示措辞或训练数据的不平衡，而非模型的“观点”。

rss · Microsoft for Developers · 6月22日 14:53

**背景**: 提示工程是精心设计输入以引导 AI 模型生成期望输出的实践，利用上下文和指令。AI 中的拟人化是指人们将人类特质（如偏好或信念）赋予给缺乏意识或主观体验的模型。理解 LLM 本质上是模式匹配系统，有助于用户避免误解。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cloud.google.com/discover/what-is-prompt-engineering">Prompt Engineering for AI Guide | Google Cloud</a></li>
<li><a href="https://www.ibm.com/think/topics/prompt-engineering">What Is Prompt Engineering? | IBM</a></li>

</ul>
</details>

**标签**: `#LLM`, `#prompt engineering`, `#AI misconceptions`, `#machine learning`

---

<a id="item-9"></a>
## [Christophe Pettus 论使用 GUC 诊断索引扫描](https://postgr.es/p/9nd) ⭐️ 7.0/10

Christophe Pettus 解释了如何通过 PostgreSQL GUC 参数 enable_indexscan 和 enable_bitmapscan 临时禁用索引扫描和位图扫描，让 DBA 观察到规划器的替代选择并诊断性能瓶颈。 这项技术提供了一种简单可逆的方法来理解规划器为何选择特定扫描类型，帮助 DBA 在不更改永久配置的情况下优化查询性能。 enable_indexscan 和 enable_bitmapscan 参数可以通过 SET 命令在会话级别设置，禁用它们会迫使规划器考虑替代方法，如顺序扫描或其他索引类型。

rss · Planet PostgreSQL · 6月24日 01:00

**背景**: PostgreSQL 使用查询规划器来确定执行查询的最有效方式，在顺序扫描、索引扫描、位图扫描等之间做出选择。Grand Unified Configuration (GUC) 系统控制许多规划器选项。临时禁用特定扫描类型是一种常见的诊断实践，用于隔离由规划器错误估算引起的性能问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.enterprisedb.com/postgres-tutorials/how-tune-postgresql-guc-parameters">How to Tune PostgreSQL GUC Parameters</a></li>
<li><a href="https://postgresqlco.nf/doc/en/param/enable_indexscan/">PostgreSQL Documentation: enable_indexscan parameter</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database performance`, `#query optimization`, `#index scan`

---

<a id="item-10"></a>
## [Tomas Vondra 更新关于 random_page_cost 的思考](https://postgr.es/p/9na) ⭐️ 7.0/10

Tomas Vondra 分享了他对调整 PostgreSQL random_page_cost 参数的最新见解，灵感来自他在 POSETTE 会议上预先录制的演讲。他的思考比早先的博客文章更进一步，提出了针对现代存储性能进行更精细调整的建议。 这很重要，因为 random_page_cost 直接影响 PostgreSQL 查询规划器在索引扫描和顺序扫描之间的选择。随着存储技术的发展，调整该参数可以显著改善实际工作负载下的数据库性能。 Vondra 最初的帖子建议将 random_page_cost 从默认值 4.0 调低，但经过社区讨论和演讲后，他的新想法提出了更细致的调整方法。他尚未给出新的推荐值，但表示讨论仍在进行中。

rss · Planet PostgreSQL · 6月23日 09:00

**背景**: random_page_cost 是 PostgreSQL 中的一个配置参数，用于估计随机磁盘页面访问的成本，相对于顺序页面访问（seq_page_cost）。默认值 4.0 是为传统硬盘（HDD）设计的，因为其随机寻道开销较高。现代存储如 SSD 和 NVMe 的随机 I/O 延迟要低得多，因此降低 random_page_cost 可以使索引扫描对查询规划器更具吸引力，从而可能提升性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pgpedia.info/r/random_page_cost.html">random _ page _ cost - pgPedia - a PostgreSQL Encyclopedia</a></li>
<li><a href="https://www.linkedin.com/pulse/postgresqls-randompagecost-isnt-just-disk-latency-default-pachot-fphre">PostgreSQL ’s " random _ page _ cost " isn’t just about disk latency...</a></li>
<li><a href="https://shaneborden.com/2023/01/03/tuning-the-postgresql-random_page_cost-parameter/">Tuning the PostgreSQL “ random _ page _ cost ” Parameter</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database performance`, `#random_page_cost`, `#storage tuning`

---

<a id="item-11"></a>
## [理解 PostgreSQL 的 pg_stats 与查询规划](https://postgr.es/p/9mG) ⭐️ 7.0/10

Richard Yen 在 POSETTE 2026 上做了演讲，解释了 PostgreSQL 的 pg_stats 视图如何工作以及内部统计信息如何影响查询规划器的决策。演讲涵盖了 pg_statistic 系统目录的作用以及规划器如何使用数据摘要来选择执行计划。 理解 pg_stats 对于旨在优化查询性能和排查意外计划选择的数据库专业人士至关重要。掌握这些知识有助于调整统计目标并解释 EXPLAIN 输出，从而实现更好的性能。 pg_stats 是 pg_statistic 系统目录的公开可读视图，存储统计摘要，如最常见值、唯一值计数和值分布。查询规划器使用这些估计来决定是进行顺序扫描还是索引扫描，如示例所示，尽管存在州索引，但规划器选择了顺序扫描。

rss · Planet PostgreSQL · 6月22日 08:00

**背景**: PostgreSQL 的查询规划器依赖存储在 pg_statistic 系统目录中的统计信息来估计符合查询条件的行数。这些统计信息由 ANALYZE 命令收集，包括最常见值、直方图边界以及物理行顺序与逻辑列顺序之间的相关性等信息。pg_stats 视图提供了这些数据的人类可读接口，允许用户检查规划器的假设。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/planner-stats.html">PostgreSQL: Documentation: 18: 14.2. Statistics Used by the Planner</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database internals`, `#query optimization`, `#statistics`

---

<a id="item-12"></a>
## [Datasette 1.0a35 新增创建/修改表的 JSON API](https://simonwillison.net/2026/Jun/23/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a35（一个 alpha 版本）引入了新的 JSON API，用于创建和修改表格，包括由文档化的 JSON 端点支持的“创建表”界面和“修改表”操作。 这是向 Datasette 1.0 迈出的重要一步，通过其 JSON API 实现了编程式的表结构管理，扩展了 Datasette 作为动态数据发布平台的实用性。 新的 API 支持定义列、主键、自定义列类型、NOT NULL 约束、字面默认值、表达式默认值和单列外键进行创建；对于修改，支持添加、重命名、重新排序、删除列，更改类型、默认值、约束、主键、外键以及重命名表。此外，该版本还包括稳定的模板上下文文档，用于自定义模板。

rss · Simon Willison · 6月23日 21:34

**背景**: Datasette 是一个开源 Python 工具，可通过 SQLite 数据库将数据发布为交互式网站并进行探索。其 JSON API 允许以编程方式与数据库内容交互。这个 alpha 版本将该 API 扩展到了表结构管理，此前仅能通过 SQL 命令实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.datasette.io/en/1.0a10/json_api.html">JSON API - Datasette documentation</a></li>
<li><a href="https://simonwillison.net/2022/Dec/2/datasette-write-api/">Datasette’s new JSON write API: The first alpha of Datasette 1.0</a></li>

</ul>
</details>

**标签**: `#datasette`, `#data-tools`, `#python`, `#open-source`, `#json-api`

---