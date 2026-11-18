---
layout: default
title: "Horizon Summary: 2026-11-18 (EN)"
date: 2026-11-18
lang: en
---

> From 229 items, 12 important content pieces were selected

---

**Technology News**
1. [Java4Shell: RCE Vulnerability in OpenJDK Base64 Processing](#item-tech-news-1) ⭐️ 9.0/10
2. [Microsoft Releases MAI Code 2 and MAI Code 2 Flash AI Coding Models](#item-tech-news-2) ⭐️ 8.0/10
3. [Harvard Research: AI Coding Agents Shift Development Bottleneck to Code Review](#item-tech-news-3) ⭐️ 8.0/10
4. [Isomorphic Labs Raises $5 Billion in Largest AI Drug Discovery Funding](#item-tech-news-4) ⭐️ 8.0/10
5. [External Sandboxes for Coding Agents Released](#item-tech-news-5) ⭐️ 7.0/10
6. [OpenAI Releases GPT-6.2 Astra and Sol with 20% Price Cut](#item-tech-news-6) ⭐️ 7.0/10

**Financial News**
1. [UK Immigration Bill Passes Commons, Moves to Lords](#item-finance-news-1) ⭐️ 8.0/10
2. [China, South Korea Conclude Services, Investment FTA Talks After 8 Years and 8 Months](#item-finance-news-2) ⭐️ 8.0/10
3. [Trump, Xi, Putin Meet at APEC Summit in Shenzhen](#item-finance-news-3) ⭐️ 7.0/10
4. [典型A股避损型内幕交易案曝光 监管部门持续打击市场操纵](#item-finance-news-4) ⭐️ 7.0/10
5. [Spot Gold Falls Below $3,800 as Rate Hike Expectations Pressurize Prices](#item-finance-news-5) ⭐️ 7.0/10
6. [NVIDIA Earnings Lift Storage Stocks Pre-Market](#item-finance-news-6) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Java4Shell: RCE Vulnerability in OpenJDK Base64 Processing](https://calif.io/java4shell/) ⭐️ 9.0/10

Security researchers at Calif discovered a critical remote code execution vulnerability \(CVE-2024-21018\) in OpenJDK&\#x27;s Base64 processing implementation. The vulnerability affects HotSpot VM implementations across OpenJDK builds, Oracle JDK, and GraalVM JDK. The attack involves heap grooming techniques over the network, with optimal stability requiring low, stable round-trip times. Semgrep has published free detection scripts that check for five specific conditions to identify vulnerable instances. Unconfirmed reports suggest the vulnerability may be related to the AVX512 implementation of Base64 decoding and could potentially be mitigated by running Java with the -XX:UseAVX=2 flag.

hackernews · werrett · Nov 17, 21:11 · [Discussion](https://news.ycombinator.com/item?id=50538240)

**「Background」** Java4Shell \(CVE-2026-114938\) is a critical memory-corruption vulnerability in OpenJDK&\#x27;s Base64 decoder that affects HotSpot-based JVMs, including OpenJDK builds, Oracle JDK, and GraalVM JDK. The vulnerability, rated 9.2 CVSS v4.0 by researchers and 8.1 by Oracle, stems from the AVX512 implementation of Base64 decoding and enables unauthenticated attackers to corrupt heap memory, read secrets, and achieve remote code execution. OpenJ9 and GCJ are not affected since they do not use the HotSpot C2 compiler stub that contains the vulnerable code. A temporary mitigation involves running Java with the -XX:UseAVX=2 flag to avoid the vulnerable code path.

**「Impact on Java deployments」** Java deployments running affected OpenJDK versions face remote code execution risk when processing untrusted Base64 input. System administrators should update to the latest JDK distributions or apply the -XX:UseAVX=2 workaround to disable the vulnerable AV512 Base64 implementation. Semgrep has published free detection scripts to identify vulnerable configurations.

**「Community Discussion」** Security researchers note that while exploit conditions are very specific, many hosts will still be impacted. One commenter warned that critical infrastructure could be seriously compromised within six months, though this could force organizations with legacy stacks to modernize their security practices. The technical attack was demonstrated over the internet through public IP addresses rather than ideal laboratory conditions, demonstrating real-world exploitability.

<details><summary>References</summary>
<ul>
<li><a href="https://semgrep.dev/blog/2026/java4shell-openjdk-base64-vulnerability/">Java4Shell: Critical OpenJDK Base64 RCE (CVE-2026-114938)</a></li>
<li><a href="https://www.sentinelone.com/blog/java4shell-vulnerability-in-openjdk-enables-rce-on-avx-512-cpus/">Defending Against Java4Shell: Vulnerability in OpenJDK ...</a></li>
<li><a href="https://blog.qualys.com/vulnerabilities-threat-research/2026/11/17/how-to-find-mitigate-and-patch-the-critical-java4shell-flaw-cve-2026-114938-now">How to Find, Mitigate, and Patch the Critical Java4Shell Flaw ...</a></li>
<li><a href="https://openjdk.org/groups/vulnerability/advisories/">OpenJDK Vulnerability Advisories</a></li>
<li><a href="https://app.opencve.io/cve/CVE-2024-20918">CVE-2024-20918 - Vulnerability Details - OpenCVE</a></li>

</ul>
</details>

**Tags**: `#security`, `#java`, `#vulnerability`

---

<a id="item-tech-news-2"></a>
### [Microsoft Releases MAI Code 2 and MAI Code 2 Flash AI Coding Models](https://microsoft.ai/news/introducing-mai-code-2-and-mai-code-2-flash/) ⭐️ 8.0/10

Microsoft announced MAI Code 2 and MAI Code 2 Flash, two AI coding models that deliver near-GPT-6.1 performance at substantially reduced costs. MAI Code 2 achieves 98% of GPT-6.1 Sol&\#x27;s performance at 40% of the cost, and 96% of Claude Opus 5.5&\#x27;s performance at just 5% of the cost. The models are now available through GitHub Copilot, with users reporting the ability to resolve complex Python build issues in Windows WSL/Ubuntu and generate passing test cases.

hackernews · lemonish97 · Nov 17, 18:25 · [Discussion](https://news.ycombinator.com/item?id=50535885)

**「Background」** Microsoft has been developing AI coding assistants through its GitHub Copilot product, competing directly with OpenAI&\#x27;s GPT models and Anthropic&\#x27;s Claude series. The AI coding assistant market has seen rapid performance improvements and cost reductions over recent years, with Microsoft leveraging its partnership with OpenAI while also building proprietary models. GitHub Copilot currently offers multiple AI model options to subscribers, with recent pricing around $19/month for individual plans.

**「Impact」** Developers and organizations using AI-assisted coding tools may see significant cost reductions, as MAI Code 2 offers comparable performance to leading models at a fraction of the price. GitHub Copilot users have already switched to the new model, with reports of solving tricky build and deployment issues without noticing a difference from Claude Opus. This could pressure OpenAI and Anthropic to reduce pricing or accelerate model development to maintain competitive positioning.

**「Community Discussion」** Commenters expressed surprise at Microsoft&\#x27;s rapid catch-up, with speculation that model distillation from OpenAI \(through their partnership\) may explain the progress, though this raises legal and ethical questions. Some users questioned whether Microsoft is cherry-picking benchmark numbers, particularly regarding Sol&\#x27;s cost advantage over Opus. One user noted they cancelled their GitHub Copilot subscription, citing insufficient value at $19/month, and expressed hope that these new models might improve the offering.

**Tags**: `#artificial-intelligence`, `#software-engineering`, `#machine-learning`

---

<a id="item-tech-news-3"></a>
### [Harvard Research: AI Coding Agents Shift Development Bottleneck to Code Review](https://complexdiscovery.com/harvard-researchers-find-ai-coding-agents-shifted-the-bottleneck-to-code-review/) ⭐️ 8.0/10

Harvard researchers have found that AI coding agents have shifted the development bottleneck from code creation to code review. As AI agents become capable of generating code quickly, the limiting factor in software development workflows has moved to the review stage, where human developers must evaluate, understand, and validate AI-generated code changes. The research highlights practical implications for engineering teams, including increased review workloads and the need for new processes to handle AI-assisted development.

hackernews · judahmeek · Nov 17, 21:16 · [Discussion](https://news.ycombinator.com/item?id=50538303)

**「Context for AI development bottleneck shift」** AI coding agents are AI systems that autonomously write, modify, and refactor software code, representing a significant advancement over earlier AI assistants that only suggested code snippets. Prior to widespread agent adoption, human developers themselves were the primary bottleneck in software development—writing code slowly and requiring extensive iteration. Harvard&\#x27;s empirical research now documents how AI agents have accelerated code generation to the point where human code review has become the limiting factor in development workflows, reversing the traditional bottleneck location.

**「Impact」** Software developers are spending significantly more time on code review tasks as AI agents handle code generation, with some engineers reporting they now spend entire workdays reviewing AI-written code. Teams may need to adopt new review workflows, potentially including AI-assisted review agents, to manage the increased volume and complexity of AI-generated code changes.

**「Community Discussion」** Developers in the discussion noted varying quality across AI model versions, with some newer models producing over-engineered solutions that required substantial cleanup. One commenter with 25 years of experience observed that AI agents can review each other&\#x27;s code effectively for issue-finding, though human review remains important for understanding context and ensuring the code does the right thing. Others expressed concern that AI-written code tends to be overblown compared to human-written solutions, and some reported finding the review-heavy workflow less enjoyable than traditional development.

**Tags**: `#software engineering`, `#AI coding`, `#development workflow`

---

<a id="item-tech-news-4"></a>
### [Isomorphic Labs Raises $5 Billion in Largest AI Drug Discovery Funding](https://news.google.com/rss/articles/CBMiV0FVX3lxTE1hMFpCU3JkS0pRaGx0X0NfSEJKNHJfWXc4cUduQ3dUTHpraklmckZIVVNtYTEyS2FWSW03SnZLaW1IMk5wSE5zUEJwMlZaS1ItdHdUVGdUMA?oc=5) ⭐️ 8.0/10

Isomorphic Labs, a drug discovery spinout from DeepMind, has raised $5 billion in what is claimed to be the world&\#x27;s largest AI pharmaceutical financing round. The funding signals significant industry investment in AI-powered pharmaceutical research.

rss · Google News AI · Nov 18, 02:40

**「Background」** Isomorphic Labs is an AI drug discovery company spun out from Google&\#x27;s DeepMind in 2021, founded by DeepMind CEO Demis Hassabis with the goal of improving human health through advanced computational approaches to drug discovery. The company announced its launch in November 2021 and has since been developing AI models to predict molecular behavior and accelerate the drug discovery process.

**「Impact」** This massive funding round demonstrates strong investor confidence in AI-driven drug discovery and could accelerate the development of computational approaches to pharmaceutical research, potentially reducing drug development timelines and costs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Isomorphic_Labs">Isomorphic Labs - Wikipedia</a></li>
<li><a href="https://techcrunch.com/2026/11/17/isomorphic-labs-raises-5b-as-it-looks-to-take-drug-candidates-to-clinical-trials/">Isomorphic Labs raises $ 5 B as it looks to take drug ... | TechCrunch</a></li>

</ul>
</details>

**Tags**: `#AI drug discovery`, `#funding`, `#Isomorphic Labs`, `#DeepMind`, `#healthcare AI`

---

<a id="item-tech-news-5"></a>
### [External Sandboxes for Coding Agents Released](https://simonwillison.net/2026/Nov/17/external-sandboxes-for-coding-agents/) ⭐️ 7.0/10

Simon Willison and Prime Radiant released three external sandbox server implementations to isolate AI coding agents from the host machine. The sandboxes use v86/WebAssembly, Apple Containers, and Microsoft&\#x27;s Quicksand library to run code in a dedicated environment separate from the agent itself. This pattern protects against prompt injection attacks and accidental damage when running local models like Claude Code, Pi, or Codex, with an optional HTTP/HTTPS allow-list proxy and credential replacement mechanism for authenticated API calls.

rss · Simon Willison \(AI\) · Nov 17, 22:52

**「Why coding agents need isolation」** Coding agents like Claude Code, Codex, and Pi can execute arbitrary code, read files, and make network requests—capabilities that make them useful but also dangerous. When these agents run local models \(rather than API-only versions\), they face two distinct risks: accidental damage from model errors, and prompt injection attacks where malicious content tricks the agent into performing harmful actions. Traditional sandboxing often runs the agent inside the sandbox, meaning a compromise of the agent also compromises the isolation boundary. The external sandbox pattern reverses this: the agent runs on the host while code execution happens in a dedicated, disposable environment.

**「Impact」** Developers building agentic systems can now run AI coding agents with local models in a protected environment where untrusted code executes in an isolated sandbox with configurable network controls, preventing the agent from directly accessing the host system or sensitive credentials.

**Tags**: `#security`, `#AI`, `#sandboxing`, `#coding-agents`, `#open-source`

---

<a id="item-tech-news-6"></a>
### [OpenAI Releases GPT-6.2 Astra and Sol with 20% Price Cut](https://simonwillison.net/2026/Nov/17/gpt62-astra-and-sol/) ⭐️ 7.0/10

OpenAI released GPT-6.2 Astra \(frontier model\) at $8/MTok input and $40/MTok output—20% cheaper than GPT-6 Astra—alongside GPT-6.2 Sol \(efficient model\) at $2/$10, maintaining the same price as previous Sol variants. Cached token pricing dropped significantly to $0.40/million for Astra, down from $1/million. Both models are available in the API as gpt-6.2-astra and gpt-6.2-sol, with LLM 0.38 adding support.

rss · Simon Willison \(AI\) · Nov 17, 22:38

**「Background」** OpenAI&\#x27;s GPT-6 series introduced a two-tier model structure: Astra models serve as frontier/high-performance variants while Sol models offer efficient, lower-cost options. The previous GPT-6 Astra was priced at $10/$50 per million input/output tokens, matching Claude Fable 5.2&\#x27;s pricing. GPT-6 Sol maintained the $2/$10 price point across versions 6 and 6.1, representing half the cost of GPT-5.6 Sol. This release continues the pattern of frontier model pricing reductions, with both Astra and Claude Fable offering their latest versions at 80% of their predecessors&\#x27; prices.

**「Impact」** Developers running long agentic sessions benefit most from the 60% cached token discount on Astra, substantially reducing costs for applications that reuse context. However, early feedback indicates mixed reception—Astra 6.2 reportedly underperforms Claude Fable 5.2 on benchmarks and exhibits confusing communication patterns, including randomly asking users about internal implementation details during extended tasks.

**「Community Discussion」** Theo Browne&\#x27;s pre-release review highlighted problematic behavior where Astra 6.2 interrupts long tasks to ask users about obscure internal details \(e.g., file naming conventions\) that users cannot reasonably answer, describing it as &quot;internal implementation detail bullshit that you could not under any earthly circumstance understand.&quot;

**Tags**: `#openai`, `#llm`, `#gpt-6`, `#ai-models`, `#pricing`

---

## Financial News

<a id="item-finance-news-1"></a>
### [UK Immigration Bill Passes Commons, Moves to Lords](https://www.bloomberg.com/news/articles/2026-11-17/uk-s-house-of-commons-passes-controversial-immigration-bill) ⭐️ 8.0/10

UK House of Commons passed the Immigration and Asylum Bill 290-94, extending standard residency requirements for settlement from 5 to 10 years while allowing healthcare and social care visa holders earning at least £25,000 to remain on a 5-year path; the bill now proceeds to the House of Lords for further review.

telegram · zaihuapd · Nov 18, 05:51

**「Background」** The Immigration and Asylum Bill 2026 implements reforms announced by the UK government in November 2025, representing what the government calls the most significant policy proposals on asylum in a generation. The bill amends both asylum and human rights rules as well as modern slavery legislation, fundamentally reshaping the UK&\#x27;s immigration system.

**「Impact」** The bill extends the standard residency requirement for settlement from 5 to 10 years, directly affecting immigrants seeking permanent UK residency, while allowing healthcare and social care visa holders earning at least £25,000 annually to remain on a faster 5-year path—potentially exacerbating staffing shortages in the NHS and social care sector if workers cannot meet the income threshold.

<details><summary>References</summary>
<ul>
<li><a href="https://commonslibrary.parliament.uk/research-briefings/cbp-10940/">Immigration and Asylum Bill 2026 - House of Commons Library</a></li>
<li><a href="https://www.gov.uk/government/collections/immigration-and-asylum-bill-2026">Immigration and Asylum Bill 2026 - GOV.UK</a></li>
<li><a href="https://nairametrics.com/2025/05/12/uk-to-overhaul-immigration-system-with-10-year-settlement-wait-and-tougher-english-tests/">UK Immigration overhaul: 10 - year residency , tougher... - Nairametrics</a></li>
<li><a href="https://londonmail.uk/increasing-the-10-year-residency-requirement-for-ilr-and-citizenship/">Increasing the 10 - year residency requirement for ILR... - London Mail</a></li>

</ul>
</details>

**Tags**: `#UK policy`, `#immigration`, `#legislation`, `#labor market`, `#healthcare`

---

<a id="item-finance-news-2"></a>
### [China, South Korea Conclude Services, Investment FTA Talks After 8 Years and 8 Months](https://x.com/Jaemyung_Lee/status/2122988472994791476) ⭐️ 8.0/10

China and South Korea announced on November 18 that follow-up negotiations on services and investment under their free trade agreement have substantively concluded after 8 years and 8 months. China committed to granting South Korea most-favored-nation treatment in film and gaming sectors, while expanding market access in tourism, legal services, construction, finance, and other areas. The two sides also agreed to broaden audiovisual co-production from films to include TV dramas, animations, variety shows, and documentaries.

telegram · zaihuapd · Nov 18, 10:02

**「Background」** China and South Korea have been negotiating the services and investment chapter of their existing FTA since March 2018, expanding the original 2015 trade deal beyond goods to cover film, gaming, tourism, legal services, construction, and finance. The agreement grants South Korea most-favored-nation treatment—the same trade terms Korea&\#x27;s competitors receive—in cultural sectors, a significant concession in China&\#x27;s typically restricted media market.

**「Impact」** South Korean entertainment companies, game developers, and service providers gain improved market access to China, while Chinese businesses in affected sectors will face greater competition. The agreement marks a significant step toward normalizing China-South Korea economic relations following recent diplomatic tensions.

<details><summary>References</summary>
<ul>
<li><a href="https://cn.bizhankook.com/articles/korea-china-fta-deal-reached.html">中韩自贸协定（FTA）第二阶段谈判历时8年8个月达成一致……游戏与演出“...</a></li>
<li><a href="https://news.boxwise.top/news/8726">中韩宣布结束自贸协定服务与投资后续谈判 - 行业快讯 - TeuWatch枢讯</a></li>
<li><a href="https://www.asiae.co.kr/cn/article/2026111820070892053">Lee Jaemyung总统谈中国给予韩国文化内容最惠国待遇：“为中韩关系开创...</a></li>

</ul>
</details>

**Tags**: `#中韩关系`, `#自由贸易协定`, `#服务贸易`, `#跨境投资`, `#娱乐产业`

---

<a id="item-finance-news-3"></a>
### [Trump, Xi, Putin Meet at APEC Summit in Shenzhen](https://www.cnbc.com/2026/11/18/apec-trump-xi-putin-shenzhen.html) ⭐️ 7.0/10

World leaders including U.S. President Trump, China&\#x27;s Xi Jinping, and Russia&\#x27;s Putin gather in Shenzhen for the APEC summit, marking the first-ever China-Russia-U.S. trilateral meeting amid low expectations for breakthroughs. The summit tests U.S.-China relations already under strain from Washington&\#x27;s tightened restrictions on AI technology access and the Nvidia controversy, while the existing trade truce extending lower tariffs on $30 billion of goods to January 2027 remains fragile.

rss · CNBC Finance · Nov 18, 06:04

**「Background」** APEC is an annual summit of Asia-Pacific economies meeting this week in Shenzhen, China, where leaders from the U.S., China and Russia will hold the first-ever trilateral meeting. The gathering occurs as U.S.-China relations face new tensions over technology restrictions, including recent scrutiny of Nvidia&\#x27;s China chip sales and the resignation of its CEO over allegations of a relationship with a Chinese spy.

**「Impact」** Technology and manufacturing companies with exposure to U.S.-China trade flows face heightened policy uncertainty as both sides implement tighter restrictions while maintaining the temporary tariff relief agreement.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/world/live/2026/nov/18/apec-summit-live-updates-xi-putin-trump-world-leaders-gather-in-china?page=with:block-6afd75c68f08d72a128dbbf7">Apec summit live: Xi welcomes Trump on China visit as Putin claims...</a></li>
<li><a href="https://sputnikglobe.com/20261117/putin-lands-in-shenzhen-for-apec-summit--and-historic-trilateral-meeting-with-trump--xi-1125082115.html">Putin Lands In Shenzhen for APEC Summit — and Historic Trilateral...</a></li>
<li><a href="https://techcrunch.com/2026/11/17/nvidia-is-abandoning-china-after-jensen-huangs-ouster/">Nvidia is abandoning China after Jensen Huang’s ouster</a></li>
<li><a href="https://www.hindustantimes.com/ht-explainers/us-china-ai-chip-war-nvidia-jensen-huang-export-controls-china-101794288198870.html">The chip war behind the Nvidia&#x27;s Jenson Huang scandal, from ...</a></li>
<li><a href="https://www.reuters.com/world/china/how-nvidia-ceo-jensen-huang-got-entangled-china-chip-spy-scandal-2026-11-11/">How Nvidia&#x27;s Jensen Huang got entangled in a China chip and ...</a></li>

</ul>
</details>

**Tags**: `#geopolitics`, `#trade policy`, `#international relations`, `#economic diplomacy`, `#technology security`

---

<a id="item-finance-news-4"></a>
### [典型A股避损型内幕交易案曝光 监管部门持续打击市场操纵](https://news.google.com/rss/articles/CBMijwFBVV95cUxNSGxEOFpVdGYtT1QxRzVJZFJDdld0U2g0bURvdUdPSm9feVBtTktwVTI4ZlFjOUZ5aHdodlF5RFdvaW9Ib0NaRERVbTJvcE1uRC1SejRPdlN0ODlCWnhSVnpleS13RTdtaGozWVlwTVFwZy1VSjNLd3FDeGJKclA4b0ZSWVZQaXJRNko3RTlxbw?oc=5) ⭐️ 7.0/10

21财经报道一起典型A股避损型内幕交易案例，涵盖消息传递、清仓操作、监管罚单等关键环节，反映监管部门对内幕交易行为的持续打击力度。

rss · Google News 财经 · Nov 18, 03:07

**「背景」** 避损型内幕交易是指内幕信息知情人在信息敏感期内，为避免损失而买卖相关股票的行为，此类型案件是A股市场监管执法重点领域，近年来监管部门持续加强对此类市场操纵行为的查处。

**「影响」** 此类案件对市场参与者具有重要警示意义，彰显监管部门保护投资者权益、维护市场诚信的执法决心，有助于强化市场信息披露制度和内幕交易防控机制。

**Tags**: `#内幕交易`, `#监管执法`, `#A股市场`, `#行政处罚`, `#投资者保护`

---

<a id="item-finance-news-5"></a>
### [Spot Gold Falls Below $3,800 as Rate Hike Expectations Pressurize Prices](https://news.google.com/rss/articles/CBMijwFBVV95cUxNcnpjWUVTYndWTU10MDZFaHZ2LUVwcEYwR0l2VW8wNDFhWU1FN18ybklydnBrUU1VcmpJUENQZDZwNTNKSTlRMHhoYjhuNGdmb3lpOGlSQjNkREdnd0gyRXRoRUNlQXBNbzJZb3ZnV2s3MU4tUmJQNGJKMHZhOTJrMTlGYVJqTHVpYXJjT0FQYw?oc=5) ⭐️ 7.0/10

Spot gold fell below the $3,800 threshold, with prices under pressure as expectations of Federal Reserve interest rate hikes intensified.

rss · Google News 财经 · Nov 18, 05:55

**「Background」** Spot gold fell below $3,800 per ounce for the first time since September 2025, as traders increasingly priced in the possibility of Federal Reserve interest rate hikes in December, January, and April. Rising rate expectations and a strengthening US dollar have been pressuring gold, which typically loses attractiveness when borrowing costs climb.

**「Impact」** Gold investors and ETF holders face mark-to-market losses as higher interest rate expectations strengthen the dollar and increase the opportunity cost of holding non-yielding gold assets.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fxstreet.com/news/breaking-gold-slides-below-3-800-lowest-since-september-2025-on-hawkish-fed-strong-usd-202611180212">Gold falls below $3,800 amid Fed hike bets and firm USD</a></li>
<li><a href="https://tradingeconomics.com/commodity/gold">Gold - Price - Chart - Historical Data - News</a></li>
<li><a href="https://www.cnbc.com/2024/11/11/gold-extends-decline-investors-await-us-data-fed-comments.html">Gold drops over 2% as dollar strengthens; investors await Fed ...</a></li>
<li><a href="https://www.reuters.com/markets/commodities/gold-drifts-higher-traders-eye-us-inflation-print-2024-11-13/">Gold extends fall as dollar, Treasury yields rise | Reuters</a></li>

</ul>
</details>

**Tags**: `#大宗商品`, `#黄金`, `#货币政策`, `#外汇市场`, `#市场走势`

---

<a id="item-finance-news-6"></a>
### [NVIDIA Earnings Lift Storage Stocks Pre-Market](https://news.google.com/rss/articles/CBMib0FVX3lxTE04d01IcEdKV3ZLQUI2RmtSdDRVejVFRE1JbWtzOWE2Q3hRNDQ4Zm9HS0M2R3BCLWJMS2E4OVYzR2NRRGRpU2JQZF9oVlRLbXMzRVlEay1XM0U3UHYzVWxxMWdVOWVCRm4zLVdQQnJwNA?oc=5) ⭐️ 7.0/10

NVIDIA&\#x27;s strong quarterly earnings drove pre-market gains in storage stocks, with SanDisk and SK Hynix each climbing more than 4%.

rss · Google News 财经 · Nov 18, 09:22

**「Background」** NVIDIA is a major purchaser of memory chips for its AI data center GPUs, and its earnings are closely watched as a barometer for semiconductor demand trends.

**「Impact」** Storage chip makers stand to benefit from expectations that continued AI infrastructure buildout will sustain memory demand, as NVIDIA&\#x27;s results signal persistent strong demand for computing hardware.

**Tags**: `#earnings`, `#market movement`, `#technology sector`

---