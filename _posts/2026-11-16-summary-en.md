---
layout: default
title: "Horizon Summary: 2026-11-16 (EN)"
date: 2026-11-16
lang: en
---

> From 237 items, 12 important content pieces were selected

---

**Technology News**
1. [Unbundling Multimodal Vision Encoding](#item-tech-news-1) ⭐️ 8.0/10
2. [Tool Visualizes LLM Token Generation and Quantization Differences](#item-tech-news-2) ⭐️ 8.0/10
3. [Qwen4-Max 上线，将开源小模型](#item-tech-news-3) ⭐️ 8.0/10
4. [Shanghai Unveils 3-Year AI+ Plan for Construction Industry](#item-tech-news-4) ⭐️ 7.0/10
5. [AI医疗诊断可靠性测试：四款大模型表现曝光](#item-tech-news-5) ⭐️ 7.0/10

**Financial News**
1. [China&\#x27;s Economic Slowdown Worsens in October](#item-finance-news-1) ⭐️ 9.0/10
2. [Lutnick Faces Scrutiny Over Nvidia Ties Amid Spy Scandal](#item-finance-news-2) ⭐️ 8.0/10
3. [59家A股公司获股票回购贷款总额超146亿元](#item-finance-news-3) ⭐️ 8.0/10
4. [美法官驳回DRAM价格操纵案撤诉动议](#item-finance-news-4) ⭐️ 8.0/10
5. [MicroStrategy被MSCI剔除指数后美股夜盘大跌超8%](#item-finance-news-5) ⭐️ 7.0/10
6. [NVIDIA&\#x27;s First Report After Huang&\#x27;s Departure Due](#item-finance-news-6) ⭐️ 7.0/10
7. [中美俄领导人在深圳举行首次三方会晤](#item-finance-news-7) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Unbundling Multimodal Vision Encoding](https://www.reddit.com/r/MachineLearning/comments/1xx1k2o/meta_fair_nyu_unbundling_multimodal_vision/) ⭐️ 8.0/10

An empirical study involving over 200 multimodal vision-language models found that encoder pretraining is optional, as models pretrained with contrastive, self-supervised, or captioning objectives perform similarly to those trained from scratch. However, vision-only parameters are essential—models without dedicated vision parameters trail significantly in performance and require 3x more compute to match encoder-based models. Additionally, placing the vision encoder before the LLM is not strictly necessary; in-fusion methods that integrate vision parameters into the LLM’s early layers achieve comparable performance with faster inference times.

reddit · r/MachineLearning · /u/trungh98 · Nov 15, 17:38

**「Multimodal Model Design Choices」** Vision-language models \(VLMs\) typically combine a vision encoder with a language model \(LLM\), often using a shared encoder pretraining phase. This setup raises questions about whether encoder pretraining, dedicated vision parameters, or encoder placement before the LLM are truly necessary for optimal performance. Previous models like Gemma 4 12B and Kimi K3 have experimented with dropping or reintroducing encoders, but lack of standardized comparison across models has left these trade-offs unresolved.

**「Practical Implications for Model Development」** Developers building multimodal models can optimize resource allocation by eliminating encoder pretraining without sacrificing performance, but should retain dedicated vision parameters. Furthermore, integrating vision components directly into the LLM during training may offer efficiency gains and improved inference speed, particularly in scenarios requiring fast token generation.

**「Community Discussion」** No community comments were available to summarize.

**Tags**: `#multimodal learning`, `#vision-language models`, `#model architecture`, `#empirical research`, `#machine learning systems`

---

<a id="item-tech-news-2"></a>
### [Tool Visualizes LLM Token Generation and Quantization Differences](https://www.reddit.com/r/LocalLLaMA/comments/1xx7qbf/i_have_created_a_tool_to_observe_what_happens/) ⭐️ 8.0/10

A new open-source tool called &\#x27;inside-llm&\#x27; has been released that allows users to visualize and compare the internal operations of large language models \(LLMs\) during text generation. The tool loads one or two GGUF models using llama.cpp and displays real-time token-level differences in a browser interface. It supports both lockstep and free modes for comparison, showing probability distributions, entropy, divergence metrics, and sampler chain traces. Users can also explore branching paths and view logit layers via 2D and 3D visualizations.

reddit · r/LocalLLaMA · /u/AlternativeEnough352 · Nov 15, 21:46

**「Background」** Quantization in large language models \(LLMs\) involves reducing the precision of model weights, typically from high-precision formats like F32 or BF16 to lower-precision formats such as 4-bit integers, to decrease model size and improve inference speed. Tools like llama.cpp facilitate this process through GGUF \(Ggml General Unified Format\) models, enabling various quantization techniques including Q4\_K\_M and Q8\_0. The tool &\#x27;inside-llm&\#x27; leverages llama.cpp to visualize and compare how different quantizations of the same model behave during text generation, offering insights into token-level differences and model decision-making processes.

**「Impact」** Developers and researchers working with LLMs will benefit from being able to visually inspect how different quantizations affect model outputs token-by-token, enabling better understanding of model behavior and aiding in optimization efforts.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ggml-org/llama.cpp/blob/master/tools/quantize/README.md">llama.cpp/tools/quantize/README.md at master - GitHub</a></li>
<li><a href="https://tech-insider.org/gguf-model-quantization-2026/">GGUF Quantization with llama.cpp: A Reproducible Workflow</a></li>
<li><a href="https://towardsdatascience.com/quantize-llama-models-with-ggml-and-llama-cpp-3612dfbcc172/">Quantize Llama models with GGUF and llama.cpp</a></li>

</ul>
</details>

**Tags**: `#artificial-intelligence`, `#machine-learning`, `#tools-and-libraries`

---

<a id="item-tech-news-3"></a>
### [Qwen4-Max 上线，将开源小模型](https://mp.weixin.qq.com/s/pJUt0xwD6H-WMyzd8TjZaQ) ⭐️ 8.0/10

阿里巴巴通义千问正式推出新一代旗舰大模型 Qwen4-Max，采用全新稀疏 MoE 架构，总参数达 2.4 万亿，支持视觉理解和百万 Token 长上下文处理。该模型在编程和长程任务执行方面表现优异，且成本显著降低，单个任务平均费用由 26.58 元降至 11.16 元，降幅近 58%。此外，团队表示后续将推出并开源更小的 Qwen4 系列模型。

telegram · zaihuapd · Nov 16, 02:52

**「背景」** Qwen4-Max 是阿里巴巴通义千问系列的新一代旗舰多模态模型，具备2.4万亿参数，支持视觉理解与百万级Token长上下文处理。它针对编程、办公及复杂代理任务进行了优化，并在API定价上进行了调整，单个任务平均费用降低近58%。该模型已于2026年11月15日上线，其定价为每百万输入tokens 1.5美元，输出tokens 4.5美元。后续将推出更小规模的Qwen4系列模型并开放模型权重。

**「Impact」** 开发者和企业用户在使用 Qwen4-Max 执行复杂任务时可获得更高的性价比，但需注意其推理速度仍低于部分竞品，如 GPT-6.1 和 Claude 系列模型，可能影响实时应用部署的选择。

**「Community Discussion」** 社区讨论中，有用户指出 Qwen4-Max 在推理效率上仍有提升空间，例如其每秒仅生成约 30 个 token，远低于其他高性能模型；也有评论提到其开源计划值得期待，但当前定价与性能尚需进一步验证。部分用户对 Anthropic 的封闭策略表达了批评意见。

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/models/qwen4-max">Qwen 4 Max - Intelligence, Performance &amp; Price... | Artificial Analysis</a></li>
<li><a href="https://www.qwencloud.com/models/qwen4-max?region=ap-southeast-1">Qwen 4 - Max - QwenCloud</a></li>
<li><a href="https://openrouter.ai/qwen/qwen4-max">Qwen 4 Max - API Pricing &amp; Providers | OpenRouter</a></li>
<li><a href="https://freakyjolly.com/qwen4-max-guide/">Qwen4-Max Is Out: $1.50 API Price, Benchmarks, Setup</a></li>
<li><a href="https://costgoat.com/pricing/qwen-api">Qwen API Pricing: Calculator &amp; Cost Guide (Nov 2026)</a></li>
<li><a href="https://docs.qwencloud.com/developer-guides/getting-started/pricing">Pricing - QwenCloud</a></li>

</ul>
</details>

**Tags**: `#AI模型`, `#大语言模型`, `#技术发布`, `#开源计划`, `#阿里巴巴`

---

<a id="item-tech-news-4"></a>
### [Shanghai Unveils 3-Year AI+ Plan for Construction Industry](https://news.google.com/rss/articles/CBMivAJBVV95cUxOUTdjYTFBZWVMdlRBeXB1ZkZDTnFndWhXQjNPdU5aU3ExUXdIa2NOUC1rZzg0MDVMR2JOelJuY3pvMlFCLXg1SF90VWt2emZ5Tk1ZZ192aFhxNlIxSk5GbldSMWVCeHpDZEdQU1lpbk9nQzE4Sk95OXdUc3o0ZjNuYVctWUNYdVZsVXp6d0hDWk1mbzRxc1JSNXRtckM5eG52eVo5LS1Dd0pZbkdTWVZ5OVBrUEI0UHpic01jQkcwazkxTk95LTlwY1E0SlBucGJfUUM5Q19EZTMwYWtFVWRJUENGeUJhZ1BtaV9EdGlMVy1qc180ZVlNN1FGcUY2Rk1ZOXpMSDFFT3RoU1JmMzN4UnA0c1hBbG5oZ09EV0VhbmhuVm5wNDBrYjRlV0lxbk1tbDAtMmFxaTJUSnBF?oc=5) ⭐️ 7.0/10

The Shanghai municipal government has released a three-year action plan \(2026–2028\) to promote the integration of artificial intelligence \(AI\) in the housing and urban-rural construction sector. The plan aims to drive AI adoption for smart city development and infrastructure management. It represents a significant policy commitment to advancing AI technologies in traditional construction industries, although specific technical implementations or milestones were not detailed in the announcement.

rss · Google News AI · Nov 16, 09:45

**「背景」** 上海市发布的《住房和城乡建设行业“人工智能+”行动计划（2026—2028年）》是该市在人工智能与城市建设融合方面的政策部署，旨在推动AI技术在建筑和基础设施管理中的应用。该计划反映了地方政府对智能建造和智慧城市发展的持续支持，与国家层面的“人工智能+”战略相呼应。类似地，广州市也发布了相关的鸿蒙智能城市建设行动计划（2026—2028年），显示了中国多个城市正在推进AI与城市治理、产业发展及民生服务的深度融合。

**「Impact」** Companies and engineers working in urban technology, smart city infrastructure, and construction sectors may see increased opportunities for AI-driven solutions, as the plan signals strong regulatory support and potential investment direction from the Shanghai government.

<details><summary>References</summary>
<ul>
<li><a href="https://www.smartcity.team/policies/digitaleconomy/guangzhou_harmonycity/">广州 市 鸿蒙 智 城 建 设 行 动 计 划 （ 2026 - 2028 ...</a></li>
<li><a href="https://www.workercn.cn/papers/grrb/2026/04/06/7/grrb202604067.pdf">grrb0720260406B</a></li>
<li><a href="https://paper.people.com.cn/rmrb/pc/attachement/202607/18/bde27cd0-3262-4cdf-b01f-dfcbc7bb635f.pdf">paper.people.com.cn/rmrb/pc/attachement/202607/18/bde27cd0-3262...</a></li>

</ul>
</details>

**Tags**: `#artificial-intelligence`, `#smart-cities`, `#government-policy`, `#construction`, `#china`

---

<a id="item-tech-news-5"></a>
### [AI医疗诊断可靠性测试：四款大模型表现曝光](https://news.google.com/rss/articles/CBMijwFBVV95cUxNamUxaTdJU3NzLU0xNV96RDFHRkh6SXpHeUgwUU5leG1tNHA4MTlhWERnRm8xREVZNW5QOW00S2tLeGs1T3FBVXZsTm96d1hiWTh1NXFlMldCUTNXMFRjUHFvY1hmVGR2X0lROTlNX3R0TS1UQlhBU2FDRWEzRHRPZkIzRExtZXlZcmV0ZDR1NA?oc=5) ⭐️ 7.0/10

一篇中文新闻报道测试了四款主流大语言模型在医疗诊断中的表现，结果揭示其在实际应用中存在显著局限性。该研究由一起因过度依赖AI诊断而延误治疗导致儿童发展为重症肺炎的真实案例引发。测试结果显示，尽管这些模型在某些任务上表现出色，但它们在复杂病情判断和紧急情况处理方面仍远未达到临床可信水平。

rss · Google News AI · Nov 16, 07:07

**「背景」** 在医疗诊断领域，大型语言模型（LLM）正被研究用于辅助或替代传统诊疗方式。已有研究如DiReCT基准测试系统和Synergizing Predictive Models with Large Language Models等，旨在提升AI在临床诊断中的准确性和推理能力。这些工作表明，尽管LLM具有处理复杂临床信息的潜力，但其诊断可靠性仍需与传统医学判断及预测模型结合验证。近期一项案例显示，过度依赖AI可能导致延误治疗，凸显了在实际应用中评估AI模型性能的重要性。

**「AI diagnostic reliability questioned in pediatric pneumonia cases」** A Chinese news article reported on a case where a child’s condition worsened due to reliance on AI rather than a doctor for pneumonia diagnosis, prompting tests of four major AI models. While AI has shown potential in early diagnosis and treatment guidance for pneumonia using chest X-rays, the real-world reliability and safety of these systems remain uncertain, especially in critical pediatric cases. The article highlights concerns about over-reliance on AI without sufficient clinical validation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/synergizing-predictive-models-large-language-medical-obiri-affram-gpahe">Synergizing Predictive Models with Large Language Models in...</a></li>
<li><a href="https://www.promptlayer.com/research-papers/direct-diagnostic-reasoning-for-clinical-notes-via-large-language-models">DiReCT: Diagnostic Reasoning for Clinical Notes via Large Language ...</a></li>
<li><a href="https://www.mdpi.com/2077-0383/9/1/248">Can Artificial Intelligence Improve the Management of Pneumonia</a></li>
<li><a href="https://journals.plos.org/digitalhealth/article?id=10.1371/journal.pdig.0000713">Detection of pneumonia in children through chest radiographs ...</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC13488239/">Determinants of delay in treatment-seeking for under-five ...</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#medical AI`, `#LLM evaluation`, `#AI reliability`, `#healthcare technology`

---

## Financial News

<a id="item-finance-news-1"></a>
### [China&\#x27;s Economic Slowdown Worsens in October](https://www.cnbc.com/2026/11/16/china-retail-sales-october-industrial-output-investment.html) ⭐️ 9.0/10

China&\#x27;s economic slowdown intensified in October as industrial output, retail sales, and investment all missed estimates. Industrial output grew 4.8% year-on-year, below the 5.3% estimate, while retail sales rose 0.4% versus a forecast 0.8% increase.

rss · CNBC Finance · Nov 16, 03:53

**「Background」** China&\#x27;s economy has been struggling with a prolonged property market downturn now in its fifth year, with multiple months of weak retail sales, industrial output and investment data this year raising pressure on Beijing to step up policy support. The October figures represent a continuation of the slowdown that began earlier in 2026, with key indicators consistently missing analyst expectations.

**「Impact on Global Trade and Investment」** China&\#x27;s deepening economic slowdown, with fixed-asset investments falling 8.1% year-on-year through the first ten months, threatens global supply chains and export-dependent economies, especially those reliant on AI-related goods.

<details><summary>References</summary>
<ul>
<li><a href="https://www.business-standard.com/world-news/china-s-economic-slowdown-revives-calls-for-stronger-stimulus-measures-126051801744_1.html">China &#x27; s economic slowdown revives calls for... - Business Standard</a></li>
<li><a href="https://www.theguardian.com/business/2026/aug/17/china-economy-slowdown-signs-extending">China ’ s economy showing signs that slowdown may... | The Guardian</a></li>
<li><a href="https://www.rand.org/pubs/commentary/2025/02/focus-on-the-new-economy-not-the-old-why-chinas-economic.html">Focus on the New Economy , Not the Old: Why China &#x27; s Economic ...</a></li>

</ul>
</details>

**Tags**: `#economic indicators`, `#trade policy`, `#export growth`, `#labor market`, `#AI economy`

---

<a id="item-finance-news-2"></a>
### [Lutnick Faces Scrutiny Over Nvidia Ties Amid Spy Scandal](https://www.cnbc.com/2026/11/13/howard-lutnick-nvidia-jensen-huang-china-cantor-fitzgerald.html) ⭐️ 8.0/10

Commerce Secretary Howard Lutnick faces questions over his sons&\#x27; firm Cantor Fitzgerald&\#x27;s ties to Nvidia amid a spy scandal involving chip smuggling to China. Cantor reduced its Nvidia holdings by nearly 50% between September 2025 and March 2026, while Lutnick resisted pressure to crack down on suspected chip smugglers.

rss · CNBC Finance · Nov 15, 19:58

**「Background」** Commerce Secretary Howard Lutnick faces scrutiny over his sons&\#x27; firm Cantor Fitzgerald&\#x27;s ties to Nvidia amid a spy scandal involving chip smuggling to China. The firm reduced its Nvidia holdings by nearly 50% between September 2025 and March 2026, while Lutnick resisted White House pressure to restrict Megaspeed, a Singapore-based company suspected of funneling Nvidia chips to China. Lutnick had received classified warnings about Nvidia CEO Jensen Huang’s ties to a suspected Chinese spy and was briefed on the risks before hosting Huang in New York.

**「Impact on Ethics Oversight and Public Trust」** The declining Nvidia holdings at Cantor Fitzgerald, a firm formerly led by Commerce Secretary Howard Lutnick and now run by his sons, raise questions about potential conflicts of interest amid ongoing national security concerns over chip exports to China.

<details><summary>References</summary>
<ul>
<li><a href="https://edition.cnn.com/2026/11/16/tech/nvidia-sex-spies-serious-problems">Lies, spies and sex are just one part of the Nvidia story.</a></li>
<li><a href="https://www.youtube.com/watch?v=L--M7Ok-y4M">NVIDIA SPY SCANDAL : GOP TURNS ON LUTNICK ? - YouTube</a></li>
<li><a href="https://www.nytimes.com/2026/11/13/opinion/jensen-huang-nvidia-howard-lutnick-commerce.html">Opinion | Howard Lutnick Has Got to Go - The New York Times</a></li>
<li><a href="https://gpusmith.com/articles/en/nvidia-gpu-export-restrictions">NVIDIA Export Controls 2026: H200, H20 &amp; China Rules</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/billions-worth-of-export-restricted-ai-accelerators-sold-to-china-report-details-how-chinese-firms-skirt-trumps-regulations">Investigative report details how export-restricted Nvidia AI ...</a></li>
<li><a href="https://nationalsecurity.news/2026-07-01-nvidia-ai-chip-china-face-export-restrictions.html">Nvidia AI Chip Sales to China Face New U.S. Export Restrictions</a></li>
<li><a href="https://en.wikipedia.org/wiki/Howard_Lutnick">Howard Lutnick - Wikipedia</a></li>
<li><a href="https://www.cnbc.com/2026/11/13/howard-lutnick-nvidia-jensen-huang-china-cantor-fitzgerald.html">Howard Lutnick &#x27;s sons &#x27; Nvidia ties amid Jensen Huang China spy...</a></li>
<li><a href="https://www.nytimes.com/2026/11/15/us/politics/trump-lutnick-ai-chips-nvidia-cantor-fitzgerald.html">Lutnick Pushed to Weaken Chip Rules That Overlap With His Family...</a></li>

</ul>
</details>

**Tags**: `#government`, `#conflict of interest`, `#national security`, `#technology`, `#regulation`

---

<a id="item-finance-news-3"></a>
### [59家A股公司获股票回购贷款总额超146亿元](https://news.google.com/rss/articles/CBMiZ0FVX3lxTE9TYzc3b0ZIeE1OWWYtRkxtalpCRV9SaUVWcFZNN0JTSElMcGJOcGpQTXJldVVMY01PcGp3aXVRSVEwaGZiaXNKN3d0SVB5UVRJczNlODFkeGs1WkNnY2ZKTW9GcUNQYk0?oc=5) ⭐️ 8.0/10

59家A股上市公司披露了用于股票回购的贷款总额上限超过146亿元人民币，单个公司最高额度达18亿元。

rss · Google News 财经 · Nov 16, 10:53

**「背景」** 中国央行和金融监管机构自2024年10月起推出股票回购增持再贷款政策，支持上市公司通过银行贷款进行股票回购和大股东增持。该政策已从阶段性措施转为长期制度安排，并将再贷款利率降至1%。

<details><summary>References</summary>
<ul>
<li><a href="https://www.globaltimes.cn/page/202611/1373487.shtml">CSRC rolls out policy mix to steady market, boost expectations</a></li>
<li><a href="https://www.yicaiglobal.com/news/china-turns-share-repurchase-relending-into-permanent-tool-to-stabilize-equity-market">China Turns Share Repurchase Relending Into Permanent Tool to ...</a></li>
<li><a href="https://global.chinadaily.com.cn/a/202611/03/WS6ae94d1fe4b06d4aa0566b65.html">China to expand share buyback support, cut relending rate to ...</a></li>

</ul>
</details>

**Tags**: `#China markets`, `#Policy intervention`, `#Stock repurchase`, `#A-shares`, `#Market stabilization`

---

<a id="item-finance-news-4"></a>
### [美法官驳回DRAM价格操纵案撤诉动议](https://www.tomshardware.com/tech-industry/big-tech/judge-denies-motion-to-dismiss-dram-price-fixing-lawsuit-against-micron-samsung-and-sk-hynix-says-chipmakers-acted-like-hawks-flying-in-formation-finds-evidence-of-dram-collusion-plausible-after-500-percent-price-surge) ⭐️ 8.0/10

美国法官驳回美光、三星、SK海力士关于DRAM价格操纵集体诉讼的撤诉请求，认定三家公司在一年内四次同步行动限制DRAM供应，导致价格最高上涨500%，存在协同行为的合理怀疑。

telegram · zaihuapd · Nov 15, 16:39

**「background」** A U.S. judge denied a motion to dismiss a class-action lawsuit accusing Samsung, SK Hynix, and Micron of colluding to fix DRAM prices, following a 500% price surge. The judge found evidence of coordinated behavior among the companies, likening their actions to &\#x27;flying in formation.&\#x27;

**「Affected parties face legal and financial risks」** The ruling means that the DRAM price-fixing lawsuit against Micron, Samsung, and SK Hynix will proceed, potentially exposing these major semiconductor manufacturers to significant financial liability and reputational damage. The case stems from allegations that they coordinated supply restrictions to raise prices by up to 500%, harming consumers and small businesses.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gate.com/news/detail/SK-HYNIX/samsung-sk-hynix-micron-face-dram-price-fixing-lawsuit-in-us-court-25656329">Samsung, SK Hynix, Micron Face DRAM Price-Fixing Lawsuit in ...</a></li>
<li><a href="https://www.trendforce.com/news/2026/11/16/news-u-s-judge-rejects-samsung-sk-hynix-microns-dram-price-fixing-dismissal-bid-citing-plausible-collusion/">[News] U.S. Judge Rejects Samsung, SK hynix, Micron’s DRAM ...</a></li>
<li><a href="https://www.trendforce.com/news/2026/07/08/news-new-dram-price-fixing-case-against-samsung-sk-hynix-and-micron-tests-whether-hbm-expansion-can-prove-collusion/">[News] New DRAM Price-Fixing Case Against Samsung, SK hynix ...</a></li>
<li><a href="https://www.geeky-gadgets.com/dram-price-fixing-lawsuit-2026/">What the 700% DRAM Price Spike Means for Your Next PC Build</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/samsung-sk-hynix-and-micron-sued-over-alleged-dram-price-fixing-amid-record-memory-costs">Samsung, SK hynix, and Micron sued over alleged DRAM price ...</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#antitrust`, `#legal`

---

<a id="item-finance-news-5"></a>
### [MicroStrategy被MSCI剔除指数后美股夜盘大跌超8%](https://news.google.com/rss/articles/CBMiYEFVX3lxTE5hMXVZWFAtd1FhUVU0UWY3LTBhbGFvS0ctY3Fmd0JOMG9WQ3RWdERHZlVfVkdha1pONjVzRnhWbHF5VTdCanMydHZmMFZKb3NaLUpDd3Z1OXEwbjZUWkdhWQ?oc=5) ⭐️ 7.0/10

MicroStrategy was removed from MSCI indices, causing its after-hours stock price to drop by over 8%. This decision impacts the company&\#x27;s inclusion in major equity benchmarks.

rss · Google News 财经 · Nov 16, 10:04

**「Background」** MSCI removed Strategy from its USA and global equity indexes, classifying it as a non-operating company due to its large Bitcoin holdings, which triggers forced selling by passive index funds.

**「Impact on Investors」** MicroStrategy \(MSTR\) stock fell over 8% in after-hours trading after MSCI confirmed its removal from major global equity indexes, which may force index funds to sell shares and reduce liquidity for investors.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/index-removal-impact-strategy-stock-042405769.html?fr=sycsrp_catchall">How Index Removal Will Impact Strategy Stock Investors</a></li>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/why-msci-removed-mstr-indexes-031517367.html?fr=sycsrp_catchall">Why MSCI Removed MSTR From Its Indexes – And What It Means ...</a></li>
<li><a href="https://stocktwits.com/news-articles/markets/equity/why-msci-removed-mstr-from-its-indexes-and-what-it-means-for-bitcoin-stocks/cNGzKhOR99h">MSTR Stock Slips: MSCI Confirms Index Removal, Metaplanet ...</a></li>

</ul>
</details>

**Tags**: `#index removal`, `#MSCI`, `#institutional investing`, `#after-hours trading`, `#market impact`

---

<a id="item-finance-news-6"></a>
### [NVIDIA&\#x27;s First Report After Huang&\#x27;s Departure Due](https://news.google.com/rss/articles/CBMiY0FVX3lxTE9TcTdOcXpfTVBKMG9qZHpuWlE0MS14aGxEMmRhYmV0azZleGVpNWpXWHJrNmFhMGM0emVhWGlRRC1DQTY0c0NhVVhKVDhmb0RuOEtOaFR2X1JmcHdkLWVudGxOWQ?oc=5) ⭐️ 7.0/10

NVIDIA is set to release its first financial report following CEO Jensen Huang&\#x27;s departure, with analysts focusing on AI demand and leadership transition.

rss · Google News 财经 · Nov 16, 09:25

**「background」** NVIDIA&\#x27;s CEO Jensen Huang resigned effective immediately, prompting a leadership transition with Colette Kress named interim CEO and Harvey C. Jones appointed chair of the board. This follows the company&\#x27;s strong financial performance, including a $26 billion revenue surge in its previous quarter.

**「Impact」** Investors and market analysts will closely watch NVIDIA&\#x27;s upcoming earnings report—the first since Jensen Huang&\#x27;s departure—as interim CEO Colette Kress faces pressure to reassure the market on AI demand and the company&\#x27;s strategic direction under new leadership.

<details><summary>References</summary>
<ul>
<li><a href="https://nvidianews.nvidia.com/news/nvidia-announces-ceo-transition">NVIDIA Announces CEO Transition | NVIDIA Newsroom</a></li>
<li><a href="https://investor.nvidia.com/news/press-release-details/2026/NVIDIA-Announces-CEO-Transition/default.aspx">NVIDIA Corporation - NVIDIA Announces CEO Transition</a></li>
<li><a href="https://www.nytimes.com/2024/05/22/technology/nvidia-quarterly-earnings-results.html">Nvidia , Powered by A.I. Boom, Reports Soaring Revenue and Profits...</a></li>
<li><a href="https://www.cnbc.com/2026/11/14/nvidia-ai-trade-data-centers-congress.html">Nvidia AI trade: Huang exit, Congress reshape Big Tech stock outlook</a></li>

</ul>
</details>

**Tags**: `#earnings`, `#corporate`, `#artificial-intelligence`

---

<a id="item-finance-news-7"></a>
### [中美俄领导人在深圳举行首次三方会晤](https://apnews.com/article/trump-xi-putin-summit-china-5fe92253ef38100bae913834a9b74d72) ⭐️ 7.0/10

中美俄三国领导人于11月19日在北京APEC峰会期间举行首次三方会晤，该会晤为非正式场合。

telegram · zaihuapd · Nov 16, 01:38

**「背景」** 中国外交部宣布，中美俄三国领导人计划于11月19日在深圳APEC峰会期间举行首次三方会晤，该会晤为非正式场合，不属APEC正式议程。此次会晤被视为三国领导人的首次专门会面，引起外界对地缘政治格局的关注。

<details><summary>References</summary>
<ul>
<li><a href="https://www.bbc.com/zhongwen/articles/c6wy4373q50go/simp">APEC ... - BBC News 中 文</a></li>
<li><a href="https://www.dw.com/zh-hant/%E9%9B%85%E7%88%BE%E5%A1%9420%E4%B8%AD%E7%BE%8E%E4%BF%84%E5%8F%AF%E8%83%BD%E7%9A%84%E4%B8%89%E6%96%B9%E5%B3%B0%E6%9C%83%E5%BC%95%E7%99%BC%E6%93%94%E6%86%82/a-79929235">中 美 俄 可能的 深 圳 三 方 峰 會引發對「雅爾塔2.0」的擔憂</a></li>
<li><a href="https://www.youtube.com/watch?v=wu2u1bKKI7Y">官宣！ 中 方 宣佈 中 美 俄 19... - YouTube</a></li>

</ul>
</details>

**Tags**: `# geopolitics`, `#international relations`, `#policy`

---