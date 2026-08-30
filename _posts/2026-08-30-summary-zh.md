---
layout: default
title: "Horizon 日报：2026-08-30 (ZH)"
date: 2026-08-30
lang: zh
---

> 从 29 条内容中筛选出 7 条重要资讯。

---

1. [NASA 罗曼太空望远镜即将发射，具备广域红外视野](#item-1) ⭐️ 9.0/10
2. [腾讯开源 Hy4 preview：770B 参数 MoE，超百万上下文](#item-2) ⭐️ 8.0/10
3. [国土安全部借鲜为人知的海关法秘密调取记者与非营利组织记录](#item-3) ⭐️ 8.0/10
4. [vphone-cli：借助 Apple Virtualization.framework 启动虚拟 iPhone](#item-4) ⭐️ 8.0/10
5. [漏洞传闻几分钟内即遭 AI 代理攻击探测](#item-5) ⭐️ 8.0/10
6. [德州车险加收 1 美元 资助 Flock 监控摄像头](#item-6) ⭐️ 7.0/10
7. [PostgreSQL 发布 28 个 CVE 安全更新后，务必缩短生产环境补丁延迟](#item-7) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [NASA 罗曼太空望远镜即将发射，具备广域红外视野](https://science.nasa.gov/mission/roman-space-telescope/) ⭐️ 9.0/10

南希·格蕾丝·罗曼太空望远镜定于 2026 年 8 月 30 日由猎鹰重型火箭发射。该望远镜配备 2.4 米主镜和宽视场仪器，能提供与哈勃相当的图像质量，但视场是其 100 倍。 这一里程碑将通过宽域巡天推动天文学发展，研究暗能量、利用微引力透镜搜寻系外行星，并观测多达十亿个星系。其完全开放的数据政策有望使数据获取民主化，让任何人都能探索宇宙观测数据。 该望远镜基于捐赠的间谍卫星主镜，于 2025 年 11 月 25 日完工，据称预算低于预期且进度提前。它将搭载宽场仪器和日冕仪仪器，用于高对比度成像，所有数据将公开无保留地发布。

hackernews · JumpCrisscross · 8月29日 15:48 · [社区讨论](https://news.ycombinator.com/item?id=49490870)

**背景**: 罗曼太空望远镜以 NASA 首位女天文学主管南希·格蕾丝·罗曼命名。该任务在 2010 年被美国国家研究委员会十年调查列为最高优先事项，并于 2016 年获批研制。其宽视场能力旨在解决暗能量、宇宙结构和系外行星等基础问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Nancy_Grace_Roman_Space_Telescope">Nancy Grace Roman Space Telescope</a></li>
<li><a href="https://science.nasa.gov/mission/roman-space-telescope/">Nancy Grace Roman Space Telescope - NASA Science</a></li>

</ul>
</details>

**社区讨论**: 评论者对完全开放的数据感到兴奋，提到每天可达 1.4TB 的公开观测数据。有评论者讨论该望远镜源自间谍卫星改造的“出身”，认为这使其预算和进度好于预期；也有人质疑 NASA 为何不建造两套相同望远镜以防范发射失败风险。

**标签**: `#space-telescope`, `#astronomy`, `#NASA`, `#open-data`, `#scientific-research`

---

<a id="item-2"></a>
## [腾讯开源 Hy4 preview：770B 参数 MoE，超百万上下文](https://www.tencent.com/tencent-releases-and-open-sources-tencent-hy4-preview/) ⭐️ 8.0/10

腾讯发布并开源了下一代大语言模型 Hy4 preview，总参数 770B，激活参数 49B，上下文窗口超过 1M tokens。 作为中国科技巨头发布的重要开源模型，它在编程和科研领域展现出强大的推理与问题解决能力。在 OpenRouter 上迅速获得大规模采用，数天内处理了数万亿 tokens，基于低缓存的定价也更具吸引力，凸显其实用价值和行业影响力。 Hy4 preview 是混合专家（MoE）模型，每次仅激活 49B 参数，兼顾规模与推理效率。它还在自身开发中参与了训练方法、数据策略、评估框架和底层算子的自动化优化，形成了早期的递归式自我改进闭环，并与 CodeBuddy、WorkBuddy 等腾讯产品协同设计。

hackernews · shenli3514 · 8月29日 19:33 · [社区讨论](https://news.ycombinator.com/item?id=49492632)

**背景**: Hy4 preview 是基于混合专家架构的大语言模型，该架构每次推理只激活部分参数，从而在扩大模型规模的同时控制计算成本。此次开源延续了主流实验室发布强大开放模型的趋势；所谓“自我改进闭环”，是指利用模型自身的输出和反馈来辅助优化训练数据、算子、评估流程等环节，属于前沿但存有争议的研究方向。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tencent.com/tencent-releases-and-open-sources-tencent-hy4-preview/">Tencent Releases and Open-Sources Tencent Hy4 preview - Tencent</a></li>
<li><a href="https://huggingface.co/tencent/Hy4-preview">tencent/Hy4-preview · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：有人强调 Hy4 preview 在 OpenRouter 上的大规模采用和成本优势，也有人对递归式自我改进表示担忧，并讨论为追求 token 密度而精简词表是否会让语言变得贫乏，甚至被比作“新话（Newspeak）”。

**标签**: `#AI`, `#LLM`, `#Open Source`, `#Tencent`, `#Machine Learning`

---

<a id="item-3"></a>
## [国土安全部借鲜为人知的海关法秘密调取记者与非营利组织记录](https://www.theguardian.com/us-news/2026/aug/29/trump-dhs-1509-summons-records-journalists-nonprofits) ⭐️ 8.0/10

美国国土安全部（DHS）正利用一项鲜为人知的行政传票权限——19 U.S.C. § 1509——在未经司法批准的情况下秘密获取记者、非营利组织和工会的通信记录。《卫报》的调查发现，DHS 已向 Google 和 T-Mobile 发出传票，其中一次甚至获取了一名记者六个月的电话和短信记录。 这一事件揭示了重大的监控漏洞：一项原本用于海关执法的老法规正被挪用来绕过获取记者记录时通常需要遵守的更严格法律审查。这可能威胁新闻自由和公民自由，并对调查报道、社会倡导和劳工组织活动造成寒蝉效应。 这些传票依据 19 U.S.C. § 1509 签发，该法原先旨在检查海关相关账册和证人，现在可由 DHS 官员而非法官批准。在数起案件中，DHS 在传票受到法庭挑战后主动撤回，可能是为了避免形成不利的合法性判例；据报道 T-Mobile 选择配合，而 Google 则予以抵制。

hackernews · firefax · 8月29日 18:44 · [社区讨论](https://news.ycombinator.com/item?id=49492219)

**背景**: 19 U.S.C. § 1509 是一项海关法，允许相关机构为海关目的传唤账册、文件和证人；美国海关与边境保护局（CBP）使用 DHS 3115 表格行使这一传票权限。2017 年 DHS 监察长办公室的一份管理警报已就 CBP 使用该检查与传票权限提出警告。批评者认为，用该法获取通信记录的做法远远超出了其原始适用范围，并剥夺了当事人通常享有的正当程序保护（如事先通知和司法监督）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theguardian.com/us-news/2026/aug/29/trump-dhs-1509-summons-records-journalists-nonprofits">Trump’s DHS is using an obscure law to secretly snoop on ...</a></li>
<li><a href="https://www.law.cornell.edu/uscode/text/19/1509">19 U.S. Code § 1509 - Examination of books and witnesses</a></li>
<li><a href="https://www.oig.dhs.gov/sites/default/files/assets/Mga/2017/oig-18-18-nov17.pdf">Management Alert - CBP's Use of Examination and Summons Authority Under</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍持批评态度，认为 DHS 可能是在被挑战时故意撤回传票，以避免法院作出限制该工具使用的裁决；也有人指出企业完全可以先无视要求，等 DHS 向法院申请强制令再作配合。还有人提到 T-Mobile 交出了记录而 Google 没有，并建议记者使用 tmailplus 等自托管工具；另一些人则用讽刺口吻将事件说成是 DHS 在监控中俄，或批评该机构的预算规模。

**标签**: `#surveillance`, `#privacy`, `#DHS`, `#civil liberties`, `#journalism`

---

<a id="item-4"></a>
## [vphone-cli：借助 Apple Virtualization.framework 启动虚拟 iPhone](https://github.com/Lakr233/vphone-cli) ⭐️ 8.0/10

vphone-cli 是一款新的开源工具，它通过 Apple 的 Virtualization.framework，将 Apple PCC/cloudOS 镜像中的 iOS 内核与 iOS 用户空间配对，从而在 Apple silicon Mac 上启动虚拟 iPhone。它支持多种补丁变体，并支持应用测试以及 agent 驱动的 UI 控制。 该项目为 Corellium 等商业服务提供了一个免费且易于获取的替代方案，打破了 iOS 虚拟化领域的垄断，为开发者与安全研究人员打开了一扇门，让他们可以在虚拟 iPhone 上测试应用、运行自动化以及执行 UI 控制。它创造性地以 Apple 官方不支持的方式重新利用了 Apple 自己的框架，可能改变 iOS 开发与测试的工作流程。 它不是模拟器：该工具使用 Apple 在 Private Cloud Compute（PCC）镜像中提供的真实 iOS 内核，然后对启动链进行修补以使其在虚拟机中运行。项目提供五种安全绕过程度递增的补丁变体，并建议用户在 iOS 设置过程中避免选择日本或欧盟地区，因为虚拟机无法满足这些地区额外的监管检查。所有生成的文件都存放在 ~/.vphone/ 目录下，以保证已签名应用包的可移植性。

hackernews · hentrep · 8月28日 23:02 · [社区讨论](https://news.ycombinator.com/item?id=49485267)

**背景**: Apple 的 Virtualization.framework 是一个高级 API，用于在 Apple silicon 和 Intel Mac 上创建和管理虚拟机，官方支持 macOS 和 Linux 客户机。Private Cloud Compute（PCC）是 Apple 的云端 AI 基础设施，其 cloudOS 镜像恰好包含可用的 Apple silicon iOS 内核。vphone-cli 将该内核与 iOS 用户空间组合，生成可启动的 iPhone 虚拟机，这与 Tart 等工具使用同一框架运行 macOS/Linux 虚拟机的方式类似。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.apple.com/documentation/virtualization">Virtualization | Apple Developer Documentation</a></li>
<li><a href="https://security.apple.com/blog/private-cloud-compute/">Private Cloud Compute: A new frontier for AI privacy in the cloud</a></li>
<li><a href="https://github.com/Lakr233/vphone-cli">GitHub - Lakr233/vphone-cli · GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区反响总体积极热烈，用户强调该工具在应用测试中的实用性，并提到配套的 vphone-mcp 可让 agent 控制 UI。有置顶评论强调这并非模拟器，并附上详细的技术分析文章链接；也有用户询问它与 iOS Simulator 的区别，以及欧盟/日本地区具体有哪些监管检查。

**标签**: `#iOS`, `#Virtualization`, `#Apple`, `#App Testing`, `#Automation`

---

<a id="item-5"></a>
## [漏洞传闻几分钟内即遭 AI 代理攻击探测](https://simonwillison.net/2026/Aug/28/just-a-rumour-of-a-bug/) ⭐️ 8.0/10

剑桥大学教授、OCaml 核心维护者 Anil Madhavapeddy 报告称，供讨论的安全补丁在约十分钟内就会遭到自动化 AI 驱动的攻击探测。rclone 项目过去十年收到约 20 份安全披露，而最近一个月就超过 40 份。 这标志着漏洞利用范式的转变：只要有最轻微的漏洞传闻，AI 代理就足以定位并攻击该漏洞。现有的开源保密（embargo）实践可能难以为继，维护者正被大量真实有效的安全披露所淹没。 安全补丁被分享后几分钟内，Madhavapeddy 的网站就遭到百分号编码遍历序列（典型的目录遍历攻击）探测。他还演示了在 Claude 拒绝任务时改用 DeepSeek V4 Pro 可让智能体找到漏洞；rclone 的 Nick Craig-Wood 提到 GitHub 的 CVE 分配从 2-3 天延缓到 3-4 周。

rss · Simon Willison · 8月28日 22:12

**背景**: 目录遍历攻击利用不充分的路径校验，通常借助百分号编码序列（如 %2e%2e%2f，解码后为 '../'）来访问 Web 根目录之外的文件。现代 AI 编程智能体已经非常擅长阅读代码和追踪逻辑，只要有一丝漏洞提示就能转化为可用攻击。DeepSeek-V4-Pro 是 2026 年发布的最强开源模型之一，具备出色的推理和编码能力。这些智能体现在既被防御者使用，也被攻击者使用，使得公开仓库成为自动化探测的载体。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Directory_traversal_attack">Directory traversal attack - Wikipedia</a></li>
<li><a href="https://deepseek.com/en/index.html">DeepSeek | Into the Unknown</a></li>
<li><a href="https://owasp.org/www-community/attacks/Path_Traversal">Path Traversal | OWASP Foundation</a></li>

</ul>
</details>

**社区讨论**: 在 Hacker News 的评论中，rclone 维护者 Nick Craig-Wood 确认他的项目也遇到同样现象，最近 75% 的安全披露包含真实问题。他还提到 AI 工具帮助进行分类和修复，但数量仍然消耗大量时间，同时 GitHub 的 CVE 分配延迟导致发布版本只能标注 CVE-PENDING。

**标签**: `#security`, `#AI agents`, `#open source`, `#OCaml`, `#vulnerability exploitation`

---

<a id="item-6"></a>
## [德州车险加收 1 美元 资助 Flock 监控摄像头](https://www.texastribune.org/2026/08/28/texas-flock-cameras-auto-insurance-fee-mvcpa-grants/) ⭐️ 7.0/10

2023 年德州立法者通过的 1 美元汽车保险费附加费，本意是打击催化转换器盗窃，如今已被用于在全州部署至少 3200 个 Flock 车牌识别摄像头，且数量还在增加。 这件事说明，一笔不起眼、无争议的小额费用可能悄悄资助大规模监控基础设施，引发严重的隐私担忧。Flock 车牌识别网络的快速扩张表明，车牌追踪正成为美国警务的常规手段，影响数百万驾车者。 德州机动车犯罪预防管理局（Motor Vehicle Crime Prevention Authority）管理这笔资金，其董事会成员大多由州长格雷格·阿博特任命。Flock 摄像头执行自动车牌识别并与警方共享数据，批评者称该系统属于大规模监控。

hackernews · DeepLogin · 8月29日 23:17 · [社区讨论](https://news.ycombinator.com/item?id=49494182)

**背景**: Flock Safety 是一家成立于 2017 年的私营公司，向执法部门和社区团体销售自动车牌识别（ALPR）摄像头、枪声定位器和视频监控设备。截至 2025 年，Flock 称其业务覆盖全美 49 个州的 5000 多个社区，每月执行超过 200 亿次车辆扫描。德州立法机构在 2023 年一致通过了 1 美元的附加费以应对催化转换器盗窃，但该项目已远远超出最初目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Flock_Safety">Flock Safety - Wikipedia</a></li>
<li><a href="https://www.aclu.org/news/privacy-technology/tracking-alpr-cameras/flock-roundup">Flock’s Aggressive Expansions Go Far Beyond Simple Driver Surveillance | American Civil Liberties Union</a></li>

</ul>
</details>

**社区讨论**: 评论者对项目的扩张和隐私影响表示担忧，有人指出电动汽车电池可能是继催化转换器之后的下一目标。还有评论者希望负面宣传能阻止 Flock 向海外扩张；同时也有讨论聚焦于摄像头是否真的减少了催化转换器盗窃，有用户抱怨一个直接相关的问题被点踩。

**标签**: `#surveillance`, `#privacy`, `#policy`, `#cameras`, `#Texas`

---

<a id="item-7"></a>
## [PostgreSQL 发布 28 个 CVE 安全更新后，务必缩短生产环境补丁延迟](https://postgr.es/p/9ts) ⭐️ 7.0/10

2026 年 8 月 13 日，PostgreSQL 发布了有史以来最大规模的安全更新，一天内修复了 28 个 CVE。文章呼吁生产环境用户重点关注缩短补丁延迟——即从修复发布到实际部署的时间。 公开披露的 CVE 可能被迅速利用：补丁一经发布，攻击者就能得知漏洞细节，而 AI 工具进一步加速了漏洞利用的开发。为关键负载运行 PostgreSQL 的数据库管理员必须尽可能缩小这一时间差，以避免被入侵。 PostgreSQL 在 2025 年全年修复了 7 个 CVE，而 2026 年至今已修复 44 个，其中 28 个集中在一次发布中。这些漏洞包括缓冲区溢出等典型内存安全问题，多由 AI 辅助模糊测试发现；其中 to_char() 的一个远程代码执行漏洞已有公开的 POC（概念验证）。

rss · Planet PostgreSQL · 8月28日 11:41

**背景**: CVE（Common Vulnerabilities and Exposures，通用漏洞与披露）是一个公开的已知信息安全漏洞目录，由 MITRE 在美国政府资助下维护。补丁延迟（patch latency）是指组织将已发布的安全修复部署到生产环境所需的时间；延迟越长，系统暴露风险越大，因为攻击者可以对补丁进行逆向分析来找到漏洞。Postgres 的小版本更新是累积式的且保持二进制兼容，因此应用起来相对容易——停止服务、替换二进制文件、再重启即可，这也让快速打补丁变得可行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Common_Vulnerabilities_and_Exposures">Common Vulnerabilities and Exposures - Wikipedia</a></li>
<li><a href="https://www.redhat.com/en/topics/security/what-is-cve">What is a CVE? - Red Hat</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#Security`, `#Patching`, `#Production`, `#CVE`

---