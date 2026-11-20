---
layout: default
title: "Horizon Summary: 2026-11-20 (EN)"
date: 2026-11-20
lang: en
---

> From 211 items, 15 important content pieces were selected

---

**Technology News**
1. [Claude solves two open problems in black hole physics](#item-tech-news-1) ⭐️ 9.0/10
2. [PostgreSQL 19 Adds WAIT FOR LSN for Read-Your-Writes on Standbys](#item-tech-news-2) ⭐️ 9.0/10
3. [Anthropic Goes Public on Nasdaq in Record AI IPO](#item-tech-news-3) ⭐️ 9.0/10
4. [FFmpeg 9.1 &\#x27;Gauss&\#x27; Released with New Codecs, Vulkan Encoder, and Improved AAC](#item-tech-news-4) ⭐️ 8.0/10
5. [PHP&\#x27;s mishandling of uppercase &\#x27;S&\#x27; in HTTPS scheme silently disables TLS, fixed after 20 years](#item-tech-news-5) ⭐️ 8.0/10
6. [UK Tribunal Forces Public Hearing on Government’s Secret iPhone Encryption Backdoor Order](#item-tech-news-6) ⭐️ 8.0/10
7. [US Approved 880,000 AI Chips for China, No Shipments Yet](#item-tech-news-7) ⭐️ 8.0/10
8. [Chinese AI Giants Adjust Safety Strategies, Third-Party Inspectors Deployed](#item-tech-news-8) ⭐️ 7.0/10
9. [Micron President Warns AI Storage Shortages Will Worsen by 2027](#item-tech-news-9) ⭐️ 7.0/10
10. [AI Power Policies Surge, but Storage and Data Shortfalls Persist](#item-tech-news-10) ⭐️ 7.0/10
11. [Taotian Group Gets 7 Papers Accepted at KDD 2027, Including LLM-Discovered Bidding Algorithms](#item-tech-news-11) ⭐️ 7.0/10
12. [CNKI’s AI detection rate surge alarms academic authors](#item-tech-news-12) ⭐️ 7.0/10

**Financial News**
1. [A-Shares Extend Losing Streak to Seven Days with Over 4,000 Stocks Down; Broad ETF Volume Spikes at Close](#item-finance-news-1) ⭐️ 8.0/10
2. [ICBC Reclaims Crown as China&\#x27;s Most Valuable A-Share Company](#item-finance-news-2) ⭐️ 7.0/10
3. [Baidu turns loss into 1.4 billion yuan profit as AI revenue exceeds 50%](#item-finance-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Claude solves two open problems in black hole physics](https://www.anthropic.com/research/claude-black-hole-physics) ⭐️ 9.0/10

Anthropic announced that Claude \(the newly released Fable 5.2 model\) solved two open problems in black hole physics: an error-prone bootstrap calculation and a proof establishing an upper bound on black hole mass for a consistent quantum gravity theory with a given central charge. The result, which implies any theory exceeding that mass bound cannot describe quantum gravity in that universe, was detailed in a Hexagon entry and two research papers, though the technical exposition was noted as dense. The claim appeared as a launch highlight rather than a peer-reviewed finding.

hackernews · cybermango · Nov 19, 17:30 · [Discussion](https://news.ycombinator.com/item?id=50563148)

**「Background」** The search for a consistent theory of quantum gravity has long relied on black hole physics, where two open problems involved calculating complex properties of black holes and proving an upper bound on black hole mass compatible with a given central charge—a condition for a theory to be a valid quantum gravity theory.

**「Community Discussion」** A physicist commenter cautioned that the phrase &\#x27;open problem&\#x27; often refers to specialized research questions and does not necessarily signal a major breakthrough, while another user observed that the papers list no human authors, raising novel questions about attribution norms in AI-driven research.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/research/claude-black-hole-physics">Claude solves two open problems in the physics of black holes</a></li>

</ul>
</details>

**Tags**: `#ai`, `#physics`, `#black-holes`, `#claude`, `#scientific-research`

---

<a id="item-tech-news-2"></a>
### [PostgreSQL 19 Adds WAIT FOR LSN for Read-Your-Writes on Standbys](https://simonwillison.net/2026/Nov/19/postgresql-19/) ⭐️ 9.0/10

PostgreSQL 19 was released on November 19, 2026, two months later than typical after developers addressed a surge of AI-reported vulnerabilities. The release adds the WAIT FOR LSN command, enabling read-your-writes consistency on standby replicas by having a session on the standby wait until a specified log sequence number has been replayed. An optional timeout can raise an error if the standby does not catch up within the given interval.

rss · Simon Willison \(AI\) · Nov 19, 20:43

**「Background」** In primary-standby PostgreSQL clusters, reads often go to read replicas, but replication lag can cause a client to not see its own writes. Previously, developers had to implement application-level tracking of replication positions, as seen in MediaWiki&\#x27;s MySQL-based workaround. WAIT FOR LSN provides a built-in server-side wait for a specific WAL position.

**「Impact」** Developers can now implement read-your-writes consistency without custom replication tracking, simplifying application code for setups that distribute reads to standby servers.

**「Community Discussion」** One commenter described WAIT FOR LSN as a &quot;game-changer&quot; for read replicas, while another considered this the most bug-free .0 release and questioned whether waiting for a later point release is still necessary.

**Tags**: `#postgresql`, `#databases`, `#release`, `#consistency`, `#open-source`

---

<a id="item-tech-news-3"></a>
### [Anthropic Goes Public on Nasdaq in Record AI IPO](https://news.google.com/rss/articles/CBMi0AJBVV95cUxOa1JXZ2llZ3BVUXdmUEVWb1h6blRkOFNfaFgwNjFxS1B0RDZyUVA0b3Rkc1plVGJBYmlaQVo2QjJaWkVBMW9JMXp4YWZoUjFHVUttZUZqeE96WGs4dFk0SnEyZGNPUk9ZYmVTVktINmlqSFAzazVqN25Zc2hScXQyblRVRUJrQnB1VGVWTUswZGRSYW0tQlc5Z25JT211dVh3WVU3dmc0TlRMUmpXYjd4aDdhUEw2Tk1tX1NmLW9DQTd3UzNtMFVxQmdUanM1alkzZFcyUkRuMGxWU194eS15QTBFQ3Z0MWlyQXl4UUNCNTR5MkhOaENtTzJaOXpLQUxlVW50QVdoaFR3c19TalM5bHNtYk52U2xXWVlrakc2Vngwbkx6Q0E3WGEwMlZLT1JRYVhnendsWHgzdXVQaGtsUXI2aEZnOW5CWnVJSDdYM2c?oc=5) ⭐️ 9.0/10

AI company Anthropic began trading on the Nasdaq stock exchange on November 19, 2026, in what the reporting describes as a record-setting initial public offering, potentially the largest on record for an artificial intelligence company. No specific financial figures—such as valuation, share price, or total capital raised—were available in the provided source material.

rss · Google News AI · Nov 19, 18:15

**「AI company IPO milestone」** Anthropic is the first major AI company to go public; competitor OpenAI has reportedly pushed its IPO to 2027. The offering surpasses SpaceX’s June listing as the largest IPO in history.

<details><summary>References</summary>
<ul>
<li><a href="https://www.france24.com/en/business/20261119-anthropic-begins-trading-1-5-trillion-company-biggest-ipo-record-ai">Anthropic blows past $2 trillion in Nasdaq debut, beating... - France 24</a></li>
<li><a href="https://www.dw.com/en/anthropic-trading-tests-investors-appetite-for-ai/a-79993163">Anthropic trading tests investors&#x27; appetite for AI</a></li>

</ul>
</details>

**Tags**: `#artificial intelligence`, `#IPO`, `#Anthropic`, `#Nasdaq`, `#technology industry`

---

<a id="item-tech-news-4"></a>
### [FFmpeg 9.1 &\#x27;Gauss&\#x27; Released with New Codecs, Vulkan Encoder, and Improved AAC](https://ffmpeg.org/download.html#release_9.1) ⭐️ 8.0/10

FFmpeg 9.1, codenamed &\#x27;Gauss&\#x27;, has been released, introducing the ASTC image codec via libastcenc, an APV Vulkan video encoder, NVDEC CUARRAY hardware acceleration, and a significantly improved AAC encoder. The update also adds LCEVC payload merging as a bitstream filter, the libcurl network protocol, a new AMF Video Quality Enhancer filter, and support for DVD-Audio LPCM demuxing. These capabilities are available now and extend FFmpeg&\#x27;s handling of modern codecs and GPU-accelerated workflows for developers and media pipelines.

hackernews · gyan · Nov 20, 04:02 · [Discussion](https://news.ycombinator.com/item?id=50569998)

**「Background」** FFmpeg is the widely used open-source multimedia framework for decoding, encoding, and streaming audio and video. The 9.1 point release builds on this tooling by expanding codec support and hardware acceleration options.

**「Impact」** The extensively reworked AAC encoder can deliver higher perceptual audio quality at lower bitrates, directly benefiting streaming services and content creators who rely on AAC for distribution.

**Tags**: `#open-source`, `#ffmpeg`, `#multimedia`, `#video-processing`, `#codecs`

---

<a id="item-tech-news-5"></a>
### [PHP&\#x27;s mishandling of uppercase &\#x27;S&\#x27; in HTTPS scheme silently disables TLS, fixed after 20 years](https://x.com/ljachowicz/status/2123477025268924514) ⭐️ 8.0/10

PHP&\#x27;s HTTP/FTP stream wrapper previously ignored the case of the scheme but only enabled TLS when the fifth character was a lowercase &\#x27;s&\#x27;. This meant URLs like HTTPS://, httpS://, and FTPS:// were silently downgraded to plaintext, exposing authentication data and request bodies. The vulnerability \(CVE-2026-128064, CVSS 8.2\) went unnoticed for 20 years. It is fixed in PHP 8.2.36, 8.3.37, 8.4.28, 8.5.13, and 8.6.0; earlier end-of-life versions remain unpatched, requiring users to normalize URL schemes to lowercase.

telegram · zaihuapd · Nov 20, 03:04

**「Background」** PHP&\#x27;s HTTP/FTP stream wrapper accepts URL schemes case-insensitively but historically required the fifth character to be a lowercase &\#x27;s&\#x27; to activate TLS encryption. This meant that variants like &quot;HTTPS://&quot; or &quot;httpS://&quot; were treated as plain text HTTP/FTP, leaving credentials, tokens, and other sensitive data exposed.

**「Impact」** Applications using affected PHP versions that construct URLs with an uppercase &\#x27;S&\#x27; in the scheme risk leaking credentials and sensitive data over plain HTTP/FTP; redirects to such URLs also trigger the downgrade, so developers must ensure scheme normalization on EOL versions.

**Tags**: `#PHP`, `#security`, `#vulnerability`, `#TLS`, `#stream-wrapper`

---

<a id="item-tech-news-6"></a>
### [UK Tribunal Forces Public Hearing on Government’s Secret iPhone Encryption Backdoor Order](https://appleinsider.com/articles/26/11/19/uk-cant-hide-that-it-tried-ordering-apple-to-allow-access-to-user-data) ⭐️ 8.0/10

The UK Investigatory Powers Tribunal ruled in Apple’s favor, ending the Home Office’s ability to keep secret its demand for backdoor access to encrypted iPhone data; the majority of the case will now be heard publicly. The Home Office later confirmed it had issued a Technical Capability Notice \(TCN\), claiming it was meant to bring criminals to justice. The tribunal dismissed the national security justification as “unrealistic.”

telegram · zaihuapd · Nov 20, 04:13

**「Background」** Under the UK&\#x27;s Investigatory Powers Act 2016, the Home Office can secretly issue a Technical Capability Notice \(TCN\) compelling a company to bypass encryption on devices. These orders typically include a gag clause forbidding the recipient from acknowledging their existence. The tribunal ruling is the result of Apple&\#x27;s challenge to the Home Office&\#x27;s attempt to maintain that secrecy.

**「Impact」** By forcing public disclosure, the ruling undercuts the Home Office’s ability to secretly issue Technical Capability Notices that require tech companies to weaken encryption, thereby strengthening legal protections for end‑to‑end encrypted data in the UK and setting a precedent for similar challenges elsewhere.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/11/19/u-k-government-forced-to-disclose-secret-apple-backdoor-order/">UK government forced to disclose secret Apple backdoor order</a></li>

</ul>
</details>

**Tags**: `#encryption`, `#privacy`, `#Apple`, `#government surveillance`, `#tech policy`

---

<a id="item-tech-news-7"></a>
### [US Approved 880,000 AI Chips for China, No Shipments Yet](https://foreignaffairs.house.gov/news/press-releases/chairman-brian-mast-exercises-legislative-authority-to-publicly-release-ai-chip-license-information-for-china) ⭐️ 8.0/10

The US House Foreign Affairs Committee released licensing data showing that from December 2025 to May 2026, the government approved 879,868 AI chip exports to China, including NVIDIA H200 and AMD MI325X, for companies such as Tencent, ByteDance, Alibaba, Kuaishou, and Didi. The approved licenses covered only about a quarter of the 3.44 million chips requested, and as of May 11, none of the 21 approved licenses had resulted in actual shipments.

telegram · zaihuapd · Nov 20, 04:25

**「Background」** The committee’s release provides rare public visibility into US export licensing for advanced AI chips to China, revealing the gap between approved volumes and actual deliveries. Both the H200 and MI325X are subject to US export controls intended to restrict China’s access to high-performance AI accelerators, and several recipients, including Alibaba, Tencent, Baidu, and BYD, are on a US list of entities with alleged military ties.

**Tags**: `#AI chips`, `#export controls`, `#US-China trade`, `#NVIDIA`, `#AMD`

---

<a id="item-tech-news-8"></a>
### [Chinese AI Giants Adjust Safety Strategies, Third-Party Inspectors Deployed](https://news.google.com/rss/articles/CBMijwFBVV95cUxPaHFUbnlDbnlGM2xidm5Vckw0N05pSGVyendyQzZXZWpnSlBjR211Q0lhWXp1ZDQtMVhfY3U1d2ZSTjNoMEtxZUM1Y1N1TzdVWmNZeml1T0h4QUItNVdHN1dDVFRQQmVmSVlrc25hRE5LMmNGT2tBMmZLOFpWbzJ0NWpHdTZkQURmZTdwTzF5aw?oc=5) ⭐️ 7.0/10

Multiple major AI companies in China are collectively revising their safety strategies and have begun placing third-party inspectors within their offices, according to a report from 21财经. The firms are implementing external oversight as part of a broader shift in AI governance. Specific company names, the number of inspectors, or the precise safety protocols were not disclosed.

rss · Google News AI · Nov 20, 08:24

**「近期头部 AI 实验室的安全转向」** 在本次集体调整之前，OpenAI 于当地时间 11 月 18 日首次全面披露其《应对前沿 AI 风险》安全说明，并表示正在调整训练与模型发布速度（tool-1-1）。一个月前，Anthropic 亦宣布与第三方安全机构合作，让外部人员进驻办公室，对前沿模型训练开展独立评估，并将此做法类比为监管机构在银行内部派驻检查员（tool-1-2）。此前在 9 月，OpenAI、Anthropic 与 xAI 三家公司罕见达成共识，共同呼吁行业主动放缓前沿 AI 开发速度（tool-1-3）。

<details><summary>References</summary>
<ul>
<li><a href="https://cj.sina.com.cn/articles/view/1651428902/626ece2602001lwfc">AI巨头集体调整安全策略，第三方“安检员”开始入驻办公室_新浪财经</a></li>
<li><a href="https://guba.eastmoney.com/news,usant,1799347174.html">AI巨头集体调整安全策略 第三方“安检员”开始入驻办公室_Anthropic (us...</a></li>
<li><a href="https://news.qq.com/rain/a/20260914A0AJI000">三巨头达成“AI减速”安全共识，AI板块利空，芯片股跳水</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#regulation`, `#industry news`, `#China`, `#third-party oversight`

---

<a id="item-tech-news-9"></a>
### [Micron President Warns AI Storage Shortages Will Worsen by 2027](https://news.google.com/rss/articles/CBMiSEFVX3lxTE9XR19jQmZvbE9lLTZBRzVWZmtMNl9jbWh0R1o4TnplaFRaUnY2MXpBVXpoNFVwQ2FmSWFQelNTMV9ER2JnaWxfXw?oc=5) ⭐️ 7.0/10

Micron’s president stated that the supply-demand balance for AI-related storage will tighten further by 2027, becoming even more strained than it is today. The warning signals sustained hardware constraints for AI systems, though the source report is limited to a headline and provides no quantitative forecasts, product details, or specific market conditions.

rss · Google News AI · Nov 20, 00:10

**「Prior warnings from Micron leadership」** Micron executives have been issuing escalating warnings about memory supply constraints driven by AI demand. In June 2026, CEO Sanjay Mehrotra said the company expected tight conditions to persist beyond calendar 2027, and in October 2026 he forecast that supply-demand would be &quot;much tighter in fiscal 2027 and 2028 than in 2026.&quot; These earlier projections provide context for the president&\#x27;s recent statement that 2027 will be &quot;tighter than 2026.&quot;

**「Prolonged AI Storage Procurement Cycles」** AI data center operators and cloud providers may need to prepare for extended lead times and higher costs for storage hardware such as NAND flash into 2027, as tight semiconductor supply-demand forecasts suggest capacity expansions could be delayed.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techspot.com/news/112894-micron-ceo-expects-memory-shortages-stretch-beyond-2027.html">Micron CEO expects memory shortages to stretch beyond 2027 as ...</a></li>
<li><a href="https://www.techpowerup.com/353296/micron-ceo-says-memory-supply-will-be-much-tighter-in-2027-and-2028-than-in-2026">Micron CEO Says Memory Supply Will Be Much Tighter in 2027 ...</a></li>
<li><a href="https://www.analyticsinsight.net/news/smic-warns-ai-chip-supply-chain-shortages-may-last-until-2027">SMIC Warns AI Chip Supply Chain Shortages May Last Until 2027</a></li>
<li><a href="https://www.microchipusa.com/industry-news/ai-hardware-shortage-beyond-gpus">The AI Hardware Shortage Beyond GPUs: 8 Components Facing ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#storage`, `#hardware`, `#semiconductor`, `#supply chain`

---

<a id="item-tech-news-10"></a>
### [AI Power Policies Surge, but Storage and Data Shortfalls Persist](https://news.google.com/rss/articles/CBMiSEFVX3lxTE9KNDJBLXNadjFEY0syS1YtRDkxMnlZUE9BeFhaeDdjTE9PdEZXeTI3NGdtM3F5UG9KZTJjd2NXOTIxc0xSZW1MRQ?oc=5) ⭐️ 7.0/10

Following a wave of policy initiatives designed to reconcile AI&\#x27;s massive power consumption with energy systems, a 财联社 analysis finds that two essential components are still absent: adequate energy storage capacity and the data platforms required for effective power management. These gaps leave the AI industry unable to fully match its electricity use with available supply, despite the new regulations.

rss · Google News AI · Nov 20, 01:00

**「Background」** Earlier in 2025, China published a research report on the coordinated development of computing power and electricity, and subsequently issued a policy implementation guideline for advancing “AI + energy” quality development. These documents forecast the energy demand from computing and set a framework for integrating AI with the energy sector.

<details><summary>References</summary>
<ul>
<li><a href="https://fdi.mofcom.gov.cn/resource/pdf/2025/07/09/c45f080cb9064a219eb3629685190ba0.pdf">算力电力协同发展研究报告 (2025 年)</a></li>
<li><a href="https://www.gov.cn/zhengce/zhengceku/202509/content_7040253.htm">国家发展改革委 国家能源局关于推进“人工智能+”能源高质量发展的实施...</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#energy consumption`, `#policy`, `#data centers`, `#sustainability`

---

<a id="item-tech-news-11"></a>
### [Taotian Group Gets 7 Papers Accepted at KDD 2027, Including LLM-Discovered Bidding Algorithms](https://news.google.com/rss/articles/CBMiSEFVX3lxTE52Vzh5NFQwaEltbzVwQzEtOGh6Y2tWQWJaTEktUkRRa19tQWpXR0JzN3Jqa1BtWUlJbEkyRmlLY29aRV8zbVNNSA?oc=5) ⭐️ 7.0/10

Taotian Group had seven papers accepted in the first round of the ACM SIGKDD 2027 conference. One paper introduces a method that uses large language models to automatically discover bidding algorithms. Several other papers present new benchmarks that fill previously unaddressed gaps in the field. The acceptances represent early-stage research contributions, and no details about production deployment were provided.

rss · Google News AI · Nov 20, 11:20

**「Background」** ACM KDD is a premier conference for data mining and knowledge discovery. The upcoming KDD 2027 edition, scheduled for August 2027 in San Jose, includes a Datasets and Benchmarks Track that solicits new resources to address gaps in the field.

<details><summary>References</summary>
<ul>
<li><a href="https://kdd2027.kdd.org/">KDD 2027 – KDD 2027 | San Jose</a></li>
<li><a href="https://www.myhuiban.com/conference/136">KDD 2027 (CCF A): ACM SIGKDD Conference on Knowledge Disc...</a></li>

</ul>
</details>

**Tags**: `#KDD 2027`, `#algorithm discovery`, `#benchmark`, `#large language models`, `#e-commerce AI`

---

<a id="item-tech-news-12"></a>
### [CNKI’s AI detection rate surge alarms academic authors](https://news.google.com/rss/articles/CBMiYEFVX3lxTFBFSm1YMi1ZekFQR2lTN2ZBTVZIajctVUlJRnYzWnlURU5FRl83NnJabzdBYndGLTNTazlyWlpiV0pobk1QcmtnV3Z4RVVKM2cwYjJmY3JsMWJsVnpQSzkzeA?oc=5) ⭐️ 7.0/10

CNKI, the Chinese academic database, has experienced a pronounced surge in its AI detection rate, raising concerns about the reliability of its underlying algorithm. The increase has left authors confused and triggered debate over the ethical limits of using AI to assist academic writing, as reported by ThePaper.cn. No specific magnitude of the surge or technical details of the algorithm were provided.

rss · Google News AI · Nov 19, 23:46

**「Background」** CNKI, China’s major academic database, introduced AI content detection in its plagiarism checking system to flag suspected AI-generated text in submitted papers. The recent surge in its detection rate has drawn attention to potential algorithm changes, such as updated models or lower detection thresholds, which affect how scholars’ AI-assisted writing is categorized.

**Tags**: `#AI detection`, `#academic integrity`, `#CNKI`, `#algorithms`, `#AI ethics`

---

## Financial News

<a id="item-finance-news-1"></a>
### [A-Shares Extend Losing Streak to Seven Days with Over 4,000 Stocks Down; Broad ETF Volume Spikes at Close](https://news.google.com/rss/articles/CBMiYkFVX3lxTE1IcHB6bzRheEdZaDhoTTl0RGxjTUJuM2xNdC1IX3pzb3ROX0V1aVJQcEN2ZDJQUGxGcXlvYjdfVVdnSzJWVjN2SVVqZkM5dTRLVGlfTjFsbDJTQXFwY043OC1n?oc=5) ⭐️ 8.0/10

China’s A-share market fell for a seventh straight session on November 20, with more than 4,000 individual stocks declining each day. Trading volume in broad-based exchange-traded funds \(ETFs\) surged in the final minutes of trading, a pattern Caixin suggests may indicate state-backed purchases aimed at stabilizing the market.

rss · Google News 财经 · Nov 20, 09:26

**「A-shares and broad-based ETFs」** A-shares are stocks of mainland Chinese companies listed on the Shanghai and Shenzhen exchanges. Broad-based ETFs track major indexes like the CSI 300 and are often purchased by state-linked funds to stabilize the market when it falls sharply.

**Tags**: `#A-shares`, `#market decline`, `#ETF volumes`, `#market breadth`, `#Chinese stock market`

---

<a id="item-finance-news-2"></a>
### [ICBC Reclaims Crown as China&\#x27;s Most Valuable A-Share Company](https://news.google.com/rss/articles/CBMiUEFVX3lxTE1iS0lDLUFTQmd2a3pTWUZfZjJNaGp5OEpUM3N1SUk4UHdFN1VaUUIyQkp3bm5Dc2tEZTVwNENBcjc4MFRxVFBYUU1Wd1VfTTct?oc=5) ⭐️ 7.0/10

Industrial and Commercial Bank of China \(ICBC\) has once again become the largest company by market capitalization on China&\#x27;s A-share market \(the mainland stock exchanges\).

rss · Google News 财经 · Nov 20, 08:43

**「Background」** The previous A-share market capitalization leader was semiconductor firm ChangXin Technology, which ICBC has now passed.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.eastmoney.com/a/202611203936210777.html">工商银行，重夺A股市值冠军！工商银行，重夺A股市值冠军！</a></li>

</ul>
</details>

**Tags**: `#ICBC`, `#A-share market`, `#market capitalization`, `#Chinese stocks`, `#banking`

---

<a id="item-finance-news-3"></a>
### [Baidu turns loss into 1.4 billion yuan profit as AI revenue exceeds 50%](https://news.google.com/rss/articles/CBMiZEFVX3lxTE9Bc3FzOUkxTUNtT1FHUlA1ZkdVV1E4QVhIZk9CX1c5LWZvTnNPWF82UHo0bWlUWld1QVhIdGpPdktSajhGWUtKWGNqZTM5TFJncldnOHM3d0trczB3SjF4M1dBdVI?oc=5) ⭐️ 7.0/10

Baidu reported a profit of 1.4 billion yuan, reversing a previous loss, while AI-driven revenue surpassed 50% of total revenue for the first time, according to a report from Securities Star.

rss · Google News 财经 · Nov 20, 06:03

**「Background」** In the third quarter of 2026, Baidu reported a net profit of 1.4 billion yuan, reversing a prior loss, as AI revenue accounted for 53% of its general business income for the third consecutive quarter.

**「Impact」** The AI revenue milestone may reinforce investor confidence in Baidu&\#x27;s strategic pivot to artificial intelligence, potentially influencing the technology sector&\#x27;s focus on AI monetization.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.sina.com.cn/jjxw/2026-11-17/doc-iniyyzyp7724580.shtml">百度Q3财报：AI收入已过半，利润贡献尚未接棒_新浪财经_新浪网</a></li>

</ul>
</details>

**Tags**: `#Earnings`, `#Artificial Intelligence`, `#Chinese Stocks`, `#Technology`, `#Baidu`

---