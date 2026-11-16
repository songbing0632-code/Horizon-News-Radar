---
layout: default
title: "Horizon Summary: 2026-11-16 (ZH)"
date: 2026-11-16
lang: zh
---

> 从 237 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [解耦多模态视觉编码：预训练并非必需](#item-tech-news-1) ⭐️ 8.0/10
2. [LLM 内部行为可视化工具 inside-llm 发布](#item-tech-news-2) ⭐️ 8.0/10
3. [Qwen4-Max 正式上线并计划开源小模型](#item-tech-news-3) ⭐️ 8.0/10
4. [上海发布住建行业 AI+行动计划](#item-tech-news-4) ⭐️ 7.0/10
5. [AI 医疗诊断可靠性测试：四款大模型表现曝光](#item-tech-news-5) ⭐️ 7.0/10

**财经新闻**
1. [中国 10 月经济放缓加剧 零售、工业产出、投资均不及预期](#item-finance-news-1) ⭐️ 9.0/10
2. [Lutnick 因 Nvidia 丑闻面临质疑](#item-finance-news-2) ⭐️ 8.0/10
3. [59 家 A 股公司披露股票回购贷款上限超 146 亿元](#item-finance-news-3) ⭐️ 8.0/10
4. [美法官驳回 DRAM 价格操纵案撤诉请求](#item-finance-news-4) ⭐️ 8.0/10
5. [MicroStrategy 因被 MSCI 剔除指数后夜盘暴跌超 8%](#item-finance-news-5) ⭐️ 7.0/10
6. [英伟达黄仁勋离任后首份财报将揭晓](#item-finance-news-6) ⭐️ 7.0/10
7. [中美俄领导人在深圳举行首次三方会晤](#item-finance-news-7) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [解耦多模态视觉编码：预训练并非必需](https://www.reddit.com/r/MachineLearning/comments/1xx1k2o/meta_fair_nyu_unbundling_multimodal_vision/) ⭐️ 8.0/10

Meta FAIR 与 NYU 的一项研究通过训练超过 200 个模型，发现多模态视觉语言模型中的视觉编码器预训练是可选的，而仅用于视觉的参数则是必需的。在相同计算预算下，预训练编码器在 VQA 任务上并未优于从头训练的编码器。研究还表明，在 LLM 前放置编码器也并非必要，使用“in-fusion”方法（将视觉参数添加到 LLM 前几层）可以达到相近性能。

reddit · r/MachineLearning · /u/trungh98 · 11月15日 17:38

**「多模态模型架构研究背景」** 当前主流多模态视觉语言模型（VLM）通常采用统一的视觉编码器，该编码器可能经过预训练或与语言模型联合训练。然而，不同模型在是否使用预训练编码器、是否为视觉任务专门设计参数等方面存在分歧。这项研究旨在系统评估这些设计选择的实际影响，通过构建大量变体模型进行实证分析。

**「对模型设计和训练的影响」** 研究人员发现，视觉编码器的预训练并非提升性能的关键因素，这可能促使开发者在构建轻量级多模态模型时减少对预训练步骤的依赖。同时，研究指出视觉专用参数对于模型性能至关重要，因此在资源受限的情况下，应优先考虑为视觉任务分配独立参数而非预训练过程。

**标签**: `#multimodal learning`, `#vision-language models`, `#model architecture`, `#empirical research`, `#machine learning systems`

---

<a id="item-tech-news-2"></a>
### [LLM 内部行为可视化工具 inside-llm 发布](https://www.reddit.com/r/LocalLLaMA/comments/1xx7qbf/i_have_created_a_tool_to_observe_what_happens/) ⭐️ 8.0/10

开发者发布了一个名为 inside-llm 的开源工具，用于在浏览器中实时查看和比较两个 GGUF 模型在文本生成过程中的行为。该工具支持锁步（lockstep）和自由模式（free），可显示每个 token 的概率、模型分歧点、采样器链路、熵值及 JS 散度等指标，并允许用户点击分支进行回溯分析。它基于 llama.cpp 构建，支持 Linux 和 Windows 平台，使用 WebSocket 实时传输数据并嵌入网页界面。

reddit · r/LocalLLaMA · /u/AlternativeEnough352 · 11月15日 21:46

**「背景」** GGUF 是 llama.cpp 使用的模型格式，量化（quantization）将模型权重从高精度（如 FP32）转换为低精度（如 Q4\_K\_M、Q8\_0），显著减小模型体积并加速推理。不同量化级别会导致模型在 token 预测概率上产生微小差异，累积后可能造成输出分歧。该工具 inside-llm 通过可视化方式展示模型生成过程中的 logits 分布、采样链各阶段、以及两个量化版本之间的分歧点，帮助开发者理解量化对模型行为的具体影响。

**「对研究者和开发者的实用价值」** 该工具为研究人员和开发者提供了一种直观的方式来分析不同量化版本或变体模型之间的差异，特别是在推理过程中如何产生不同的输出。这有助于理解量化带来的性能与精度权衡，以及模型决策机制的细微差别。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ggml-org/llama.cpp/blob/master/tools/quantize/README.md">llama.cpp/tools/quantize/README.md at master - GitHub</a></li>
<li><a href="https://tech-insider.org/gguf-model-quantization-2026/">GGUF Quantization with llama.cpp: A Reproducible Workflow</a></li>

</ul>
</details>

**标签**: `#artificial-intelligence`, `#machine-learning`, `#tools-and-libraries`

---

<a id="item-tech-news-3"></a>
### [Qwen4-Max 正式上线并计划开源小模型](https://mp.weixin.qq.com/s/pJUt0xwD6H-WMyzd8TjZaQ) ⭐️ 8.0/10

阿里巴巴通义千问发布了新一代旗舰大模型 Qwen4-Max，采用全新稀疏 MoE 架构，参数量达 2.4 万亿，支持视觉理解和百万 Token 长上下文处理。该模型在编程与长程任务中表现优异，并在成本控制上相较上一代降低近 58%。此外，团队宣布未来将开源更小规模的 Qwen4 系列模型。

telegram · zaihuapd · 11月16日 02:52

**「背景介绍」** 阿里巴巴推出了新一代旗舰大模型 Qwen4-Max，该模型基于全新的稀疏 MoE 架构，参数总量达到 2.4 万亿，具备视觉理解与百万 Token 上下文长度的支持能力。它在编程、办公及复杂任务执行方面表现出色，且 API 定价已调整为每百万输入 token 1.5 美元、输出 token 4.5 美元，相较上一代显著降低成本。此外，Qwen4-Max 已正式上线，并计划后续开源更小规模的 Qwen4 系列模型。

**「对开发者的影响」** Qwen4-Max 的低成本与高性能可能促使更多开发者采用该模型进行开发，尤其在需要长上下文或复杂推理任务的场景中。同时，后续开源的小模型将为研究者和中小企业提供更多实验与部署的可能性。

**「社区讨论摘要」** 部分用户对比了 Qwen4-Max 与其他模型的表现，指出其在推理效率和速度方面仍有提升空间；也有评论认为开源计划有助于推动行业竞争，但也有人批评某些厂商限制开源以维持市场地位。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/models/qwen4-max">Qwen 4 Max - Intelligence, Performance &amp; Price... | Artificial Analysis</a></li>
<li><a href="https://www.qwencloud.com/models/qwen4-max?region=ap-southeast-1">Qwen 4 - Max - QwenCloud</a></li>
<li><a href="https://openrouter.ai/qwen/qwen4-max">Qwen 4 Max - API Pricing &amp; Providers | OpenRouter</a></li>
<li><a href="https://freakyjolly.com/qwen4-max-guide/">Qwen4-Max Is Out: $1.50 API Price, Benchmarks, Setup</a></li>

</ul>
</details>

**标签**: `#AI模型`, `#大语言模型`, `#技术发布`, `#开源计划`, `#阿里巴巴`

---

<a id="item-tech-news-4"></a>
### [上海发布住建行业 AI+行动计划](https://news.google.com/rss/articles/CBMivAJBVV95cUxOUTdjYTFBZWVMdlRBeXB1ZkZDTnFndWhXQjNPdU5aU3ExUXdIa2NOUC1rZzg0MDVMR2JOelJuY3pvMlFCLXg1SF90VWt2emZ5Tk1ZZ192aFhxNlIxSk5GbldSMWVCeHpDZEdQU1lpbk9nQzE4Sk95OXdUc3o0ZjNuYVctWUNYdVZsVXp6d0hDWk1mbzRxc1JSNXRtckM5eG52eVo5LS1Dd0pZbkdTWVZ5OVBrUEI0UHpic01jQkcwazkxTk95LTlwY1E0SlBucGJfUUM5Q19EZTMwYWtFVWRJUENGeUJhZ1BtaV9EdGlMVy1qc180ZVlNN1FGcUY2Rk1ZOXpMSDFFT3RoU1JmMzN4UnA0c1hBbG5oZ09EV0VhbmhuVm5wNDBrYjRlV0lxbk1tbDAtMmFxaTJUSnBF?oc=5) ⭐️ 7.0/10

上海市发布了面向住房与城乡建设行业的‘人工智能+’行动计划，覆盖 2026 至 2028 年。该计划旨在推动人工智能技术在建筑和基础设施管理中的应用，明确支持方向并提供政策保障。此举标志着上海对智能城市建设及传统行业数字化转型的持续投入。

rss · Google News AI · 11月16日 09:45

**「背景」** 上海市发布的《住房和城乡建设行业“人工智能+”行动计划（2026—2028 年）》是该市在人工智能与城市建设融合方面的政策引导性文件。该计划旨在推动 AI 技术在建筑、基础设施管理等领域的应用，体现了政府对智能建造和智慧城市发展的支持方向。此前，如广州等地也发布了类似的行动计划，显示了中国多个城市在推进 AI 与城市治理、产业发展结合方面的政策连续性和区域协同趋势。

**「实际影响」** 该行动计划将促使相关企业加大在智能建造、城市基础设施智能化管理等领域的研发投入和技术引进，有助于提升行业整体效率和管理水平。对于从事智慧城市解决方案的企业而言，这可能带来新的市场机遇和政策支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.smartcity.team/policies/digitaleconomy/guangzhou_harmonycity/">广州 市 鸿蒙 智 城 建 设 行 动 计 划 （ 2026 - 2028 ...</a></li>
<li><a href="https://www.workercn.cn/papers/grrb/2026/04/06/7/grrb202604067.pdf">grrb0720260406B</a></li>

</ul>
</details>

**标签**: `#artificial-intelligence`, `#smart-cities`, `#government-policy`, `#construction`, `#china`

---

<a id="item-tech-news-5"></a>
### [AI 医疗诊断可靠性测试：四款大模型表现曝光](https://news.google.com/rss/articles/CBMijwFBVV95cUxNamUxaTdJU3NzLU0xNV96RDFHRkh6SXpHeUgwUU5leG1tNHA4MTlhWERnRm8xREVZNW5QOW00S2tLeGs1T3FBVXZsTm96d1hiWTh1NXFlMldCUTNXMFRjUHFvY1hmVGR2X0lROTlNX3R0TS1UQlhBU2FDRWEzRHRPZkIzRExtZXlZcmV0ZDR1NA?oc=5) ⭐️ 7.0/10

一篇中国媒体报道了对四款主流大语言模型在医疗诊断中可靠性的测试结果，这些模型在模拟病例中的表现参差不齐。该文章由一个真实案例引发：一名儿童因过度依赖 AI 诊断而延误治疗，最终发展为重症肺炎。测试旨在评估 AI 在临床决策支持中的适用性与风险。

rss · Google News AI · 11月16日 07:07

**「医疗 AI 诊断的评估背景」** 在医疗诊断领域，大型语言模型（LLM）的应用正日益广泛，但其准确性和可靠性仍存在争议。已有研究尝试将 LLM 与传统预测模型结合以提升诊断精度，并通过临床笔记测试 AI 的诊断能力和推理过程。例如，DiReCT 基准系统要求 AI 模型不仅提供诊断结果，还需解释诊断逻辑，以评估其在实际医疗场景中的适用性。

**「AI 医疗诊断的现实风险」** 该案例显示，家长盲目信任 AI 而非寻求专业医疗建议，导致孩子病情延误至重症肺炎，凸显当前大模型在医学诊断领域的局限性。AI 可辅助肺炎早期筛查（如胸部 X 光分析），但不应替代临床诊断，就医延迟仍是儿童肺炎预后恶化的关键风险因素。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/synergizing-predictive-models-large-language-medical-obiri-affram-gpahe">Synergizing Predictive Models with Large Language Models in...</a></li>
<li><a href="https://www.promptlayer.com/research-papers/direct-diagnostic-reasoning-for-clinical-notes-via-large-language-models">DiReCT: Diagnostic Reasoning for Clinical Notes via Large Language ...</a></li>
<li><a href="https://www.mdpi.com/2077-0383/9/1/248">Can Artificial Intelligence Improve the Management of Pneumonia</a></li>
<li><a href="https://journals.plos.org/digitalhealth/article?id=10.1371/journal.pdig.0000713">Detection of pneumonia in children through chest radiographs ...</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC13488239/">Determinants of delay in treatment-seeking for under-five ...</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#medical AI`, `#LLM evaluation`, `#AI reliability`, `#healthcare technology`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [中国 10 月经济放缓加剧 零售、工业产出、投资均不及预期](https://www.cnbc.com/2026/11/16/china-retail-sales-october-industrial-output-investment.html) ⭐️ 9.0/10

中国 10 月经济放缓加剧，零售销售同比仅增长 0.4%，低于分析师预期的 0.8%；工业产出同比增长 4.8%，低于预期的 5.3%；固定资产投资前 10 个月同比下降 8.1%，降幅大于预期的 7%，为除新冠时期外前所未有的深度下滑。高盛预计中国经济今年增长 4.6%，明年进一步放缓至 4.5%。

rss · CNBC Finance · 11月16日 03:53

**「背景」** 中国 10 月份经济放缓加剧，工业产出、零售销售和投资均未达到分析师预期。此前在 7 月数据已显示经济疲软，而此次进一步恶化，凸显了房地产市场下滑对家庭财富的持续冲击。

**「中国经济放缓加剧影响全球贸易」** 中国 10 月份工业产出、零售销售和投资均未达预期，显示经济疲软可能进一步冲击全球市场。由于房地产市场低迷和消费支出疲弱，固定资产投资同比下降 8.1%，为疫情以来罕见的降幅。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/16/china-retail-sales-october-industrial-output-investment.html">China ’ s slowdown deepens in October as key economic data...</a></li>
<li><a href="https://www.business-standard.com/world-news/china-s-economic-slowdown-revives-calls-for-stronger-stimulus-measures-126051801744_1.html">China &#x27; s economic slowdown revives calls for... - Business Standard</a></li>
<li><a href="https://www.theguardian.com/business/2026/aug/17/china-economy-slowdown-signs-extending">China ’ s economy showing signs that slowdown may... | The Guardian</a></li>
<li><a href="https://www.rand.org/pubs/commentary/2025/02/focus-on-the-new-economy-not-the-old-why-chinas-economic.html">Focus on the New Economy , Not the Old: Why China &#x27; s Economic ...</a></li>

</ul>
</details>

**标签**: `#economic indicators`, `#trade policy`, `#export growth`, `#labor market`, `#AI economy`

---

<a id="item-finance-news-2"></a>
### [Lutnick 因 Nvidia 丑闻面临质疑](https://www.cnbc.com/2026/11/13/howard-lutnick-nvidia-jensen-huang-china-cantor-fitzgerald.html) ⭐️ 8.0/10

美国商务部长 Howard Lutnick 因旗下公司 Cantor Fitzgerald 减持英伟达股票而受到质疑，其子所持英伟达股份在 2025 年 9 月至 2026 年 3 月间减少了近 50%。同时，Lutnick 曾拒绝配合打击涉嫌向中国走私英伟达芯片的公司 Megaspeed。

rss · CNBC Finance · 11月15日 19:58

**「背景」** 美国商务部长霍华德·卢特尼克（Howard Lutnick）曾执掌华尔街投行康托·菲茨杰拉德（Cantor Fitzgerald），其子布兰登和凯尔现已成为该公司领导人。该公司长期持有大量英伟达股票，并在 9 月接待了英伟达 CEO 黄仁勋。与此同时，美国情报部门已向卢特尼克发出关于黄仁勋与疑似中国间谍关系的机密警告，政府也在加大力度打击涉嫌向中国走私英伟达 AI 芯片的企业。

**「影响」** 由于美国商务部长 Howard Lutnick 之子所持的 Cantor Fitzgerald 公司大幅减持英伟达股票，且其父在知情情况下未采取行动限制涉嫌向中国走私先进 AI 芯片的公司，引发利益冲突质疑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://edition.cnn.com/2026/11/16/tech/nvidia-sex-spies-serious-problems">Lies, spies and sex are just one part of the Nvidia story.</a></li>
<li><a href="https://gpusmith.com/articles/en/nvidia-gpu-export-restrictions">NVIDIA Export Controls 2026: H200, H20 &amp; China Rules</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/billions-worth-of-export-restricted-ai-accelerators-sold-to-china-report-details-how-chinese-firms-skirt-trumps-regulations">Investigative report details how export-restricted Nvidia AI ...</a></li>
<li><a href="https://www.cnbc.com/2026/11/13/howard-lutnick-nvidia-jensen-huang-china-cantor-fitzgerald.html">Howard Lutnick &#x27;s sons &#x27; Nvidia ties amid Jensen Huang China spy...</a></li>
<li><a href="https://www.nytimes.com/2026/11/15/us/politics/trump-lutnick-ai-chips-nvidia-cantor-fitzgerald.html">Lutnick Pushed to Weaken Chip Rules That Overlap With His Family...</a></li>

</ul>
</details>

**标签**: `#government`, `#conflict of interest`, `#national security`, `#technology`, `#regulation`

---

<a id="item-finance-news-3"></a>
### [59 家 A 股公司披露股票回购贷款上限超 146 亿元](https://news.google.com/rss/articles/CBMiZ0FVX3lxTE9TYzc3b0ZIeE1OWWYtRkxtalpCRV9SaUVWcFZNN0JTSElMcGJOcGpQTXJldVVMY01PcGp3aXVRSVEwaGZiaXNKN3d0SVB5UVRJczNlODFkeGs1WkNnY2ZKTW9GcUNQYk0?oc=5) ⭐️ 8.0/10

59 家 A 股上市公司披露了用于股票回购的贷款总额上限超过 146 亿元人民币，单个公司最高额度达 18 亿元。

rss · Google News 财经 · 11月16日 10:53

**「背景」** 为稳定股市，中国央行自 2024 年 10 月起推出专项再贷款政策，支持上市公司进行股票回购和大股东增持。该政策已从临时措施转为长期制度安排，并将再贷款利率降至 1%。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.globaltimes.cn/page/202611/1373487.shtml">CSRC rolls out policy mix to steady market, boost expectations</a></li>
<li><a href="https://www.yicaiglobal.com/news/china-turns-share-repurchase-relending-into-permanent-tool-to-stabilize-equity-market">China Turns Share Repurchase Relending Into Permanent Tool to ...</a></li>
<li><a href="https://global.chinadaily.com.cn/a/202611/03/WS6ae94d1fe4b06d4aa0566b65.html">China to expand share buyback support, cut relending rate to ...</a></li>

</ul>
</details>

**标签**: `#China markets`, `#Policy intervention`, `#Stock repurchase`, `#A-shares`, `#Market stabilization`

---

<a id="item-finance-news-4"></a>
### [美法官驳回 DRAM 价格操纵案撤诉请求](https://www.tomshardware.com/tech-industry/big-tech/judge-denies-motion-to-dismiss-dram-price-fixing-lawsuit-against-micron-samsung-and-sk-hynix-says-chipmakers-acted-like-hawks-flying-in-formation-finds-evidence-of-dram-collusion-plausible-after-500-percent-price-surge) ⭐️ 8.0/10

美国法官驳回了美光、三星和 SK 海力士关于 DRAM 价格操纵集体诉讼的撤诉动议，认定三家公司存在协同行为。

telegram · zaihuapd · 11月15日 16:39

**「背景」** 美国法官驳回了美光、三星和 SK 海力士关于 DRAM 价格操纵集体诉讼的撤诉动议，认为三家公司在限制 DRAM 供应和推动价格上涨方面存在协同行为，类似于“编队飞行”。此前，原告指控这些公司在一年内四次同步行动，导致 DRAM 价格最高上涨了 500%。

**「影响」** 此次诉讼可能对半导体行业及消费者产生重大影响，因涉案公司控制全球约 90%的 DRAM 市场，其被指控的协同行为可能导致内存价格上涨，损害小企业和普通消费者的利益。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DRAM_industry_price_fixing">DRAM industry price fixing - Wikipedia</a></li>
<li><a href="https://www.gate.com/news/detail/SK-HYNIX/samsung-sk-hynix-micron-face-dram-price-fixing-lawsuit-in-us-court-25656329">Samsung, SK Hynix, Micron Face DRAM Price-Fixing Lawsuit in ...</a></li>
<li><a href="https://www.trendforce.com/news/2026/11/16/news-u-s-judge-rejects-samsung-sk-hynix-microns-dram-price-fixing-dismissal-bid-citing-plausible-collusion/">[News] U.S. Judge Rejects Samsung, SK hynix, Micron’s DRAM ...</a></li>
<li><a href="https://www.trendforce.com/news/2026/07/08/news-new-dram-price-fixing-case-against-samsung-sk-hynix-and-micron-tests-whether-hbm-expansion-can-prove-collusion/">[News] New DRAM Price-Fixing Case Against Samsung, SK hynix ...</a></li>
<li><a href="https://www.geeky-gadgets.com/dram-price-fixing-lawsuit-2026/">What the 700% DRAM Price Spike Means for Your Next PC Build</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/samsung-sk-hynix-and-micron-sued-over-alleged-dram-price-fixing-amid-record-memory-costs">Samsung, SK hynix, and Micron sued over alleged DRAM price ...</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#antitrust`, `#legal`

---

<a id="item-finance-news-5"></a>
### [MicroStrategy 因被 MSCI 剔除指数后夜盘暴跌超 8%](https://news.google.com/rss/articles/CBMiYEFVX3lxTE5hMXVZWFAtd1FhUVU0UWY3LTBhbGFvS0ctY3Fmd0JOMG9WQ3RWdERHZlVfVkdha1pONjVzRnhWbHF5VTdCanMydHZmMFZKb3NaLUpDd3Z1OXEwbjZUWkdhWQ?oc=5) ⭐️ 7.0/10

MicroStrategy 因被 MSCI 剔除相关指数，美股夜盘跌幅超过 8%。

rss · Google News 财经 · 11月16日 10:04

**「背景」** 美国市场指数编制公司 MSCI 因 MicroStrategy（简称 Strategy）将其大部分资金投入比特币，而将其从美国和全球股票指数中移除。此举通常会导致被动型基金卖出该股票，从而影响其价格和流动性。

**「影响」** 由于被 MSCI 指数剔除，MicroStrategy（MSTR）股票在美股夜盘下跌超过 8%，可能影响其机构投资者基础和流动性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/index-removal-impact-strategy-stock-042405769.html?fr=sycsrp_catchall">How Index Removal Will Impact Strategy Stock Investors</a></li>
<li><a href="https://www.gate.com/blog/strategy-mstr-stock-impact-msci-index-removal">How Much Could Strategy (MSTR) Stock Be Affected if MSCI ...</a></li>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/why-msci-removed-mstr-indexes-031517367.html?fr=sycsrp_catchall">Why MSCI Removed MSTR From Its Indexes – And What It Means ...</a></li>
<li><a href="https://stocktwits.com/news-articles/markets/equity/why-msci-removed-mstr-from-its-indexes-and-what-it-means-for-bitcoin-stocks/cNGzKhOR99h">MSTR Stock Slips: MSCI Confirms Index Removal, Metaplanet ...</a></li>

</ul>
</details>

**标签**: `#index removal`, `#MSCI`, `#institutional investing`, `#after-hours trading`, `#market impact`

---

<a id="item-finance-news-6"></a>
### [英伟达黄仁勋离任后首份财报将揭晓](https://news.google.com/rss/articles/CBMiY0FVX3lxTE9TcTdOcXpfTVBKMG9qZHpuWlE0MS14aGxEMmRhYmV0azZleGVpNWpXWHJrNmFhMGM0emVhWGlRRC1DQTY0c0NhVVhKVDhmb0RuOEtOaFR2X1JmcHdkLWVudGxOWQ?oc=5) ⭐️ 7.0/10

英伟达在 CEO 黄仁勋离任后发布的首份财报即将公布，市场关注其 AI 需求和新领导层的表现。

rss · Google News 财经 · 11月16日 09:25

**「背景」** 英伟达创始人黄仁勋辞任首席执行官，由执行副总裁科莱特·克雷斯暂代职务。此前公司股价因 AI 需求强劲而表现良好，其最新季度营收达到 260 亿美元，同比增长三倍。

**「影响」** 英伟达在 CEO 黄仁勋离职后发布的首份财报将影响市场对其 AI 需求和新领导层的信心，进而可能影响其股价表现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nvidianews.nvidia.com/news/nvidia-announces-ceo-transition">NVIDIA Announces CEO Transition | NVIDIA Newsroom</a></li>
<li><a href="https://investor.nvidia.com/news/press-release-details/2026/NVIDIA-Announces-CEO-Transition/default.aspx">NVIDIA Corporation - NVIDIA Announces CEO Transition</a></li>
<li><a href="https://www.nytimes.com/2024/05/22/technology/nvidia-quarterly-earnings-results.html">Nvidia , Powered by A.I. Boom, Reports Soaring Revenue and Profits...</a></li>
<li><a href="https://www.gate.com/blog/nvidia-after-jensen-huang-impact-on-nvda-stock">NVIDIA After Jensen Huang: What Could It Mean for NVDA... | Gate Blog</a></li>
<li><a href="https://www.cnbc.com/2026/11/14/nvidia-ai-trade-data-centers-congress.html">Nvidia AI trade: Huang exit, Congress reshape Big Tech stock outlook</a></li>
<li><a href="https://www.youtube.com/watch?v=nfCpralKE9M">Nvidia &#x27;s CEO Resigned Overnight. Here Is What It Means for AI</a></li>

</ul>
</details>

**标签**: `#earnings`, `#corporate`, `#artificial-intelligence`

---

<a id="item-finance-news-7"></a>
### [中美俄领导人在深圳举行首次三方会晤](https://apnews.com/article/trump-xi-putin-summit-china-5fe92253ef38100bae913834a9b74d72) ⭐️ 7.0/10

中美俄三国领导人于 11 月 19 日深圳 APEC 峰会期间举行首次三方会晤，该会晤为场边非正式会晤。

telegram · zaihuapd · 11月16日 01:38

**「背景」** 亚太经合组织（APEC）峰会将于 11 月 18 日至 19 日在深圳举行，这是中美俄三国领导人首次专门举行三方会晤。媒体分析指出，此次会晤引发国际社会对所谓&quot;雅尔塔 2.0&quot;格局的讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bbc.com/zhongwen/articles/c6wy4373q50go/simp">APEC ... - BBC News 中 文</a></li>
<li><a href="https://www.dw.com/zh-hant/%E9%9B%85%E7%88%BE%E5%A1%9420%E4%B8%AD%E7%BE%8E%E4%BF%84%E5%8F%AF%E8%83%BD%E7%9A%84%E4%B8%89%E6%96%B9%E5%B3%B0%E6%9C%83%E5%BC%95%E7%99%BC%E6%93%94%E6%86%82/a-79929235">中 美 俄 可能的 深 圳 三 方 峰 会引发对「雅尔塔2.0」的担忧</a></li>

</ul>
</details>

**标签**: `# geopolitics`, `#international relations`, `#policy`

---