---
layout: default
title: "Horizon 日报：2026-06-29 (ZH)"
date: 2026-06-29
lang: zh
---

> 从 24 条内容中筛选出 7 条重要资讯。

---

1. [GLM 5.2 在网络安全基准测试中击败 Claude](#item-1) ⭐️ 8.0/10
2. [布朗大学教授揭露大规模 AI 作弊事件](#item-2) ⭐️ 8.0/10
3. [航天飞机 I/O 处理器电路板详细分析](#item-3) ⭐️ 8.0/10
4. [KIDS 法案强制在线年龄验证](#item-4) ⭐️ 8.0/10
5. [PostgreSQL 中浮点 SUM 查询结果可能不一致](#item-5) ⭐️ 8.0/10
6. [作者用 Claude Code 为 MRI 获取第二意见](#item-6) ⭐️ 7.0/10
7. [重新定义智能体开发：智能体作为团队成员](#item-7) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [GLM 5.2 在网络安全基准测试中击败 Claude](https://semgrep.dev/blog/2026/we-have-mythos-at-home-glm-52-beats-claude-in-our-cyber-benchmarks/) ⭐️ 8.0/10

Z.ai 发布了拥有 7530 亿参数的 GLM 5.2 模型，在 Semgrep 的网络安全基准测试中击败了 Claude，漏洞检测率达到 40%，而 Claude Code 为 32%。 这表明开源模型在特定领域可以超越领先的专有模型，凸显了开源 AI 的快速进步及其降低网络安全任务成本的潜力。 GLM 5.2 支持 100 万 token 的上下文窗口，适用于长期智能体工作流；但其 7530 亿的参数量需要大量硬件资源，对大多数用户来说本地部署具有挑战性。

hackernews · jms703 · 6月28日 17:50 · [社区讨论](https://news.ycombinator.com/item?id=48709670)

**背景**: 网络安全基准测试评估 AI 模型检测代码漏洞的能力。Semgrep 的基准测试使用其 Mythos 引擎发现的漏洞。像 GLM 5.2 这样的开源模型由于训练技术和模型架构的进步，正日益与 Claude 等专有模型竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://registry.ollama.ai/library/glm-5.2">GLM - 5 . 2 is Z.ai’s flagship model for the era of long-horizon tasks.</a></li>
<li><a href="https://openrouter.ai/z-ai/glm-5.2">GLM 5 . 2 - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://www.buildfastwithai.com/blogs/glm-5-2-review-2026">GLM - 5 . 2 Review 2026: Z.ai's 1M-Context AI Model</a></li>

</ul>
</details>

**社区讨论**: 一些用户称赞 GLM 5.2 在日常编程中表现良好，而另一些用户指出 DeepSeek V4 Pro 在他们自己的基准测试中表现更好。还有关于将 GLM 5.2 与“Claude Code”进行比较是否合适的争论，因为 Claude Code 是一个智能体工具，而非纯 LLM。

**标签**: `#LLM`, `#benchmark`, `#cybersecurity`, `#GLM`, `#AI`

---

<a id="item-2"></a>
## [布朗大学教授揭露大规模 AI 作弊事件](https://english.elpais.com/education/2026-06-28/ai-fraud-at-brown-university-academic-integrity-is-at-risk.html) ⭐️ 8.0/10

布朗大学一位教授公开谴责考试中普遍的 AI 辅助作弊行为，指出 GPTZero 等当前检测工具的失效。这引发了关于学术诚信和根本性评估改革必要性的新一轮讨论。 这一事件凸显了 AI 检测软件的不足以及为 AI 时代重新设计评估的紧迫性。它迫使教育工作者和机构重新思考评分、监考乃至考试本身的目的是什么。 这位教授是博弈论研究者，他指出学生面临囚徒困境，使用 AI 成为理性选择。该事件涉及一次开卷但闭网的考试，批评者认为这本身就是矛盾且问题的一部分。

hackernews · geox · 6月28日 16:41 · [社区讨论](https://news.ycombinator.com/item?id=48708991)

**背景**: AI 生成文本检测是一个二分类任务，但 GPTZero 等工具仍不可靠，误报率很高。许多教育工作者现在提倡现场手写考试和口头面试作为更稳健的替代方案。更广泛的挑战在于，大语言模型能瞬间生成连贯答案，使传统的带回家考试变得过时。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPTZero">GPTZero</a></li>
<li><a href="https://arxiv.org/abs/2310.14724">[2310.14724] A Survey on LLM-Generated Text Detection: Necessity, Methods, and Future Directions</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者普遍赞同该教授的评估，许多人主张采用对抗性课程设计和现场考试。有人指出评分本身就是为公司在做免费服务，而另一些人则注意到学生使用 AI 是博弈论下的必然选择。讨论中还批评了“带回家、闭卷”考试这一自相矛盾的概念。

**标签**: `#AI in education`, `#academic integrity`, `#assessment reform`, `#Hacker News discussion`

---

<a id="item-3"></a>
## [航天飞机 I/O 处理器电路板详细分析](https://www.righto.com/2026/06/space-shuttle-io-processor-boards.html) ⭐️ 8.0/10

文章对航天飞机 I/O 处理器的电路板进行了详细检查，重点介绍了玻璃电容器的使用，并讨论了抗辐射性能。 这项分析提供了对历史太空系统硬件设计的罕见见解，揭示了在抗辐射和冗余方面的工程权衡，这些权衡影响了未来的航空航天计算。 I/O 处理器是 IBM AP-101B 计算机中独立于 CPU 的单元，其电路板上采用了康宁公司制造的玻璃电容器，该电容器以耐高温和抗辐射性能著称。

hackernews · pwg · 6月28日 16:16 · [社区讨论](https://news.ycombinator.com/item?id=48708700)

**背景**: 航天飞机的数据处理系统（DPS）采用了五台通用计算机（GPC）以实现冗余。每台 GPC 由 IBM AP-101B CPU 和独立的 I/O 处理器组成。玻璃电容器是一种小众元件，因其在高温和辐射等恶劣环境中的稳定性而受到重视。抗辐射加固对于在太空运行的电子设备至关重要，可防止宇宙射线和粒子辐射导致的故障。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/IBM_System/4_Pi">IBM System/4 Pi - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Space_Shuttle">Space Shuttle - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Radiation_hardening">Radiation hardening - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区对玻璃电容器的使用表现出浓厚兴趣，一位评论者表示之前不知道存在这种元件。另一位评论者推测了低密度电路板的抗辐射能力，并询问了五台计算机的冗余方案。

**标签**: `#space shuttle`, `#hardware`, `#vintage computing`, `#reverse engineering`

---

<a id="item-4"></a>
## [KIDS 法案强制在线年龄验证](https://www.eff.org/deeplinks/2026/06/kids-act-would-require-age-checks-get-online) ⭐️ 8.0/10

美国众议院提出的 KIDS 法案要求在线平台在允许访问前验证用户年龄，违规将面临处罚。 该法案可能从根本上改变用户与互联网的互动方式，对所有用户（不仅是未成年人）的隐私、言论自由和安全构成重大担忧。 法案覆盖使用个人数据进行广告、营销或内容推荐的平台，但排除了许多网站如讨论论坛和银行网站；执法依赖于从身份证件上传到 AI 生物识别的年龄验证方法。

hackernews · bilsbie · 6月28日 11:56 · [社区讨论](https://news.ycombinator.com/item?id=48706560)

**背景**: 年龄验证法律在全球范围内因儿童在线安全问题而获得关注，但批评者警告称，此类系统会带来身份盗窃和监控等隐私风险。技术方法包括政府身份证件检查、信用卡验证以及基于自拍的 AI 年龄估计。KIDS 法案是美国多项提案之一，反映了政治推动，但一些人认为社交媒体对心理健康的危害缺乏科学证据支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Age_verification_system">Age verification - Wikipedia</a></li>
<li><a href="https://www.eff.org/deeplinks/2025/12/10-not-so-hidden-dangers-age-verification">10 (Not So) Hidden Dangers of Age Verification | Electronic Frontier Foundation</a></li>
<li><a href="https://realeyes.ai/blog/how-does-online-age-verification-work/">How Does Age Verification Work Online? A Simple Guide</a></li>

</ul>
</details>

**社区讨论**: 评论者对法案的有效性和动机表示怀疑，指出缺乏社交媒体损害心理健康的明确证据。有人指出科技公司的政治游说，另一些人则强调在多年建议用户保护隐私后反而要求提供个人信息的讽刺之处。

**标签**: `#internet regulation`, `#age verification`, `#privacy`, `#policy`, `#civil liberties`

---

<a id="item-5"></a>
## [PostgreSQL 中浮点 SUM 查询结果可能不一致](https://postgr.es/p/9nx) ⭐️ 8.0/10

在 PostgreSQL 中，对 double precision 列进行 SUM 查询时，即使数据未变，重复执行也可能得到不同结果，原因是并行聚合和浮点数运算的非结合性。 这种微妙的非确定性可能导致报表和仪表盘中的迷惑，依赖稳定 SUM 结果的开发者可能需要禁用并行查询或改用精确数值类型。 该行为源于并行工作者以不同顺序对部分结果求和，而浮点数加法不满足结合律，最终结果取决于执行计划，而执行计划可能因代价估算变化。

rss · Planet PostgreSQL · 6月28日 19:45

**背景**: 浮点数（如 double precision）是近似表示，加法不满足结合律；(a+b)+c 可能不同于 a+(b+c)。PostgreSQL 并行查询将 SUM 拆分为由工作者计算的局部和，再组合，组合顺序可能改变，导致不同的舍入误差。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://boringsql.com/posts/same-rows-different-sum/">Same rows, different SUM | boringSQL</a></li>
<li><a href="https://www.postgresql.org/docs/current/parallel-query.html">PostgreSQL : Documentation: 18: Chapter 15. Parallel Query</a></li>
<li><a href="https://en.wikipedia.org/wiki/Floating-point_arithmetic">Floating-point arithmetic - Wikipedia</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#floating-point`, `#database`, `#SQL`, `#query execution`

---

<a id="item-6"></a>
## [作者用 Claude Code 为 MRI 获取第二意见](https://antoine.fi/mri-analysis-using-claude-code-opus) ⭐️ 7.0/10

一位作者使用 Anthropic 的 Claude Code（一种 AI 编码代理）来分析其 MRI 报告，并挑战了医生关于肩部肌腱病的治疗建议。 这展示了大型语言模型在医疗保健中的新颖、真实应用，既凸显了 AI 辅助第二意见的潜力，也强调了在医疗 AI 使用中信任和验证的迫切需求。 Claude Code 原本设计用于编码任务，但被搭配 Opus 模型用于解读 MRI 报告。作者指出，AI 帮助澄清了歧义，但同时也承认超声波在检测钙化方面并不可靠，而钙化是治疗指南中的关键因素。

hackernews · engmarketer · 6月28日 16:35 · [社区讨论](https://news.ycombinator.com/item?id=48708941)

**背景**: Claude Code 是 Anthropic 推出的一款代理式编码工具，驻留在终端中，帮助开发者编辑文件、运行命令和分析代码。在此案例中，用户将它改用于分析医疗文本，展现了其多功能性。这一事件也触及了关于 AI 在医疗诊断中可靠性的更广泛讨论，即使是专家也警告不要过度依赖不完整的数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://docs.anthropic.com/en/docs/claude-code/overview">Claude Code overview - Anthropic</a></li>

</ul>
</details>

**社区讨论**: 一位放射科医生评论说，没有完整的 3D MRI 数据集很难评估，并指出超声波在检测钙化方面效果不佳。另一位用户反思了 AI 在医学中带来的不适感，还有一位用户分享了自己被误诊的个人经历，突显了问题的严重性。社区态度复杂：AI 提供了清晰度和可及性，但信任仍然是重大挑战。

**标签**: `#AI in healthcare`, `#LLM applications`, `#medical diagnosis`, `#Claude Code`

---

<a id="item-7"></a>
## [重新定义智能体开发：智能体作为团队成员](https://simonwillison.net/2026/Jun/28/jon-udell/#atom-everything) ⭐️ 7.0/10

Jon Udell 主张将叙事从“人机回环”转向“智能体加入我们的回环”，提议开发者邀请 AI 智能体进入现有的人主导流程，而非被排除在回环之外。 这种重新定义挑战了围绕智能体 AI 的主流话语，强调人的权威和协作开发，可能影响团队在不失去监督的情况下采用 AI 辅助编码的方式。 Udell 批评“人机回环”一词将权威让渡给机器，并提倡透明、可审查的智能体辅助流程，避免产生不可审查的拉取请求。

rss · Simon Willison · 6月28日 21:57

**背景**: 智能体开发指使用 AI 智能体自主规划和执行软件开发任务。“人机回环”（human in the loop）传统上让人监督 AI，但 Udell 认为这暗示人是次要的。相反，他提出“智能体在回环中”（agent in the loop），将智能体邀请到现有人类工作流中，保留人的控制和审查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/ai-agentic-development-road-ahead-from-tech-mind-organisation-irfan-m-7lh9e">AI Agentic Development – The Road Ahead from the Tech Mind to...</a></li>
<li><a href="https://www.ibm.com/think/topics/ai-agents">What Are AI Agents ? | IBM</a></li>
<li><a href="https://angular.love/onboarding-ai-agents-into-your-angular-team">Onboarding AI Agents into Your Angular Team - Angular.love</a></li>

</ul>
</details>

**标签**: `#agentic development`, `#human-in-the-loop`, `#AI-assisted coding`, `#software engineering`, `#code review`

---