---
layout: default
title: "Horizon Summary: 2026-11-15 (EN)"
date: 2026-11-15
lang: en
---

> From 184 items, 7 important content pieces were selected

---

**Technology News**
1. [DeepSeek V3 Implemented in 200 Lines of JAX](#item-tech-news-1) ⭐️ 8.0/10
2. [PyPI Redesigned Project Pages Now Live](#item-tech-news-2) ⭐️ 7.0/10
3. [Lovable Apps Expose User Data Due to Security Flaws](#item-tech-news-3) ⭐️ 7.0/10
4. [LongMemEval-S Benchmark Achieves 96.0% Accuracy](#item-tech-news-4) ⭐️ 7.0/10

**Financial News**
1. [Central Bank Raises Interest Rate from 4% to 6%](#item-finance-news-1) ⭐️ 9.0/10
2. [Nvidia Turmoil and Democratic Congress May Shift AI Trade Dynamics](#item-finance-news-2) ⭐️ 7.0/10
3. [Meta Fined Over 800 Million Euros by EU](#item-finance-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [DeepSeek V3 Implemented in 200 Lines of JAX](https://github.com/Vaibhaav-Tiwari/deepseek-v3-jax) ⭐️ 8.0/10

A developer has created a functional implementation of the DeepSeek V3 language model using approximately 200 lines of pure JAX code. This minimal implementation demonstrates core AI model development concepts and provides a practical example for understanding transformer architectures. The code is available on GitHub and runs on various hardware configurations including CPU-only systems and AMD GPUs via ROCm support.

hackernews · VaibhaavTiwari · Nov 14, 15:04 · [Discussion](https://news.ycombinator.com/item?id=50497589)

**「Background」** DeepSeek V3 is a large language model released by DeepSeek in August 2025, featuring a Mixture-of-Experts \(MoE\) architecture with 671 billion total parameters and 37 billion activated per token. It supports a context length of up to 128,000 tokens and was made available under the MIT License. JAX, developed by Google, is a framework for numerical computing that combines automatic differentiation with XLA \(Accelerated Linear Algebra\), enabling high-performance machine learning computations. Libraries such as Flax and Haiku are built on top of JAX to support deep learning applications.

**「Practical Learning Resource for Developers」** This implementation serves as an accessible educational tool for developers seeking to understand large language model internals. It enables practitioners to experiment with transformer architectures on diverse hardware setups, including those without dedicated CUDA support, making advanced AI research more broadly accessible.

**「Community Engagement on Hardware Compatibility and Learning Pathways」** Community members have confirmed successful operation on Intel CPU hardware and AMD Radeon RX 7600 XT GPUs using ROCm support. Discussion also emerged around learning pathways for newcomers interested in building similar implementations, with some developers expressing interest in creating similar projects in other languages like C++.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V3-Base">deepseek -ai/ DeepSeek - V 3 -Base · Hugging Face</a></li>
<li><a href="https://dev.to/zuplo/deepseek-api-complete-guide-mastering-the-deepseek-api-for-developers-450a">Deepseek API Complete Guide: Mastering the... - DEV Community</a></li>
<li><a href="https://en.wikipedia.org/wiki/Google_JAX">Google JAX - Wikipedia</a></li>
<li><a href="https://www.assemblyai.com/blog/why-you-should-or-shouldnt-be-using-jax-in-2023">Why You Should (or Shouldn&#x27;t) be Using Google&#x27;s JAX in... | AssemblyAI</a></li>
<li><a href="https://github.com/jax-ml/jax">GitHub - jax -ml/ jax : Composable transformations of Python+NumPy...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#JAX`, `#DeepLearning`

---

<a id="item-tech-news-2"></a>
### [PyPI Redesigned Project Pages Now Live](https://blog.pypi.org/posts/2026-11-06-ui-updates-complete/) ⭐️ 7.0/10

PyPI has launched redesigned project pages with improved security indicators to help developers identify potentially compromised packages. The new interface now displays clearer signals about package integrity and provenance information, making it easier to spot security issues. The update focuses on enhancing transparency around package authenticity and supply chain trust.

hackernews · rbanffy · Nov 14, 15:40 · [Discussion](https://news.ycombinator.com/item?id=50497892)

**「Background」** Python Package Index \(PyPI\) serves as the primary repository for Python packages, making package security critical for the Python ecosystem. Previous versions of PyPI did not prominently display provenance information or clear indicators of package compromise. The redesign addresses growing concerns about supply chain attacks where legitimate packages may be hijacked but retain valid signatures.

**「Impact」** Developers can now more easily distinguish between packages with verified provenance and those that lack such information, improving their ability to make informed decisions about which packages to install. Projects without provenance information, such as &\#x27;dlt&\#x27;, will appear differently from those with provenance like &\#x27;datasette&\#x27;, helping identify potential security risks.

**「Community Discussion」** Some community members expressed concern about the centralized approach to trust management, viewing it as promoting vendor lock-in rather than maintaining Python&\#x27;s decentralized ethos. Others praised the move toward better provenance exposure while noting that the current implementation doesn&\#x27;t address all security scenarios, particularly malicious packages that are intentionally created to be harmful.

**Tags**: `#python`, `#security`, `#package-management`, `#software-supply-chain`

---

<a id="item-tech-news-3"></a>
### [Lovable Apps Expose User Data Due to Security Flaws](https://www.crissyfield.de/research/lovable-en/) ⭐️ 7.0/10

Security researchers found that the mobile app &\#x27;Lovable&\#x27; and similar applications exposed sensitive user data, including passport details and over 200,000 private messages, due to insufficient security configurations. The vulnerability was traced back to weak Row-Level Security settings and default configurations in Supabase, a backend-as-a-service platform used by the apps. Supabase had previously addressed the issue on October 30, but reports indicate that existing projects still use insecure defaults.

hackernews · armcat · Nov 14, 17:43 · [Discussion](https://news.ycombinator.com/item?id=50499017)

**「Background」** Security researchers found that the mobile app Lovable and similar applications exposed sensitive user data due to misconfigurations in Supabase, a backend-as-a-service platform. The vulnerability, related to insufficient Row-Level Security \(RLS\) and default insecure settings in Supabase templates, allowed unauthorized access to private messages and passport details. Supabase had previously addressed a similar issue \(CVE-2026-16503\) where default credentials and open PostgreSQL instances were exposed, though some reports suggest fixes were not fully applied to existing projects. Lovable’s security team acknowledged the issue and stated they scan for such vulnerabilities automatically.

**「Impact」** Developers and users of apps built with Supabase may face data exposure risks if they fail to update their configurations, as insecure defaults persist in older setups. Organizations should verify their database access controls and ensure proper implementation of Row-Level Security to prevent unauthorized data access.

**「Community Discussion」** Commenters pointed out that while Lovable is partially at fault for not securing its apps properly, Supabase bears responsibility for enabling insecure defaults to ease onboarding. Some users noted that AI-generated apps are particularly vulnerable due to lack of security awareness among developers and users alike.

<details><summary>References</summary>
<ul>
<li><a href="https://www.thehackerwire.com/vulnerability/CVE-2026-16503/">CVE-2026-16503: Supabase Template Security Vulnerability ...</a></li>
<li><a href="https://www.sentinelone.com/vulnerability-database/cve-2026-16503/">CVE-2026-16503: VPS.org Supabase Auth Bypass Vulnerability</a></li>

</ul>
</details>

**Tags**: `#security`, `#mobile-apps`, `#data-protection`, `#vulnerability`

---

<a id="item-tech-news-4"></a>
### [LongMemEval-S Benchmark Achieves 96.0% Accuracy](https://www.reddit.com/r/MachineLearning/comments/1xwnloh/longmemevals_960_with_the_official_judge_and_what/) ⭐️ 7.0/10

A new memory retrieval system called Papr achieved 96.0% accuracy on the LongMemEval-S benchmark, using the official judge and unmodified gpt-4o-2024-08-06 model. This result surpasses previous benchmarks such as Chronos \(95.6%\), Hindsight \(94.6%\), and gbrain \(90.6%\). The system utilized the Papr-Embed 0.6B embedding model, gemini flash 2.5 reranker, and a single-turn answer model. Performance was optimized for token efficiency, and the result was tuned on a subset of top-20 retrievals after reviewing top-5 misses.

reddit · r/MachineLearning · /u/remoteinspace · Nov 15, 05:40

**「Background」** LongMemEval-S is a benchmark designed to evaluate long-term memory capabilities in conversational AI agents, focusing on tasks like information extraction, temporal reasoning, and knowledge updates. It was introduced in 2024 as part of the LongMemEval suite to assess how well chat assistants retain and retrieve information over extended conversations. Papr, a memory infrastructure for AI agents, achieved 96.0% accuracy on this benchmark using its retrieval system, which leverages embeddings and reranking techniques. Other systems like Chronos, Hindsight, and gbrain have also been evaluated on LongMemEval, with varying degrees of success, showing that effective retrieval strategies are critical for high performance.

**「Impact」** Developers working on long-context AI systems can leverage Papr&\#x27;s retrieval strategy to improve performance on memory-intensive tasks. The finding that top-20 retrieval offers only marginal gains over top-5 suggests potential optimization in resource allocation for similar systems.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/longmemeval-s-benchmark">LongMemEval - S Memory Benchmark</a></li>
<li><a href="https://arxiv.org/abs/2410.10813">[2410.10813] LongMemEval : Benchmarking Chat Assistants on...</a></li>
<li><a href="https://www.papr.ai/landing/how-it-works">How Papr Works — Predictive Memory &amp; Context for AI Agents</a></li>
<li><a href="https://arxiv.org/abs/2603.16862">[2603.16862] Chronos: Temporal-Aware Conversational Agents ... Chronos: Temporal-Aware Conversational Agents with GBrain vs Hindsight vs Mem0 vs Zep: Memory Compared GitHub - vectorize-io/hindsight: Hindsight: Agent Memory That ... Overview | Hindsight Recall: How Hindsight Retrieves Memories | Hindsight</a></li>

</ul>
</details>

**Tags**: `#artificial intelligence`, `#machine learning`, `#computer systems`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Central Bank Raises Interest Rate from 4% to 6%](https://news.google.com/rss/articles/CBMif0FVX3lxTE5CS1NMS182Q0h0UDNseUVYV2ZMeFZSZHduWG13czhwVTJzSmtxeUFrVTNOS1dYeFE3SEJYNWNFcXZZM3d5Wmtibzhnb3locnBWUFQ1d1pIWFZmR1VPZGNMMHJaMFNqMzdab2FzTUVUbkZuY1hOV2xiZTVsR3VvN2c?oc=5) ⭐️ 9.0/10

The central bank today raised its key interest rate from 4% to 6%.

rss · Google News 财经 · Nov 15, 02:22

**「background」** Central banks raise interest rates to control inflation, and rapid increases can slow economic growth. A 2 percentage point rise from 4% to 6% is considered a significant policy shift that typically aims to cool down an overheating economy.

<details><summary>References</summary>
<ul>
<li><a href="https://www.investopedia.com/ask/answers/101615/what-happens-if-interest-rates-increase-too-quickly.asp">How Rapid Interest Rate Hikes Impact Economic Growth</a></li>
<li><a href="https://www.economicshelp.org/macroeconomics/monetary-policy/effect-raising-interest-rates/">Effect of raising interest rates - Economics Help</a></li>

</ul>
</details>

**Tags**: `#monetary policy`, `#interest rates`, `#economic policy`, `#central bank`

---

<a id="item-finance-news-2"></a>
### [Nvidia Turmoil and Democratic Congress May Shift AI Trade Dynamics](https://www.cnbc.com/2026/11/14/nvidia-ai-trade-data-centers-congress.html) ⭐️ 7.0/10

Nvidia&\#x27;s leadership turmoil and potential Congressional restrictions on data centers could shift AI trade dynamics, according to ETF experts. The Roundhill Magnificent Seven ETF gained less than 1% while the Roundhill Neocloud ETF rose over 1%.

rss · CNBC Finance · Nov 14, 15:50

**「Background」** Nvidia&\#x27;s CEO Jensen Huang resigned in November 2026 amid personal scandals, leading to a sharp drop in the company&\#x27;s stock price. The Democratic Party&\#x27;s control of Congress following the 2026 midterms may lead to reduced data center expansion plans, although demand for AI computing power remains strong.

**「Impact on AI Chipmakers and Data Center Sector」** If Nvidia faces prolonged headwinds due to leadership turmoil and a Democratic Congress slows data center expansion, other AI chipmakers like AMD and Alphabet may gain market share, while the broader AI trade could see a shift toward alternative suppliers and investments.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fool.com/investing/2026/11/14/think-nvidia-stock-bargain-6-reasons-face-ai-build-out-can-plunge-50-after-jensen-huang-resignation/">Think Nvidia Stock Is a Bargain? 6 Reasons the... | The Motley Fool</a></li>
<li><a href="https://www.gamespot.com/articles/nvidias-board-is-weighing-jensen-huangs-future-after-second-affair-revelation/">Nvidia CEO Jensen Huang Resigns , Effective Immediately - GameSpot</a></li>
<li><a href="https://www.cnet.com/tech/services-and-software/nvidia-ceo-jensen-huang-resigns/">Nvidia CEO Jensen Huang Resigns , Creating a &#x27;Stress Test... - CNET</a></li>
<li><a href="https://en.wikipedia.org/wiki/2026_United_States_elections">2026 United States elections - Wikipedia</a></li>
<li><a href="https://uspollingdata.com/polls/2026-midterm-tracker/">2026 Midterm Tracker: Generic Ballot D+6.3, Trump Approval 38%</a></li>
<li><a href="https://www.theguardian.com/us-news/2026/nov/14/democrats-moderate-progressive-congress">Progressive versus moderate? Democrats deny party ... | The Guardian</a></li>
<li><a href="https://www.linkedin.com/posts/michaelkspencer_anthropics-mythos-model-reaching-mythic-activity-7447602419519184896-Zgbq">AI Datacenter Slowdown Looms Amid Bottlenecks and... | LinkedIn</a></li>
<li><a href="https://www.crn.com/news/data-center/2026/lenovo-leader-calls-data-center-backlash-a-constraint-but-sees-no-ai-slowdown">Lenovo Leader Calls Data Center Backlash A ‘Constraint’ But Sees No...</a></li>
<li><a href="https://beincrypto.com/vitalik-buterin-anti-data-center-movement/">Vitalik Buterin Wants AI to Slow Down , Backs Anti- Data Center ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Technology`, `#Markets`, `#Investing`

---

<a id="item-finance-news-3"></a>
### [Meta Fined Over 800 Million Euros by EU](https://news.google.com/rss/articles/CBMib0FVX3lxTFBMUERlRGNvRkFoRnNIWVBQSlh2RUVjVG8zVXNxMkZHaTdnNk9FaVppMnI4SkwtQmlSVEJQX0FsNU5aYU9nQ0RrN0xxOUxwaGZoMnZicU9OT2duWHBtN1hQOEpFNm1oSkJlN3VLM1J2TQ?oc=5) ⭐️ 7.0/10

Meta has been fined over 800 million euros by the European Union for antitrust violations.

rss · Google News 财经 · Nov 15, 05:55

**「background」** The European Union fined Meta €797.72 million for violating antitrust rules by tying its Facebook Marketplace service to its main social network, Facebook, in a way that disadvantaged competitors. This was the EU’s first antitrust fine against Meta.

<details><summary>References</summary>
<ul>
<li><a href="https://apnews.com/article/meta-facebook-european-union-competition-fine-6886192353a344126a15886d6ca7c627">EU slaps Meta with a nearly 800 million euro fine for ... Meta&#x27;s €800 Million EU Fine: Big Penalty, Small Hit to Earnings? Meta Fined $840 Million by EU for Antitrust Violations EU&#x27;s €800 Million Meta Blowback: Real Trap Signal or Just ... EU slaps Meta with a nearly 800 million euro fine for ... Meta fined 800 million euros by the EU for antitrust ... Facebook Marketplace violations: EU imposes 800 million euro fine</a></li>

</ul>
</details>

**Tags**: `#regulation`, `#tech industry`, `#financial penalty`, `#policy`

---