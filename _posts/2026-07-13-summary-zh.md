---
layout: default
title: "Horizon 日报：2026-07-13 (ZH)"
date: 2026-07-13
lang: zh
---

> 从 32 条内容中筛选出 6 条重要资讯。

---

1. [陶哲轩拥抱 LLM 编码代理](#item-1) ⭐️ 9.0/10
2. [Chromium 148 中 Math.tanh 泄露操作系统指纹](#item-2) ⭐️ 8.0/10
3. [Claude Code 每个请求多花 33k Token，OpenCode 仅 7k](#item-3) ⭐️ 8.0/10
4. [无理解的自动化：AI 过度依赖的风险](#item-4) ⭐️ 8.0/10
5. [机械可解释性利用因果性理解大语言模型](#item-5) ⭐️ 8.0/10
6. [RegreSQL 2.0 测试执行计划而非仅行结果](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [陶哲轩拥抱 LLM 编码代理](https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/) ⭐️ 9.0/10

菲尔兹奖得主陶哲轩演示了使用基于 LLM 的现代编码代理来构建可视化和小型应用，强调了它们在非关键软件任务中的实用性。 来自顶尖数学家的认可表明，LLM 编码代理正在成为甚至专家也能使用强大工具，可能加速许多领域的软件开发。 陶哲轩使用与 LLM 代理的引导式交互来生成其研究论文的补充可视化，并指出对于非关键组件而言，风险是可接受的。

hackernews · subset · 7月12日 11:09 · [社区讨论](https://news.ycombinator.com/item?id=48880170)

**背景**: 编码代理是基于自然语言提示生成或协助编写代码的人工智能系统。GPT-4 等大型语言模型使这些代理能够生成功能性软件，但输出可能需要针对关键任务进行验证。

**社区讨论**: 评论者对于 LLM 揭示的软件潜在需求感到兴奋，其中一位指出即使 LLM 停止进步，我们仍需要十年才能消化当前的能力。其他人开玩笑说专家使用 AI 就像用微波炉做晚餐，而另一位则称赞陶哲轩对风险的平衡看法。

**标签**: `#AI-assisted coding`, `#LLM`, `#software development`, `#productivity`, `#Terry Tao`

---

<a id="item-2"></a>
## [Chromium 148 中 Math.tanh 泄露操作系统指纹](https://scrapfly.dev/posts/browser-math-os-fingerprint/) ⭐️ 8.0/10

自 Chromium 148 起，V8 的 Math.tanh 实现改为调用平台的 std::tanh 函数，导致输出因操作系统而异，形成了新的指纹识别向量。 这打破了 JavaScript 数学运算跨平台一致的假设，使得反机器人系统可通过一次函数调用检测操作系统不匹配，进一步削弱了浏览器隐私。 在所有 Math.*函数中，只有 Math.tanh 展现出这种依赖操作系统的行为，因为它是唯一改用宿主数学库（libm）的函数，其他函数仍使用 V8 内置例程。

hackernews · joahnn_s · 7月12日 21:12 · [社区讨论](https://news.ycombinator.com/item?id=48884853)

**背景**: 浏览器指纹识别通过收集浏览器行为的细微差异来识别用户。由于浮点运算实现的差异，JavaScript 数学运算在不同平台上可能略有不同。此前，V8 使用自己的数学例程来确保一致性，但从 Chrome 148 开始，Math.tanh 改为使用操作系统的实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://scrapfly.dev/posts/browser-math-os-fingerprint/">Your Browser Does Math Differently on Every OS, and Anti-Bot Systems Read the Bits · scrapfly.dev</a></li>
<li><a href="https://news.ycombinator.com/item?id=48884853">Since Chromium 148, Math.tanh is now fingerprintable to link underlying OS | Hacker News</a></li>
<li><a href="https://www.darkwavetech.com/projects/device-fingerprinting/math-routine-fingerprinting">Darkwave Technologies, LLC - Math Routine Fingerprinting</a></li>

</ul>
</details>

**社区讨论**: 评论者指出这个向量也可能暴露浏览器版本范围，多数用户不会将 User-Agent 伪装成不同操作系统。有人批评文章由 LLM 生成，怀疑是抓取公司施压修复。其他人主张使用正确舍入的超越函数作为长期解决方案。

**标签**: `#browser fingerprinting`, `#Chromium`, `#JavaScript`, `#privacy`, `#operating system fingerprinting`

---

<a id="item-3"></a>
## [Claude Code 每个请求多花 33k Token，OpenCode 仅 7k](https://systima.ai/blog/claude-code-vs-opencode-token-overhead) ⭐️ 8.0/10

系统性测量发现，Claude Code 每个请求额外发送约 33,000 个 token，而 OpenCode 仅发送约 7,000 个 token，表明其缓存策略和工具调用效率更低，导致 4.7 倍的 token 浪费。 这种低效直接增加了用户成本，并引发对 AI 编程工具开发者是否存在烧 token 动机的质疑。该结果迫使 Anthropic 优化 Claude Code，否则可能失去注重成本的用户，转向更轻量的 OpenCode 等替代工具。 该研究记录了工具与 API 端点之间的所有请求，测量了 harness token 使用量和缓存行为。值得注意的是，Claude Code 中的子代理可能启动多个并行任务，每个任务都产生额外开销，进一步放大 token 消耗。

hackernews · systima · 7月12日 18:25 · [社区讨论](https://news.ycombinator.com/item?id=48883275)

**背景**: Claude Code 和 OpenCode 等 AI 编程工具作为代理助手，自动读取代码库、执行命令和调用工具。每次交互都会产生系统提示、工具定义和编排逻辑的 token 开销。高效的缓存（如 prompt prefix caching）和最小化工具调用对降低成本至关重要。子代理是为处理子任务而派生的独立 AI 进程，但会重复开销并快速消耗 token。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://systima.ai/blog/claude-code-vs-opencode-token-overhead">Claude Code Sends 4.7x More Tokens Than... | Systima Blog</a></li>
<li><a href="https://levelup.gitconnected.com/claude-code-token-burn-the-unplanned-100-month-reality-48587c6a92ce">Claude Code Token Burn: The Unplanned $100... | Level Up Coding</a></li>

</ul>
</details>

**社区讨论**: 社区成员对子代理烧光预算表示不满，有用户指出 Claude Code 甚至对大任务也会启动 7 个子代理。其他人猜测 Anthropic 可能故意设计低效以推动用户升级订阅，并指出系统提示开销已膨胀。该研究的作者承诺后续会进行更详细的任务和定性结果比较。

**标签**: `#AI coding tools`, `#token efficiency`, `#Claude Code`, `#OpenCode`, `#cost analysis`

---

<a id="item-4"></a>
## [无理解的自动化：AI 过度依赖的风险](https://arxiv.org/abs/2607.06377) ⭐️ 8.0/10

一篇题为《无理解的自动化》的新论文警告，在不深入理解 AI 系统的情况下增加自动化可能导致灾难性失败，社区强调了可解释性和人类监督的迫切需求。 随着 AI 系统变得更加复杂和不透明，依赖其输出而不理解其推理过程的风险增加，可能侵蚀医疗、法律和工程等关键领域的专业知识和信任。 该论文及讨论强调，即使是 AI 开发者也可能无法发现模型自信犯错的情况，并提议更严格的要求，如强制 AI 展示工作过程、生成证明以及为事实提供来源。

hackernews · root-parent · 7月12日 16:54 · [社区讨论](https://news.ycombinator.com/item?id=48882554)

**背景**: 可解释人工智能（XAI）是一个专注于使 AI 决策对人类透明且可理解的领域。它对抗许多机器学习模型的‘黑箱’特性，即使是设计者也无法解释特定输出。XAI 对于安全关键应用和维护人类监督至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Explainable_artificial_intelligence">Explainable artificial intelligence - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/explainable-ai">What is Explainable AI (XAI)? | IBM</a></li>
<li><a href="https://www.seangoedecke.com/ai-interpretability/">AI interpretability is further along than I thought | sean goedecke</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了深切担忧：一位指出过度依赖 AI 可能导致不再培养能够发现 AI 错误的专家；另一位要求强制 AI 展示工作过程并生成证明。第三位评论者暗示，‘奇点’不是 AI 在进步，而是人类被推回到无法理解的状态。

**标签**: `#AI`, `#automation`, `#explainability`, `#education`, `#reliability`

---

<a id="item-5"></a>
## [机械可解释性利用因果性理解大语言模型](https://cacm.acm.org/news/can-we-understand-how-large-language-models-reason/) ⭐️ 8.0/10

研究者正在将因果理论应用于机械可解释性，旨在揭示大型语言模型中的隐藏算法和推理结构。 这项工作通过识别实际执行推理的内部组件，而非将模型视为黑箱，有望使大语言模型更加透明和可信。 研究者使用因果发现和干预技术来定位负责推理行为的特定电路和特征，例如时钟时间计算研究中的示例。

hackernews · adunk · 7月12日 18:04 · [社区讨论](https://news.ycombinator.com/item?id=48883090)

**背景**: 机械可解释性是可解释人工智能的一个子领域，旨在通过分析神经元和电路等内部结构来逆向工程神经网络。它通常使用因果理论中的因果方法来理解模型组件如何影响输出，超越了简单的特征归因。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability - Wikipedia</a></li>
<li><a href="https://cloudsecurityalliance.org/blog/2024/09/05/mechanistic-interpretability-101">Mechanistic Interpretability | Decode Neural Networks | CSA</a></li>

</ul>
</details>

**社区讨论**: 评论者对其复杂性表示怀疑，将神经网络比作“意大利面条式代码”，难以完全理解。但部分人对因果方法感兴趣，并分享了相关论文的视频。

**标签**: `#mechanistic interpretability`, `#LLMs`, `#causality`, `#AI reasoning`

---

<a id="item-6"></a>
## [RegreSQL 2.0 测试执行计划而非仅行结果](https://postgr.es/p/9pn) ⭐️ 8.0/10

RegreSQL 2.0 新增执行计划验证功能，使用生产环境的表统计信息来检测因查询计划变化（如从索引扫描变为顺序扫描）导致的性能回退。 这填补了数据库测试中的一个关键盲区：查询返回正确结果但执行路径变慢，这是数据库模式迁移后生产环境宕机的常见原因。 RegreSQL 2.0 比较 EXPLAIN 输出的缓冲区数量和估算成本，标记超出可配置阈值（如基线的 102%）的变化，并高亮显示计划节点类型的变化，例如 'Bitmap Heap Scan → Seq Scan'。

rss · Planet PostgreSQL · 7月12日 18:16

**背景**: PostgreSQL 的查询优化器根据表统计信息选择执行计划。传统的回归测试仅检查输出行，忽略了导致性能下降的计划变化。EXPLAIN 提供估算成本和实际缓冲区使用情况；RegreSQL 自动比较这些指标在代码变更前后的差异。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://boringsql.com/posts/regresql-testing-queries/">RegreSQL: Regression Testing for PostgreSQL Queries | boringSQL</a></li>
<li><a href="https://github.com/dimitri/regresql">GitHub - dimitri/regresql: Regression Testing your SQL queries · GitHub</a></li>
<li><a href="https://www.postgresql.org/docs/current/using-explain.html">PostgreSQL: Documentation: 18: 14.1. Using EXPLAIN</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database testing`, `#performance regression`, `#SQL`, `#RegreSQL`

---