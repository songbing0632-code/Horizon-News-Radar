---
layout: default
title: "Horizon Summary: 2026-11-14 (ZH)"
date: 2026-11-14
lang: zh
---

> 从 201 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [GGML v1.0.0 发布：生产就绪的 CPU 优化张量库](#item-tech-news-1) ⭐️ 8.0/10
2. [英伟达被指通过资助 AI 初创企业购买其 GPU 制造人为短缺](#item-tech-news-2) ⭐️ 8.0/10
3. [发现驱动衰老但不引发炎症的蛋白 Granzyme K](#item-tech-news-3) ⭐️ 8.0/10
4. [TorchTitan 实现 1T MoE 模型在 384 块 GH200 GPU 上训练](#item-tech-news-4) ⭐️ 8.0/10
5. [四款前沿模型在材料科学研究七项测试中得分 97.8–100](#item-tech-news-5) ⭐️ 8.0/10
6. [自变量机器人通用具身智能大模型完成中国监管备案](#item-tech-news-6) ⭐️ 7.0/10
7. [欧盟首次举行领导人 AI 专题峰会 聚焦产业竞争力与风险监管](#item-tech-news-7) ⭐️ 7.0/10

**财经新闻**
1. [芝加哥联储行长古尔斯比：美联储抗通胀“确实还有工作要做”](#item-finance-news-1) ⭐️ 7.0/10
2. [透视 10 月金融数据：资金流向与结构变化](#item-finance-news-2) ⭐️ 7.0/10
3. [美联储报告警示 AI 热潮推高美股估值并加剧网络风险](#item-finance-news-3) ⭐️ 7.0/10
4. [中国出台 22 项措施推进全面节约战略](#item-finance-news-4) ⭐️ 7.0/10
5. [企业贷款利率首次跌破 3%](#item-finance-news-5) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [GGML v1.0.0 发布：生产就绪的 CPU 优化张量库](https://github.com/ggml-org/ggml/releases/tag/v1.0.0) ⭐️ 8.0/10

GGML 项目正式发布 v1.0.0 版本，标志着该轻量级、开源张量库首次达到生产就绪（production-ready）状态。该版本专为 CPU 高效推理优化，支持 x86、ARM（包括 Apple Silicon）及 Vulkan 兼容 GPU 等多种硬件平台，无需 CUDA 或专用 AI 加速器。v1.0.0 已被 llama.cpp 等主流本地大模型推理工具链集成，提供稳定 ABI 和向后兼容的 C API。发布于 2026 年 11 月 14 日，源码托管于 GitHub 的 ggml-org/ggml 仓库。

hackernews · cobychapple · 11月14日 02:28 · [社区讨论](https://news.ycombinator.com/item?id=50493062)

**「GGML 的演进背景」** GGML 是一个专为 CPU 上高效张量运算设计的开源 C 语言库，最初作为 llama.cpp 的底层依赖而开发，用于在资源受限设备上运行大型语言模型。其设计强调零依赖、内存效率和跨平台可移植性，不依赖 CUDA 或 ROCm 等专有加速框架。

**「API 稳定性承诺影响下游项目维护」** GGML v1.0.0 首次正式承诺公共 C API 的向后兼容性：未来任何破坏性变更都将通过主版本号升级显式标识，这使依赖 libggml 的项目（如 llama.cpp）可将 GGML 视为具备语义化版本控制的稳定基础库，降低集成与升级维护成本。

**「社区讨论」** 多位用户报告实际性能提升：一名开发者在升级后对 50K token 长提示进行基准测试，端到端运行时间从 4 分 22 秒缩短至 3 分 59 秒；另一名用户强调其 AMD 显卡仅支持 Vulkan，但借助 GGML 仍可流畅运行本地 AI 应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grafy.ai/news/llama-cpp-and-ggml-hit-1-0-0-with-a-stable-api-promise">llama.cpp and ggml hit 1.0.0 — Grafy News</a></li>
<li><a href="https://dev.to/delimitter/llamacpp-and-ggml-ship-v100-semantic-versioning-comes-to-the-local-ai-stack-1ag4">llama.cpp and ggml ship v1.0.0 — semantic versioning comes to ...</a></li>

</ul>
</details>

**标签**: `#AI systems`, `#open source`, `#machine learning`, `#software engineering`, `#hardware acceleration`

---

<a id="item-tech-news-2"></a>
### [英伟达被指通过资助 AI 初创企业购买其 GPU 制造人为短缺](https://www.techpowerup.com/354814/nvidia-allegedly-engineered-scarcity-by-funding-ai-startups-to-buy-its-gpus) ⭐️ 8.0/10

据《华尔街日报》原始报道（经 Wccftech 和 TechPowerUp 转引），英伟达被指战略性地向多家 AI 初创企业提供风险投资，条件是这些公司必须采购英伟达 GPU；此举 allegedly 旨在维持市场对 GPU 的高需求感知、缓解台积电（TSMC）端可能存在的芯片过剩压力，并巩固其定价权与市场主导地位。报道未说明具体涉及多少家初创企业、融资总额、GPU 型号或交付数量，也未提供独立验证的供应链数据或监管调查进展。该说法目前仍属媒体指控，尚未有官方确认或反垄断机构公开立案。

hackernews · speckx · 11月14日 02:52 · [社区讨论](https://news.ycombinator.com/item?id=50493251)

**「背景」** 此前，自 2025 年底起，媒体已报道英伟达被指存在“循环融资”（circular financing）行为，即通过向 AI 基础设施公司注资，促使其采购英伟达 GPU，从而将资本支出转化为自身营收。2026 年 8 月，《华尔街日报》曾就此类安排进行报道并引述英伟达的回应，称其为正常战略合作；而 2026 年 11 月的新指控则进一步指向该做法被系统性用于人为制造 GPU 稀缺性。

**「对 AI 云基础设施采购和融资模式产生实际影响」** NVIDIA 已正式披露持有 Nebius 公司 9.3%的股份，且双方合作涉及 GPU 优先供应、联合 AI 工厂架构及 GPU 支持型债务融资；这导致 Nebius 股价在 2026 年 7 月披露后显著上涨，并为其他新兴云厂商（neoclouds）采用类似 GPU-backed debt 模式设定了可复制的先例。

**「社区讨论」** 部分 Hacker News 用户指出该模式并非新现象，援引《卫报》2025 年 12 月报道称英伟达此前已存在‘循环融资’（circular financing）实践；另有评论将此事置于更长历史脉络中，提及 GameWorks、G-Sync 等过往被质疑具有排他性或反竞争性质的商业策略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wsj.com/livecoverage/stock-market-today-dow-sp-500-nasdaq-08-27-2026/card/XdHmb8VRy4xMH42k7Z2M">Nvidia Pushes Back on Circular Financing Criticism</a></li>
<li><a href="https://www.techpowerup.com/354814/nvidia-allegedly-engineered-scarcity-by-funding-ai-startups-to-buy-its-gpus">NVIDIA Allegedly Engineered Scarcity By Funding AI Startups ...</a></li>
<li><a href="https://investor.nvidia.com/news/press-release-details/2026/NVIDIA-and-Nebius-Partner-to-Scale-Full-Stack-AI-Cloud/default.aspx">NVIDIA Corporation - NVIDIA and Nebius Partner to Scale Full ...</a></li>
<li><a href="https://noqta.tn/en/news/nvidia-9-3-percent-stake-nebius-gpu-backed-debt-2026">Nvidia Discloses 9.3% Stake in Nebius as Neoclouds Turn GPUs ...</a></li>
<li><a href="https://cryptobriefing.com/nebius-stock-surges-nvidia-9-percent-stake/">Nebius stock surges after Nvidia discloses 9% stake</a></li>

</ul>
</details>

**标签**: `#AI-hardware`, `#market-dynamics`, `#NVIDIA`, `#cloud-infrastructure`, `#antitrust`

---

<a id="item-tech-news-3"></a>
### [发现驱动衰老但不引发炎症的蛋白 Granzyme K](https://www.nature.com/articles/d41586-026-03638-3) ⭐️ 8.0/10

一项发表于《Immunity》期刊的研究鉴定出颗粒酶 K（Granzyme K，GzmK）是一种在不触发炎症或免疫衰老的情况下直接驱动组织器官衰老的蛋白。该结论基于 GzmK 缺陷小鼠模型：尽管其免疫系统仍呈现典型衰老表型，但多个器官的衰老进程显著减缓，证实组织衰老与免疫衰老可被解耦。研究明确将 GzmK 定位为组织特异性衰老驱动因子，而非系统性炎性衰老（inflammaging）的介质。

hackernews · gumby · 11月13日 19:25 · [社区讨论](https://news.ycombinator.com/item?id=50488470)

**「Granzyme K 的已知生物学功能」** Granzyme K（GzmK）是一种由人类 5 号染色体上 GZMK 基因编码的丝氨酸蛋白酶，属于颗粒酶家族，传统上被认为在细胞毒性淋巴细胞介导的靶细胞凋亡中起作用。此前研究已提示其在免疫衰老轨迹分化中的作用：健康个体随年龄增长，免疫细胞逐渐向 GzmK 高表达状态偏移，而过早向 GzmB 高表达状态转变则与病理性衰老相关。

**「实际影响」** 该发现为开发靶向 GzmK 的抗衰老干预策略提供了新路径，尤其适用于避免全身性免疫抑制风险的组织特异性抗衰治疗；研究人员需重新评估现有衰老模型中炎症标志物的必要性，并在动物实验中验证 GzmK 抑制剂对器官功能维持的效果。

**「社区讨论要点」** 评论者 ethanj8011 援引论文摘要强调 GzmK 缺失仅缓解器官衰老、并不改善免疫衰老或系统性炎性衰老，纠正了部分评论（如 StilesCrisis）对‘小鼠不再衰老’的过度简化解读；而 dimavolo 的评论则反映了公众对衰老表型可逆性的认知局限，未触及该研究解耦组织与免疫衰老的核心机制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GZMK">GZMK - Wikipedia</a></li>
<li><a href="https://medicalxpress.com/news/2026-10-immune-cell-uncovers-individual-aging.html">Immune cell map uncovers how individual aging trajectories diverge</a></li>

</ul>
</details>

**标签**: `#aging`, `#immunology`, `#molecular-biology`, `#longevity`, `#cell-biology`

---

<a id="item-tech-news-4"></a>
### [TorchTitan 实现 1T MoE 模型在 384 块 GH200 GPU 上训练](https://www.reddit.com/r/MachineLearning/comments/1xvce5h/scaling_to_1t_moe_on_torchtitan_p/) ⭐️ 8.0/10

工程师团队在 JUPITER 超级计算机的 384 块 NVIDIA GH200 GPU 上，使用 TorchTitan 成功实现了约 1 万亿参数（~1T）Mixture of Experts（MoE）模型的训练，达到约 1300 tokens/s/GPU 的吞吐量，相较初始基线提升 14 倍。该实现采用 FSDP（Fully Sharded Data Parallel）与节点内 4 路 Expert Parallelism（EP）的混合策略，规避了 Pipeline Parallelism；关键优化包括：全激活检查点+Grace CPU 内存卸载、Muon 优化器配合 FlexShard 参数分片、注意力计算负载均衡、bf16 梯度 all-to-all 替代 reduce-scatter、FP8 专家通信、以及修复 PyTorch 缓存分配器导致的虚假 OOM 问题。所有改进均在无 root 权限、纯用户态环境下完成。

reddit · r/MachineLearning · /u/f14-bertolotti · 11月13日 16:28

**「TorchTitan 背景」** TorchTitan 是一个开源的、原生 PyTorch 的分布式训练框架，旨在统一并简化前沿大模型训练中的多维并行技术（如 FSDP、专家并行、流水线并行），其设计目标是易理解、易扩展且面向生产就绪。它并非独立运行时，而是构建在 PyTorch 原生分布式原语之上，支持从单节点到千卡集群的可组合式并行策略。

**「影响」** 该成果为大规模 MoE 模型训练提供了可复现、高吞吐、低通信开销的开源工程范式，直接支持研究者和机构在非定制化 Hopper 架构（如 GH200）上高效扩展至万亿参数量级，且无需依赖 Pipeline Parallelism 或特权系统访问权限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://discuss.pytorch.org/t/distributed-w-torchtitan-training-with-zero-bubble-pipeline-parallelism/214420">[Distributed w/ TorchTitan ] Training with... - PyTorch Forums</a></li>
<li><a href="https://arxiv.org/pdf/2410.06511">TorchTitan : One-stop PyTorch native solution for production ready...</a></li>

</ul>
</details>

**标签**: `#large-language-models`, `#distributed-training`, `#mixture-of-experts`, `#pytorch`, `#gpu-scaling`

---

<a id="item-tech-news-5"></a>
### [四款前沿模型在材料科学研究七项测试中得分 97.8–100](https://www.reddit.com/r/MachineLearning/comments/1xvgf6h/four_frontier_models_scored_978100_on_a_7part/) ⭐️ 8.0/10

一位材料科学领域研究者设计并实施了一套包含 7 个环节的合成基准测试，覆盖张力数据处理、CIF 密度函数编写、物理估算、论文审阅、虚假前提识别、实验设计及受限摘要撰写，全部使用合成数据与代码自动生成答案和评分；Gemini 4 Carbon、Gemini 4 Hydrogen（Antigravity）、Claude Opus 5.5 和 Claude Fable 5.2 在启用网页搜索与代码执行、设置为“High”而非最高模式下，三轮独立运行的平均分分别为 100.0、99.7、99.3 和 98.5，全部 12 次运行得分介于 97.8 至 100 之间，失分仅源于格式等次要细节；该测试未评估长周期开放性科研任务能力。

reddit · r/MachineLearning · /u/v\_aravind · 11月13日 18:58

**「背景」** 当前主流大语言模型评测多聚焦于短周期、单步响应任务（如 MMLU、GPQA），而对需多步骤推理、工具调用、错误恢复与长期目标管理的科研级代理（agent）行为缺乏系统评估框架；此前 METR、FrontierScience 和 PaperBench 等项目已指出，封闭式、流程明确的技术任务性能趋于饱和，瓶颈转向长周期、开放性科研工作流。

**「影响」** 该测试表明，在受控、流程清晰的材料科学研究子任务中，前沿闭源模型已接近人类专家水平，但其高分不反映真实科研中应对模糊目标、资源约束与意外干扰的能力；研究者正构建模拟实验室环境（含预算、仪器、目标规格与植入式意外事件），以支持持续 2–6 小时的代理行为轨迹评估。

**「社区讨论」** 无可用评论，社区未就该测试方法、结果解释或长周期评估指标展开实质性讨论。

**标签**: `#AI evaluation`, `#scientific computing`, `#LLM benchmarks`, `#materials science`, `#agent reasoning`

---

<a id="item-tech-news-6"></a>
### [自变量机器人通用具身智能大模型完成中国监管备案](https://news.google.com/rss/articles/CBMib0FVX3lxTE5SSUg0VllsNXRCRlJGRmZTZzJUVW92aEppWllJSGhYWDZzZmpjT2N2d1E2UmtYYUdZZGt6WkEwLXpkYjFZSHFaOHBET0lRb1JETU1qZlJ5aW05c1pxcUxZNEJ3V1BZV2p1bjZkV0oyQQ?oc=5) ⭐️ 7.0/10

自变量机器人（Zibian Robot）自主研发的通用具身智能大模型已在中国国家网信办完成生成式人工智能服务备案。该备案于 2026 年 11 月 14 日前正式生效，面向公众提供服务需满足《生成式人工智能服务管理暂行办法》要求。备案主体为自变量机器人公司，模型类型明确标注为‘通用具身智能大模型’，区别于纯语言或视觉大模型。目前公开信息未披露模型名称、参数规模、训练数据来源、推理平台兼容性或具体落地场景。

rss · Google News AI · 11月14日 03:49

**「具身智能的监管进展」** 在中国，生成式人工智能服务需依据《生成式人工智能服务管理暂行办法》完成备案，方可面向公众提供服务；该要求自 2023 年 8 月 15 日起施行，适用于大语言模型及具备感知、决策、执行能力的具身智能系统。此前，国内多家 AI 企业已为文本或图像生成模型完成备案，但面向通用具身智能（即支持多任务、跨场景物理交互的自主智能体）的大模型备案尚属罕见。

**标签**: `#embodied AI`, `#large language models`, `#AI regulation`, `#robotics`, `#China tech policy`

---

<a id="item-tech-news-7"></a>
### [欧盟首次举行领导人 AI 专题峰会 聚焦产业竞争力与风险监管](https://news.google.com/rss/articles/CBMiSEFVX3lxTE9WUjhfVGFNX0hlOUZyXzBicENMYjZvRnI5Y3Q5UVNzR2d2QVd3WFBwTW1IM0xWWlhOaGY4cHZ2eldSMFNUSFhUQw?oc=5) ⭐️ 7.0/10

2026 年 11 月 13 日，欧盟首次召开由成员国国家元首和政府首脑参与的 AI 专题峰会，核心议程是协调提升欧洲 AI 产业竞争力与建立统一、可执行的风险监管框架。会议未宣布具体立法草案、技术标准或资金计划，也未达成具有约束力的联合承诺，仅确认将加快《人工智能法案》（AI Act）实施准备及跨成员国 AI 测试沙盒协调。该峰会为政治宣示性质，不涉及产品发布、系统部署或技术规格变更。

rss · Google News AI · 11月13日 17:34

**「欧盟 AI 治理框架演进背景」** 欧盟此前已通过《人工智能法案》（AI Act），于 2024 年 3 月由欧洲议会正式批准，成为全球首个全面规制 AI 系统的区域性法律框架；该法案按风险等级对 AI 应用实施分级监管，并确立了高风险 AI 系统上市前合规评估义务。本次峰会是继 AI Act 立法落地后，欧盟首次由成员国领导人层面召开的 AI 专题会议，标志着监管重心正从规则制定转向产业部署与国际竞争力协同。

**标签**: `#AI policy`, `#regulation`, `#EU`, `#technology strategy`, `#AI governance`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [芝加哥联储行长古尔斯比：美联储抗通胀“确实还有工作要做”](https://www.cnbc.com/2026/11/13/chicago-feds-goolsbee-says-central-bank-has-definitely-got-work-to-do-on-inflation.html) ⭐️ 7.0/10

芝加哥联储行长古尔斯比称美联储“确实还有工作要做”，以重拾抗通胀公信力；他指出 10 月生产者价格指数（PPI）同比上涨 6.5%，为 2022 年 11 月以来最高，且当前通胀正偏离 2%目标，既持续高于目标近六年，又出现由 AI 数据中心建设引发的新一轮需求过热压力。

rss · CNBC Finance · 11月13日 14:22

**「背景」** 古尔斯比是 2027 年联邦公开市场委员会（FOMC）投票委员，虽 2026 年无投票权，但其表态被视为重要政策信号；他发言前，美国劳工统计局刚公布 10 月 PPI 同比升 6.5%、CPI 涨幅略超预期。

**「影响」** 市场已完全定价 12 月 8—9 日 FOMC 会议加息 25 个基点，并计入超 10%概率的 50 个基点加息，表明该表态可能直接推动短期利率路径上移。

**标签**: `#monetary\_policy`, `#inflation\_data`, `#fed\_officials`

---

<a id="item-finance-news-2"></a>
### [透视 10 月金融数据：资金流向与结构变化](https://news.google.com/rss/articles/CBMiggFBVV95cUxQM1VIWjlvN1pKWGM4cTdXYjBXVkJzd2RkcFNtTFR3eE04a194c1c1bFVKaEVEQUpYNFJJektGWDk4UEszcUsyOS1JZDdkNS1Nc0Y2aUZUOGVtYzZwSGJEd1FIanNaQTQ1M2F0NGwtZXplVXI1MFBRNmZsSkdOZkdfbGFR?oc=5) ⭐️ 7.0/10

新华社分析称，2026 年 10 月中国社会融资规模增量为 1.85 万亿元人民币，较 9 月增加 2170 亿元；广义货币（M2）余额同比增长 8.3%，增速比 9 月末低 0.1 个百分点。

rss · Google News 财经 · 11月13日 14:47

**「背景」** 中国人民银行通常每月发布金融统计数据，包括广义货币（M2）、新增人民币贷款和社会融资规模等关键指标，用以反映信贷投放方向和金融体系流动性结构变化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://la.china-embassy.gov.cn/eng/news/202610/t20261015_12040919.htm">China&#x27;s Q1-Q3 yuan loan growth backs real economy with ...</a></li>
<li><a href="https://www.yicaiglobal.com/news/chinas-money-supply-social-financing-accelerate-in-october-as-borrowing-costs-fall">China’s Money Supply, Social Financing Grow Faster in October ...</a></li>

</ul>
</details>

**标签**: `#monetary\_policy`, `#china\_economy`, `#credit\_data`

---

<a id="item-finance-news-3"></a>
### [美联储报告警示 AI 热潮推高美股估值并加剧网络风险](https://news.google.com/rss/articles/CBMiU0FVX3lxTE5HZkVCM1UtaFZzQ2dETVRvWnhMNzJudm9RemZZRGdoMFJ4alduXzJ6NXlfaW1ZQmo0SUdqOU5INnhLRHRYNnFnSjAtZ3ZYN0FuV0Mw?oc=5) ⭐️ 7.0/10

美联储最新《金融稳定报告》指出，人工智能相关投资热情正推动美国股市估值虚高，同时金融基础设施面临的网络安全风险正在上升。

rss · Google News 财经 · 11月13日 21:37

**「背景」** 美联储每半年发布一次《金融稳定报告》，评估美国金融体系面临的主要风险；2026 年报告首次将人工智能相关风险正式纳入金融稳定议程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.federalreserve.gov/">The Federal Reserve Board of Governors in Washington DC.</a></li>
<li><a href="https://www.linkedin.com/posts/kristalina-georgieva_the-latest-global-financial-stability-report-activity-7449894400131756032-6i3k">The latest Global Financial Stability Report finds that the war in the...</a></li>

</ul>
</details>

**标签**: `#monetary\_policy`, `#market\_valuation`, `#cybersecurity\_risk`

---

<a id="item-finance-news-4"></a>
### [中国出台 22 项措施推进全面节约战略](https://news.google.com/rss/articles/CBMibkFVX3lxTE1UaGs5VGlsaDg2Z2RuY1FKVEhobzZfTUFsem9TTGRJYzVJalFFZ1A0UklSTUMwV0toR0dST1ZaQzJyVUotbk1MbTVFblpFN0tHMjlNckZneDdRYmJlR3BFdFhBdTZLTVloVGNCNkJB?oc=5) ⭐️ 7.0/10

中国官方宣布实施 22 条具体举措，以推动‘全面节约战略’落地，该战略聚焦能源、资源和工业领域的节约集约利用。

rss · Google News 财经 · 11月13日 20:47

**「背景」** 该战略是国家层面推动资源节约和绿色低碳发展的系统性部署，承接此前已发布的《全面节约战略纲要》及 2026 年 7 月出台的林业草原五年保护规划等政策框架。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://english.news.cn/20261105/9d0b57f1e9c244cb8a574d7a68571254/c.html">China issues plan to advance comprehensive resource conservation</a></li>
<li><a href="https://english.www.gov.cn/news/202607/22/content_WS6a609e8cc6d00ca5f9a0c5b8.html">China issues five-year plan for forestry, grassland conservation</a></li>

</ul>
</details>

**标签**: `#Chinese policy`, `#energy efficiency`, `#industrial policy`

---

<a id="item-finance-news-5"></a>
### [企业贷款利率首次跌破 3%](https://news.google.com/rss/articles/CBMickFVX3lxTE9DZG95VDdQTWJCcDJwbmtVVFFlLU5PUzNJVzl3VXlmbEtLWHNMQV9VLWZuYUo4SWM1M19KSjdiNnJraWs3TC1wamRQNTBCaDQtejVWLXByQl8waWRSWUJjdklaYjVIOGx4RVExaXRRVVNpQQ?oc=5) ⭐️ 7.0/10

中国金融机构企业贷款加权平均利率首次降至 3%以下，创历史新低。

rss · Google News 财经 · 11月14日 01:48

**「背景」** 中国人民银行 2026 年第三季度货币政策报告显示，2026 年 9 月新发放企业贷款加权平均利率首次跌破 3.0%，较上年同期下降约 0.2 个百分点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.biggo.com/news/22717968-5464-45e6-8b67-399509e0103f">China&#x27;s corporate loan rates fall below 3%, but why are SME ...</a></li>

</ul>
</details>

**标签**: `#monetary\_policy`, `#interest\_rates`, `#China\_economy`

---