---
layout: default
title: "Horizon Summary: 2026-11-13 (EN)"
date: 2026-11-13
lang: en
---

> From 218 items, 9 important content pieces were selected

---

**Technology News**
1. [Rust 1.100 stabilizes never type, custom allocators, adds dependency cooldowns and unused dependency detection](#item-tech-news-1) ⭐️ 9.0/10
2. [Developer replaces $300 embroidery machine&\#x27;s subscription firmware with open-source Zig app](#item-tech-news-2) ⭐️ 8.0/10
3. [Smolmaxxing runs 16B-parameter LLMs on iPad Air \(1st gen\) and sub-1GB RAM devices](#item-tech-news-3) ⭐️ 8.0/10
4. [Anthropic files for IPO with $968B implied market cap and $900.9B compute commitments](#item-tech-news-4) ⭐️ 8.0/10
5. [PostgreSQL CVE-2026-6460: 22-year-old type-confusion primitive weaponized to RCE](#item-tech-news-5) ⭐️ 8.0/10
6. [China&\#x27;s First Electricity-Hydrogen-Derivatives Coupling Large Model Published in Nature](#item-tech-news-6) ⭐️ 7.0/10
7. [Chinese AI firms seek non-U.S. NVIDIA chip capacity amid U.S. export restrictions](#item-tech-news-7) ⭐️ 7.0/10

**Financial News**
1. [Oil Prices Jump After Trump Claims U.S. &\#x27;Has&\#x27; Strait of Hormuz](#item-finance-news-1) ⭐️ 7.0/10
2. [US October CPI beats expectations, raising Fed rate hike odds](#item-finance-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Rust 1.100 stabilizes never type, custom allocators, adds dependency cooldowns and unused dependency detection](https://blog.rust-lang.org/2026/11/12/Rust-1.100.0/) ⭐️ 9.0/10

Rust 1.100, released on November 12, 2026, stabilizes the never type \(\`\!\`\) and custom allocators, introduces &\#x27;dependency cooldowns&\#x27; \(RFC 3923\) that ignore newly published crate versions unless already present in \`Cargo.lock\`, makes \`cargo install\` lockfile-aware by default \(rendering \`--locked\` a no-op\), and adds built-in detection of unused dependencies—enabled by default with \`warn\` level for \`cargo::unused\_dependencies\`. These changes apply to all Rust users targeting stable toolchains and require Cargo 1.100+; no breaking changes are introduced, but existing \`Cargo.toml\` files may now trigger new warnings or require resolver configuration updates to accommodate cooldown policies.

hackernews · mbStavola · Nov 12, 18:39 · [Discussion](https://news.ycombinator.com/item?id=50472038)

**「Prerequisites for Rust 1.100」** The never type \(\`\!\`\) was previously unstable and used only in niche contexts like diverging functions; its stabilization in 1.100 makes it a first-class part of the type system for expressing unreachable code and improving exhaustiveness checking. Custom allocators were introduced experimentally in earlier versions \(e.g., via \`\#\[global\_allocator\]\` and the \`alloc\` crate\), but the Allocator API—enabling fine-grained memory control in \`no\_std\` and embedded contexts—was not fully stabilized until this release.

**「Impact」** Developers will see new compiler warnings for unused dependencies \(e.g., \`tracing-subscriber.workspace = true\` flagged as unused\), and projects using \`cargo install\` from \`.crate\` tarballs must ensure those archives contain valid \`Cargo.lock\` files—otherwise installation may fail or behave differently than before.

**「Community discussion」** Commenters highlight the stabilization of the never type and custom allocators as personal favorites, while others note significant undocumented API additions like \`bool::toggle\(\)\` and \`Box::map\(\)\`, and one user expresses concern about persistent compilation performance and disk usage despite the release’s tooling improvements.

**Tags**: `#rust`, `#systems-programming`, `#cargo`, `#memory-safety`, `#developer-tools`

---

<a id="item-tech-news-2"></a>
### [Developer replaces $300 embroidery machine&\#x27;s subscription firmware with open-source Zig app](https://github.com/simpsoka/zigzag) ⭐️ 8.0/10

A developer reverse-engineered the firmware of a $300 consumer embroidery machine and replaced its proprietary, subscription-dependent software with an open-source application written in Zig, enabling local control without recurring fees. The app, named Zigzag, interfaces directly with the machine’s hardware—bypassing vendor lock-in—and is published on GitHub. It is a functional, user-built alternative to the original firmware, not merely a design or proposal; the source content confirms it runs on actual hardware and eliminates the need for paid subscriptions.

hackernews · simpsoka · Nov 12, 17:02 · [Discussion](https://news.ycombinator.com/item?id=50470488)

**「Proprietary embroidery machine firmware and subscription lock-in」** Many consumer embroidery machines—especially lower-cost models like the $300 device in question—rely on proprietary firmware that enforces subscription-based access to core functionality such as design loading, editing, or machine control. This model often replaces traditional one-time-purchase software with cloud-dependent services, limiting offline use and long-term ownership rights.

**「Impact」** Embroidery machine owners can now bypass mandatory subscriptions and proprietary firmware locks by flashing the open-source Zigzag app onto compatible $300 machines, restoring local control and eliminating recurring fees—mirroring similar community efforts like Owen Trueblood’s Brother PE-150 motherboard replacement.

**「Community discussion」** Commenters highlight how this project exemplifies user empowerment against entrenched &\#x27;Big Embroidery&\#x27; practices, citing widespread frustration with expensive, outdated, and cartridge-locked software ecosystems; one commenter notes their own similar effort building embroiderybreeze.com after their spouse struggled with commercial tools.

<details><summary>References</summary>
<ul>
<li><a href="https://owentrueblood.com/blog/2024/12/10/reverse-engineering-the-brother-pe-150-embroidery-machine/">Reverse Engineering the Brother PE - 150 Embroidery Machine</a></li>

</ul>
</details>

**Tags**: `#embedded-systems`, `#open-source`, `#reverse-engineering`, `#hardware-interfacing`, `#consumer-hardware`

---

<a id="item-tech-news-3"></a>
### [Smolmaxxing runs 16B-parameter LLMs on iPad Air \(1st gen\) and sub-1GB RAM devices](https://github.com/hyperionaidev/smolmaxxing/) ⭐️ 8.0/10

The open-source project Smolmaxxing enables inference of 16-billion-parameter LLMs on legacy devices with less than 1 GB of usable RAM—specifically the iPad Air \(1st gen\) and Xiaomi TV boxes—using custom GPU kernels and model modifications. The optimized models are publicly available on Hugging Face under the namespace &\#x27;hyperionaidev&\#x27;, and the inference kernels are open-sourced on GitHub. This is a shipped, reproducible capability—not an announcement or roadmap—and relies on systems-level optimizations beyond standard quantization, including memory-efficient kernel implementations tailored for older hardware.

hackernews · mrashad74 · Nov 12, 15:23 · [Discussion](https://news.ycombinator.com/item?id=50468888)

**「Background」** Running large language models on devices with under 1 GB of RAM requires overcoming severe memory and compute constraints—far beyond standard quantization—by combining custom inference kernels, model architecture modifications \(e.g., sparse or dense variants\), and low-level hardware exploitation \(e.g., NEON without dot-product support on the Apple A7\). Prior work like llama.cpp established portable CPU-based LLM inference, but smolmaxxing extends it to legacy ARM devices through MIT-licensed patches and Hugging Face-hosted adapted models.

**「Enables local LLM inference on legacy consumer hardware with &lt;1GB RAM」** Developers and hobbyists can now run 16B-parameter LLMs—such as modified models from Hugging Face \(hyperionaidev\) —on off-the-shelf, memory-constrained devices like the iPad Air \(1st gen\) and Xiaomi TV boxes \(&lt;1GB usable RAM\), using open-sourced custom kernels and quantization-aware optimizations; this removes reliance on cloud APIs or modern edge accelerators for basic inference tasks.

**「Community discussion」** Commenters highlight both enthusiasm and pragmatic skepticism: one user notes that modern LLM agents can already bootstrap inference on old hardware via SSH-accessible compute, while another asks whether models this small retain practical utility for real-world tasks. The project maintainer confirms current deployment on specific low-memory devices and invites community contributions toward even more constrained targets.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/hyperionaidev/smolmaxxing">GitHub - hyperionaidev/smolmaxxing: maxxing the ability to ...</a></li>
<li><a href="https://github.com/hyperionaidev/smolmaxxing/tree/main">GitHub - hyperionaidev/smolmaxxing: maxxing the ability to ...</a></li>
<li><a href="https://ai-tldr.dev/tools/smolmaxxing/">smolmaxxing GitHub: LLMs on a TV box and an old iPad | AI/TLDR</a></li>

</ul>
</details>

**Tags**: `#edge-ai`, `#llm-optimization`, `#systems-programming`, `#open-source-ai`, `#low-resource-computing`

---

<a id="item-tech-news-4"></a>
### [Anthropic files for IPO with $968B implied market cap and $900.9B compute commitments](https://ipo.anthropic.com/us/) ⭐️ 8.0/10

Anthropic filed an S-1 registration for an initial public offering on Nasdaq under ticker ANT, with a price range of $70–$78 per share, implying a $968 billion market cap at the midpoint. The filing discloses $85.3 billion in gross proceeds \($59.3B IPO + $26B private placement\), $81 billion in annualized revenue as of October 2026, and $900.9 billion in committed compute expenditures through 2045. It also reports over 11,900 customers generating at least $100K in trailing-twelve-month revenue, and approximately 40 million customers under $100K. These figures represent disclosed financial and operational commitments—not independently verified results or shipped product metrics.

hackernews · josephljohnston · Nov 12, 11:46 · [Discussion](https://news.ycombinator.com/item?id=50465829)

**「IPO filing and regulatory submission」** Anthropic, PBC filed its initial Form S-1 registration statement with the U.S. Securities and Exchange Commission on October 26, 2026, under registration number 333-299633, disclosing its intent to list Class A common stock on the Nasdaq Global Select Market under the ticker ANT. An amended S-1 filed on November 2, 2026 added updated Q3 2026 financials and other disclosures required for IPO readiness.

**「Impact」** The scale of Anthropic’s disclosed compute commitments \($900.9B through 2045\) and run-rate revenue \($81B\) sets a new benchmark for infrastructure intensity and commercial velocity in AI, raising concrete questions for developers and enterprises about long-term vendor lock-in, cost predictability, and the sustainability of centralized inference economics.

**「Community discussion」** Commenters express skepticism about the business model’s durability, with one noting that users can easily switch to cheaper models for most tasks outside chat interfaces, and another arguing that rapidly improving local models and affordable AI hardware will erode Anthropic’s moat; these views reflect concerns about technical substitutability rather than consensus on valuation or timing.

<details><summary>References</summary>
<ul>
<li><a href="https://www.mexc.com/learn/article/where-is-anthropics-s-1-inside-the-anthropic-ipo-filing-june-2026/1">Where Is Anthropic&#x27;s S-1? Inside the Anthropic IPO Filing and ...</a></li>
<li><a href="https://www.cnbc.com/2026/11/02/anthropic-ant-s-1-quarter-financials.html">Anthropic releases amended IPO prospectus with Q3 financials</a></li>
<li><a href="https://www.anthropic.com/news/s1-sec">Anthropic files S-1 with the SEC for proposed initial public ...</a></li>

</ul>
</details>

**Tags**: `#artificial-intelligence`, `#machine-learning`, `#software-engineering`, `#open-source`, `#technology-industry`

---

<a id="item-tech-news-5"></a>
### [PostgreSQL CVE-2026-6460: 22-year-old type-confusion primitive weaponized to RCE](https://mehmetince.net/part-3-6-how-i-ended-up-turning-a-22-year-old-postgresql-type-confusion-primitive-into-rce-cve-2026-6460/) ⭐️ 8.0/10

A researcher demonstrated remote code execution \(RCE\) in PostgreSQL by exploiting a 22-year-old type-confusion vulnerability \(CVE-2026-6460\) through prepared statement state inconsistency—specifically, by creating a prepared statement on a table, altering the table’s structure \(e.g., column type or order\), and then executing the stale prepared statement, triggering memory corruption. The exploit requires authenticated database access and targets PostgreSQL server processes, not client applications. It was confirmed to achieve arbitrary code execution on the database server host under standard configurations, not merely privilege escalation within the database. The vulnerability affects all PostgreSQL versions prior to the patch released alongside the disclosure.

hackernews · ozirus · Nov 12, 18:22 · [Discussion](https://news.ycombinator.com/item?id=50471761)

**「Background」** PostgreSQL&\#x27;s prepared statement mechanism caches query plans for reuse, assuming schema stability; a type-confusion vulnerability arises when the underlying table definition changes \(e.g., column type or structure\) after preparation but before execution, causing the cached plan to misinterpret memory layout. This class of inconsistency has existed since at least PostgreSQL 7.2 \(released in 2002\), and prior advisories have treated related issues as denial-of-service or privilege escalation rather than remote code execution.

**「Remote code execution as the database OS user」** Authenticated PostgreSQL users with object-creation privileges can execute arbitrary code on the database server as the operating system user running PostgreSQL \(e.g., \`postgres\`\), by exploiting CVE-2026-6460 via prepared statement state inconsistency after \`ALTER ... SET DATA TYPE\`. This affects PostgreSQL versions 14.25, 15.20, 16.16, 17.12, 18.7, and 19 RC 2, and requires no additional privileges beyond those needed to create objects and prepare statements.

**「Community discussion」** Several commenters—including \[logophobia\], \[jmuguy\], and \[ahartmetz\]—questioned whether the exploit constitutes true remote code execution or instead represents authenticated privilege escalation, noting that it requires prior database account access and operates within the PostgreSQL backend process context. Others, like \[igbanam\] and \[sailfast\], praised the write-up for its transparency and educational value in exposing PostgreSQL internals and exploit development reasoning.

<details><summary>References</summary>
<ul>
<li><a href="https://www.postgresql.org/support/security/CVE-2026-6460/">PostgreSQL : CVE - 2026 - 6460 : PostgreSQL type confusion after...</a></li>
<li><a href="https://security-tracker.debian.org/tracker/CVE-2026-6460">CVE - 2026 - 6460</a></li>

</ul>
</details>

**Tags**: `#PostgreSQL`, `#memory-safety`, `#exploit-development`, `#database-security`, `#vulnerability-research`

---

<a id="item-tech-news-6"></a>
### [China&\#x27;s First Electricity-Hydrogen-Derivatives Coupling Large Model Published in Nature](https://news.google.com/rss/articles/CBMicEFVX3lxTFBBTkkxbDhPWUtMbDllV2NKQklwcXpxZlE2ZDJhcHgtOHBsN2t0MmhBU2MweTVpTUU4LTV1X3hEZkdWX2RicExIN0JhU3dzbXh6aVlXeGE2cGFMcVNseWFZcFRvWHRoUy0zZE5ETUdQUlM?oc=5) ⭐️ 7.0/10

A large-scale computational model integrating electricity supply, green hydrogen production, and downstream chemical derivatives—developed in China—has been published in the journal Nature. The model is described as the first of its kind in China to couple these three energy and industrial system domains at scale. However, the source provides no technical details such as model architecture, training data, validation methodology, performance metrics, software availability, or versioning. No information is given about release date, open access status, licensing, or compatibility with existing energy system modeling tools.

rss · Google News AI · Nov 13, 03:30

**「Background」** Coupling electricity generation, hydrogen production \(e.g., via electrolysis\), and downstream chemical synthesis \(e.g., ammonia or methanol\) is a key strategy for sector-coupled decarbonization, requiring integrated modeling of energy conversion efficiency, temporal matching of renewable supply and demand, and chemical process constraints. Prior work has addressed subsets—such as co-optimizing wind farm siting and electrical export infrastructure \(tool-1-2\) or electrochemical hydrogenation of organics using water \(tool-1-3\)—but no previously published model has jointly represented all three layers—electricity, hydrogen, and derivatives—at large scale with empirical validation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sciencedirect.com/science/article/pii/S0306261926015758">Investment-operation co-optimization of layered electricity ...</a></li>
<li><a href="https://www.nature.com/articles/s41570-024-00589-z">Electrochemical hydrogenation and oxidation of organic ...</a></li>

</ul>
</details>

**Tags**: `#energy-systems`, `#ai-for-science`, `#sustainable-computing`

---

<a id="item-tech-news-7"></a>
### [Chinese AI firms seek non-U.S. NVIDIA chip capacity amid U.S. export restrictions](https://news.google.com/rss/articles/CBMi4gNBVV95cUxPcHExa1hPcFdKMTVkUkgya1gzTWpGNFY3SmJHc1pEdVpOU05rRkZqRDFwZTQ2TVVEUzhSNE5COGdMLUI0V20tNEJRWjJ5NzkwYy0tOW5SUjd5akdWMEd0bjZzRzNTUHpnYjdlR2ZWUWVJVlY5SUZWSG1ROHhiTTdEOEVobDNvVkZfU0ZSWnNFakRLaGx5a0s5bU00VFc1eWRKZ3VhLUhGUXlFeUhwMHFnNDdwVXJjU3BvSy0yeXU4X2twRlR2a2g3QWlaT2g5VTdfWXlXcnBTcFFjbHpEdUtEdFlrcnM3aUZFSVRudzBMbWhvSG1wU1dpemZzTDNTQXFURHpBRVgxRzhCYl9XamlqSXdKR2lGU0xoUlJqWGc2eFN2dlJ4NU9YeUtIdTg1V1J3MEg5TDJTREgxelNkaEFHc2F3eURpcDVGY25ldWoxYXNDbG40aWFpN2Rrckx0QUJlOWgtdW0wVmR6NUZJbTVuZnlGZXhoUDBOcVZ2NW51bmZvRjRnZWRITm1DMXJOTFlXUVAzNldmdXRNV0JrbmtVMWYtT0VUa0J2ZnJuY2hidlJlN2xJMjhUcmF2eVNYVlF6dG9CVVlMemY5TDdkN2Q5VW9CaWwxejZyc0YzNVE5SlRPdw?oc=5) ⭐️ 7.0/10

Chinese AI companies are urgently securing access to NVIDIA GPU production capacity outside the United States, following intensified U.S. export controls tied to espionage-related national security concerns. These restrictions specifically target advanced AI chips—including A100, H100, and newer models—and apply to shipments both directly from U.S. soil and via third countries where U.S. jurisdiction or licensing requirements still apply. The effort reflects a race to lock in supply before further tightening, but does not indicate newly approved exceptions or changes to NVIDIA’s official export compliance posture.

rss · Google News AI · Nov 12, 15:42

**「Background」** U.S. export controls on NVIDIA AI chips for China have been progressively tightened since 2022, with successive rule updates \(e.g., October 2023 and March 2024\) restricting sales of high-end datacenter GPUs like the A100, H100, and later the B200 and Blackwell-based chips. The current escalation follows recent reports—cited in multiple outlets—that NVIDIA CEO Jensen Huang is under internal investigation over an alleged affair with a suspected Chinese intelligence operative, prompting renewed congressional scrutiny and plans for stricter enforcement of existing restrictions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.politico.com/news/2026/11/09/nvidias-spy-scandal-china-chips-01156241">Nvidia’s spy scandal hands Hill hawks fresh ammo on China chips</a></li>
<li><a href="https://techcrunch.com/2026/11/09/jensen-huangs-affair-with-alleged-chinese-spy-puts-nvidias-china-ambitions-under-scrutiny/">Jensen Huang’s affair with alleged Chinese spy puts Nvidia’s ...</a></li>
<li><a href="https://www.atlanticcouncil.org/dispatches/beyond-the-spy-scandal-what-the-nvidia-megaspeed-case-reveals-about-export-controls/">Beyond the spy scandal: What the Nvidia-Megaspeed case ...</a></li>

</ul>
</details>

**Tags**: `#AI-hardware`, `#semiconductor-geopolitics`, `#export-controls`, `#AI-infrastructure`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Oil Prices Jump After Trump Claims U.S. &\#x27;Has&\#x27; Strait of Hormuz](https://www.cnbc.com/2026/11/12/oil-prices-jump-after-trump-says-no-iran-deal-needed-weve-got-their-strait.html) ⭐️ 7.0/10

Brent crude rose 3.3% to $95.82 per barrel and West Texas Intermediate \(WTI\) rose 2.6% to $88.74 per barrel on Thursday after Donald Trump posted on Truth Social that the U.S. &\#x27;has&\#x27; Iran&\#x27;s Strait of Hormuz and does not need a deal with Iran.

rss · CNBC Finance · Nov 13, 00:01

**「Background」** Trump’s statement reversed earlier market relief from his post-midterm comments suggesting de-escalation, including that fresh U.S. strikes on Iran were &\#x27;highly unlikely&\#x27; and military action &\#x27;did not appear necessary at this point&\#x27;.

**「Impact」** The remarks immediately raised the &\#x27;security premium&\#x27; in oil prices, as investors reassessed risks to shipping through the Strait of Hormuz—a waterway handling about 20% of global oil trade.

**Tags**: `#oil markets`, `#geopolitical risk`, `#Strait of Hormuz`, `#U.S.-Iran relations`

---

<a id="item-finance-news-2"></a>
### [US October CPI beats expectations, raising Fed rate hike odds](https://news.google.com/rss/articles/CBMiYkFVX3lxTFBfNVpCdUJrYVBpeUpidlMzM0FPT0V4Q2pzZzVEcDg2MUxySnhzNS1peW41NFRveEtvbW5rMW9POEtOa2p5R0VxdU50X0p0bkhWbjllMnlRTXdhcTNERWMtSXZR?oc=5) ⭐️ 7.0/10

US October 2026 consumer price index \(CPI\) came in higher than forecast, increasing market expectations for additional Federal Reserve interest rate hikes.

rss · Google News 财经 · Nov 13, 06:55

**「Background」** The U.S. Bureau of Labor Statistics released October 2026 CPI data on November 10, showing a 0.4% monthly increase—down from 0.6% in September but above economists’ expectations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/10/october-2026-cpi-inflation-breakdown.html">Here&#x27;s the inflation breakdown for October 2026 — in one chart</a></li>
<li><a href="https://www.financecalendar.com/event/us-cpi-report-november-2026/">US CPI Report: 2026 -10 — Tuesday, 10 November... | Finance Calendar</a></li>

</ul>
</details>

**Tags**: `#inflation`, `#monetary-policy`, `#equity-markets`

---