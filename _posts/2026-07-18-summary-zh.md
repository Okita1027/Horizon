---
layout: default
title: "Horizon 日报：2026-07-18 (ZH)"
date: 2026-07-18
lang: zh
---

> 从 38 条内容中筛选出 18 条重要资讯。

---

1. [首次在宜居带岩质系外行星上发现大气层](#item-1) ⭐️ 9.0/10
2. [Firefox 编译为 WebAssembly 在另一个浏览器中运行](#item-2) ⭐️ 9.0/10
3. [德州法院因年龄验证法下令暂停域名](#item-3) ⭐️ 8.0/10
4. [开源 AI 模型市场份额激增](#item-4) ⭐️ 8.0/10
5. [美国联邦航空管理局恢复波音 737 MAX 和 787 的自认证权限](#item-5) ⭐️ 8.0/10
6. [使用 LLM、Docker 和测试实现遗留 Java 现代化](#item-6) ⭐️ 8.0/10
7. [GPT-5.6 Codex 漏洞导致意外删除文件](#item-7) ⭐️ 8.0/10
8. [Mira Murati 的 Thinking Machines Lab 发布 Inkling，一个 975B 开放权重模型](#item-8) ⭐️ 8.0/10
9. [凯泽护士称 AI 和工作场所监控损害护理](#item-9) ⭐️ 7.0/10
10. [Kimi K3：2.8 万亿参数模型，承诺开源权重](#item-10) ⭐️ 7.0/10
11. [WebStorm 2026.2：支持 TypeScript 7、Copilot 和 Agent Skills](#item-11) ⭐️ 7.0/10
12. [PostgreSQL 18 引入 extension_control_path，扩展可存放任意目录](#item-12) ⭐️ 7.0/10
13. [Postgres 19 增加更精细的检查点控制](#item-13) ⭐️ 7.0/10
14. [exit_on_error：PostgreSQL 的快速失败设置可能具有破坏性](#item-14) ⭐️ 7.0/10
15. [pgEdge Spock 6 Beta：更快、更可靠的多主复制](#item-15) ⭐️ 7.0/10
16. [Postgres 19 将默认 TOAST 压缩从 pglz 切换为 LZ4](#item-16) ⭐️ 7.0/10
17. [使用 pg_upgrade --link 将 PostgreSQL 从 9.6 升级到 17](#item-17) ⭐️ 7.0/10
18. [Linus Torvalds：Linux 不反 AI，AI 是有用工具](#item-18) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [首次在宜居带岩质系外行星上发现大气层](https://www.bbc.com/news/articles/cy4kdd1e0ejo) ⭐️ 9.0/10

利用詹姆斯·韦伯空间望远镜（JWST），天文学家首次明确检测到 LHS 1140b——一颗距离地球 48 光年、位于红矮星宜居带内的岩质系外行星——拥有大气层。 这一发现挑战了活跃红矮星周围的岩质行星无法保留大气层的普遍假设，极大扩展了潜在宜居世界及生物特征信号的搜索范围。 LHS 1140b 的质量约为地球的 6.4 倍，每 24.7 天绕其恒星一周；JWST 的发射光谱观测排除了其迷你海王星成分，显示其大气层富含氦气。

hackernews · neversaydie · 7月17日 14:06 · [社区讨论](https://news.ycombinator.com/item?id=48947560)

**背景**: 宜居带（液态水可能存在的区域）内的系外行星是搜寻生命的主要目标。红矮星比太阳更冷更暗，其宜居带离恒星非常近，强烈的恒星耀斑和辐射会剥离行星大气。此前，尚未有该区域的岩质行星被确认保留大气层。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://science.nasa.gov/exoplanet-catalog/lhs-1140-b/">LHS 1140 b - NASA Science</a></li>
<li><a href="https://www.bbc.com/news/articles/cy4kdd1e0ejo">First atmosphere found around Earth-like planet LHS 1140 b</a></li>

</ul>
</details>

**社区讨论**: 评论者惊讶于红矮星周围的岩质行星竟能保留大气层，但引用的一篇论文（arXiv）利用 JWST 数据明确排除了迷你海王星的分类，验证了此次探测。有人指出 48 光年相对较近，引发了关于未来星际探测器及费米悖论的讨论。

**标签**: `#exoplanet`, `#atmosphere`, `#JWST`, `#astronomy`, `#habitable zone`

---

<a id="item-2"></a>
## [Firefox 编译为 WebAssembly 在另一个浏览器中运行](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter 成功将完整的 Firefox 浏览器（Gecko 引擎）编译为 WebAssembly，使其能够在 Chrome 等另一个浏览器内运行，期间借助了 Claude Opus 和 Fable 代币进行 AI 辅助开发以应对移植挑战。 这一突破表明，功能完整的浏览器可以被交叉编译为 WebAssembly，从而为浏览器模拟、跨平台测试以及在现有浏览器内进行沙盒化执行带来了新的可能性。 该项目使用 Wisp 协议将所有网络流量代理到 Puter 的服务器，因为基于浏览器的 WASM 无法打开任意网络连接；AI 代币总成本估计为 25,000 美元，但由于订阅计划实际支出更低。

rss · Simon Willison · 7月16日 23:34

**背景**: WebAssembly（WASM）是一种二进制指令格式，允许在浏览器中执行高性能代码，使 C++ 等语言编写的应用能以接近原生的速度运行。将 Gecko 这样的完整浏览器引擎编译为 WASM 是一项巨大的技术挑战，因为其体量庞大且复杂度高，需要大量的工程投入和 AI 工具来处理庞大的代码库。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.puter.com/labs/firefox-wasm/">Firefox in WebAssembly</a></li>
<li><a href="https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/">Firefox in WebAssembly</a></li>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/wisp-protocol: Wisp is a low-overhead, easy to implement protocol for proxying multiple TCP/UDP sockets over a single websocket. · GitHub</a></li>

</ul>
</details>

**标签**: `#WebAssembly`, `#Firefox`, `#browser emulation`, `#cross-platform`, `#AI-assisted development`

---

<a id="item-3"></a>
## [德州法院因年龄验证法下令暂停域名](https://www.texasattorneygeneral.gov/news/releases/attorney-general-ken-paxton-secures-landmark-legal-victory-lock-pornographic-website-domain-and) ⭐️ 8.0/10

德克萨斯州一家州法院作出缺席判决，命令暂停色情网站 motherless.com 的域名，因其未遵守要求成人内容进行年龄验证的德州众议院第 1181 号法案。 这一裁决开创了一个州对在州外注册和运营的互联网域名执行其法律的先例，引发了关于违反州际商业和域名系统稳定性的担忧。它可能助长其他州采取类似行动，从而损害互联网的全球性。 被告 motherless.com 的所有者未出庭，导致缺席判决；该案未涉及法律合宪性的实质性裁决。域名暂停通过要求注册局（Verisign）更改名称服务器记录来执行，从而有效使网站下线。

hackernews · letmevoteplease · 7月17日 22:35 · [社区讨论](https://news.ycombinator.com/item?id=48952939)

**背景**: 德州众议院第 1181 号法案于 2023 年 9 月 1 日生效，要求成人网站验证用户年满 18 岁。域名暂停是一种机制，法院命令注册局更改名称服务器记录，将域名重定向至扣押通知或使其无法解析。这一技术曾用于联邦层面的反盗版行动（如“我们的网站行动”），但州级使用较为罕见且存在法律争议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Operation_In_Our_Sites">Operation In Our Sites - Wikipedia</a></li>
<li><a href="https://www.nbcdfw.com/news/local/texas-news/a-timeline-of-the-legal-battle-over-texas-age-verification-law/3706903/">What is HB 1181 and why Texas AG is suing porn websites – NBC...</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍批评该裁决是管辖权的过度延伸，指出 motherless.com 可能在德州没有业务运营，而且缺席判决削弱了先例效力。一些人担忧这违反了州际商业，并可能导致 DNS 分裂的滑坡，其他州或国家也可能要求暂停域名。

**标签**: `#internet governance`, `#age-verification`, `#domain seizure`, `#legal`, `#censorship`

---

<a id="item-4"></a>
## [开源 AI 模型市场份额激增](https://stateofopensource.ai/) ⭐️ 8.0/10

根据 OpenRouter 的数据，开源 AI 模型现在占据 63%的代币市场份额，高于四个月前的 40%，每日代币处理量从 8880 亿增长近 5 倍至 4.19 万亿个代币。 这种快速转变威胁着 OpenAI 和 Anthropic 等主要闭源模型公司，因为开源模型使超大规模企业可以免费部署，硬件公司可以优化到设备上，可能重塑 AI 行业的竞争格局。 数据来自 OpenRouter，这是一个服务于 25 万多个应用和 420 万以上用户的统一 API 平台；一位社区成员创建了一个每日更新的仪表盘来追踪这一增长。不过，Mozilla 的原始演示被批评为 LLM 生成且结构糟糕。

hackernews · rellem · 7月17日 14:31 · [社区讨论](https://news.ycombinator.com/item?id=48947825)

**背景**: OpenRouter 提供单一 API 来访问来自开源和闭源提供商的 400 多个 AI 模型，并以代币（AI 模型处理的文本单位）衡量使用量。开源模型已变得与闭源模型越来越具有竞争力，从而推动了这一增长。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openrouter.ai/">OpenRouter</a></li>
<li><a href="https://blogs.nvidia.com/blog/ai-tokens-explained/">What Are AI Tokens ? The Language and Currency... | NVIDIA Blog</a></li>

</ul>
</details>

**社区讨论**: 评论者广泛讨论了其影响：有人推测开源模型将因无许可费和设备优化而杀死闭源模型公司，而详细的数据分析显示 4 个月内代币量增长 5 倍。然而，几位用户批评 Mozilla 的原始演示制作粗糙，很可能是由 LLM 生成的。

**标签**: `#open source`, `#AI`, `#models`, `#market share`, `#community analysis`

---

<a id="item-5"></a>
## [美国联邦航空管理局恢复波音 737 MAX 和 787 的自认证权限](https://www.cnbc.com/2026/07/17/faa-boeing-737-max-787.html) ⭐️ 8.0/10

美国联邦航空管理局（FAA）恢复了波音公司自行签发 737 MAX 和 787 梦想客机适航证书的权限，此前该权限因 2018 年和 2019 年的 737 MAX 致命坠机事故被撤销。 这一监管变化表明 FAA 对波音安全改进的信心，但也引发了对利益冲突的担忧，因为自认证可能削弱独立监督。这将对航空安全、波音声誉以及整个飞机认证流程产生重大影响。 根据恢复的授权，波音的质量代表可以通过组织指定授权（ODA）计划批准合规步骤。FAA 从 2025 年 9 月开始允许有限授权，如今在 2026 年完全恢复。

hackernews · hmm37 · 7月17日 21:22 · [社区讨论](https://news.ycombinator.com/item?id=48952439)

**背景**: 适航证书确认单架飞机安全可运行，与验证设计的型号证书不同。FAA 的 ODA 计划允许波音等制造商在 FAA 监督下自行认证，这是常见做法，但在 MAX 坠机后受到批评。波音拥有超过 1500 名 ODA 代表。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Airworthiness_certificate">Airworthiness certificate</a></li>
<li><a href="https://www.faa.gov/newsroom/faa-statement-boeing-airworthiness-certificates">FAA Statement - Boeing Airworthiness Certificates | Federal Aviation Administration</a></li>
<li><a href="https://en.wikipedia.org/wiki/Organization_Designation_Authorization">Organization Designation Authorization - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论指出了适航证书与型号证书之间的混淆，用户强调两者的区别。一些人表示不信任，认为靠政府维持生存的公司无法保证安全。另一些用户讨论了商业压力推动重新认证，并怀疑消费者反应是否改变了行为。

**标签**: `#aviation`, `#safety`, `#regulation`, `#Boeing`, `#FAA`

---

<a id="item-6"></a>
## [使用 LLM、Docker 和测试实现遗留 Java 现代化](https://martinfowler.com/articles/archaeologist-copilot.html) ⭐️ 8.0/10

Nik Malykhin 在 Martin Fowler 的网站上发表了详细文章，描述了一种基于证据的实用方法，利用 LLM、Docker 和自动化测试将遗留的 Java 1.5 代码库现代化，使其能在现代硬件上运行。 该方法为解决遗留代码现代化这一普遍挑战提供了可复制的方案，展示了如何通过证据和测试有效约束 AI 的使用，而非用于推测性代码生成。 关键见解是将 LLM 生成的建议置于稳定的 Docker 环境中，并通过测试保护逐步重构，从而防止看似合理但错误的 AI 答案引发问题。

rss · Martin Fowler · 7月16日 13:25

**背景**: 遗留现代化涉及更新旧软件系统以在当前平台上运行，通常需要大量努力重构过时代码。LLM 可以通过建议代码更改来辅助，但其输出需要验证。Docker 提供了可复现的测试环境，自动化测试则确保重构后的代码保持正确行为。

**标签**: `#legacy modernization`, `#LLMs`, `#refactoring`, `#Java`, `#software engineering`

---

<a id="item-7"></a>
## [GPT-5.6 Codex 漏洞导致意外删除文件](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

GPT-5.6 的 Codex 存在一个漏洞：在启用完全访问模式且未开启沙盒保护时，可能导致意外删除文件。该漏洞发生在模型试图覆盖 $HOME 环境变量但错误地删除了 $HOME 目录时。 该漏洞凸显了 AI 编程代理在拥有文件系统无限制访问权限时存在的重大安全风险。用户可能遭遇数据丢失，这强调了在生产环境中使用 AI 代理时需采取沙盒和审查机制的重要性。 该漏洞最常见于启用完全访问模式、未使用沙盒运行 Codex 且关闭自动审查的情况下。OpenAI 的 Thibault Sottiaux 调查了多起意外删除文件的报告，并将根本原因描述为模型的偶然失误。

rss · Simon Willison · 7月16日 17:45

**背景**: GPT-5.6 Codex 是 OpenAI 专门用于代码生成、调试和执行终端命令的大型语言模型。'完全访问模式'授予模型读取、修改和删除用户系统上文件的权限。沙盒是一种安全技术，将 AI 代理与底层操作系统隔离，以防止意外操作（如文件删除）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.3-Codex">GPT-5.3-Codex</a></li>
<li><a href="https://vertu.com/guides/gpt-5-6-sol-ultra-codex-integration">GPT-5.6 Sol Ultra in Codex (July 6, 2026 Update) - vertu.com</a></li>

</ul>
</details>

**标签**: `#codex`, `#coding-agents`, `#generative-ai`, `#ai-safety`, `#gpt-5.6`

---

<a id="item-8"></a>
## [Mira Murati 的 Thinking Machines Lab 发布 Inkling，一个 975B 开放权重模型](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 8.0/10

由前 OpenAI CTO Mira Murati 领导的 Thinking Machines Lab 发布了 Inkling，这是一个开放权重的混合专家多模态模型，总参数量 9750 亿（活跃参数 410 亿），采用 Apache-2.0 许可，并在 45 万亿个文本、图像、音频和视频 token 上训练。 此次发布标志着美国开放权重 AI 生态系统的重要补充，为中国开源模型提供了竞争替代方案，并通过 Tinker 平台为微调提供了强大的基础，可能使大规模多模态 AI 的访问更加民主化。 虽然规模令人印象深刻，但 Inkling 并非前沿模型；它旨在作为定制基础，且附带的模型卡和训练数据文档相当简略，缺乏关于训练数据构成的详细披露。

rss · Simon Willison · 7月16日 15:35

**背景**: 开放权重模型提供对训练好的神经网络权重的公开访问，使开发者能够独立微调或部署模型。混合专家（MoE）是一种架构，使用多个专门的子网络（专家）为每个输入选择性激活，从而实现大总参数同时降低计算成本。Inkling 是多模态的，处理文本、图像、音频和视频，这一能力对实际应用越来越重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.unite.ai/thinking-machines-lab-unveils-inkling-its-first-open-weights-multimodal-ai-model/">Thinking Machines Lab Unveils Inkling, Its First Open-Weights ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>

</ul>
</details>

**标签**: `#open-weights`, `#AI`, `#machine learning`, `#Mixture-of-Experts`, `#multimodal`

---

<a id="item-9"></a>
## [凯泽护士称 AI 和工作场所监控损害护理](https://localnewsmatters.org/2026/07/15/kaiser-nurses-say-ai-workplace-surveillance-are-making-their-jobs-and-patient-care-worse/) ⭐️ 7.0/10

凯泽永久医疗集团的护士报告称，AI 工具和工作场所监控指标使工作更困难并降低患者护理质量，但一些医生认为 AI 有助于笔记记录和翻译。 这凸显了 AI 带来的效率提升与对护理质量和员工福祉的潜在负面影响之间的紧张关系，尤其是在同理心和人文关怀至关重要的医疗领域。 大多数投诉集中在呼叫中心指标和限制护理的压力上，而非 AI 本身；一个 AI 同理心试点项目已于 2024 年终止。一些护士报告称，AI 工具通过实时翻译和笔记摘要节省时间并改善护理。

hackernews · gnabgib · 7月17日 22:26 · [社区讨论](https://news.ycombinator.com/item?id=48952880)

**背景**: AI 和工作场所监控越来越多地用于医疗行业，以监控绩效、自动化行政任务并提高效率。然而，批评者认为，这类系统可能使护理非人化、增加员工压力，并优先考虑指标而非患者需求。护士经常面临可能无法反映其护理质量的生产力指标。

**社区讨论**: 评论揭示了不同的观点：一些员工指责指标滥用损害护理，指出持续追踪和缩短患者互动的压力。其他人则捍卫 AI 工具，指出它们减少了行政负担并允许更多时间陪伴患者。讨论强调，问题不在于 AI 本身，而在于如何实施以及优先考虑哪些指标。

**标签**: `#AI`, `#healthcare`, `#workplace surveillance`, `#labor`

---

<a id="item-10"></a>
## [Kimi K3：2.8 万亿参数模型，承诺开源权重](https://simonwillison.net/2026/Jul/16/kimi-k3/#atom-everything) ⭐️ 7.0/10

中国人工智能实验室 Moonshot AI 发布了 Kimi K3，一个拥有 2.8 万亿参数的模型，并承诺在 2026 年 7 月 27 日前开源其权重。目前可通过官网和 API 使用，在自报基准测试中超越了多个顶级模型。 Kimi K3 是迄今最大的开源权重模型，超越了 DeepSeek 的 1.6T 模型，其定价和性能可能重塑 AI 实验室间的竞争。开源权重的发布对于希望本地运行模型的研究人员和开发者尤其重要。 定价为每百万输入 tokens 3 美元，每百万输出 tokens 15 美元，使其成为中国 AI 实验室迄今为止最昂贵的模型。该模型使用的输出 tokens 比前代 K2.6 少得多，并在 Arena.ai 前端代码竞技场中领先，甚至超过了 Claude Fable 5。

rss · Simon Willison · 7月16日 20:19 · [社区讨论](https://news.ycombinator.com/item?id=48947717)

**背景**: “骑自行车的鹈鹕”基准测试是由开发者 Simon Willison 创建的非正式测试，要求 LLM 生成一张鹈鹕骑自行车的 SVG 图像。虽然不是一个严格的基准测试，但它提供了一种快速、可视化的方式来比较模型的质量、成本和速度。该测试已在各种模型上使用了超过 21 个月。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Pelican_on_a_bicycle_AI_benchmark">Pelican on a bicycle (AI benchmark)</a></li>
<li><a href="https://ndurner.github.io/pelican-benchmark">Pelican vs. Llama 3.1 405B and others | Nils Durner’s Blog</a></li>
<li><a href="https://asibiont.com/en/blog/kimi-k3-i-uroki-pelican-benchmark-chto-my-znaem-o-novom-kitayskom-ii-rekorde">Kimi K3 and What We Can Still Learn from the Pelican Benchmark</a></li>

</ul>
</details>

**社区讨论**: 社区成员对数据污染表示担忧，指出鹈鹕图片在训练数据中很常见。其他人指出了分词器的异常，一位用户发现 Kimi K3 将一个简单提示计为 95 个 tokens，暗示可能存在隐藏的系统提示。有人提出了一个更稳健的基准测试，如 SWE-bench-adversarial-pelican-gen，用于测试在压力下的代理工具调用能力。

**标签**: `#AI`, `#LLM`, `#Kimi K3`, `#benchmark`, `#open weights`

---

<a id="item-11"></a>
## [WebStorm 2026.2：支持 TypeScript 7、Copilot 和 Agent Skills](https://blog.jetbrains.com/webstorm/2026/07/webstorm-2026-2/) ⭐️ 7.0/10

WebStorm 2026.2 原生支持 TypeScript 7，无需完整迁移项目即可获得更快的类型检查。同时内置了 GitHub Copilot 集成，并引入了 agent skills（代理技能），让开发者能跨会话复用框架知识。 该版本通过消除单独安装 Copilot 插件的需要并实现持久的 AI 上下文，显著提升了大型 TypeScript 代码库的生产力。Agent Skills 减少了重复配置，使 AI 辅助编码更高效、更具可扩展性。 TypeScript 7 以独立包形式发布，重新导出 TypeScript 6 API，使得 tsc 可以使用新版本，而其他工具可通过 npm 别名继续使用 6.0。本版本新增了 agent skills 管理器，支持 Agent Client Protocol (ACP) 以连接外部 AI 代理。

rss · JetBrains WebStorm · 7月16日 14:46

**背景**: TypeScript 7 是 JavaScript 静态类型检查器的最新主要版本，提供更快的分析和新的语言特性。GitHub Copilot 是一款 AI 驱动的代码补全工具，此前在 WebStorm 中需要安装插件。Agent Skills 是可复用的知识包，通过 ACP 标准为 AI 代理提供框架、约定和工具链的上下文。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.jetbrains.com/webstorm/2026/07/webstorm-2026-2/">Download WebStorm 2026.2: TypeScript 7 Support, AI, and more</a></li>
<li><a href="https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/">Announcing TypeScript 7.0 - devblogs.microsoft.com</a></li>
<li><a href="https://www.jetbrains.com/help/webstorm/use-ai-agents-with-webstorm.html">Use AI agents with WebStorm | WebStorm Documentation - JetBrains</a></li>

</ul>
</details>

**标签**: `#WebStorm`, `#TypeScript`, `#GitHub Copilot`, `#IDE`, `#JetBrains`

---

<a id="item-12"></a>
## [PostgreSQL 18 引入 extension_control_path，扩展可存放任意目录](https://postgr.es/p/9pY) ⭐️ 7.0/10

PostgreSQL 18 引入了新的 GUC 参数 `extension_control_path`，允许数据库管理员将扩展的控制文件和 SQL 文件存放在任何目录，而不仅限于系统默认位置。 这一功能为扩展管理提供了更大的灵活性，用户可以根据项目或环境组织扩展，无需系统级权限，并减少冲突。它解决了数据库管理员常见的痛点。 该 GUC 是一个冒号分隔的路径列表（Windows 上使用分号），并包含 `$system` 以保留默认位置。扩展需要有一个子目录 `extension`，其中包含 `.control` 和 `.sql` 文件。

rss · Planet PostgreSQL · 7月18日 01:00

**背景**: PostgreSQL 扩展是包含 SQL 对象和函数的包，用于添加功能。以前，扩展控制文件必须放在一个编译时指定的单一目录（例如 `SHAREDIR/extension`），使得在自定义或隔离环境中管理很繁琐。新的 `extension_control_path` GUC 遵循了 `dynamic_library_path`（用于共享库）的模式，允许管理员指定多个搜索路径。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/postgres/postgres/commit/4f7f7b0">extension_control_path · postgres/postgres@4f7f7b0</a></li>
<li><a href="https://postgresqlco.nf/doc/en/param/extension_control_path/">PostgreSQL Documentation: extension_control_path parameter</a></li>
<li><a href="https://runebook.dev/en/docs/postgresql/runtime-config-client/GUC-EXTENSION-CONTROL-PATH">postgresql - The Twin Paths: extension_control_path and dynamic_library_path Explained</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#extensions`, `#database management`, `#open source`

---

<a id="item-13"></a>
## [Postgres 19 增加更精细的检查点控制](https://postgr.es/p/9pX) ⭐️ 7.0/10

Postgres 19 为 CHECKPOINT 命令引入了新选项，允许 DBA 指定 MODE（IMMEDIATE 或 SPREAD）和 WAIT 行为，从而更精细地控制 I/O 影响。 这一增强使 DBA 能够在繁忙期间避免写风暴，同时仍然能够在需要时强制执行检查点，提高了生产环境中的操作灵活性。 新的 MODE 选项支持 IMMEDIATE（原始行为）和 SPREAD（节奏写入）。WAIT 选项控制命令是否在启动检查点后返回。选项可以在括号列表中组合。

rss · Planet PostgreSQL · 7月17日 06:05

**背景**: PostgreSQL 使用预写日志 (WAL) 来确保数据完整性。检查点将所有修改的数据从 WAL 刷新到主存储。以前，CHECKPOINT 命令只有一种行为：立即刷新所有内容。这可能会导致繁忙服务器上的 I/O 峰值（写风暴）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/wal-intro.html">PostgreSQL : Documentation: 18: 28.3. Write - Ahead Logging ( WAL )</a></li>
<li><a href="https://www.postgresql.org/docs/current/sql-checkpoint.html">PostgreSQL : Documentation: 18: CHECKPOINT</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database`, `#WAL`, `#checkpoint`, `#Postgres 19`

---

<a id="item-14"></a>
## [exit_on_error：PostgreSQL 的快速失败设置可能具有破坏性](https://postgr.es/p/9pW) ⭐️ 7.0/10

Christophe Pettus 的文章揭示了 PostgreSQL 的 exit_on_error 配置参数（在发生任何错误时终止会话）可能比表面看起来更具破坏性，因为它可能导致不必要的会话终止和数据丢失。 这一点很重要，因为数据库从业者通常为了安全而启用快速失败设置，但在生产系统中，过度激进的错误升级可能会中断操作并降低可用性，尤其是在复杂工作负载下。 exit_on_error 参数默认为关闭。启用后，它会将所有错误（包括可恢复的错误）升级为会话终止，这在长时间运行或批量工作负载中可能特别具有破坏性。

rss · Planet PostgreSQL · 7月17日 01:00

**背景**: PostgreSQL 的 GUC（Grand Unified Configuration，统一配置系统）管理服务器配置参数。exit_on_error 设置控制错误是否终止当前会话。默认情况下（关闭），会话继续；当开启时，任何错误都会杀死连接。这种设计旨在实现快速失败行为，但可能导致意外后果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pgpedia.info/e/exit_on_error.html">exit_on_error - pgPedia - a PostgreSQL Encyclopedia</a></li>
<li><a href="https://www.postgresql.org/docs/current/runtime-config-error-handling.html">PostgreSQL: Documentation: 18: 19.14. Error Handling</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#configuration`, `#error handling`, `#database`

---

<a id="item-15"></a>
## [pgEdge Spock 6 Beta：更快、更可靠的多主复制](https://postgr.es/p/9pV) ⭐️ 7.0/10

Spock 6，PostgreSQL 的多主复制扩展，进入 beta 阶段，引入了自定义 WAL 资源管理器、共享内存进度跟踪、超大重放队列的磁盘溢出支持，并支持 PostgreSQL 16 至 19 版本。 此版本通过消除目录写入争用、减少内存压力以及增强崩溃恢复保证，显著提升了生产环境中多主 PostgreSQL 集群的性能和可靠性，这对高可用分布式数据库部署至关重要。 自定义 WAL 资源管理器使 Spock 能够将进度快照写入 WAL，从而可以使用 pg_waldump 检查复制状态，而共享内存进度跟踪取代了旧的 spock.progress 目录表，减少了 I/O 开销。磁盘溢出功能使得多 GB 的事务可以在不耗尽内存的情况下重放。

rss · Planet PostgreSQL · 7月16日 20:16

**背景**: 多主复制允许多个数据库节点接受写入并相互同步更改，提供高可用性和地理分布。PostgreSQL 的 WAL（预写式日志）是一个持久的日志，记录所有更改；自定义 WAL 资源管理器允许扩展直接与 WAL 集成，从而实现高级复制功能。共享内存进度跟踪通过避免复制期间每个事务的目录写入来减少争用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/custom-rmgr.html">64.2. Custom WAL Resource Managers - PostgreSQL</a></li>
<li><a href="https://wiki.postgresql.org/wiki/CustomWALResourceManagers">CustomWALResourceManagers - PostgreSQL wiki</a></li>
<li><a href="https://docs.pgedge.com/postgresql/v16/internals/custom-wal-resource-managers/">Custom WAL Resource Managers - pgEdge Documentation</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#multi-master replication`, `#pgEdge`, `#WAL`, `#database replication`

---

<a id="item-16"></a>
## [Postgres 19 将默认 TOAST 压缩从 pglz 切换为 LZ4](https://postgr.es/p/9pU) ⭐️ 7.0/10

Postgres 19 计划将默认的 TOAST 压缩算法从 pglz 改为 LZ4，该消息由 Christopher Winslett 宣布。此更改适用于 TEXT、VARCHAR、BYTEA 和 JSONB 等可变长度数据类型。 与 pglz 相比，LZ4 提供更快的压缩和解压速度，这可以提升涉及大量文本或二进制数据的工作负载的整体数据库性能。此更改反映了 PostgreSQL 对性能优化的持续关注。 pglz 是一种自定义算法，设计上优先考虑速度而非压缩比，使用 4096 字节滑动窗口；而 LZ4 是一种广泛使用的高速度开源算法。此更改可通过 default_toast_compression 参数配置，用户如有需要可回退至 pglz。

rss · Planet PostgreSQL · 7月16日 12:00

**背景**: PostgreSQL 中的 TOAST（超大属性存储技术）用于处理超过页面大小（通常 8 kB）的大值，通过压缩和/或行外存储来解决。TOAST 中的压缩历史上使用 pglz，这是一种在 PostgreSQL 7.0 中引入的 LZ77 变体。LZ4 是由 Yann Collet 开发的快速无损压缩算法，于 2011 年首次发布，自 PostgreSQL 14 起已作为可选压缩方法受到支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/storage-toast.html">PostgreSQL: Documentation: 18: 66.2. TOAST</a></li>
<li><a href="https://www.tigerdata.com/blog/optimizing-postgresql-performance-compression-pglz-vs-lz4">PostgreSQL Compression: pglz vs. LZ4 | Tiger Data</a></li>
<li><a href="https://en.wikipedia.org/wiki/LZ4_(compression_algorithm)">LZ4 (compression algorithm)</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#compression`, `#LZ4`, `#database`, `#performance`

---

<a id="item-17"></a>
## [使用 pg_upgrade --link 将 PostgreSQL 从 9.6 升级到 17](https://postgr.es/p/9pT) ⭐️ 7.0/10

本文提供了使用 pg_upgrade 的 --link 标志将 PostgreSQL 直接从 9.6 升级到 17 的实用指南，该标志通过硬链接避免复制数据文件，即使对于多 TB 的数据库也能实现快速升级。 由于 PostgreSQL 9.6 已于 2021 年终止支持，许多组织需要可靠的升级路径到受支持版本。本指南解决了重大版本差距，并阐述了转储/恢复、逻辑复制（对 9.6 不可用）和 pg_upgrade 之间的权衡。 升级使用 --link 标志创建硬链接而非复制数据，使得升级步骤本身快速，与数据库大小无关。文章警告了 9.6 和 17 版本之间已弃用的配置参数，必须在运行 pg_upgrade 之前进行调整。

rss · Planet PostgreSQL · 7月16日 09:35

**背景**: PostgreSQL 主版本升级需要将数据迁移到新集群，因为内部数据格式会发生变化。pg_upgrade 是一个社区维护的工具，通过链接或复制数据文件执行就地升级。不使用 --link 时，pg_upgrade 复制数据，对于大型数据库可能很慢。使用 --link 时，它创建硬链接，使升级几乎瞬间完成，但需要旧集群的数据目录保留到新集群验证通过。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dba.stackexchange.com/questions/222059/pg-upgrade-link-fails-directory-already-in-use-as-a-tablespace">pg _ upgrade -- link fails: `directory "/..." already in use as a ta...</a></li>
<li><a href="https://jasonralph.org/?p=667">CENTOS6 Postgres pg _ upgrade 9 to 11 – In Place – Link – No Copy...</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#pg_upgrade`, `#database upgrade`, `#version migration`

---

<a id="item-18"></a>
## [Linus Torvalds：Linux 不反 AI，AI 是有用工具](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 7.0/10

Linux 内核的创建者和维护者 Linus Torvalds 在 Linux Media 邮件列表上声明，Linux 不是一个反 AI 的项目，AI 是一种有用的工具，并驳斥了任何反对意见。 这一来自顶级维护者的明确表态表明 Linux 内核项目欢迎 AI 工具，可能会影响更广泛的开源社区对 AI 在开发工作流中的接受程度。 Torvalds 承认一年前 AI 的有用性还存在疑问，但如今已不再存疑，不过他指出关于 AI 的经济影响还有其他未解决的问题。

rss · Simon Willison · 7月16日 13:26

**背景**: Linus Torvalds 是 Linux 内核（Linux 操作系统的核心）的原始作者和长期维护者。Linux 内核是最大的开源项目之一，其维护者的观点具有重要影响力。

**标签**: `#linux`, `#kernel`, `#AI`, `#linus-torvalds`, `#open-source`

---