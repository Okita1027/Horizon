---
layout: default
title: "Horizon 日报：2026-08-03 (ZH)"
date: 2026-08-03
lang: zh
---

> 从 18 条内容中筛选出 7 条重要资讯。

---

1. [数学和理论计算机科学的十项进步](#item-1) ⭐️ 9.0/10
2. [Kakehashi：实验性用户空间让 macOS 命令行程序在 Linux ARM 上运行](#item-2) ⭐️ 8.0/10
3. [eBay 骚扰活动导致 5600 万美元赔偿与监禁](#item-3) ⭐️ 8.0/10
4. [AI 行业公开信：开放权重与监管之争](#item-4) ⭐️ 8.0/10
5. [卡帕西：AI 测试超越‘自行车上的鹈鹕’提示](#item-5) ⭐️ 7.0/10
6. [NixOS-DGX-Spark 为 DGX Spark 带来 Nix 支持](#item-6) ⭐️ 7.0/10
7. [加州 DROP 数据删除请求 8 月 1 日起强制执行](#item-7) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [数学和理论计算机科学的十项进步](https://simonwillison.net/2026/Aug/1/ten-advances-in-mathematics/#atom-everything) ⭐️ 9.0/10

据报道，OpenAI 的下一个主要模型以每个不到 2000 美元的成本解决了数学和理论计算机科学中十个长期未解的问题。

rss · Simon Willison · 8月1日 20:34

**标签**: `#AI`, `#mathematics`, `#OpenAI`, `#theoretical computer science`, `#research`

---

<a id="item-2"></a>
## [Kakehashi：实验性用户空间让 macOS 命令行程序在 Linux ARM 上运行](https://github.com/wie-project/kakehashi) ⭐️ 8.0/10

Kakehashi 是一个实验性用户空间项目，能够在 Linux ARM 上直接运行 macOS 命令行二进制文件。目前已有 7-Zip、curl 和 Xcode Tools Git 等工作原型。 该项目为 Linux ARM 平台上的 macOS 二进制兼容性开辟了一条新路径，目前该领域可用的解决方案很少。如果项目成熟，它可以让开发者和用户在不需要 Apple 硬件或 macOS 授权的情况下运行 macOS 命令行工具，类似 WINE/Proton 对 Windows 应用的意义。 当前原型性能还处于早期阶段，7-Zip 比原生 Linux 慢约 5.2 倍，但作者已经制定了优化计划。该项目仅工作在用户态，避免内核级二进制翻译；社区讨论也已提到与 Darling 项目进行比较或合作，后者有开放的 ARM64 PR。

hackernews · vlad_kalinkin · 8月2日 16:26 · [社区讨论](https://news.ycombinator.com/item?id=49145937)

**背景**: 在操作系统中，用户空间是用户程序运行的区域，通过系统调用与内核隔离。要在 Linux 上运行为 macOS 编译的二进制文件，需要二进制兼容性，这通常要求重新实现 macOS 的库、动态加载器和系统调用行为。现有项目如 Darling 也致力于此，但 ARM64 支持仍不完整，因此 Kakehashi 这样的实验项目很受关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Filesystem_in_Userspace">Filesystem in Userspace - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Binary-code_compatibility">Binary-code compatibility - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者对该项目表现出兴趣，并询问是否可与正在开发 ARM64 支持的 Darling 项目合作。有人称赞项目，但也指出方案仍处在早期阶段；还有用户抱怨“Kakehashi”这个名字不好。另有讨论问：如果采用类似老游戏反编译项目的做法，而不是从头重写库文件，这类虚拟化框架是否会更容易实现。

**标签**: `#macOS`, `#Linux`, `#ARM`, `#compatibility`, `#emulation`

---

<a id="item-3"></a>
## [eBay 骚扰活动导致 5600 万美元赔偿与监禁](https://www.ft.com/content/06ec1b03-d4af-40cf-b12a-4ba5a410f6d2) ⭐️ 8.0/10

前 eBay 安全主管因策划骚扰一对批评该公司的夫妇而被判刑，eBay 也已支付 5600 万美元和解金。eBay 前安全与安保高级总监 Jim Baugh 被判 57 个月监禁，前高级经理 Brian Gilbert 被判已服刑时间并罚款 2 万美元。 此案件凸显了企业问责制以及内部安全团队可能滥用权力对付批评者的风险。它向科技公司发出警示：针对个人的私刑式行动将面临严重的法律和财务后果。 骚扰行动涉及 eBay 全球安全团队的七名成员，其中包括前警察队长，他们协作恐吓 Steiner 夫妇。各被告判刑不一，Baugh 刑期最长，Gilbert 则获已服刑时间并处罚金。

hackernews · JumpCrisscross · 8月2日 19:19 · [社区讨论](https://news.ycombinator.com/item?id=49147435)

**背景**: eBay 是一个主要的电子商务平台，用户在此买卖商品。Steiner 夫妇运营一份批评 eBay 的在线通讯，促使 eBay 安全人员发起骚扰行动，包括发送威胁信息和不受欢迎的包裹。该行为导致了联邦刑事指控和民事和解。

**社区讨论**: 评论者怀疑骚扰行为仅限于 Steiner 夫妇，并暗示其他批评者也可能成为目标。有人呼吁对涉案的前警察队长进行审查，还有人转向抱怨 eBay 的费用和商业做法。

**标签**: `#eBay`, `#corporate accountability`, `#legal`, `#ethics`, `#tech industry`

---

<a id="item-4"></a>
## [AI 行业公开信：开放权重与监管之争](https://simonwillison.net/2026/Aug/2/open-letters/#atom-everything) ⭐️ 8.0/10

2026 年 7 月 24 日，微软发表了公开信《开放权重与美国 AI 领导力》，获得包括 NVIDIA、亚马逊和 OpenAI 在内的 235 家公司签署，反对限制开放权重模型。7 月 28 日，另一封来自前沿 AI 实验室 1324 名员工的《Pacing the Frontier》公开信呼吁美国政府支持对自动化 AI 发展进行国际治理。 这些公开信之争将影响美国及其他地区的 AI 监管和开源政策。微软的信件直接反驳了以安全为由禁止开放权重模型的提案，而 Anthropic 的反对意见则凸显了对威权滥用的担忧，因此结果将影响研究人员、初创企业和全球 AI 竞争力。 微软的信件明确支持蒸馏——即使用一个模型的输出训练另一个模型——作为合法技术，并敦促政策制定者不要将其与盗用混为一谈。值得注意的是，Anthropic 并未签署，而是在三天后由 CEO Dario Amodei 呼吁打击“工业规模的蒸馏操作”，同时坚称该公司从未主张彻底禁止开放权重。

rss · Simon Willison · 8月2日 04:16

**背景**: 开放权重模型公开发布训练后的参数，任何人都可以下载、研究和微调，但它与完整的开源 AI 不同，后者还包括训练数据和代码。政策之争的焦点在于，开放权重能促进透明度、竞争和创新，还是可能被用于网络攻击或威权政府滥用。蒸馏——使用一个模型的输出来训练另一个模型——是一种常见做法，但已成为争议焦点，尤其是在未经原开发者许可的情况下进行时。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>
<li><a href="https://deasadiqbal.medium.com/understanding-open-weights-vs-open-source-models-988b50ce64d7">Understanding Open Weights vs. Open Source Models | by Asad Iqbal | Medium</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#open weights`, `#open source`, `#LLM`, `#technology industry`

---

<a id="item-5"></a>
## [卡帕西：AI 测试超越‘自行车上的鹈鹕’提示](https://twitter.com/karpathy/status/2083749667410727319) ⭐️ 7.0/10

安德烈·卡帕西发推称，像‘创建一只骑自行车的鹈鹕的 SVG’这样的简单提示已不再是测试 LLM 的有效方式。他描述了给 Claude Opus 5《指环王》第一段和 100 万 token 预算（约 10 美元），要求生成一个 three.js 渲染；Opus 花了约两小时，写出了 5500 行程序化代码。 这标志着 AI 能力评估方式的转变，从简单的代码生成提示转向需要物理世界理解和规划的复杂、长周期创造性任务。这可能会推动 AI 社区开发超越传统文本或图像测试的新定性基准。 卡帕西指出，Opus 5 的渲染结果‘有点粗糙但很有趣’，而且 LLM 必须在三维空间中放置和推理物体。评论者还提到一个历史先例：微软对 GPT-4 预发布版本的评估中包含一个用 TikZ 画独角兽的提示，而 VectorGym 等新基准也正在出现，用于 SVG 代码生成。

hackernews · delichon · 8月2日 04:05 · [社区讨论](https://news.ycombinator.com/item?id=49140998)

**背景**: 卡帕西是知名 AI 研究者、曾任特斯拉 AI 总监，他的推文经常引发行业讨论。‘自行车上的鹈鹕’SVG 提示已成为测试 LLM 将空间描述转化为矢量图形代码能力的常见非正式方法。VectorGym 和 StarVector 等基准正在将 SVG 代码生成正式化为评估视觉语言模型的方式。这条推文认为，前沿模型已经超越了这类任务，需要更宏大的评估方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://xcancel.com/karpathy/status/2083749667410727319">Andrej Karpathy (@karpathy): "We're starting to leave the territory where you'd test an LLM by e.g. "create an svg of pelican on a bicycle". As one idea to generalize it, I was interested what Opus 5 would do if I gave it the first paragraph of the Lord of the Rings, a 1M token budget (~$10) and asked for three js render of it. Opus went off for ~2 hours and wrote 5500 lines of code that (procedurally) rendered the story. It's kind of janky but fun. But it's a bit mindboggling that the LLM has to place and</a></li>
<li><a href="https://www.benzinga.com/markets/tech/26/08/60861644/andrej-karpathy-says-ai-has-moved-beyond-simple-prompts-after-claude-opus-builds-3d-lord-of-the-rings-world">Andrej Karpathy Says AI Has Moved Beyond Simple Prompts After Claude Opus Builds 3D Lord of the Rings Wor - Benzinga</a></li>
<li><a href="https://arxiv.org/abs/2603.29852">VectorGym: A Multitask Benchmark for SVG Code Generation ... StarVector VectorGym: A Multi-Task Benchmark for SVG Code Generation and... VGBench: Evaluating Large Language Models on Vector Graphics ... VectorGym: A Multitask Benchmark for SVG Code Generation ...</a></li>

</ul>
</details>

**社区讨论**: 评论者大多同意卡帕西的观点，认为这种粗糙输出恰恰是重点——这类任务能暴露模型对物理世界的理解。有人分享了相关实验，包括 Claude 配合 Blender MCP、制作《回到未来》德罗宁汽车的 3D 动画，以及尝试渲染《神经漫游者》文本（Claude 因版权问题拒绝）。一位评论者提到 GPT-4 预发布评估中曾要求用 TikZ 画独角兽的历史先例。

**标签**: `#AI`, `#LLM`, `#benchmarks`, `#vector graphics`, `#machine learning`

---

<a id="item-6"></a>
## [NixOS-DGX-Spark 为 DGX Spark 带来 Nix 支持](https://github.com/graham33/nixos-dgx-spark) ⭐️ 7.0/10

新的开源项目 NixOS-DGX-Spark 提供了可在 DGX OS（Ubuntu）上运行的 Nix playbooks，还提供了 NixOS USB 镜像和 NixOS 模块，让用户能用 Nix 完整管理 NVIDIA DGX Spark 与 Asus Ascent GX10 系统。 该项目填补了个人 AI 超级计算机在可重现、声明式管理方面的空白。它让 DGX Spark 和 Asus GX10 的用户能够沿用 Nix 生态中成熟的“基础设施即代码”实践，从而简化 AI 工作流工具链和集群部署。 该仓库包含开发环境 shells、playbooks、USB 镜像，以及为 DGX Spark 定制的硬件配置 NixOS 模块。它同时支持 NVIDIA DGX Spark 和同样搭载 NVIDIA GB10 Grace Blackwell Superchip 的 Asus Ascent GX10。

hackernews · graham33 · 8月2日 17:05 · [社区讨论](https://news.ycombinator.com/item?id=49146267)

**背景**: DGX Spark 是 NVIDIA 推出的紧凑型桌面个人 AI 超算，基于 GB10 Grace Blackwell Superchip，配备大容量统一内存和完整的 NVIDIA AI 软件栈，可在本地运行智能体和大型模型。Asus Ascent GX10 是同样基于 GB10 芯片的桌面级 AI 超算。Nix 是一种纯函数式包管理器兼操作系统，能实现可重现、声明式的系统配置，特别适合管理复杂的 GPU/AI 环境。该项目让 Nix 工具链得以在新一代 Arm 架构 AI 设备上使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/graham33/nixos-dgx-spark">GitHub - graham33/nixos-dgx-spark: Use Nix and NixOS on your DGX Spark! · GitHub</a></li>
<li><a href="https://www.nvidia.com/en-us/products/workstations/dgx-spark/">Personal AI Supercomputer Powered by Blackwell | NVIDIA DGX Spark</a></li>
<li><a href="https://www.asus.com/networking-iot-servers/desktop-ai-supercomputer/ultra-small-ai-supercomputers/asus-ascent-gx10/">ASUS Ascent GX10｜Desktop AI supercomputer｜ASUS Global</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论整体非常正面。有用户反馈已在多台 Asus GX10 上用 k3s 和 DeepSeek 跑通该项目，也有人表示这对管理自己的 DGX Spark 非常有帮助。还有评论提到 Claude Code 等 AI 工具对编写 Nix 很有效，以及 microvm.nix 可用于 Firecracker 沙箱；Graham 的工作还被 Flox 的案例研究引用。

**标签**: `#NixOS`, `#Nix`, `#DGX Spark`, `#NVIDIA`, `#Infrastructure`

---

<a id="item-7"></a>
## [加州 DROP 数据删除请求 8 月 1 日起强制执行](https://www.nbcsandiego.com/nbc-7-responds-2/californians-data-deletion-requests-drop-become-enforceable-aug-1/4054771/) ⭐️ 7.0/10

从 2026 年 8 月 1 日起，加州《删除法案》(Delete Act) 进入执法阶段：注册数据经纪商必须在 90 天内处理通过 DROP 平台提交的删除请求，否则每个受影响的加州居民每天将被罚款 200 美元。加州隐私保护局(CPPA)已开始执法，包括对未注册的数据经纪商 Datamasters 处以 45,000 美元罚款。 这是美国最有力的消费者数据删除机制之一，让加州居民可以通过一次验证，强制数百家数据经纪商删除并停止出售其个人信息。这也给数据经纪行业带来了巨大的合规压力，并可能推动其他州采用类似框架。 DROP 请求必须由加州居民提交，并通过政府管理的平台完成身份验证。执法启动时涉及 600 多家注册数据经纪商和约 26 万条排队中的删除请求；罚款按每名受影响居民每天累计，该法律也针对未注册的数据经纪商。

hackernews · MilnerRoute · 8月2日 22:16 · [社区讨论](https://news.ycombinator.com/item?id=49148987)

**背景**: 加州《删除法案》(SB 362) 创建了数据经纪商登记制度，并责成 CPPA 建立 DROP，即“删除请求与退出平台”，居民可借此向所有注册经纪商一次性发送经验证的删除请求。根据该法律，数据经纪商必须在规定时间内删除个人信息并停止出售或共享，违规将面临逐日累加的罚款。此前《加州消费者隐私法案》(CCPA) 已赋予类似的删除权，但 DROP 使这一过程集中化并自动化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://privacy.ca.gov/drop/">Delete Request and Opt-out Platform (DROP) - privacy.ca.gov</a></li>
<li><a href="https://www.techtimes.com/articles/319927/20260708/california-drop-enforcement-hits-aug-1-data-brokers-face-200-per-day-fines.htm">California DROP Enforcement Hits Aug. 1: Data Brokers Face ...</a></li>
<li><a href="https://www.bytebacklaw.com/2026/02/californias-deletion-request-and-opt-out-platform-drop-is-live/">California’s Deletion Request and Opt-Out Platform (DROP) is Live | Byte Back</a></li>

</ul>
</details>

**社区讨论**: Hacker News 评论者大多支持这一理念，并希望其他州也采用类似规则，但也提出了实际担忧：如何对州外数据经纪商执行罚款，以及该工具是否可能删除用户本不想删除的数据（如信用报告/分数）。有人开玩笑称，公司可能会把这类请求存放在名为“drop”的数据库表中；还有人建议构建服务每月自动发送删除请求，以限制监控数据的保留时间。

**标签**: `#privacy`, `#data-protection`, `#regulation`, `#california`, `#compliance`

---