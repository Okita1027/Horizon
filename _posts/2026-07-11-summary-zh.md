---
layout: default
title: "Horizon 日报：2026-07-11 (ZH)"
date: 2026-07-11
lang: zh
---

> 从 39 条内容中筛选出 8 条重要资讯。

---

1. [相对论主宰重元素化学键](#item-1) ⭐️ 8.0/10
2. [苹果起诉 OpenAI 窃取商业机密](#item-2) ⭐️ 8.0/10
3. [QuadRF：开源射频分析器可穿墙探测无人机与 WiFi](#item-3) ⭐️ 8.0/10
4. [GPT-5.6 Sol Ultra 声称证明环双覆盖猜想](#item-4) ⭐️ 8.0/10
5. [计算作为普遍基本概念](#item-5) ⭐️ 8.0/10
6. [OpenAI 发布 GPT-5.6 系列：Luna、Terra、Sol](#item-6) ⭐️ 8.0/10
7. [PostgreSQL 18 新增自连接消除 GUC](#item-7) ⭐️ 7.0/10
8. [Meta 发布 Muse Spark 1.1，新增 API 和增强的自主工具调用](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [相对论主宰重元素化学键](https://www.brown.edu/news/2026-07-09/chemical-bonds-relativity) ⭐️ 8.0/10

一项新的实验研究证实，爱因斯坦的狭义相对论通过自旋-轨道耦合主导重元素的化学键合，为这一长期预测的现象提供了直接证据。 这项确认加强了对相对论量子化学的理解，并解释了重金属（如金）的奇特颜色等特性，可能影响材料科学和重元素化合物化学。 该研究聚焦于自旋-轨道耦合，即电子在相对论速度下自旋与轨道运动耦合。实验可能测量了重元素化学键中的能级分裂，验证了狄拉克方程。

hackernews · hhs · 7月10日 22:30 · [社区讨论](https://news.ycombinator.com/item?id=48866134)

**背景**: 在量子力学中，自旋-轨道耦合是一种相对论相互作用，影响原子中的电子行为。对于核电荷高的重元素，电子以接近光速的速度绕核运动，使得相对论效应显著。这种耦合导致原子光谱的精细结构，并影响化学键合。新工作通过实验展示了这些效应对分子键的影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Spin-orbit_coupling">Spin-orbit coupling</a></li>
<li><a href="https://en.wikipedia.org/wiki/Relativistic_quantum_chemistry">Relativistic quantum chemistry - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论指出，相对论对电子轨道的影响此前已知，但这是一次直接的实验确认。用户 Svoka 提到这验证了狄拉克方程。用户 kristianp 对σ键和π键的概念感兴趣，而 cyberax 则提到了金子的颜色和铅酸电池等实例。

**标签**: `#physics`, `#quantum mechanics`, `#relativity`, `#chemical bonds`, `#spin-orbit coupling`

---

<a id="item-2"></a>
## [苹果起诉 OpenAI 窃取商业机密](https://9to5mac.com/2026/07/10/apple-sues-openai-trade-secret-theft/) ⭐️ 8.0/10

苹果对 OpenAI 提起诉讼，指控前员工窃取商业机密，并利用苹果的机密信息为 OpenAI 牟利。 这起诉讼凸显了主要 AI 公司在人才和知识产权方面的紧张关系加剧，可能重塑 AI 行业的竞争格局。 苹果指控 OpenAI 指示新员工在离开苹果时避免被察觉，且前员工将机密信息（包括用于接触苹果供应商的硬件细节）通过电子邮件发送给自己。

hackernews · stock_toaster · 7月10日 20:47 · [社区讨论](https://news.ycombinator.com/item?id=48865019)

**背景**: 商业机密诉讼在科技行业中员工跳槽至竞争对手时并不罕见。苹果和 OpenAI 均涉足 AI 领域，苹果侧重设备端 AI，而 OpenAI 则专注于云端模型。此案涉及一名在苹果工作 25 年的前员工，暗示其对专有信息有深度接触。

**社区讨论**: 评论者认为这对 OpenAI 来说是一个严重的案件，有人指出证据似乎“一目了然”，另有人表示，一家公司若在此事上行为不当，则在任何领域都不可信任。还有人惊讶于一名长期服务于苹果的员工会为此冒职业生涯风险。

**标签**: `#Apple`, `#OpenAI`, `#trade secrets`, `#lawsuit`, `#AI industry`

---

<a id="item-3"></a>
## [QuadRF：开源射频分析器可穿墙探测无人机与 WiFi](https://www.jeffgeerling.com/blog/2026/quadrf-can-spot-drones-and-see-wifi-through-my-wall/) ⭐️ 8.0/10

QuadRF 是一款新型开源 4x4 MIMO 射频分析器，能够通过增强现实叠加层穿墙探测无人机并可视化 WiFi 网络。 该工具将之前仅限于昂贵专用设备的先进射频感知能力大众化，使爱好者与安全研究人员能够探索频谱感知及射频信号的隐私影响。 QuadRF 集成了四个相干全双工射频通道、双极化天线、一个 Raspberry Pi 5 以及预装软件，用于相控阵实验，其开源设计允许用户自定义。

hackernews · speckx · 7月10日 15:59 · [社区讨论](https://news.ycombinator.com/item?id=48861717)

**背景**: 射频分析器测量射频信号，而软件定义无线电 (SDR) 可实现灵活的信号处理。相控阵系统使用多个天线电子控制波束方向。QuadRF 将这些功能结合在一个经济实惠且自成体系的套件中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.crowdsupply.com/scale-rf/quadrf">QuadRF | Crowd Supply</a></li>
<li><a href="https://scalerf.com/updates/">QuadRF Updates</a></li>

</ul>
</details>

**社区讨论**: QuadRF 的创建者直接参与讨论，回答问题并指出根据评测者的建议改进了用户界面。一些评论者对“穿墙看见 WiFi”的表述提出质疑，因为 WiFi 通常能穿透墙壁，而其他人则讨论了潜在应用，如声音定位和检测隐藏的射频发射器。

**标签**: `#RF`, `#open-source`, `#drones`, `#WiFi`, `#security`

---

<a id="item-4"></a>
## [GPT-5.6 Sol Ultra 声称证明环双覆盖猜想](https://cdn.openai.com/pdf/04d1d1e4-bc75-476a-97cf-49055cd98d31/cdc_proof.pdf) ⭐️ 8.0/10

据称，OpenAI 的 GPT-5.6 Sol Ultra 生成了图论中长期未解的环双覆盖猜想的证明，并以 PDF 形式发布。提示词中包含了大量工程化指令，以确保模型专注于解决问题。 如果得到验证，这将是人工智能驱动数学发现的重要里程碑，显示大型语言模型能够为开放猜想的正式证明做出贡献。然而，社区的怀疑态度凸显了关于人工智能自主性及此类成就意义的持续争论。 该证明据称运用了专家们未发现的巧妙技巧，提示词明确指示模型拒绝模糊的状态报告和所谓常规兼容性的声明。PDF 包含了证明和完整的提示词，显示了大量人工工程干预。

hackernews · scrlk · 7月10日 18:29 · [社区讨论](https://news.ycombinator.com/item?id=48863490)

**背景**: 环双覆盖猜想询问是否每个无边桥的无向图都存在一组环，使得每条边恰好出现两次。该猜想由 W.T. Tutte 等人于数十年前提出，至今尚未证明。GPT-5.6 Sol Ultra 是 OpenAI 最新的大型语言模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cycle_double_cover_conjecture">Cycle double cover conjecture</a></li>

</ul>
</details>

**社区讨论**: 社区评论持怀疑态度：有人指出提示词包含大量指令，质疑模型的自主性；另有人指出该猜想本身在 Hacker News 上很少受到关注。还有关于什么才是真正由人工智能生成的证明的讨论。

**标签**: `#AI`, `#mathematics`, `#proof`, `#GPT-5`, `#conjecture`

---

<a id="item-5"></a>
## [计算作为普遍基本概念](https://ergo.org/courses/computation-as-a-universal-and-fundamental-concept) ⭐️ 8.0/10

Tim Roughgarden 推出了一门新的在线讲座系列，探讨计算作为普遍基本概念的观点，并涉及形而上学、物理学和计算机科学等领域的意义。该课程托管在 Ergo.org 上，深入探讨了算法博弈论和不可判定性等主题。 该系列讲座挑战了物理学与计算之间的传统界限，可能影响我们模拟自然过程和设计算法的方式。它连接了哲学、科学和工程学，对多个领域的研究人员和实践者具有意义。 该课程在线免费提供，并邀请了算法博弈论和不可判定性领域的知名研究者参与。它讨论了现实中的例子，如不可判定的物理过程，包括谱间隙问题和流体流动的可预测性。

hackernews · simonpure · 7月10日 15:23 · [社区讨论](https://news.ycombinator.com/item?id=48861213)

**背景**: 传统上，计算被视为人类设计的过程，但一些哲学家和科学家认为它是宇宙的基本属性。算法博弈论（AGT）结合了博弈论和计算机科学来分析战略互动，而不可判定性则指那些无法通过任何算法解决的问题。这些概念支撑了该课程对计算普遍作用的探索。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Algorithmic_game_theory">Algorithmic game theory</a></li>
<li><a href="https://www.wolframscience.com/nks/p755--undecidability-and-intractability/">Undecidability and Intractability: A New Kind of Science | Online by...</a></li>

</ul>
</details>

**社区讨论**: 评论者深入讨论了相关内容：Diogenesian 警告不要过度延伸计算隐喻，而 sgt101 强调了物理学中不可判定性的具体例子。quux0r 赞扬了 Roughgarden 对算法博弈论的贡献，kaashif 则将其与历史上将宇宙解释为机器的尝试进行了类比。总体而言，讨论内容充实且尊重不同观点。

**标签**: `#computation`, `#philosophy of computer science`, `#physics`, `#algorithmic game theory`, `#undecidability`

---

<a id="item-6"></a>
## [OpenAI 发布 GPT-5.6 系列：Luna、Terra、Sol](https://simonwillison.net/2026/Jul/9/gpt-5-6/#atom-everything) ⭐️ 8.0/10

OpenAI 发布了 GPT-5.6 系列模型，包含三个尺寸：Luna、Terra 和 Sol，改进了智能体性能并具有竞争力的定价。这些模型拥有百万 token 上下文窗口和 128,000 输出 token，价格从每百万输入/输出 token 1/6 美元到 5/30 美元不等。 此次发布加剧了与 Anthropic 的 Claude 模型的竞争，尤其是在 Agents' Last Exam 等智能体基准测试上，GPT-5.6 Sol 在完全推理模式下比 Claude Fable 5 高出 13.1 分。新的 API 功能，如编程式工具调用和多智能体支持，可实现更复杂的智能体工作流，可能加速大语言模型在复杂自动化任务中的采用。 所有三个模型的知识截止日期为 2026 年 2 月 16 日，并支持编程式工具调用、多智能体子智能体生成以及提示缓存断点。OpenAI 声称 GPT-5.6 模型在 Agents' Last Exam 上以更低成本优于 Claude Fable 5，但 Claude 在 SWE-Bench Pro 上仍领先，不过 OpenAI 对该基准的可靠性提出了质疑。

rss · Simon Willison · 7月9日 19:46

**背景**: 大型语言模型通常使用推理 token 来进行思维链推理，在回答前增加额外计算。Agents' Last Exam (ALE) 是一个新的基准测试，评估 AI 智能体在长周期、高经济价值的可验证任务上的表现，旨在衡量真实世界的智能体性能。GPT-5.6 系列延续了 OpenAI 提供多种模型尺寸以平衡成本和能力的趋势，类似于 GPT-4 系列。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://agents-last-exam.org/">Agents' Last Exam</a></li>
<li><a href="https://arxiv.org/abs/2606.05405">[2606.05405] Agents' Last Exam</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#GPT-5.6`, `#AI models`, `#LLM`, `#benchmarks`

---

<a id="item-7"></a>
## [PostgreSQL 18 新增自连接消除 GUC](https://postgr.es/p/9pg) ⭐️ 7.0/10

PostgreSQL 18 引入了一个新的 GUC 变量 enable_self_join_elimination，允许查询优化器消除基于主键的冗余自连接，将其替换为简单的扫描。 此优化可提升 ORM 或嵌套视图产生不必要自连接的工作负载的查询性能，减少执行时间和资源消耗，无需手动重写查询。 该功能在证明自连接可被扫描替换且不影响结果时，移除表与自身的内连接。它由 enable_self_join_elimination GUC 控制，默认开启。

rss · Planet PostgreSQL · 7月10日 01:00

**背景**: 自连接消除是一种查询优化技术，用于检测表在其主键上与自身连接的情况，这种连接返回的行与原表相同。PostgreSQL 的查询规划器传统上会执行这些连接，而 PostgreSQL 18 现在可以安全地移除它们。GUC（Grand Unified Configuration）是 PostgreSQL 管理服务器配置参数的子系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.phoronix.com/news/PostgreSQL-Self-Join-Eliminate">PostgreSQL Lands Self-Join Elimination Optimization - Phoronix</a></li>
<li><a href="https://github.com/postgres/postgres/commit/fc069a3a6319b5bf40d2f0f1efceae1c9b7a68a8">Implement Self-Join Elimination · postgres/postgres@fc069a3</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database optimization`, `#self-join elimination`, `#query optimization`

---

<a id="item-8"></a>
## [Meta 发布 Muse Spark 1.1，新增 API 和增强的自主工具调用](https://simonwillison.net/2026/Jul/9/muse-spark-1-1/#atom-everything) ⭐️ 7.0/10

Meta 发布了 Muse Spark 1.1，这是首个提供 API 的 Spark 模型，同时在自主工具调用和计算机使用能力方面有显著改进。 此次发布标志着通过 API 使强大 AI 模型可访问的重要一步，使开发者能够将先进的自主行为集成到应用中。改进的工具调用和计算机使用功能拓宽了自主 AI 代理的潜力。 Muse Spark 1.1 具有一个有趣的技术现象——'自对话中的吸引子状态'，模型的两个副本可以产生内省式语句。社区插件 llm-meta-ai 提供了命令行和 Python 库访问该模型的方式。

rss · Simon Willison · 7月9日 16:24

**背景**: Muse Spark 是 Meta 最强大的模型，于 2026 年 4 月推出，专为复杂推理和多模态任务设计。自主工具调用允许 LLM 自主选择并执行外部函数，以桥接推理与行动。吸引子状态是指自玩轨迹成为特定模型的吸引子，在多轮对话中不对称地吸引对话伙伴。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aitinkerers.org/technologies/agentic-tool-calls">Browse 1 projects using agentic tool calls .</a></li>
<li><a href="https://arxiv.org/abs/2606.30571">[2606.30571] Attractor States Emerge in Multi-Turn LLM Conversations</a></li>
<li><a href="https://artificialanalysis.ai/models/muse-spark">Muse Spark - Intelligence, Performance & Price Analysis</a></li>

</ul>
</details>

**标签**: `#AI`, `#Meta`, `#Muse Spark`, `#agentic tool calling`, `#LLM`

---