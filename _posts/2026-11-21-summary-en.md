---
layout: default
title: "Horizon Summary: 2026-11-21 (EN)"
date: 2026-11-21
lang: en
---

> From 186 items, 14 important content pieces were selected

---

**Technology News**
1. [Terence Tao Proposes Proof Unifying Navier-Stokes and Riemann Hypothesis](#item-tech-news-1) ⭐️ 10.0/10
2. [Mathematician Rushes GRH Proof After Anthropic AI Claim](#item-tech-news-2) ⭐️ 9.0/10
3. [Levent Alpöge Claims Lean Proof of Generalized Riemann Hypothesis](#item-tech-news-3) ⭐️ 9.0/10
4. [Anthropic Mathematician Claims Riemann Hypothesis Proof Using Claude](#item-tech-news-4) ⭐️ 9.0/10
5. [First QRAM implementation on real quantum chip achieves 80.9% accuracy](#item-tech-news-5) ⭐️ 9.0/10
6. [US House reveals 880,000 AI chip exports to China approved, including military-linked firms](#item-tech-news-6) ⭐️ 8.0/10
7. [AI Detection Tools Force Researchers to Dilute Academic Writing](#item-tech-news-7) ⭐️ 7.0/10
8. [Google Claims Breakthrough in AI with Recursive Self-Improvement and Evolutionary Memory](#item-tech-news-8) ⭐️ 7.0/10

**Financial News**
1. [Stocks, Gold, Bitcoin Plunge as VIX Spikes to 40, Nasdaq Erases Year-to-Date Gains](#item-finance-news-1) ⭐️ 10.0/10
2. [Nasdaq Plunges More Than 10%, VIX Spikes as Wall Street Warns Selling May Not Be Over](#item-finance-news-2) ⭐️ 9.0/10
3. [Fed Officials Speak More Despite Warsh’s Push for Less Forward Guidance](#item-finance-news-3) ⭐️ 8.0/10
4. [US corporations shift from buybacks to issuing equity, adding 3.1% of market cap](#item-finance-news-4) ⭐️ 8.0/10
5. [Argentina approves its largest-ever investment project](#item-finance-news-5) ⭐️ 7.0/10
6. [Chinese Regulators Plan RMB 34 Million Fine for A-Share Company Over Financial Fraud](#item-finance-news-6) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Terence Tao Proposes Proof Unifying Navier-Stokes and Riemann Hypothesis](https://terrytao.wordpress.com/2026/11/20/unforced-euler-singularity-unforced-navier-stokes-singularity-and-the-generalized-riemann-hypothesis/) ⭐️ 10.0/10

Terence Tao has announced a potential proof that connects the existence of an unforced singularity in the Navier-Stokes equations to the Generalized Riemann Hypothesis. The proof is backed by a 15-million-line formalization in the Lean proof assistant, which has reportedly been accepted by two independent Lean kernels, indicating no kernel bug exploitation. If verified, this would resolve two of the most challenging open problems in mathematics. However, the proof has not yet undergone full peer review, and some observers caution that the Lean code may not actually formalize the intended statements.

hackernews · archon1410 · Nov 20, 17:21 · [Discussion](https://news.ycombinator.com/item?id=50578358)

**「Prior result on Navier–Stokes blowup」** In 2016, Terence Tao proved finite-time blowup for an averaged three-dimensional Navier–Stokes equation, highlighting a “supercriticality barrier” for the full global regularity problem, which is a Clay Millennium Prize challenge. The new announcement claims a computer-verified proof that the true unforced equations develop a singularity, and further that the Generalized Riemann Hypothesis is equivalent to the non-existence of such singularities.

**「Community Discussion」** Commenters debate whether the Lean formalization verifies the intended mathematical claims or merely demonstrates that the code compiles, with some cautioning that a passing build does not guarantee correctness of business logic. Others note that two independent Lean kernels accepting the proof reduce the risk of kernel bugs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Navier%E2%80%93Stokes_existence_and_smoothness">Navier – Stokes existence and smoothness - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#mathematics`, `#formal-verification`, `#AI`, `#Navier-Stokes`, `#Riemann-Hypothesis`

---

<a id="item-tech-news-2"></a>
### [Mathematician Rushes GRH Proof After Anthropic AI Claim](https://math216.wordpress.com/2026/11/20/hurried-announcement-alessandro-masullo-grh/) ⭐️ 9.0/10

Mathematician Alessandro Masullo published a 940-page draft proof of the Generalized Riemann Hypothesis hours after Anthropic reportedly claimed to have solved the same problem. The manuscript, posted on Masullo’s blog, reflects 12 years of work but contains incomplete sections and has not undergone peer review. The hurried release aims to establish priority amid a new reality where AI systems can preempt human discoveries.

hackernews · jasondavies · Nov 20, 18:33 · [Discussion](https://news.ycombinator.com/item?id=50579568)

**「Background」** Earlier on November 20, 2026, Anthropic employee Levent Alpöge posted a Claude-generated proof that claimed to solve the Riemann Hypothesis, of which the Generalized Riemann Hypothesis is an extension.

**「Impact」** The incident forces mathematicians to weigh rapid disclosure of unfinished work against the risk of being scooped by AI, potentially eroding the field’s traditional emphasis on meticulous verification.

**「Community Discussion」** One commenter speculated that Anthropic might have accessed portions of Masullo’s proof via previously uploaded documents, while another noted that the draft’s empty first section raises doubts about its completeness.

<details><summary>References</summary>
<ul>
<li><a href="https://www.scientificamerican.com/article/dueling-claims-of-riemann-hypothesis-proofs-emerge/">Dueling claims of Riemann hypothesis proofs emerge</a></li>

</ul>
</details>

**Tags**: `#mathematics`, `#ai`, `#research-ethics`, `#open-science`, `#academic-culture`

---

<a id="item-tech-news-3"></a>
### [Levent Alpöge Claims Lean Proof of Generalized Riemann Hypothesis](https://alpo.ge/remark.pdf) ⭐️ 9.0/10

Mathematician Levent Alpöge has announced a claimed proof of the Generalized Riemann Hypothesis, formalized in the Lean proof assistant with AI assistance. The proof is distributed as a 1.3 GB archive containing approximately 15 million lines of Lean code. The announcement has not been peer-reviewed or independently verified.

hackernews · iamronaldo · Nov 20, 14:16 · [Discussion](https://news.ycombinator.com/item?id=50574968)

**「Background」** The Generalized Riemann Hypothesis \(GRH\) is a central unsolved conjecture in number theory, extending the classical Riemann Hypothesis to Dirichlet L-functions. Levent Alpöge is a mathematician at Anthropic who previously worked in number theory and arithmetic statistics, and co-authored a proof related to Hilbert&\#x27;s tenth problem in 2025.

**「Community Discussion」** One commenter \(dawdler-purge\) expressed surprise that Claude could contribute to such a proof, while another \(djoldman\) detailed the proof&\#x27;s scale \(1.3 GB, ~15M lines\) and provided a download command. Others voiced fears about the pace of AI breakthroughs and discussed calls for a research pause.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Levent_Alp%C3%B6ge">Levent Alpöge - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#mathematics`, `#formal-verification`, `#ai`, `#research`, `#lean`

---

<a id="item-tech-news-4"></a>
### [Anthropic Mathematician Claims Riemann Hypothesis Proof Using Claude](https://www.scientificamerican.com/article/anthropic-mathematician-claims-to-prove-riemann-hypothesis-most-famous-problem-in-all-of-math/) ⭐️ 9.0/10

Levent Alpöge, a mathematician at Anthropic, announced that he proved the Riemann Hypothesis with the assistance of Claude. The proof spans over 250,000 pages and has been encoded in the Lean theorem prover, a language that can mechanically verify mathematical correctness. Alpöge also claims the proof confirms the broader Generalized Riemann Hypothesis. The claim has not yet been independently verified.

telegram · zaihuapd · Nov 20, 15:29

**「Background」** The Riemann Hypothesis, proposed by Bernhard Riemann in 1859, concerns the distribution of prime numbers and is widely regarded as the most famous unsolved problem in mathematics. The Lean theorem prover is a proof assistant that encodes mathematical arguments in a formal, mechanically checkable language, allowing verification of complex claims.

**「Impact」** Because the proof is encoded in Lean, mathematicians can now run the formal proof checker to independently verify its correctness; successful verification would resolve both the Riemann Hypothesis and the Generalized Riemann Hypothesis.

**Tags**: `#anthropic`, `#claude`, `#riemann-hypothesis`, `#lean`, `#formal-verification`, `#ai-mathematics`

---

<a id="item-tech-news-5"></a>
### [First QRAM implementation on real quantum chip achieves 80.9% accuracy](https://finance.sina.com.cn/stock/2026-11-21/doc-iniznhsk3530826.shtml) ⭐️ 9.0/10

Researchers at Zhejiang University claimed the first practical implementation of quantum random access memory \(QRAM\) on a real superconducting quantum chip. The prototype, running on the university’s “Tianmu-2” chip, fetched 4-bit and 8-bit data with accuracies of 80.9% and 60.4%, respectively, and reduced circuit depth by over 30% compared to unoptimized designs. The results were published in Nature Physics, and the team reported verifying local noise resilience of the architecture.

telegram · zaihuapd · Nov 21, 08:31

**「Quantum RAM background」** 量子随机存储器 \(QRAM\) 是经典 RAM 的量子对应物，能以叠加态高效读取经典数据，对量子机器学习等需要加载数据的量子算法至关重要。此前 QRAM 仅在原理验证或仿真层面实现，尚无真机芯片上的实际演示。

**「Impact」** This demonstration of QRAM on a physical chip could accelerate the execution of quantum algorithms that require fast data lookups, such as quantum machine learning, by providing a memory structure that reduces circuit complexity.

**Tags**: `#quantum-computing`, `#QRAM`, `#quantum-memory`, `#superconducting-qubit`, `#research`

---

<a id="item-tech-news-6"></a>
### [US House reveals 880,000 AI chip exports to China approved, including military-linked firms](https://news.google.com/rss/articles/CBMi5gNBVV95cUxPdFdPMWhPN3duNG5mNzd5T293WlhzRnZFaWVGa1cxa3dnbng5WU92eVY1LWd5WW9JRE1JRmJRZkI3UE90XzhlRHlTazRRMVMyVnk5X2xsRlpUS1E1dE8zVW8wZGozWDh4RXo2MV8tekVvaW90Y0d0OXl3aE1Fb1F1cHZOb2xMTUFCTTJFNDZDdVRCdTNDNGlZZlJRRTlaZEZNMDhNTmEyZEdGS3QxalNUUnB6NWIyZ3VMSlZYSHlrcG4ydDhUZnc1SGwzUjA1M0VWc1NrM1RHc3NHTWFrT09kYW53SUhhU1MzMW5ESlRwRjR3MkFiUU4tT0hzR0EwUGtiYkVfd1UyM1htNk9JcHRndE5aSEhHZElpSnN0enRfb05Idkp1NGJzVDhRcWNMYkxBZnppQjJnMVlxVjV4b0dFNUNEZE83RVZhUlpkbWpKcFRPWWFrZGpUNm94OWx2SGJqSzlycTBzZGZEVkJER0gzeC1PTkhsMTl3aVRDNDN5TGdfVmxXTnpTVkxic2N0MEt0RS1RbGYydXFxVHBhU3RzUmtCNFIwdXpGVTVwMmN2ckowVHlWZzJlNEJ4NXJUeFpYOWdCN2xSbHVHVVJQbEpCd1hqbzJCMnp4MnJ6andKelRrVlcwNFE?oc=5) ⭐️ 8.0/10

The U.S. House of Representatives disclosed that approximately 880,000 export licenses for AI-related chips to China had been approved, including shipments to companies identified by the Department of Defense as military-linked enterprises, according to a report by RFI on November 20, 2026. The specific chip models and the timeframe of the approvals were not detailed in the disclosure. The revelation highlights potential gaps in export controls aimed at preventing advanced technology from reaching Chinese military entities.

rss · Google News AI · Nov 20, 11:40

**「Background」** In recent years, the U.S. has imposed strict export controls on advanced AI chips to China, aiming to limit the latter&\#x27;s capabilities in artificial intelligence and high-performance computing. Despite these restrictions, U.S. companies have continued to apply for licenses to export certain chips, some of which have been approved by the Department of Commerce. The Pentagon has previously identified specific Chinese firms as having military ties, raising concerns over the potential use of exported technology in defense applications.

<details><summary>References</summary>
<ul>
<li><a href="https://cn.nytimes.com/china/20261103/chinas-message-to-its-rivals-you-need-what-we-make/">中 国 技术 出 口 管制升级：利用 工 业 优势构建经济武器库 - 纽约时报 中 文网</a></li>

</ul>
</details>

**Tags**: `#AI chips`, `#export controls`, `#China`, `#technology policy`, `#hardware`

---

<a id="item-tech-news-7"></a>
### [AI Detection Tools Force Researchers to Dilute Academic Writing](https://news.google.com/rss/articles/CBMiZkFVX3lxTE53Q3ViRHAyWjhaODdTV2hGTWNVXzl6NnlMdDc2Q0JIeHdvRm9IcWFQc3JUelpOeW41c3VEbUdnU3RQRjg5ZFdrQmttX2d5M3htaDB0WXJzQ0ZRdkRVTEw4aXR6dm1rZw?oc=5) ⭐️ 7.0/10

AI detection tools are causing researchers to oversimplify their writing to avoid false positives, leading to a decline in academic rigor. Authors reportedly revise papers to &quot;student essay level&quot; to pass AI scrutiny, sacrificing scholarly quality and complexity.

rss · Google News AI · Nov 21, 05:08

**「Background on AI Detection in Academic Writing」** AI content detection tools are increasingly used in academic settings to identify texts potentially generated by AI, but these tools often produce false positives, misidentifying human-written work as AI-generated. Recent studies highlight concerns about the reliability of these systems and their unintended consequences, such as discouraging stylistic diversity and pressuring authors to simplify their writing to avoid suspicion. This context helps frame the current report of researchers altering their papers to evade detection, inadvertently compromising academic quality.

**「Impact」** Researchers and academic institutions must now balance AI detection compliance with maintaining scholarly standards, potentially compromising the integrity of academic publishing and evaluation processes.

<details><summary>References</summary>
<ul>
<li><a href="https://link.springer.com/article/10.1007/s44217-026-02307-x">AI content detection in student text assignments, false ...</a></li>

</ul>
</details>

**Tags**: `#ai detection`, `#academic integrity`, `#nlp`, `#education technology`, `#ai ethics`

---

<a id="item-tech-news-8"></a>
### [Google Claims Breakthrough in AI with Recursive Self-Improvement and Evolutionary Memory](https://news.google.com/rss/articles/CBMiTkFVX3lxTE5SOTdmTjhkWXJpemhxbzZPWFppSnd1Q0dfRnZaSmlmaGRHUzJUdnp1VEM5MXYxWXhGa3NoZDNxNEJSdmQ5RzV1Um5Tc0QwUQ?oc=5) ⭐️ 7.0/10

A Chinese tech outlet reports that Google has published a paper describing recursive self-improvement \(RSI\) in AI, cross-model experience transfer from Anthropic&\#x27;s Opus to Google&\#x27;s Gemini, and the development of persistent &\#x27;evolutionary memory&\#x27; in AI systems. The report suggests these advancements were achieved internally at Google, though no details or verification methods are provided in the source.

rss · Google News AI · Nov 21, 04:12

**「Background on Recursive Self-Improvement and Google&\#x27;s AI Development」** Recursive self-improvement \(RSI\) refers to a hypothetical process where an AI system iteratively designs more capable successors, potentially accelerating AI development exponentially. Horizon&\#x27;s September 17 digest reported on Google&\#x27;s &\#x27;Dream RSI&\#x27; paper, which explored mechanisms for simulating AI research to improve discovery efficiency. Sergey Brin recently noted that Google&\#x27;s AI development, including the iterative release of Flash models preceding Gemini 4, suggests progress toward RSI.

**「Impact」** If confirmed, these developments could significantly influence AI research and deployment, particularly in self-evolving systems and knowledge transfer between models, potentially shifting expectations for AI autonomy and long-term learning capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self - improvement - Wikipedia</a></li>
<li><a href="https://www.businessinsider.com/sergey-brin-google-gemini-ai-argon-recursive-self-improvement-rsi-2026-10">Sergey Brin Says Google &#x27;s AI Is Approaching... - Business Insider</a></li>
<li><a href="https://www.mindstudio.ai/blog/google-dream-rsi-recursive-self-improvement">What Is Dream RSI ? Google &#x27;s Recursive Self - Improvement , Explained</a></li>

</ul>
</details>

**Tags**: `#artificial-intelligence`, `#recursive-self-improvement`, `#google`, `#gemini`, `#large-language-models`, `#research`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Stocks, Gold, Bitcoin Plunge as VIX Spikes to 40, Nasdaq Erases Year-to-Date Gains](https://news.google.com/rss/articles/CBMicEFVX3lxTE5ybEZqVEZ6Q3lIbF9OdEZqUFdTZXdRdW9PYl9zLUFLa1RBNTVjbFdwcTNCUDRya3RPaGpMOEYyaFVNUGtZT1hjZ1BkNzRicUI0SXFkbWhfT3Ita2RYNFk1X3ZlWGxOWlFES1BIOUdYYlU?oc=5) ⭐️ 10.0/10

Overnight, stocks, gold, and bitcoin tumbled in a broad selloff, with the Nasdaq erasing all its year-to-date gains and the CBOE Volatility Index \(VIX\), a fear gauge, briefly hitting 40.

rss · Google News 财经 · Nov 20, 23:00

**「Background」** The rout was led by a sharp reversal in the artificial intelligence trade, pushing Nvidia shares down 14% and the Nasdaq into a technical correction.

**「Impact」** Several banks responded by issuing risk warnings on precious metals, signaling heightened concern over further volatility.

**Tags**: `#market turmoil`, `#VIX spike`, `#equity selloff`, `#bitcoin crash`, `#systemic risk`

---

<a id="item-finance-news-2"></a>
### [Nasdaq Plunges More Than 10%, VIX Spikes as Wall Street Warns Selling May Not Be Over](https://news.google.com/rss/articles/CBMiiAFBVV95cUxPYkRJbU5aVlVneUlhUG5ySU9TMHBTQ0R3TGt6dy1Qbm9VSFFQRDdaU19lT1FRV2J3Nlc3ZjNtSzdKeVBrWXJDRWlPbFNJYk5pYWpyTWd2R1R6ck5hNVZWT1F2dWI5ZHZMU0g4R3QtUnlPend3dWJQbmltUUlHRXplZFdTcFplRktX?oc=5) ⭐️ 9.0/10

The Nasdaq Composite fell over 10% and the CBOE Volatility Index surged, according to a Sohu report. Wall Street strategists warned that the sell-off may continue.

rss · Google News 财经 · Nov 21, 08:30

**「Background」** The CBOE Volatility Index \(VIX\), often called the &quot;fear gauge,&quot; closed at 35.89 on November 20, up 26.2%, after touching 40.03 intraday—a level last reached in April 2025.

<details><summary>References</summary>
<ul>
<li><a href="https://qhweb.eastmoney.com/news/202611213936813054.html">恐慌指数飙升：纳指狂泻逾10%，华尔街警告抛售“未完待续”</a></li>

</ul>
</details>

**Tags**: `#美股`, `#纳斯达克`, `#恐慌指数`, `#抛售`, `#市场波动`

---

<a id="item-finance-news-3"></a>
### [Fed Officials Speak More Despite Warsh’s Push for Less Forward Guidance](https://www.cnbc.com/2026/11/20/warsh-fed-forward-guidance-rate-hikes.html) ⭐️ 8.0/10

Fed officials’ public commentary surged in the past two weeks to the highest volume since early 2025, according to Bank of America, even as Chairman Kevin Warsh sticks to his refusal to offer forward guidance.

rss · CNBC Finance · Nov 20, 21:10

**「Background」** Warsh took office six months ago and has consistently avoided pre-committing to future interest-rate moves, arguing that forward guidance handcuffs policymakers.

**「Impact」** The public disagreement may contribute to heightened interest-rate volatility, BofA economist Aditya Bhave warned.

**Tags**: `#Federal Reserve`, `#monetary policy`, `#forward guidance`, `#interest rates`, `#FOMC communications`

---

<a id="item-finance-news-4"></a>
### [US corporations shift from buybacks to issuing equity, adding 3.1% of market cap](https://www.cnbc.com/2026/11/20/equity-issuance-bull-market-problem.html) ⭐️ 8.0/10

US corporations have shifted from repurchasing shares to issuing new equity over the past two years. Net issuance now equals 3.1% of total market capitalization, Acadian Asset Management reports, ending a buyback era that had supported stock prices.

rss · CNBC Finance · Nov 20, 14:15

**「Background」** Since 2024, companies had been net repurchasers of their own shares, shrinking the supply of stock available for trading and thereby helping to lift share prices and earnings per share.

**Tags**: `#equity issuance`, `#stock buybacks`, `#bull market`, `#capital allocation`, `#market trends`

---

<a id="item-finance-news-5"></a>
### [Argentina approves its largest-ever investment project](https://news.google.com/rss/articles/CBMiZ0FVX3lxTE1oTTJ4b1NBbWZIMXBGZ1E4cjg5R2prS3pYNlhHdEhGSWZld1g0am5xRWVDQ3VxYmo0RWxFUlk4eEFzN2JpR21IRDJCTlhFMlJacHotdDRnaHNJVTkyMExVbzhsY1NXdG8?oc=5) ⭐️ 7.0/10

Argentina&\#x27;s government has approved the largest investment project in the country&\#x27;s history, according to a report, though the sector, amount, and participating parties were not disclosed.

rss · Google News 财经 · Nov 21, 01:37

**「Background」** A web search is needed to provide necessary context for this approval, as the source item does not specify details about the project. Without such context, only generic background on Argentina&\#x27;s investment climate can be offered: the country has been pursuing economic reforms under President Javier Milei, including deregulation and incentives to attract foreign capital, aiming to reverse a long history of capital flight and recession.

**Tags**: `#Argentina`, `#investment project`, `#government approval`, `#economic development`, `#foreign investment`

---

<a id="item-finance-news-6"></a>
### [Chinese Regulators Plan RMB 34 Million Fine for A-Share Company Over Financial Fraud](https://news.google.com/rss/articles/CBMiY0FVX3lxTE9Hb0NGLWxKUV9hWUg2Zy1uZTB4c1dpZjRCeThWa1F4QmxLMEtWYXU2d29vWUdjdVVuTGpFeW1ka1YtZW10eTVEeHRHZFRueTFkV3FiLUhxVWpVS0tfUElqRXhrZw?oc=5) ⭐️ 7.0/10

Chinese regulators plan to fine an A-share company RMB 34 million for financial fraud, following a stock decline of over 70% year-to-date and the company&\#x27;s public apology.

rss · Google News 财经 · Nov 20, 18:35

**「Background」** The company faced regulatory penalties due to financial fraud, with proposed fines totaling RMB 34 million, including individual penalties for executives, and its stock has fallen over 70% this year.

<details><summary>References</summary>
<ul>
<li><a href="https://stock.10jqka.com.cn/20260531/c677103234.shtml">stock.10jqka.com.cn/20260531/c677103234.shtml</a></li>
<li><a href="https://finance.sina.cn/stock/ggyj/2026-05-31/detail-inhzurim9208298.d.html?vt=4">finance.sina.cn/stock/ggyj/ 2026 -05-31/detail-inhzurim9208298.d.html?...</a></li>

</ul>
</details>

**Tags**: `#financial fraud`, `#regulatory penalty`, `#A-shares`, `#stock decline`, `#China`

---