---
layout: default
title: "Horizon Summary: 2026-11-14 (EN)"
date: 2026-11-14
lang: en
---

> From 201 items, 12 important content pieces were selected

---

**Technology News**
1. [GGML v1.0.0 released as production-ready CPU-optimized tensor library](#item-tech-news-1) ⭐️ 8.0/10
2. [Nvidia allegedly funded AI startups to buy its GPUs, engineering artificial scarcity](#item-tech-news-2) ⭐️ 8.0/10
3. [Granzyme K identified as inflammation-independent driver of tissue aging](#item-tech-news-3) ⭐️ 8.0/10
4. [1T-parameter MoE trained on TorchTitan across 384 GH200 GPUs](#item-tech-news-4) ⭐️ 8.0/10
5. [Four frontier LLMs score 97.8–100 on 7-part materials science research benchmark](#item-tech-news-5) ⭐️ 8.0/10
6. [Zibian Robot&\#x27;s self-developed general embodied intelligence large model completes Chinese regulatory filing](#item-tech-news-6) ⭐️ 7.0/10
7. [EU holds first AI summit of national leaders focusing on competitiveness and regulation](#item-tech-news-7) ⭐️ 7.0/10

**Financial News**
1. [Goolsbee: Fed Has &\#x27;Definitely Got Work to Do&\#x27; on Inflation](#item-finance-news-1) ⭐️ 7.0/10
2. [China&\#x27;s October Financial Data: Fund Flows and Structural Shifts](#item-finance-news-2) ⭐️ 7.0/10
3. [Fed Warns AI Hype Is Inflating US Stock Valuations, Cyber Risks Rise](#item-finance-news-3) ⭐️ 7.0/10
4. [China Announces 22 Measures to Advance National Conservation Strategy](#item-finance-news-4) ⭐️ 7.0/10
5. [China Corporate Loan Rates Fall Below 3% for First Time](#item-finance-news-5) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [GGML v1.0.0 released as production-ready CPU-optimized tensor library](https://github.com/ggml-org/ggml/releases/tag/v1.0.0) ⭐️ 8.0/10

GGML v1.0.0 is a stable, production-ready release of the open-source ggml tensor library, optimized for high-performance CPU inference of large language models on diverse hardware including low-end x86, ARM, and Vulkan-capable GPUs. It ships with improved quantization support, enhanced memory management, and verified compatibility across llama.cpp, whisper.cpp, and other downstream tools. The release is available now on GitHub under the MIT license and requires no CUDA or vendor-specific drivers.

hackernews · cobychapple · Nov 14, 02:28 · [Discussion](https://news.ycombinator.com/item?id=50493062)

**「Background」** GGML is an open-source, CPU-optimized tensor library originally developed to support efficient local inference of large language models without GPU dependencies. It underpins widely used tools like llama.cpp and serves as a lightweight, portable alternative to CUDA-based frameworks such as PyTorch or TensorFlow.

**「Stable C API enables long-term integration for downstream projects」** The v1.0.0 release commits to semantic versioning for the public C API of libggml, meaning future breaking changes will require a major-version bump—transforming ggml from a fast-moving dependency into a managed compatibility contract for applications like llama.cpp and other embedded or production tools that link against it directly.

**「Community discussion」** Users report consistent real-world performance gains—e.g., one commenter measured a runtime reduction from 4:22 to 3:59 on a 50K-token prompt after upgrading—and praise GGML’s ability to enable usable LLM inference on constrained hardware like AMD GPUs with Vulkan-only support. Several commenters explicitly compare GGML and llama.cpp to foundational, community-driven infrastructure like Linux, emphasizing their role in democratizing local AI.

<details><summary>References</summary>
<ul>
<li><a href="https://grafy.ai/news/llama-cpp-and-ggml-hit-1-0-0-with-a-stable-api-promise">llama.cpp and ggml hit 1.0.0 — Grafy News</a></li>
<li><a href="https://dev.to/delimitter/llamacpp-and-ggml-ship-v100-semantic-versioning-comes-to-the-local-ai-stack-1ag4">llama.cpp and ggml ship v1.0.0 — semantic versioning comes to ...</a></li>

</ul>
</details>

**Tags**: `#AI systems`, `#open source`, `#machine learning`, `#software engineering`, `#hardware acceleration`

---

<a id="item-tech-news-2"></a>
### [Nvidia allegedly funded AI startups to buy its GPUs, engineering artificial scarcity](https://www.techpowerup.com/354814/nvidia-allegedly-engineered-scarcity-by-funding-ai-startups-to-buy-its-gpus) ⭐️ 8.0/10

Reports allege that Nvidia strategically funded AI startups—through direct investment or venture arms—to purchase its GPUs, thereby sustaining artificial demand and reinforcing perceived scarcity in the AI chip market. The claim, originally reported by the Wall Street Journal and cited by multiple secondary outlets, suggests this practice helped maintain pricing power and revenue recognition timing, particularly amid concerns about oversupply from TSMC. No official confirmation or denial from Nvidia is reported, and the allegations remain unproven; the reports do not specify dollar amounts, startup names, funding vehicles, or dates of such arrangements.

hackernews · speckx · Nov 14, 02:52 · [Discussion](https://news.ycombinator.com/item?id=50493251)

**「Circular financing allegations against Nvidia」** For over a year, reports—including from The Guardian in December 2025—have alleged that Nvidia engaged in circular financing arrangements, where it invested in AI infrastructure startups that then purchased its GPUs, effectively recycling capital to inflate demand signals and sustain pricing power. These claims resurfaced in a November 2026 Wall Street Journal report cited by multiple outlets, now tied to leadership changes following Jensen Huang’s resignation and Colette Kress’s appointment as interim CEO.

**「Impact」** Nvidia&\#x27;s disclosed 9.3% equity stake in Nebius—coupled with GPU-backed debt financing and first-access chip agreements—enables Nvidia to recognize revenue upfront while constraining supply of its latest GPUs for competitors&\#x27; cloud infrastructure providers, directly affecting AI cloud operators&\#x27; hardware procurement options and cost structures.

**「Community discussion」** Commenters reference prior patterns—including &\#x27;circular financing&\#x27; reported by The Guardian in December 2025—and draw parallels to Nvidia’s historical business practices like GameWorks and G-Sync, suggesting skepticism toward the company’s market conduct. One commenter notes that Nvidia’s partnerships with AI infrastructure firms \(e.g., Nebius\) involve equity stakes, first access to chips, and upfront revenue recognition, framing such arrangements as rational business strategy rather than inherently anti-competitive.

<details><summary>References</summary>
<ul>
<li><a href="https://www.explainx.ai/blog/nvidia-engineered-gpu-scarcity-startup-funding-wsj-claimed-vs-verified-2026">WSJ: Nvidia Funded Startups to Buy GPUs — What&#x27;s Verified ...</a></li>
<li><a href="https://www.wsj.com/livecoverage/stock-market-today-dow-sp-500-nasdaq-08-27-2026/card/XdHmb8VRy4xMH42k7Z2M">Nvidia Pushes Back on Circular Financing Criticism</a></li>
<li><a href="https://www.techpowerup.com/354814/nvidia-allegedly-engineered-scarcity-by-funding-ai-startups-to-buy-its-gpus">NVIDIA Allegedly Engineered Scarcity By Funding AI Startups ...</a></li>
<li><a href="https://investor.nvidia.com/news/press-release-details/2026/NVIDIA-and-Nebius-Partner-to-Scale-Full-Stack-AI-Cloud/default.aspx">NVIDIA Corporation - NVIDIA and Nebius Partner to Scale Full ...</a></li>
<li><a href="https://noqta.tn/en/news/nvidia-9-3-percent-stake-nebius-gpu-backed-debt-2026">Nvidia Discloses 9.3% Stake in Nebius as Neoclouds Turn GPUs ...</a></li>
<li><a href="https://cryptobriefing.com/nebius-stock-surges-nvidia-9-percent-stake/">Nebius stock surges after Nvidia discloses 9% stake</a></li>

</ul>
</details>

**Tags**: `#AI-hardware`, `#market-dynamics`, `#NVIDIA`, `#cloud-infrastructure`, `#antitrust`

---

<a id="item-tech-news-3"></a>
### [Granzyme K identified as inflammation-independent driver of tissue aging](https://www.nature.com/articles/d41586-026-03638-3) ⭐️ 8.0/10

A study published in Immunity identifies Granzyme K \(GzmK\) as a protein that drives organ aging without triggering inflammation or accelerating immune aging. In mouse models, GzmK deficiency markedly attenuated age-related decline in multiple organs—including liver, kidney, and heart—despite persistent immune aging phenotypes such as thymic involution and T-cell exhaustion. The finding decouples tissue aging from systemic inflammaging and immune senescence, establishing GzmK as a tissue-specific, non-inflammatory driver of organismal aging. The work is based on loss-of-function experiments and is currently limited to preclinical models.

hackernews · gumby · Nov 13, 19:25 · [Discussion](https://news.ycombinator.com/item?id=50488470)

**「Granzyme K and its established roles」** Granzyme K \(GzmK\) is a serine protease encoded by the GZMK gene on human chromosome 5, part of a family of immune-associated proteases traditionally studied for roles in cytotoxic lymphocyte function and apoptosis. Prior work had linked elevated GzmK expression to immune aging trajectories—specifically, a shift toward GzmK-expressing cells in healthy aging, in contrast to GzmB-dominant profiles associated with pathological aging—but had not established a direct, inflammation-independent role in tissue aging.

**「Impact」** This discovery provides a new mechanistic target for interventions aimed specifically at delaying tissue degeneration without modulating immune function—potentially avoiding trade-offs associated with broad anti-inflammatory or immunomodulatory therapies.

**「Community discussion」** Commenters highlight the conceptual significance of uncoupling tissue and immune aging, with one noting the paper&\#x27;s key nuance—that GzmK deficiency attenuates organ aging &\#x27;despite persistent immune aging phenotypes&\#x27;—while another expresses skepticism about evolutionary rationale for retaining such a protein.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GZMK">GZMK - Wikipedia</a></li>
<li><a href="https://medicalxpress.com/news/2026-10-immune-cell-uncovers-individual-aging.html">Immune cell map uncovers how individual aging trajectories diverge</a></li>
<li><a href="https://www.news-medical.net/news/20261112/Blocking-Granzyme-K-protein-may-protect-organs-from-age-related-damage.aspx">Blocking Granzyme K protein may protect organs from age-related...</a></li>

</ul>
</details>

**Tags**: `#aging`, `#immunology`, `#molecular-biology`, `#longevity`, `#cell-biology`

---

<a id="item-tech-news-4"></a>
### [1T-parameter MoE trained on TorchTitan across 384 GH200 GPUs](https://www.reddit.com/r/MachineLearning/comments/1xvce5h/scaling_to_1t_moe_on_torchtitan_p/) ⭐️ 8.0/10

Engineers successfully trained a ~1-trillion-parameter Mixture of Experts \(MoE\) model on TorchTitan using 384 NVIDIA GH200 GPUs, achieving ~1,300 tokens/s per GPU — a 14× improvement over their initial baseline. The implementation used FSDP \(Fully Sharded Data Parallelism\) with 384-way sharding plus 4-way Expert Parallelism \(EP\) confined within nodes, avoiding Pipeline Parallelism due to its debugging and iteration overhead. Key technical enablers included FlexShard for expert-local Newton-Schulz optimization, FP8 expert all-gather with blockwise scaling, node-local resharding of dense weights over NVLink, and a fix to run Muon optimizer steps on GPU even when parameters are offloaded to Grace CPU memory. The system ran on the JUPITER supercomputer with user-level access and no root privileges.

reddit · r/MachineLearning · /u/f14-bertolotti · Nov 13, 16:28

**「What is TorchTitan?」** TorchTitan is an open-source, PyTorch-native distributed training system designed to unify and advance state-of-the-art parallelism techniques—including FSDP, pipeline parallelism, and expert parallelism—for large language models. It serves as a modular, extensible proof of concept for frontier-scale LLM training, emphasizing readability and ease of extension over abstraction-heavy frameworks.

**「Practical consequence」** This work demonstrates that frontier-scale MoE training is feasible on commodity Hopper-generation infrastructure without custom kernels or privileged access — enabling academic and public-sector teams to replicate trillion-parameter training using publicly documented, open PyTorch/TorchTitan tooling and standard InfiniBand interconnects, provided they adopt the described communication-avoiding sharding, offloading, and precision strategies.

<details><summary>References</summary>
<ul>
<li><a href="https://discuss.pytorch.org/t/distributed-w-torchtitan-training-with-zero-bubble-pipeline-parallelism/214420">[Distributed w/ TorchTitan ] Training with... - PyTorch Forums</a></li>
<li><a href="https://arxiv.org/pdf/2410.06511">TorchTitan : One-stop PyTorch native solution for production ready...</a></li>

</ul>
</details>

**Tags**: `#large-language-models`, `#distributed-training`, `#mixture-of-experts`, `#pytorch`, `#gpu-scaling`

---

<a id="item-tech-news-5"></a>
### [Four frontier LLMs score 97.8–100 on 7-part materials science research benchmark](https://www.reddit.com/r/MachineLearning/comments/1xvgf6h/four_frontier_models_scored_978100_on_a_7part/) ⭐️ 8.0/10

A domain-expert researcher in graphene and 2D materials designed and administered a synthetic, seven-part benchmark covering real-world materials science research tasks—including tensile data reduction, CIF density function generation, back-of-envelope physics calculations, manuscript critique with planted errors, false-premise detection, experimental design, and constrained abstract writing. Four frontier models—Gemini 4 Carbon, Gemini 4 Hydrogen \(Antigravity\), Claude Opus 5.5, and Claude Fable 5.2—achieved mean scores of 100.0, 99.7, 99.3, and 98.5 respectively across three fresh runs each, with all 12 runs scoring between 97.8 and 100; web search and code execution were enabled, and all models ran at &\#x27;High&\#x27; \(not max\) settings. Scoring was fully automated using computed answer keys on synthetic data, and the only points lost were for minor formatting issues—not technical failures. The test explicitly excluded long-horizon, open-ended workflows, which the author identifies as the remaining capability gap.

reddit · r/MachineLearning · /u/v\_aravind · Nov 13, 18:58

**「Background」** This benchmark builds on recent efforts to move beyond narrow, short-horizon agent evaluations—such as single-step tool use or API call accuracy—toward multi-step, domain-grounded scientific reasoning. It aligns methodologically with prior domain-specific benchmarks like FrontierScience and PaperBench, which emphasize realistic research procedures and expert-validated ground truth, but distinguishes itself through full automation, synthetic data control, and explicit coverage of lab SOP compliance, physical intuition, and scientific skepticism.

**「Impact」** The benchmark provides a reproducible, automated, and domain-rigorous evaluation standard that reveals near-saturation on bounded, procedure-driven scientific tasks—suggesting developers and evaluators should shift focus toward long-horizon, budget-constrained, and surprise-resilient agent behaviors, such as those planned in the author’s upcoming simulated-lab campaign.

**Tags**: `#AI evaluation`, `#scientific computing`, `#LLM benchmarks`, `#materials science`, `#agent reasoning`

---

<a id="item-tech-news-6"></a>
### [Zibian Robot&\#x27;s self-developed general embodied intelligence large model completes Chinese regulatory filing](https://news.google.com/rss/articles/CBMib0FVX3lxTE5SSUg0VllsNXRCRlJGRmZTZzJUVW92aEppWllJSGhYWDZzZmpjT2N2d1E2UmtYYUdZZGt6WkEwLXpkYjFZSHFaOHBET0lRb1JETU1qZlJ5aW05c1pxcUxZNEJ3V1BZV2p1bjZkV0oyQQ?oc=5) ⭐️ 7.0/10

Zibian Robot’s self-developed general embodied intelligence large model has completed official regulatory filing with China’s Ministry of Science and Technology, as confirmed by the China Securities Journal \(zqrb.cn\). The filing signifies formal recognition under China’s AI governance framework for large models, which requires safety assessments and registration before public deployment. No technical specifications—such as model name, architecture, training data, or performance metrics—were disclosed in the source. The filing applies to the model itself, not a specific robot product or commercial service, and no release date, availability timeline, or compatibility details were provided.

rss · Google News AI · Nov 14, 03:49

**「Background」** Embodied intelligence refers to AI systems that perceive, reason, and act in physical environments—often through robotic platforms—integrating vision, language, planning, and motor control. In China, such models must undergo mandatory filing under the Interim Measures for the Management of Generative AI Services \(effective August 2023\), which requires providers to submit technical details, safety assessments, and content moderation plans before public deployment.

**Tags**: `#embodied AI`, `#large language models`, `#AI regulation`, `#robotics`, `#China tech policy`

---

<a id="item-tech-news-7"></a>
### [EU holds first AI summit of national leaders focusing on competitiveness and regulation](https://news.google.com/rss/articles/CBMiSEFVX3lxTE9WUjhfVGFNX0hlOUZyXzBicENMYjZvRnI5Y3Q5UVNzR2d2QVd3WFBwTW1IM0xWWlhOaGY4cHZ2eldSMFNUSFhUQw?oc=5) ⭐️ 7.0/10

The European Union held its first summit dedicated exclusively to artificial intelligence, convening heads of state to address the dual priorities of strengthening Europe&\#x27;s industrial competitiveness in AI and establishing robust risk-based regulatory frameworks. The summit took place on November 13, 2026, and marked the EU’s highest-level coordinated political engagement on AI to date. No binding agreements, new legislation, or technical standards were announced during the event; the outcome was a political declaration reaffirming commitment to the AI Act and strategic investment in AI infrastructure and talent. The summit applied to all EU member states and associated candidate countries participating at the leader level.

rss · Google News AI · Nov 13, 17:34

**「EU&\#x27;s first AI summit of national leaders」** The European Union had not previously convened a dedicated summit of heads of state focused solely on artificial intelligence; this Dublin meeting marks the bloc’s inaugural such gathering. Earlier EU AI policy milestones include the 2024 adoption of the AI Act—the world’s first comprehensive horizontal AI regulation—but that legislation was negotiated at the technical and ministerial level, not by national leaders in a standalone AI summit format.

**Tags**: `#AI policy`, `#regulation`, `#EU`, `#technology strategy`, `#AI governance`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Goolsbee: Fed Has &\#x27;Definitely Got Work to Do&\#x27; on Inflation](https://www.cnbc.com/2026/11/13/chicago-feds-goolsbee-says-central-bank-has-definitely-got-work-to-do-on-inflation.html) ⭐️ 7.0/10

Chicago Fed President Austan Goolsbee said the Federal Reserve &\#x27;has definitely got work to do&\#x27; on inflation after October’s 6.5% annual PPI — the highest since November 2022 — and hotter-than-expected CPI, underscoring that progress toward the 2% target has stalled.

rss · CNBC Finance · Nov 13, 14:22

**「Background」** Goolsbee, a non-voting Fed official in 2026 but set to vote in 2027, cited both persistent supply-driven inflation and new demand-driven pressure from AI data center construction as factors pushing prices up.

**「Impact」** Markets now fully price in a 25 bps rate hike at the December 8–9 FOMC meeting, with over 10% odds of a 50 bps increase, tightening financial conditions for borrowers and investors.

**Tags**: `#monetary\_policy`, `#inflation\_data`, `#fed\_officials`

---

<a id="item-finance-news-2"></a>
### [China&\#x27;s October Financial Data: Fund Flows and Structural Shifts](https://news.google.com/rss/articles/CBMiggFBVV95cUxQM1VIWjlvN1pKWGM4cTdXYjBXVkJzd2RkcFNtTFR3eE04a194c1c1bFVKaEVEQUpYNFJJektGWDk4UEszcUsyOS1JZDdkNS1Nc0Y2aUZUOGVtYzZwSGJEd1FIanNaQTQ1M2F0NGwtZXplVXI1MFBRNmZsSkdOZkdfbGFR?oc=5) ⭐️ 7.0/10

The People&\#x27;s Bank of China released October 2026 financial data showing M2 money supply grew 8.3% year-on-year, while new RMB loans totaled 738 billion yuan — down 12% from October 2025 and the lowest for that month since 2022.

rss · Google News 财经 · Nov 13, 14:47

**「Background」** China&\#x27;s People&\#x27;s Bank of China releases monthly financial data—including M2 money supply, new yuan loans, and aggregate financing to the real economy—to track credit conditions and policy effectiveness.

**Tags**: `#monetary\_policy`, `#china\_economy`, `#credit\_data`

---

<a id="item-finance-news-3"></a>
### [Fed Warns AI Hype Is Inflating US Stock Valuations, Cyber Risks Rise](https://news.google.com/rss/articles/CBMiU0FVX3lxTE5HZkVCM1UtaFZzQ2dETVRvWnhMNzJudm9RemZZRGdoMFJ4alduXzJ6NXlfaW1ZQmo0SUdqOU5INnhLRHRYNnFnSjAtZ3ZYN0FuV0Mw?oc=5) ⭐️ 7.0/10

The Federal Reserve’s Financial Stability Report states that investor enthusiasm for AI is contributing to elevated U.S. equity valuations and identifies intensifying cybersecurity threats to financial infrastructure.

rss · Google News 财经 · Nov 13, 21:37

**「Background」** The Federal Reserve publishes a semiannual Financial Stability Report to assess vulnerabilities in the U.S. financial system; the latest edition \(2026\) explicitly adds AI-related valuation pressures and cybersecurity threats to its official risk framework.

<details><summary>References</summary>
<ul>
<li><a href="https://www.federalreserve.gov/">The Federal Reserve Board of Governors in Washington DC.</a></li>
<li><a href="https://www.linkedin.com/posts/kristalina-georgieva_the-latest-global-financial-stability-report-activity-7449894400131756032-6i3k">The latest Global Financial Stability Report finds that the war in the...</a></li>

</ul>
</details>

**Tags**: `#monetary\_policy`, `#market\_valuation`, `#cybersecurity\_risk`

---

<a id="item-finance-news-4"></a>
### [China Announces 22 Measures to Advance National Conservation Strategy](https://news.google.com/rss/articles/CBMibkFVX3lxTE1UaGs5VGlsaDg2Z2RuY1FKVEhobzZfTUFsem9TTGRJYzVJalFFZ1A0UklSTUMwV0toR0dST1ZaQzJyVUotbk1MbTVFblpFN0tHMjlNckZneDdRYmJlR3BFdFhBdTZLTVloVGNCNkJB?oc=5) ⭐️ 7.0/10

China’s State Council announced 22 policy measures to implement a national &\#x27;comprehensive conservation strategy&\#x27;, targeting reductions in energy and resource consumption across industry, infrastructure, and public services.

rss · Google News 财经 · Nov 13, 20:47

**「Background」** The 22 measures are part of a newly issued national action plan to advance comprehensive resource conservation, announced by China on November 4–5, 2026, as a strategic priority to support high-quality development and carbon reduction.

<details><summary>References</summary>
<ul>
<li><a href="https://english.news.cn/20261105/9d0b57f1e9c244cb8a574d7a68571254/c.html">China issues plan to advance comprehensive resource conservation</a></li>
<li><a href="https://english.news.cn/20261105/6c32ace61ab54691949fa33a80dd8673/c.html">China issues plan to advance comprehensive resource conservation</a></li>

</ul>
</details>

**Tags**: `#Chinese policy`, `#energy efficiency`, `#industrial policy`

---

<a id="item-finance-news-5"></a>
### [China Corporate Loan Rates Fall Below 3% for First Time](https://news.google.com/rss/articles/CBMickFVX3lxTE9DZG95VDdQTWJCcDJwbmtVVFFlLU5PUzNJVzl3VXlmbEtLWHNMQV9VLWZuYUo4SWM1M19KSjdiNnJraWs3TC1wamRQNTBCaDQtejVWLXByQl8waWRSWUJjdklaYjVIOGx4RVExaXRRVVNpQQ?oc=5) ⭐️ 7.0/10

China’s corporate loan interest rate fell below 3% for the first time, reaching a new low — a figure reported as an actual result by Mobile Sina Net.

rss · Google News 财经 · Nov 14, 01:48

**「Background」** The People&\#x27;s Bank of China reported that the weighted average interest rate on newly issued corporate loans fell to just below 3.0% in August 2026, about 0.2 percentage point lower than a year earlier.

<details><summary>References</summary>
<ul>
<li><a href="https://global.chinadaily.com.cn/a/202609/20/WS6aaf4071e4b06d4aa055f029.html">China&#x27;s loan prime rates remain unchanged - Chinadaily.com.cn</a></li>

</ul>
</details>

**Tags**: `#monetary\_policy`, `#interest\_rates`, `#China\_economy`

---