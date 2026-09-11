---
layout: default
title: "Horizon 日报：2026-09-11 (ZH)"
date: 2026-09-11
lang: zh
---

> 从 48 条内容中筛选出 9 条重要资讯。

---

1. [苹果发布首款折叠屏 iPhone Duo，起售价 1999 美元](#item-1) ⭐️ 9.0/10
2. [DeepSeek 发布 V4-1 Flash：552B 多模态 MoE 模型，支持百万级上下文](#item-2) ⭐️ 9.0/10
3. [Shopify 将移动应用从 React Native 迁回原生 Swift 和 Kotlin](#item-3) ⭐️ 8.0/10
4. [研究者还能信任 OpenAI 保管未发表的数学成果吗？](#item-4) ⭐️ 8.0/10
5. [OpenAI 发布 Agents API，支持自托管沙箱](#item-5) ⭐️ 8.0/10
6. [trynix.dev 让你在浏览器中启动过去 13 年的任意 Nix 包](#item-6) ⭐️ 8.0/10
7. [Calif Research 发布 WeWorm：AI 打造的微信零点击蠕虫](#item-7) ⭐️ 8.0/10
8. [JetBrains：微软 Defender 导致 Rider 与 ReSharper 启动缓慢](#item-8) ⭐️ 7.0/10
9. [PostgreSQL 的 max_connections 是内存预算，而非并发上限](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [苹果发布首款折叠屏 iPhone Duo，起售价 1999 美元](https://www.apple.com/iphone-duo/) ⭐️ 9.0/10

苹果在库比蒂诺总部举行的一场 75 分钟录播发布会上正式推出其首款折叠屏手机 iPhone Duo。这款书本式设备可以像书一样开合，起售价 1999 美元，预计最早于 10 月上市。 这是苹果首次正式进入它观望多年的硬件品类，也将迫使所有大屏应用开发者适配折叠屏形态。约 2000 美元的定价同时也在测试：在 Android 折叠屏已经成熟的市场上，消费者愿意为新形态的 iPhone 付多少钱。 被重点讨论的技术细节包括内屏对 Apple Pencil 的支持、铰链与折痕的控制水平，以及设备半折叠时应用的适配方式。早期报道称其入门价约为 2000 美元，并可能于 10 月初开售，这将是史上最贵的主流 iPhone 之一。

hackernews · thecosmicfrog · 9月9日 18:15 · [社区讨论](https://news.ycombinator.com/item?id=49630931)

**背景**: 折叠屏手机把柔性 OLED 面板与机械铰链结合起来，让一台设备既能当手机又能当小平板，代价则长期集中在可见折痕、铰链耐用性以及额外的重量和成本上。三星自 2019 年的 Galaxy Z Fold 系列起带火了这一品类，三星和 Google 都发布了关于自适应布局、折叠姿态处理和应用连续性的开发者指南。苹果此前一直未涉足该市场，因此 iPhone Duo 是它第一次尝试解决同样的铰链、折痕与软件适配难题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/09/09/technology/apple-iphone-duo-foldable-phone.html">Apple Unveils the iPhone Duo, a Foldable Phone That Costs $1,999 - The New York Times</a></li>
<li><a href="https://www.apple.com/newsroom/2026/09/apple-unveils-iphone-duo/">Apple unveils iPhone Duo - Apple</a></li>
<li><a href="https://www.tomsguide.com/phones/iphones/iphone-duo-is-apples-first-foldable-usd2-000-price-release-date-as-early-as-october">iPhone Duo is reportedly Apple's first foldable — $2,000 price, release date 'as early as October' | Tom's Guide</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论（1415 分、2441 条评论）整体对硬件表示认可：有评论者认为支持 Apple Pencil 意义重大，可以直接和客户做白板演示，并称苹果这次或许真的解决了铰链和折痕问题。质疑声主要围绕价格——“我不会花两千美元买它”；也有人抱怨手机越做越大，还有人希望苹果的入场能真正推动开发者为折叠屏设计专门的应用布局，而不是简单拉伸手机界面。

**标签**: `#Apple`, `#iPhone Duo`, `#Foldable Phones`, `#Hardware`, `#Consumer Tech`

---

<a id="item-2"></a>
## [DeepSeek 发布 V4-1 Flash：552B 多模态 MoE 模型，支持百万级上下文](https://www.reddit.com/r/LocalLLaMA/comments/1wcbid7/deepseek_v41_flash_is_out/) ⭐️ 9.0/10

DeepSeek 发布了新模型 V4-1 Flash，这是一款多模态的混合专家（MoE）模型，拥有 552B 主干参数，并支持最高一百万 token 的上下文长度。该消息通过 r/LocalLLaMA 上的一则 Reddit 帖子曝光，发帖人调侃这是“以市场崩盘为服务”。 DeepSeek 一向以高影响力且定价激进的模型著称，因此这一规模的多模态 MoE 可能给竞争对手带来新的压力，并进一步拉低业界对开放权重模型能力与成本的预期。如果百万 token 的上下文在实际使用中确实成立，那么过去只有少数前沿模型才能胜任的长文档、图像与视频驱动的智能体工作流将变得更易实现。 该 Reddit 帖本身几乎没有提供技术细节：既未说明每次前向激活的参数数量，也没有基准测试结果、许可条款、量化与本地部署要求，甚至没有发布日期。552B 指的是 MoE 架构中典型的主干参数总量，而 MoE 对每个输入只会激活其中一部分专家，因此实际推理成本预计会远低于同等规模的稠密模型。

reddit · r/LocalLLaMA · /u/tiguidoio · 9月10日 06:54

**背景**: 混合专家（MoE）是一种机器学习技术，其中多个被称为“专家”的子网络各自负责问题空间的一部分，再由路由机制决定由哪些专家处理特定输入；这样模型可以在总参数量极大的同时，每次只计算其中一小部分。所谓“多模态”，是指模型能够跨文本、图像、音频、视频等多种数据类型进行理解与推理，而不只是处理文本，这一路线因 GPT-4o、Google Gemini 等模型而流行。“主干参数”指的是网络主体部分，与处理非文本模态的辅助编码器或适配器相区分。上下文长度则指模型一次能够关注的最大文本量（以 token 计，约为词或子词片段），百万 token 的窗口意味着它可以一次性读完整本书或很长的代码仓库。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/Multimodal_AI">Multimodal AI</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#LLM`, `#Mixture-of-Experts`, `#Multimodal`, `#LocalLLaMA`

---

<a id="item-3"></a>
## [Shopify 将移动应用从 React Native 迁回原生 Swift 和 Kotlin](https://shopify.engineering/back-to-native) ⭐️ 8.0/10

Shopify 工程团队宣布将其移动应用从 React Native 迁回完全原生开发，iOS 使用 Swift、Android 使用 Kotlin，推翻了其在 2020 年做出的跨平台技术选型。该博文在 Hacker News 上引发大规模讨论（798 分、538 条评论），话题集中在原生与跨平台之间的取舍以及 LLM 辅助重写代码上。 Shopify 是 React Native 最重要、最知名的公开采用者之一（与 Meta、微软并列），因此这样一家大型工程组织公开回退到原生，是跨平台与原生之争中极具信号意义的案例。这也让行业内一个更大的问题浮出水面：LLM 辅助的代码重写是否真正改变了平台迁移的成本收益结构。 Shopify 表示 LLM 改变了其 2020 年决策背后的一个核心假设，促使团队从第一性原理重新评估移动端技术栈，最终选择回到原生。讨论中一个值得注意的反方观点是，'LLM 才让迁移变得可行'这一说法存在争议：至少有一位实践者表示，自己主导的一次中型 React Native 转原生迁移大部分工作在 2026 年 1 月之前就已完成，而且几乎没有依赖 LLM 代码辅助。

hackernews · fnthawar2 · 9月10日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=49643982)

**背景**: React Native 是 Meta 最初开发的一套开源框架，让开发者用 JavaScript 和 React 编写 iOS 与 Android 应用，并共享大部分代码，底层仍映射到各平台的原生组件。而完全采用 Swift 和 Kotlin 的原生开发通常能带来更好的性能、更贴合平台的体验以及更少的依赖问题，代价是需要维护两套独立的代码库。共享代码库与原生体验之间的取舍在移动开发社区已争论多年，而近来 LLM 编程助手常被视为降低此类重写成本的可行手段。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/React_Native">React Native</a></li>
<li><a href="https://reactnative.dev/">React Native · Learn once, write anywhere</a></li>

</ul>
</details>

**社区讨论**: 整体讨论氛围倾向于支持迁回原生：有开发者表示自己用 Codex 配合 Maestro，几乎在一夜之间就把一个 15-20 个屏幕的应用迁移到 iOS 和 Android，之后只用几天做打磨；一位长期反对共享代码库的资深 iOS 工程师则称自己感到'非常被验证'。最主要的反方声音来自 netshade：他认同应该离开 React Native，但明确反对'是 LLM 让原本过于昂贵的迁移变得可行'这一叙事，并以自己主导、大部分在 2026 年之前且无 LLM 辅助完成的大型原生重写为例；也有人提到精简 JS 库后获得了 1.5 到 3 倍的性能提升。

**标签**: `#react-native`, `#mobile-development`, `#ios`, `#android`, `#software-architecture`

---

<a id="item-4"></a>
## [研究者还能信任 OpenAI 保管未发表的数学成果吗？](https://mathstodon.xyz/@andreasthom/117240535270608201) ⭐️ 8.0/10

Hacker News 上一条获得 686 分、635 条评论的讨论帖，重新点燃了「数学家能否安全地把未发表成果交给 OpenAI」的争论：数学家 Andreas Thom 及其合作者声称，他们与 OpenAI 模型的私下交流中提出的想法，后来出现在该公司公开发表的结果里，却没有被署名。帖子还链接了 @andreasthom 在 Mathstodon 上的系列贴文以及 Valerio Capraro 在社交平台上的相关发言。 这一事件涉及科研诚信、成果归属与训练数据来源三大问题，也可能直接影响到学术界是否还愿意把新想法交给专有 AI 系统。如果研究者认定自己的未发表工作会变成厂商的成果，学术界与 AI 实验室之间的合作、以及公众对「AI 攻克开放难题」这类宣称的信任都可能被削弱。 有评论指出，OpenAI 据称向约 10 万名研究者提供免费模型访问权限，其内部模型被描述为能以惊人速度解决开放问题，并且曾让一个仍在训练中的模型生成了约 3000 亿个输出 token——一些读者认为这一连串事件「过于凑巧」。另一些人则提醒说，在可验证数学任务上做强化学习并叠加海量算力，完全有可能独立产生超越人类的结果，而与某次具体对话数据无关。

hackernews · pred_ · 9月10日 06:49 · [社区讨论](https://news.ycombinator.com/item?id=49639408)

**背景**: 大语言模型通常在包含网页文本、论坛内容和用户交互的海量语料上训练；而对于推理模型，训练流程越来越多地加入「在答案可校验的问题（如数学题）上做强化学习」这一环节。与之相对，学术规范要求贡献必须通过署名或引用得到承认，因此当某个想法未加署名地出现在厂商论文中时，即便其机制只是统计式训练而非刻意抄袭，看起来也等同于剽窃。本次讨论的源头在 Mathstodon——一个面向数学爱好者的 Mastodon（联邦宇宙）实例，帖子还引用了 Bluesky 以及镜像版 Twitter/X 的内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mathstodon.xyz/">About - Mathstodon</a></li>
<li><a href="https://en.wikipedia.org/wiki/Decentralized_identifier">Decentralized identifier - Wikipedia</a></li>
<li><a href="https://discuss.privacyguides.net/t/recommend-xcancel-com-twitter-frontend/21177">Recommend xcancel.com (Twitter Frontend) - Tool Suggestions ...</a></li>

</ul>
</details>

**社区讨论**: 整体情绪对 OpenAI 持怀疑态度，但并非一边倒。一派（nezi）认为，如果 OpenAI 是一个人类合作者，沿着共同讨论的方向发表成果却不署名，显然是不道德的；另一派（sashank_1509）承认对话数据可能改善模型的潜在直觉，但坚持认为「可验证数学上的强化学习 + 巨量算力」足以独立产出超人级结果。还有第三种观点（bertonvv、fwlr）质疑 AI 在开放问题上的快速进展是否部分属于错觉——因为使用这些工具的研究者不断把新鲜的未发表数学喂进去，而那个「仍在训练中的模型生成 3000 亿 token」的时间点尤其令人生疑。

**标签**: `#AI ethics`, `#OpenAI`, `#research integrity`, `#LLM training data`, `#academia`

---

<a id="item-5"></a>
## [OpenAI 发布 Agents API，支持自托管沙箱](https://developers.openai.com/api/docs/guides/agents-api/overview) ⭐️ 8.0/10

OpenAI 推出了 Agents API，让应用可以通过 OpenAI 托管的接口调用 Codex harness，由 OpenAI 负责会话管理、编排和上下文压缩。官方文档中还提供了一个可选方案，允许用户自行托管 Agent 的沙箱，而不是完全依赖 OpenAI 的基础设施。 这是 OpenAI 把 Agent 执行能力作为托管基础设施来售卖的一步，而不再只是提供原始的模型 token，这可能形成一道相对持久、可抵御众多本地开源 Agent harness 的护城河。与此同时，它也让供应商锁定、状态归属和可迁移性成为开发者选择 Agent 平台时的核心议题。 该服务把 Codex harness 以托管 API 的形式暴露出来，负责会话、编排和上下文压缩，OpenAI 的文档还提到可通过配置选择自托管沙箱，从而降低在不同供应商之间迁移的难度。不过由于抽象层和执行环境仍由 OpenAI 定义，团队需要评估 Agent 状态存放在哪里，以及有多少工作流会与这套 harness 绑定。

hackernews · aquir · 9月10日 19:43 · [社区讨论](https://news.ycombinator.com/item?id=49649213)

**背景**: AI Agent 通常是把大模型放进一个循环里，让它调用工具、执行代码并维护状态，而运行这个循环的脚手架常被称为 harness。自己搭建 harness 是一项不小的工程，还需要一个能安全执行代码的环境，因此隔离沙箱——可随时销毁的容器或虚拟机，让 Agent 在不影响宿主机的条件下读写和运行代码——已经成为常见的构建模块。OpenAI 此前已经发布了抽象很少的开源 Agents SDK，而这次托管的 Agents API 则是面向不想自行运维整套栈的团队的更省心选择。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.openai.com/api/docs/guides/agents-api/overview">Agents API | OpenAI API</a></li>
<li><a href="https://openai.github.io/openai-agents-python/">OpenAI Agents SDK</a></li>
<li><a href="https://developers.cloudflare.com/sandbox/tutorials/openai-agents-api/">Run Codex with Cloudflare Containers using the OpenAI Agents API ...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的评论者普遍认为业界仍在探索“Agent 即产品”的正确抽象方式，多人把供应商锁定视为主要顾虑，其中一位用户直言希望拿到自己付费购买的推理 token。也有不少人持更积极的态度：有人指出文档深处提到的自托管沙箱选项让这项服务诱人得多，也便于在供应商之间迁移；有人分享自己在普通 QEMU 虚拟机里运行 Codex 当个人助理效果很好；还有人认为这是 OpenAI 面对众多本地 harness 构建持久护城河、甚至进行捆绑销售的一步。

**标签**: `#OpenAI`, `#AI Agents`, `#API`, `#Vendor Lock-in`, `#Self-hosting`

---

<a id="item-6"></a>
## [trynix.dev 让你在浏览器中启动过去 13 年的任意 Nix 包](https://simonwillison.net/2026/Sep/10/trynix/) ⭐️ 8.0/10

Farid Zakaria 发布了 trynix.dev，它借助 qemu-wasm 通过 WebAssembly 在浏览器内运行完整的 x86_64 Linux 虚拟机，并能以 URL 寻址的方式启动过去 13 年间的任意 Nix 包，获得交互式 shell。他还推出了 trynix-preview——一个 GitHub Action，它会在 Pull Request 下评论一条链接，让任何人都能在浏览器中直接启动该 PR 的构建结果，全程无需服务器。 它几乎消除了复现和检视历史软件的全部门槛：无需在本地安装 Nix 或准备容器，评审者或好奇的用户只要打开一个 URL 就能得到可用环境。用在代码评审上，这意味着启动一个 Pull Request 的真实构建结果变得像点链接一样简单，也进一步强化了 Nix 生态最核心的可复现性叙事。 包可以直接通过 URL 寻址，例如 https://trynix.dev/?pkg=python3%403.6.2，点击 "Load" 后即可获得一个运行 2017 年 Python 3.6.2 的交互式 shell。所有内容都在浏览器端的 WebAssembly 虚拟机中执行，因此不需要任何后端服务器，但速度与内存也受限于用户浏览器的性能。

rss · Simon Willison · 9月10日 23:44

**背景**: Nix 是 Eelco Dolstra 于 2003 年创建的纯函数式包管理器，它把软件包当作不可变的值处理，从而保证构建可复现，并能从二进制缓存中取出精确的历史版本。qemu-wasm 则是把 QEMU 系统模拟器实验性移植到浏览器的项目，通过 WebAssembly 和 QEMU 的 TCG 引擎执行客户机代码。trynix.dev 把两者结合起来：把多达 13 年前的 Nix 派生（derivation）下载下来，在浏览器标签页中的模拟 Linux 机器里启动运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ktock/qemu-wasm">GitHub - ktock/qemu-wasm: QEMU on browser · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Nix_(package_manager)">Nix (package manager)</a></li>
<li><a href="https://nixos.org/">Nix & NixOS | Declarative builds and deployments</a></li>

</ul>
</details>

**标签**: `#Nix`, `#WebAssembly`, `#qemu-wasm`, `#browser VM`, `#reproducibility`

---

<a id="item-7"></a>
## [Calif Research 发布 WeWorm：AI 打造的微信零点击蠕虫](https://simonwillison.net/2026/Sep/10/calif-research/) ⭐️ 8.0/10

Calif Research 发布了一个名为 WeWorm 的演示，声称这是首个可通过微信通话在 iOS 和 Android 上传播的零点击蠕虫，受害者在完全不接听电话、不触碰手机的情况下账号即被攻陷。该团队表示，借助 AI，他们在约两天内发现漏洞并写出首个远程代码执行（RCE）利用程序，随后又用一周时间构建出完整的蠕虫。 这是一个强烈信号：AI 正在大幅压缩攻击性安全研究所需的时间与人力——过去需要更大团队耗时数月才能完成的蠕虫，据称被小团队在约十天内做出来。考虑到微信在 iOS 和 Android 上拥有超过十亿用户，若该说法在实际环境中可复现，这样一个跨平台零点击蠕虫将对移动通信安全构成严重威胁。 根据相关报道，WeWorm 利用了一个 VoIP 内存破坏漏洞，并通过已有联系人发起的来电接触受害者；Calif Research 已将该漏洞报告给腾讯，据称腾讯已封堵该利用方式。这些说法来自一份演示发布，而非经过同行评审或独立验证的技术报告，因此其确切可靠性、受影响的版本范围以及可复现性仍未得到确认。

rss · Simon Willison · 9月10日 00:56

**背景**: “零点击”漏洞利用无需受害者做任何操作即可攻陷设备或账号——不用点击、不用接听，因此比需要诱导用户交互的攻击危险得多。远程代码执行（RCE）指攻击者能够通过网络在远端机器上运行自己的代码，这类漏洞几乎总被列为严重级别；而蠕虫是无需用户操作即可从一个受害者自动传播到下一个的恶意软件，因此即时通讯应用通话处理环节中的零点击 RCE 正是构建蠕虫的理想基础。这条新闻也契合 2025 至 2026 年间的一个更广泛趋势：威胁行为者与研究人员都在利用大语言模型加速漏洞挖掘以及漏洞利用与恶意软件的开发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/09/wechat-zero-click-worm-took-over.html">WeChat Zero-Click Worm Took Over Accounts on iPhone and ...</a></li>
<li><a href="https://cybersecuritynews.com/weworm-first-0-click-worm/">WeWorm – First 0-Click Worm Spreading Through WeChat Calls ...</a></li>
<li><a href="https://www.techtimes.com/articles/327153/20260910/wechat-zero-click-worm-built-ai-days-voip-bug-put-billion-accounts-risk.htm">WeChat Zero-Click Worm Built By AI In Days: VoIP Bug Put ...</a></li>

</ul>
</details>

**标签**: `#ai-security`, `#exploit-development`, `#zero-click-worm`, `#mobile-security`, `#wechat`

---

<a id="item-8"></a>
## [JetBrains：微软 Defender 导致 Rider 与 ReSharper 启动缓慢](https://blog.jetbrains.com/dotnet/2026/09/09/why-rider-and-resharper-were-slow-to-start-and-how-microsoft-helped-fix-the-problem/) ⭐️ 7.0/10

JetBrains 发布文章说明：在推出 ReSharper 的进程外（OOP）架构后，用户反馈 Windows 上 IDE 启动变慢；性能分析显示，微软 Defender 对 JetBrains 相关进程的扫描时间远超预期。JetBrains 随后与微软合作定位原因、修复了该问题，并为此开发了一款排查工具。 这一问题直接影响 Windows 上的 .NET 开发者，IDE 启动变慢会打断日常编码节奏，也凸显了杀毒软件实时扫描可能在不知不觉中拖垮开发工具的性能。此次跨厂商合作还产出了一款诊断工具，有望帮助其他软件厂商排查类似的 Defender 导致的性能问题。 性能下降出现在 JetBrains 将 ReSharper 的核心功能从 Visual Studio 进程迁移到独立进程之后，而 Defender 对该进程的扫描开销比预期大得多。常见的缓解手段如添加杀毒排除项或启用 Defender 性能模式虽然能提速，但每一项排除都会扩大安全缺口，因此在扫描层面做正式修复更为重要。

rss · JetBrains .NET Tools (Rider/ReSharper) · 9月9日 16:45

**背景**: ReSharper 是 JetBrains 为 Visual Studio 提供的生产力扩展，其新的进程外架构把依赖 Visual Studio API 的代码保留在 Visual Studio 进程内，而将 ReSharper 的核心分析与重构功能移到独立进程中，以提升稳定性与性能。Rider 则是 JetBrains 推出的独立 .NET IDE。微软 Defender 杀毒软件会实时扫描进程与文件以检测威胁，而这种扫描是开发工作负载变慢的常见原因，因此微软提供了排除项设置以及面向 Dev Drive 的性能模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.jetbrains.com/help/resharper/Out_of_process.html">Out-of-Process mode | ReSharper Documentation - JetBrains</a></li>
<li><a href="https://blog.jetbrains.com/dotnet/2025/04/01/resharper-out-of-process-update/">ReSharper's Out-of-Process Journey: Major Progress and Next ...</a></li>
<li><a href="https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-endpoint-antivirus-performance-mode">Protect Dev Drive using performance mode - Microsoft Defender ... Windows Defender exclusions for Visual Studio development Microsoft Defender Antivirus exclusions design — Solving ... Performance analyzer for Microsoft Defender Antivirus Visual Studio Performance with Microsoft Defender Useful Windows Defender exclusions to speed up development ... 5 tweaks every developer should make in Windows 11</a></li>

</ul>
</details>

**标签**: `#.NET`, `#ReSharper`, `#Rider`, `#performance`, `#Microsoft Defender`

---

<a id="item-9"></a>
## [PostgreSQL 的 max_connections 是内存预算，而非并发上限](https://postgr.es/p/9ug) ⭐️ 7.0/10

Christophe Pettus 发表了一篇技术文章，指出 PostgreSQL 的 max_connections 参数并不决定服务器实际能同时运行多少查询，它本质上是内存预算和一道断路器。尽管该参数普遍被描述为“最大并发连接数”，但 Pettus 解释说，真正的查询并发能力由 CPU 核心数和存储性能决定，而这些在购买硬件时就已经固定下来了。 这一重新解读之所以重要，是因为许多 DBA 在负载高峰时会调高 max_connections，误以为这样能提升吞吐量，而实际上它主要只是膨胀内存占用，甚至拖慢性能。把 max_connections 视为资源预算而非吞吐量旋钮，有助于团队正确设置连接池规模，并考虑使用 PgBouncer 之类的连接池中间件。 PostgreSQL 中每一个客户端后端连接槽都对应真实的内存开销（每连接的基础开销，再加上每会话的 work_mem 等缓冲区），因此 max_connections 实际上限定了服务器在拒绝新连接之前能接纳多少个客户端后端进程，也就是一道断路器。该参数默认值通常为 100，其中一部分连接会通过 superuser_reserved_connections 专门保留给超级用户，而实际可用的上限还可能受 initdb 时确定的内核设置限制。

rss · Planet PostgreSQL · 9月11日 01:00

**背景**: max_connections 是 PostgreSQL 的 GUC（Grand Unified Configuration，统一配置）系统所管理的数百个参数之一，该系统是集中式、类型安全的配置声明与校验框架。在 PostgreSQL 的“每连接一进程”架构下，每个客户端连接都会派生一个独立的后端进程并占用自己的内存，因此连接数会直接转化为内存压力。这也是为什么常见的并发调优建议强调让工作进程数匹配 CPU 核心数，以及在连接量很大的场景中推荐使用连接池。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pgpedia.info/g/guc.html">GUC - Grand Unified Configuration - pgPedia - a PostgreSQL ...</a></li>
<li><a href="https://postgresqlco.nf/doc/en/param/max_connections/">PostgreSQL Documentation: max_connections parameter</a></li>
<li><a href="https://www.cybertec-postgresql.com/en/tuning-max_connections-in-postgresql/">max _ connections tuning in PostgreSQL | CYBERTEC</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#Database Configuration`, `#max_connections`, `#Performance Tuning`, `#Scalability`

---