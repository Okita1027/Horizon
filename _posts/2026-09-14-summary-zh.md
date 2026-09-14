---
layout: default
title: "Horizon 日报：2026-09-14 (ZH)"
date: 2026-09-14
lang: zh
---

> 从 31 条内容中筛选出 6 条重要资讯。

---

1. [谷歌为何仍在通过 AdSense 投放诈骗广告？](#item-1) ⭐️ 8.0/10
2. [The Verge 专栏揭露联网汽车如何出售车主数据](#item-2) ⭐️ 8.0/10
3. [Bryan Cantrill 批评极端化 AI 恐慌，呼吁基于证据评估风险](#item-3) ⭐️ 8.0/10
4. [Fable 5.1 破解 370 年历史的 Cyphral Distich 密码](#item-4) ⭐️ 7.0/10
5. [Signal 将借助零知识证明实现无需手机号注册](#item-5) ⭐️ 7.0/10
6. [GPT-6 Astra 智能体基于 OpenStreetMap 自动生成 5K 与 10K 跑步路线](#item-6) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [谷歌为何仍在通过 AdSense 投放诈骗广告？](https://www.atomic14.com/2026/09/13/why-is-google-still-serving-dodgy-ads) ⭐️ 8.0/10

atomic14.com 上的一篇文章在 Hacker News 引发了 619 分、295 条评论的热议，讨论谷歌为何仍持续通过 AdSense 广告网络投放诈骗类广告。评论者中包括网站发布者，他们表示自家网站上已被注入数以千计的诈骗广告素材（例如“你已被记录，需缴纳 100 美元罚款”之类的假弹窗），且持续了数月之久。 AdSense 是开放网络中大量网站的主要变现渠道，因此失控的诈骗广告既直接伤害看到广告的用户，也损害承载这些广告的发布者域名信誉。这场讨论还提出了责任归属问题：谷歌作为广告的中间商与获利方，是否应当像传统媒体那样对所刊广告承担严格责任。 发布者反映，谷歌不允许他们屏蔽 netlify.app、herokuapp.com、azurewebsites.net、ondigitalocean.app、digitaloceanspaces.com 等被诈骗者滥用的整站域名，因为谷歌把它们视作 TLD（顶级域），而诈骗者每天都会更换新的子域名。一位评论者援引一位在 Google Ads 上投入超过 1 亿美元的广告主的话称，谷歌目前正以前所未见的激进方式榨取广告收入。

hackernews · iamflimflam1 · 9月13日 17:37 · [社区讨论](https://news.ycombinator.com/item?id=49686445)

**背景**: Google AdSense 是一个广告网络，允许网站发布者在自己的页面上展示与内容和受众匹配的文字、图片、视频或互动广告，并与谷歌分成广告收入。它与广告主用来投放 campaign 的买方平台 Google Ads 不同，两者共同构成了谷歌广告业务的核心。广告欺诈（ad fraud）是一个更宽泛的概念，指通过虚假曝光、虚假点击或误导性广告素材等欺骗性、自动化手段从广告预算中套取资金，这一问题在数字广告网络中早已被广泛记录。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Google_Adsense">Google AdSense - Wikipedia</a></li>
<li><a href="https://datadome.co/guides/click-fraud/what-it-is-ad-fraud/">What is ad fraud ? 13 Common Types & How to Prevent Ad Fraud</a></li>
<li><a href="http://cloudflare-dev-platform.r.workers.dev/learning/bots/what-is-ad-fraud/">What Is Ad Fraud ? | Ad Click Fraud</a></li>

</ul>
</details>

**社区讨论**: 评论区对谷歌的批评几乎是一边倒的：多位评论者认为谷歌是共谋者，并主张对其施加严格责任，指出在前互联网时代，报纸绝不会刊登这种档次的广告。另一些人则将问题归因于激励结构，推测谷歌正在猛榨广告收入，以掩盖其在 AI 领域的失利，并在 AI 摧毁其广告业务之前尽量套现；也有人猜测人工审核能力根本跟不上投放量，因此举报会被自动驳回，直到举报数量超过阈值才会有人工介入。

**标签**: `#Google Ads`, `#AdSense`, `#ad fraud`, `#online advertising`, `#platform responsibility`

---

<a id="item-2"></a>
## [The Verge 专栏揭露联网汽车如何出售车主数据](https://www.theverge.com/column/994172/your-car-is-selling-your-data) ⭐️ 8.0/10

The Verge 的一篇专栏文章详细披露了联网汽车如何持续采集驾驶数据——车速、位置、时间戳以及各类车辆运行信号——并将其出售给第三方数据经纪商。该文在 Hacker News 上引发热议，获得 319 分和 165 条评论。评论者补充了具体证据：一位拥有七年车龄大众汽车的车主关闭了手机应用内所有可找到的数据采集选项和远程访问服务，但后来申请 Carfax 报告时仍看到了与该车关联的里程数据。 这篇文章把日常驾驶与一个几乎不可见的数据经纪产业联系起来，而讨论表明这个问题已不再是理论上的：加州 AB-1542 法案已获州众议院通过，预计将在本周内由州长签署。该法案将禁止出售和共享“敏感”个人信息，其中包含精度可定位到 1850 英尺（约 564 米）半径的地理位置数据。若得以执行，它实际上可能使这类驾驶行为数据集的出售变为非法——而这正是 GM 前合作伙伴 Wejo 等经纪商的商业模式基础。 AB-1542 中 1850 英尺的地理位置门槛是关键的技术基准，因为细粒度的车辆遥测数据很容易把个人定位到远比这更小的范围内；评论者还指出，经纪商拿到的所谓“匿名化”数据流实际上依然极为精细——GM 曾与 Wejo 共享约 1000 万辆联网汽车的数据，包含精确位置，甚至包括雨刷是否开启。另一个要点是退出机制漏洞百出：Carfax 的里程数据由车主以外的其他方提供，因此即使车主注销账号并关闭车内采集，车辆的里程读数仍可能被上报。

hackernews · bookofjoe · 9月13日 13:45 · [社区讨论](https://news.ycombinator.com/item?id=49683953)

**背景**: 现代“联网汽车”内置蜂窝调制解调器和车联网（telematics）模块，会把驾驶数据上传给汽车制造商，厂商再将其授权给数据经纪商。这些经纪商汇集数百万辆汽车的数据流，转售给保险公司、营销机构、车队运营方和分析公司，通常宣称输出结果是匿名化的。匿名化的本意是切断数据与身份之间的关联，但研究和过往事件反复表明，细粒度的移动轨迹仍可被重新识别。美国目前没有覆盖这一交易领域的综合性联邦隐私法，因此监管责任落到了加州等各州身上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://privacyfirst.nl/en/articles/connected-cars-as-a-revenue-model-for-data-brokers/">Connected cars as a revenue model for data brokers | Privacy First</a></li>
<li><a href="https://www.cars.com/articles/how-to-keep-your-car-from-sharing-your-sensitive-data-behind-your-back-483328/">How to Keep Your Car From Sharing Your Sensitive Data Behind Your Back | Cars.com</a></li>
<li><a href="https://legalclarity.org/anonymized-data-legal-standards-methods-and-penalties/">Anonymized Data : Legal Standards, Methods, and... - LegalClarity</a></li>

</ul>
</details>

**社区讨论**: 讨论整体上对该行业持强烈批评态度，并对“退出选项”或“匿名化”能否奏效表示怀疑。一位评论者提出一个鲜明的概念区分：一类是“车辆事实”（VIN、规格、召回状态、里程表），由车主以外的第三方提供，寿命长于每一位车主；另一类是“驾驶者事实”（速度、位置、时间戳），也就是 GM 实际出售的东西。他认为 DRIVER 法案之所以无效，正是因为把两者混为一谈，而第二类数据需要的是一刀切的禁令。其他人指出，那位关闭了所有采集开关的大众车主的数据仍被上报给 Carfax；加州的 AB-1542 带来了真正的执法希望；而根本原因在于数据保护法律过于软弱。还有评论者从实用角度发问：法拉第笼能否屏蔽车联网的上行通信。

**标签**: `#privacy`, `#connected-cars`, `#data-brokerage`, `#consumer-protection`, `#surveillance`

---

<a id="item-3"></a>
## [Bryan Cantrill 批评极端化 AI 恐慌，呼吁基于证据评估风险](https://bcantrill.dtrace.org/2026/09/13/the-contagion-of-fear/) ⭐️ 8.0/10

Oxide Computer 联合创始人兼 CTO、知名系统工程师 Bryan Cantrill 于 2026 年 9 月 13 日在其个人博客发表题为《The contagion of fear》（恐惧的传染）的文章，认为关于 AI 导致人类灭绝的极端化论断更像是一种社会性传染，而非基于证据的推理。该文并不否认 AI 存在风险，而是主张那些缺乏强有力证据、耸人听闻的近期灾难概率断言不应被当作严肃分析对待；文章随后在 Hacker News 上引发了 145 分、110 条评论的讨论。 这场讨论之所以重要，是因为 AI 风险话语正在越来越多地影响研究经费、监管方向与公众认知；一位知名系统工程师公开反驳难以验证的末日论调，可能会改变业界权衡"臆测性风险"与"具体现实危害"的方式。这也呼应了日益明显的分歧：一边是把近期存在性风险视为紧急议题的"AI 极端主义者"，另一边是更关注恶意行为者滥用等可衡量近期危害的怀疑者。 Cantrill 的核心论点属于认识论层面而非技术层面：他区分了"承认存在无法度量的理论风险"与"断言具体量化的概率"这两件事，认为后者不可证伪，因而应当被直接拒斥。文章并未提出任何新的技术机制、评测基准或安全工具，因此其贡献在于风险沟通而非工程实践。

hackernews · elffjs · 9月13日 22:38 · [社区讨论](https://news.ycombinator.com/item?id=49689460)

**背景**: Bryan Cantrill 是一位美国软件工程师，在 Sun Microsystems 期间共同创造了 DTrace 动态追踪框架，之后担任 Joyent 的 CTO，并联合创办了 Oxide Computer——一家自研硬件、固件与软件栈、构建机架级服务器的公司。此处所说的"极端主义者（maximalist）"指认为先进 AI 构成极端乃至生存性威胁、应被列为紧急优先事项的立场；批评者用这一标签来形容他们认为建立在无法验证的臆测之上的论证。讨论中提到的"拟人化（anthropomorphism）"指的是用类人的意图或欲望来描述 AI 系统，批评者认为这会扭曲对风险的判断。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bryan_Cantrill">Bryan Cantrill</a></li>
<li><a href="https://www.linkedin.com/pulse/ai-minimalists-vs-ai-maximalists-stefano-brunelli-oqzvf">AI -Minimalists vs AI - Maximalists</a></li>

</ul>
</details>

**社区讨论**: 评论者大体认同 Cantrill 在认识论上的观点，但对威胁量级看法不一：一位机器人研究者表示自己确实担忧，但更担忧人类行为者，并指出机器人技术本身很难，十年内科技经济不太可能完全自动化。也有人强调，Cantrill 并非否认 AI 风险，而是反对缺乏强证据的耸动性断言，其中一位评论者说，若有人声称到 2036 年人类灭绝概率为 10%，就应当立即不再被认真对待。讨论中反复出现的一个主题是"行为应比言辞更可信"——如果某人真预期会有十亿人死亡，很难解释为何还能一切照旧；此外多位评论者批评了知名人物对 AI 的拟人化表述。

**标签**: `#AI risk`, `#AI safety`, `#technology criticism`, `#Hacker News`, `#risk communication`

---

<a id="item-4"></a>
## [Fable 5.1 破解 370 年历史的 Cyphral Distich 密码](https://www.vals.ai/blogs/fable-solves-cyphral-distich) ⭐️ 7.0/10

AI 模型 Fable 5.1 破解了 Cyphral Distich——这是苏格兰作家托马斯·厄克特（Sir Thomas Urquhart）于 1653 年发表的一段密码文，由两行、每行 32 个数字组成；有报道称该模型在大约 44 分钟内解出，而此前三百多年间无数人尝试均告失败。 这一结果进一步点燃了关于大语言模型在历史密码分析上能走多远的争论：它究竟代表推理能力的真正跃升，还是仅仅因为这些问题几乎无人认真钻研过。它也提高了人们的期待，认为 AI 可以被用来攻克其他长期未解的密码与档案难题。 这段密码本身非常短——总共只有 64 个数字，附在厄克特著作《Logopandecteision》的末尾——因此它的难度更多来自冷门而非密码学上的复杂。评论者指出，所谓“破解”可能只是把公开的未解密码清单（例如 Klaus Schmeh 的 Top 50 榜单）喂给模型，而且在这类任务上该模型据说最终会回退到 Anthropic 的 Opus 模型。

hackernews · u1hcw9nx · 9月13日 21:06 · [社区讨论](https://news.ycombinator.com/item?id=49688695)

**背景**: 密码文（cryptogram）是一段被刻意编码的短消息，若不知道生成规则就无法读懂；数百年来，未解的历史密码一直是密码分析者的长期挑战。托马斯·厄克特是 17 世纪的苏格兰作家与翻译家，他 1653 年的著作《Logopandecteision》提出了一种通用语言，而 Cyphral Distich 就附在该书末尾。Fable 5.1 是 Anthropic 近期推出的 Claude 模型之一，社区成员通常通过 Klaus Schmeh 的密码学博客和 Satoshi Tomokiyo 的 Cryptiana 网站来追踪未解密码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.vals.ai/blogs/fable-solves-cyphral-distich">Claude Fable 5.1 Solves the Cyphral Distich</a></li>
<li><a href="https://nashaniva.com/en/403935">New Claude model cracked a 373-year-old unsolveable cipher in 44 minutes</a></li>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-1">Introducing Claude Fable 5 . 1 and Claude Mythos 5 . 1 \ Anthropic</a></li>

</ul>
</details>

**社区讨论**: 社区情绪在赞叹与怀疑之间摇摆：有评论者在“一切完了”和“我们又行了”之间来回切换，也有人认为近期这类成果多属于“低垂的果实”——真正的瓶颈只是没人愿意投入注意力，而非问题本身有多难。多位用户补充了背景：作者可能只是把公开的未解密码清单喂给了模型、这类任务最终会回退到 Opus，还有人分享了 ChatGPT 在 20 分钟内破解其家族私人密码的经历；另有评论把这次成果类比为 LLM 生成的游戏 demo——它给出的是模型能做出的东西，而不是你真正想要的东西。

**标签**: `#AI`, `#cryptography`, `#LLM`, `#historical ciphers`, `#Hacker News`

---

<a id="item-5"></a>
## [Signal 将借助零知识证明实现无需手机号注册](https://community.signalusers.org/t/registration-without-a-phone-number/2222?page=10) ⭐️ 7.0/10

据报道，Signal 正在实现一套基于零知识证明的注册流程，允许用户在无需手机号的情况下创建账号。根据社区成员对提交记录的解读，免手机号路径需要通过 Google Play Billing 完成一次付费以抑制垃圾账号，同时现有的短信验证方式仍会保留。 在一款主流端到端加密通讯应用中去掉手机号要求，削弱了用户身份与 SIM 卡或运营商账户之间的绑定，而这正是长期存在的元数据与隐私弱点。这也让没有 SIM 卡的设备（例如仅支持 Wi-Fi 的 Android 平板）能够作为一等公民设备使用 Signal，而不必依赖变通做法或第三方客户端。 零知识证明让证明方能够使验证方相信某个陈述为真，同时不泄露除该陈述为真之外的任何信息，这正是让 Signal 在不获取手机号的前提下完成资格验证的思路。但具体设计仍不清晰：究竟证明了什么、如何与 Google Play Billing 付费绑定、后端代码是否会开源，以及免手机号注册是否已经真正上线，都是讨论中悬而未决的问题。

hackernews · Cider9986 · 9月13日 21:47 · [社区讨论](https://news.ycombinator.com/item?id=49689048)

**背景**: Signal 是一款广泛使用的通讯应用，对消息进行端到端加密，只有发送方和接收方能够读取内容。过去注册 Signal 必须提供手机号，这使每个账号都与 SIM 卡和运营商绑定，既带来隐私与元数据暴露，也给平板等没有蜂窝网络的设备造成实际使用障碍。零知识证明是一种密码学协议，一方可以在不披露底层秘密的情况下向另一方证明某个命题成立，它可以是交互式的，也可以是非交互式的。Signal 的服务端基础设施仅部分开源，这也是部分社区成员长期批评的一点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zero-knowledge_proof">Zero-knowledge proof</a></li>
<li><a href="https://ethereum.org/zero-knowledge-proofs">Zero-knowledge proofs | ethereum.org</a></li>

</ul>
</details>

**社区讨论**: 有评论者指出，同一轮发布还让没有 SIM 卡的 Android 平板成为一等附属设备，其中一人表示自己现在可以在平板上使用真正的 Signal，而不必借助 Molly 之类的第三方客户端。也有人持怀疑态度：一位评论者依据提交记录指出，为抑制垃圾账号需要通过 Google Play Billing 付费；另一位要求 Signal 开源其后端自动化代码；还有人认为信息太少，称不能“挥挥手说一句‘零知识’就宣称隐私”。还有评论者只想知道，究竟现在能不能不用手机号完成注册。

**标签**: `#signal`, `#zero-knowledge-proofs`, `#privacy`, `#cryptography`, `#authentication`

---

<a id="item-6"></a>
## [GPT-6 Astra 智能体基于 OpenStreetMap 自动生成 5K 与 10K 跑步路线](https://simonwillison.net/2026/Sep/12/astra-running-routes/) ⭐️ 7.0/10

Simon Willison 只给运行 GPT-6 Astra（Max）的 ChatGPT Work 发了一句提示词，要求它基于 OpenStreetMap 数据从他家出发设计 5K 和 10K 的环形跑步路线。该智能体自主运行了 27 分钟，并完整交付了所要求的结果：内嵌的地图可视化，以及可下载的 GPX 和 GeoJSON 文件，其中 5K 路线的实际长度为 5.1 公里。 这是一个长时运行智能体工作流的具体案例：它把地理编码、批量地理数据下载、本地计算和渲染等多个不同工具串联起来，仅凭一句自然语言提示就交付了成品。对技术型用户而言，这说明通用对话式智能体正在侵入过去需要专业 GIS 脚本才能完成的任务，同时也暴露出智能体透明度与记忆管理方面的未解难题。 Willison 表示，该智能体用 Nominatim 定位地址，用 Overpass API 下载本地的 OpenStreetMap 道路与步道数据，然后在本地计算环路，并通过一个名为 "visualize" 的技能渲染出 /workspace/el-granada-5k-share.html 文件，以便内嵌到 ChatGPT 界面中。他无法取回底层 Python 代码，因为该会话线程已被压缩（compaction）；他认为任何使用压缩机制的 LLM 系统都应保留压缩前的文本，并通过智能体工具调用将其暴露出来。

rss · Simon Willison · 9月12日 23:56

**背景**: OpenStreetMap 是由志愿者贡献者共同构建、以开放数据库许可（ODbL）免费开放的世界地图，而 Nominatim 与 Overpass 是用于地址地理编码和查询其底层数据的两个标准服务。GPX（GPS Exchange Format）是一种轻量级 XML 格式，用于在 GPS 设备与网络服务之间交换航点、路线和轨迹，因此生成的路线可以导入手表或码表使用。GeoJSON 则是基于 JSON 的地理要素编码格式，可表示线串、多边形等结构，已被标准化为 RFC 7946，在网页地图工具中广泛使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenStreetMap">OpenStreetMap - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPS_Exchange_Format">GPS Exchange Format - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/GeoJSON">GeoJSON - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#LLM`, `#geospatial`, `#OpenStreetMap`, `#ChatGPT`

---