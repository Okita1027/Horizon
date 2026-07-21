---
layout: default
title: "Horizon 日报：2026-07-21 (ZH)"
date: 2026-07-21
lang: zh
---

> 从 44 条内容中筛选出 11 条重要资讯。

---

1. [黑客清空罗马尼亚全部土地登记数据库](#item-1) ⭐️ 9.0/10
2. [谁在担心中国 AI 模型？](#item-2) ⭐️ 8.0/10
3. [AI 在寻找反例方面超越人类](#item-3) ⭐️ 8.0/10
4. [中国开放权重 AI 策略正在战胜美国专有模型](#item-4) ⭐️ 8.0/10
5. [arXiv 上 AI 写作测量显示 ChatGPT 后激增](#item-5) ⭐️ 8.0/10
6. [Ben Thompson 提议美国立法将 AI 训练数据视为合理使用并禁止蒸馏限制](#item-6) ⭐️ 8.0/10
7. [泄露的 Sam Altman 邮件揭示开源 AI 策略](#item-7) ⭐️ 8.0/10
8. [AI 狂热损害企业决策](#item-8) ⭐️ 8.0/10
9. [PostgreSQL 18 实现近乎瞬时的数据库克隆](#item-9) ⭐️ 7.0/10
10. [AI 编程代理大幅降低家用设备逆向工程成本](#item-10) ⭐️ 7.0/10
11. [Claude Code 采用 Rust 重写的 Bun 实现更快启动](#item-11) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [黑客清空罗马尼亚全部土地登记数据库](https://news.risky.biz/risky-bulletin-hacker-wipes-romanias-entire-land-registry-database/) ⭐️ 9.0/10

一名黑客在勒索未遂后入侵了罗马尼亚国家地籍与不动产广告局（ANCPI），并清空了整个土地登记数据库（包括备份）。该攻击发生于 2026 年 7 月 14 日前后，导致该国房地产市场瘫痪，所有房产交易暂停。 此事件是国家关键基础设施的一次重大网络安全漏洞，具有严重的社会和经济后果，因为土地所有权记录是产权和经济活动的基础。仅有一个离线备份挽救了数据，这凸显了数字治理的脆弱性以及稳健灾难恢复规划的重要性。 ANCPI 已启动将其应用程序迁移至罗马尼亚政府云的工作，由特别电信服务局（STS）协调，预计于 2026 年 7 月 22 日完成。安全公司 KELA 将黑客识别为来自阿尔及利亚奥兰的 Zakaria Mahdjoub；罗马尼亚与阿尔及利亚签有引渡条约。

hackernews · speckx · 7月20日 13:28 · [社区讨论](https://news.ycombinator.com/item?id=48978605)

**背景**: 罗马尼亚的土地登记由 ANCPI 通过 e-Terra 系统管理，该系统支撑着全国每一笔房产交易。黑客清空了生产环境和备份副本，但一个离线备份得以保留，避免了完全损失。罗马尼亚的政府云计划由国家复苏与韧性计划（NRRP）资助，旨在集中并保护公共机构的数据存储。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybernews.com/security/hacker-deletes-romanian-land-registry-database/">Hacker deletes country’s entire land registry database after ...</a></li>
<li><a href="https://news.risky.biz/risky-bulletin-hacker-wipes-romanias-entire-land-registry-database/">Hacker wipes Romania's entire land registry database</a></li>
<li><a href="https://byteiota.com/romania-land-registry-hack-wipe/">Romania’s Land Registry Was Wiped. One Backup Saved It.</a></li>

</ul>
</details>

**社区讨论**: 社区评论对潜在的腐败表示担忧，有罗马尼亚朋友指出政府 IT 合同常交给关系户，而这些关系户未能实施适当的安全措施。讨论还聚焦于黑客身份以及罗马尼亚与阿尔及利亚之间存在的引渡条约，但一些人对问责持怀疑态度。还有人将其与之前韩国政府数据中心因电池火灾丢失 900TB 数据且无备份的事件进行对比。

**标签**: `#cybersecurity`, `#data breach`, `#critical infrastructure`, `#Romania`, `#land registry`

---

<a id="item-2"></a>
## [谁在担心中国 AI 模型？](https://stratechery.com/2026/whos-afraid-of-chinese-models/) ⭐️ 8.0/10

Stratechery 的一篇分析文章探讨了中国 AI 模型（如 DeepSeek 和 Qwen）如何以更低的成本提供有竞争力的性能，且通常为开源，从而威胁到像 OpenAI 和 Anthropic 这样的风投支持的美国实验室。 这很重要，因为它颠覆了高估值 AI 实验室的商业模式，迫使他们可能降价，并质疑大规模 API 定价的可持续性。同时，它使先进 AI 的获取更加普及，改变了竞争格局。 文章指出中国模型正在压低溢价 API 定价，社区成员报告了模型切换的经验证据以及来自中国数据中心的巨大流量。技术细节包括 DeepSeek-V3 的混合专家架构（671B 总参数）和 Qwen 近十亿次累计下载。

hackernews · mfiguiere · 7月20日 11:05 · [社区讨论](https://news.ycombinator.com/item?id=48977128)

**背景**: 中国 AI 公司如 DeepSeek（由对冲基金 High-Flyer 支持）和 Qwen（来自阿里云）发布了强大的开放权重模型，与美国的顶级系统相抗衡。例如，DeepSeek-V3 采用混合专家架构和多头隐式注意力机制，实现了高效推理。这种开源趋势降低了门槛，威胁到依赖专有模型和高 API 定价的风投实验室。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://www.technologyreview.com/2026/02/12/1132811/whats-next-for-chinese-open-source-ai/">What’s next for Chinese open-source AI | MIT Technology Review</a></li>
<li><a href="https://www.nytimes.com/2026/06/25/technology/zai-china-artificial-intelligence-models.html">Chinese A.I. Models Gain Ground on Anthropic and OpenAI - The New York Times</a></li>

</ul>
</details>

**社区讨论**: 社区评论显示了不同的体验：一位测试了约 50 个模型的用户发现中国模型性能具有竞争力；另一位担心风投对价格压低的恐惧。有评论者轻松从 Claude Code 切换到 Codex，反驳了用户粘性的假设。还有一位注意到来自中国的数据中心对分析网站产生巨大流量。

**标签**: `#AI`, `#Chinese models`, `#industry dynamics`, `#open source`

---

<a id="item-3"></a>
## [AI 在寻找反例方面超越人类](https://xenaproject.wordpress.com/2026/07/20/human-mathematicians-are-being-outcounterexampled/) ⭐️ 8.0/10

最近一篇题为“人类数学家正被反例超越”的博客文章指出，AI 系统越来越能够找到数学猜想的反例，在某些情况下超越了人类数学家。 这种能力可以通过快速证伪错误猜想为数学家节省时间，使他们专注于有前景的方向，并标志着数学研究方法论的重大转变。 文章引用了 AI 发现开放猜想反例的例子，包括 2026 年 5 月福布斯报道的 OpenAI 的 AI 证伪了一个已有数十年历史的数学理论的案例。

hackernews · artninja1988 · 7月20日 19:03 · [社区讨论](https://news.ycombinator.com/item?id=48983382)

**背景**: 在数学中，反例是证伪猜想或陈述的具体实例。传统上，寻找反例需要人类的洞察力或暴力搜索。近年来 AI 的进步，特别是在模式识别和自动推理方面，使机器能够系统地探索大搜索空间并更有效地识别反例。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.forbes.com/sites/lanceeliot/2026/05/26/openais-breakthrough-on-famed-math-problem-actually-proves-that-using-ai-to-find-counterexamples-is-a-smart-strategy-for-everyone/">OpenAI’s Breakthrough On Famed Math Problem Actually Proves That Using AI To Find Counterexamples Is A Smart Strategy For Everyone</a></li>
<li><a href="https://www.forbes.com/sites/lanceeliot/2026/05/26/openai-ai-disproves-math-conjecture/">OpenAI AI Finds Counterexample To Decades-Old Math Theory</a></li>
<li><a href="https://bigdata.duke.edu/projects/ai-powered-discovery-of-counterexamples-in-discrete-mathematics/">AI-Powered Discovery of Counterexamples in Discrete Mathematics - JOINT Math+/Data+ Project - Duke Rhodes iiD</a></li>

</ul>
</details>

**社区讨论**: 评论者反应不一：一些人欢迎这一发展，认为可以节省时间（satvikpendem）；另一些人则思考是否存在能胜过 AI 的“人类冠军”（dzdt）。一条评论提到一个历史案例，一个有缺陷的猜想导致一位数学家的职业困境，暗示 AI 本可以避免这种情况（hintymad）。

**标签**: `#AI`, `#mathematics`, `#research`, `#counterexample`, `#machine learning`

---

<a id="item-4"></a>
## [中国开放权重 AI 策略正在战胜美国专有模型](https://werd.io/american-ai-is-locked-down-and-proprietary-its-losing/) ⭐️ 8.0/10

一篇文章指出，中国的开放权重 AI 模型正在获得市场份额并战胜美国的专有模型，声称 80%的初创公司现在使用中国的开放权重模型。这标志着全球 AI 格局的重大转变。 这很重要，因为它挑战了美国专有 AI 模型的主导地位，可能重塑市场动态，鼓励更多开放模型采用，减少对封闭系统的依赖。同时也凸显了开放性在 AI 发展中的战略重要性。 文章引用了一项具体统计，即 80%的初创公司使用中国模型，但社区评论者质疑这一证据，指出许多初创公司仍然依赖像 Claude 和 Codex 这样的美国模型。争论还涉及开放权重模型是否适用于生产级 LLM 任务。

hackernews · benwerd · 7月20日 14:21 · [社区讨论](https://news.ycombinator.com/item?id=48979269)

**背景**: 开放权重的 AI 模型是指其训练参数公开发布的模型，任何人都可以运行、微调和部署，而无需受限于供应商，这与仅通过 API 访问的专有模型不同。中国通过百度、阿里巴巴和 DeepSeek 等公司积极发布开放权重模型，以与美国的前沿模型竞争。这一策略与美国的方法形成对比，美国领先公司如 OpenAI 保持其模型专有。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/open-models/">Open models by OpenAI</a></li>
<li><a href="https://lmmarketcap.com/open-source-ai-models">Best Open Source AI Models & LLM Leaderboard (2026)</a></li>
<li><a href="https://www.gumloop.com/blog/open-weight-ai-models">7 best open weight AI models I've tested in 2026 - gumloop.com</a></li>

</ul>
</details>

**社区讨论**: 评论者意见不一：一些人同意文章观点，引用历史趋势表明免费开放系统最终会主导（例如个人电脑对小型计算机，Linux 对 UNIX）。其他人质疑这一说法，指出开放权重模型在生产中使用有限，并质疑 80%的统计数据。对文章的证据和轶事性质表示怀疑。

**标签**: `#AI`, `#open-source`, `#China`, `#LLMs`, `#strategy`

---

<a id="item-5"></a>
## [arXiv 上 AI 写作测量显示 ChatGPT 后激增](https://unslop.run/blog/measuring-ai-writing-on-arxiv) ⭐️ 8.0/10

这一测量提供了有力证据，表明大语言模型已迅速改变学术写作，尤其在计算机科学领域，引发了关于研究真实性、同行评审及学术交流未来的关键问题。 该检测器结合了三种评分方法，并有意调整以减少误报，但社区成员报告称其个人在 LLM 之前的文本误报率很高，对方法的可靠性提出质疑。

hackernews · dopamine_daddy · 7月20日 16:36 · [社区讨论](https://news.ycombinator.com/item?id=48981206)

**背景**: arXiv 是一个广泛使用的科学论文预印本存储库，尤其在物理学、数学和计算机科学领域。AI 文本检测工具通过分析统计模式来区分人类撰写与机器生成的文本，但其准确性存在争议。2022 年底 ChatGPT 的发布引发了大语言模型在许多领域（包括学术写作）的激增。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hastewire.com/blog/how-ai-text-detection-works-methods-explained">How AI Text Detection Works: Methods Explained</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC12231813/">ChatGPT in Academic Writing: A Scientometric Analysis of ...</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S1475158526000986">A systematic review of AI-assisted academic writing: Tools ...</a></li>

</ul>
</details>

**社区讨论**: 社区评论对检测准确性深表怀疑，用户上传自己 LLM 之前的论文却得到高分机器撰写分数（如 40%至 74%）。一位评论者质疑检测器分数的最终组合方式以及缺乏开源代码，使得复现变得困难。

**标签**: `#AI detection`, `#arXiv`, `#machine learning`, `#academic publishing`, `#LLM`

---

<a id="item-6"></a>
## [Ben Thompson 提议美国立法将 AI 训练数据视为合理使用并禁止蒸馏限制](https://simonwillison.net/2026/Jul/20/afraid-of-chinese-models/#atom-everything) ⭐️ 8.0/10

Ben Thompson 提议美国通过一项法律，明确将收集数据用于 AI 训练视为合理使用，并禁止禁止蒸馏的服务条款，以帮助美国开源模型与中国对手竞争。他将此与阿里巴巴开源 Qwen 3.8 Max 权重联系起来，此前习近平发表讲话鼓励开源。 该提案可能通过澄清版权法并消除模型蒸馏的障碍，从根本上重塑美国 AI 政策，从而加速创新并与中国模型竞争。如果通过，它将为实验室提供保护，并确保大型模型的知识为他人进一步开发所用。 蒸馏涉及通过 API 查询来训练较小的模型，Thompson 认为这几乎无法阻止。该提案至少适用于美国公司。阿里巴巴的 Qwen 3.8 Max 是一个 2.4 万亿参数模型，几乎与 Kimi K3 的 2.8T 一样大。

rss · Simon Willison · 7月20日 17:09

**背景**: 知识蒸馏将知识从大型模型转移到较小的模型，常用于创建高效模型。版权法中的合理使用是一种未经许可使用受版权保护材料的抗辩，但其在 AI 训练数据上的适用目前在法庭上存在争议。Thompson 的提案旨在解决这一不确定性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/knowledge-distillation">What is Knowledge distillation? | IBM</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#open source AI`, `#Chinese AI models`, `#distillation`, `#copyright`

---

<a id="item-7"></a>
## [泄露的 Sam Altman 邮件揭示开源 AI 策略](https://simonwillison.net/2026/Jul/20/sam-altman/#atom-everything) ⭐️ 8.0/10

一封泄露的 2022 年 Sam Altman 发给 OpenAI 董事会的邮件概述了一项策略：发布一个能在消费级硬件上运行、能力接近 GPT-3 的开源模型，以抢占先机并阻止类似项目获得资金。 这一揭露提供了罕见的内幕，展示了 OpenAI 的竞争策略，并引发质疑：以开源发布作为遏制竞争的战略工具而非纯粹为公共利益，这种做法的道德影响如何？ 这封邮件写于 2022 年 10 月 1 日，在 2026 年马斯克诉奥特曼案中被曝光。奥特曼特别提到希望在'Stability 或其他人之前'发布该模型，以使得新项目更难以获得资金。

rss · Simon Willison · 7月20日 03:47

**背景**: 到 2022 年底，像 GPT-3 这样的大语言模型需要庞大的服务器集群，个人用户和小型组织无法使用。由于计算需求高，在消费级硬件上本地运行此类模型被认为不切实际。然而，到 2026 年，模型压缩、量化和高效架构的进步使得本地运行有能力的模型变得切实可行——正如搜索结果所提及。这一背景凸显了奥特曼 2022 年策略的前瞻性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.computeleap.com/blog/how-to-run-ai-locally-2026/">Running LLMs on Your Own Hardware: What Actually Works in ...</a></li>
<li><a href="https://hardwarepedia.com/learn/local-ai">Running AI Locally: Complete Hardware & Software Guide (2026 ...</a></li>

</ul>
</details>

**标签**: `#ai-ethics`, `#sam-altman`, `#open-source`, `#generative-ai`, `#openai`

---

<a id="item-8"></a>
## [AI 狂热损害企业决策](https://simonwillison.net/2026/Jul/19/ai-mania/#atom-everything) ⭐️ 8.0/10

Nik Suresh 的文章《AI 狂热正在摧毁全球决策》揭露了非理性的 AI 热情如何导致大公司做出破坏性决策，包括从未使用过 AI 的高管撰写以 AI 为中心的战略，以及工程师为了显得投入 AI 而将 Go 仓库重写为 Zig。 这很重要，因为它揭示了一个危险的反馈循环：供应商和客户双方的高管出于恐惧而 perpetuation 不切实际的 AI 生产力声明，导致整个科技行业资源浪费和战略失误。 文章包含了一些轶事：一家公司设有 token 排行榜，工程师竞相使用 AI token；还有一位高管承认从未用过 ChatGPT 却支持全面 AI 战略。这种动态源于害怕被视为异端或失去合同。

rss · Simon Willison · 7月19日 05:06

**背景**: Zig 是一门系统编程语言，旨在作为 C 语言的现代替代品，以关注健壮性和编译时特性而闻名。Token 排行榜是公司内部追踪员工使用 AI 工具情况的指标，常常鼓励浪费性消耗。科技行业目前正处于对 AI 生产力提升的过高期望中，类似于过去的炒作周期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://whoburnedmore.com/">Who Burned More? AI Token Leaderboard — whoburnedmore</a></li>

</ul>
</details>

**标签**: `#AI`, `#hype`, `#decision-making`, `#corporate`, `#software engineering`

---

<a id="item-9"></a>
## [PostgreSQL 18 实现近乎瞬时的数据库克隆](https://postgr.es/p/9q4) ⭐️ 7.0/10

PostgreSQL 18 新增了 `file_copy_method = clone` 参数，在写时复制文件系统上通过创建元数据指针而非复制数据，实现接近瞬时的 TB 级数据库复制。 这极大减少了数据库克隆的停机时间和资源消耗，为 PostgreSQL 用户带来更快的开发工作流、更高效的测试以及改进的灾难恢复场景。 `clone` 方法需要写时复制文件系统（如 ZFS 或 Btrfs）；文件系统会创建指向相同物理 8KB 页的新元数据条目，只有在页面被修改时才会实际复制数据。

rss · Planet PostgreSQL · 7月21日 01:00

**背景**: 写时复制（COW）是一种资源管理技术，数据在进程或快照间共享，直到有人尝试修改时才创建私有副本。传统上，PostgreSQL 的 `pg_copyfile` 方法会读写每个数据块，使得 TB 级复制非常耗时。新的 `clone` 方法利用 COW 文件系统的能力，仅通过重新映射元数据即可实现瞬时克隆。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://boringsql.com/posts/instant-database-clones/">Instant database clones with PostgreSQL 18 | boringSQL</a></li>
<li><a href="https://postgresqlco.nf/doc/en/param/file_copy_method/">PostgreSQL Documentation: file_copy_method parameter</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#performance`, `#database`, `#copy-on-write`, `#filesystem`

---

<a id="item-10"></a>
## [AI 编程代理大幅降低家用设备逆向工程成本](https://simonwillison.net/2026/Jul/20/cheap-reverse-engineering/#atom-everything) ⭐️ 7.0/10

西蒙·威利森指出，使用 AI 编程代理降低了编码成本，使得逆向工程家用设备更加实用，减少了努力和维护投入。 这改变了爱好者和修补者的投资回报计算方式，使得那些因初始和维护成本高而之前不值得投入的设备自动化成为可能。 关键变化在于，编程代理降低了实现简单自动化的努力，并且减少了维护或丢弃代码的心理负担，因为现在重写代码成本低廉。

rss · Simon Willison · 7月20日 19:24

**背景**: 逆向工程家用设备涉及解析未公开的协议以编程控制它们。传统上，这需要大量努力和持续维护，因为 API 不稳定。AI 编程代理（如 Qoder 或 Zencoder 中使用的）可以自动化部分流程，使得非专家也能操作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@daniel.potts/i-used-an-ai-coding-agent-on-my-phone-to-reverse-engineer-a-smart-light-heres-what-happened-1ca0bfc24499">I Used an AI Coding Agent on My Phone to Reverse - Engineer ...</a></li>

</ul>
</details>

**标签**: `#reverse-engineering`, `#AI agents`, `#coding assistants`, `#home automation`, `#software cost`

---

<a id="item-11"></a>
## [Claude Code 采用 Rust 重写的 Bun 实现更快启动](https://simonwillison.net/2026/Jul/19/claude-code-in-bun-in-rust/#atom-everything) ⭐️ 7.0/10

这一改进直接为千万级 Claude Code 用户降低了启动延迟，同时证明了基于 Rust 重写关键基础设施能在生产环境中带来切实的性能提升。 Claude Code 内嵌的 Bun 版本为 v1.4.0（尚未正式发布的 canary 构建），其二进制文件中包含超过 560 个 Rust 源文件引用，证实 Rust 移植版已投入生产使用。

rss · Simon Willison · 7月19日 03:54

**背景**: Bun 是一个快速的全能 JavaScript 运行环境，最初用 Zig 语言编写，旨在作为 Node.js 的即插即用替代品。Claude Code 是 Anthropic 推出的智能编码工具，运行在终端中，帮助开发者编辑文件、执行命令并加速交付。将 Bun 用 Rust 重写是为了在保持兼容性的同时提升性能与安全性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://docs.anthropic.com/en/docs/claude-code/overview">Claude Code overview - Anthropic</a></li>

</ul>
</details>

**标签**: `#Claude Code`, `#Bun`, `#Rust`, `#performance`, `#AI tools`

---