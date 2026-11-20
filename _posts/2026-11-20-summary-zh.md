---
layout: default
title: "Horizon Summary: 2026-11-20 (ZH)"
date: 2026-11-20
lang: zh
---

> 从 211 条内容中筛选出 15 条重要资讯。

---

**科技新闻**
1. [Claude 解决两个黑洞物理开放问题](#item-tech-news-1) ⭐️ 9.0/10
2. [PostgreSQL 19 发布：WAIT FOR LSN 实现读写一致性](#item-tech-news-2) ⭐️ 9.0/10
3. [Anthropic 登陆纳斯达克，AI IPO 创纪录](#item-tech-news-3) ⭐️ 9.0/10
4. [FFmpeg 9.1 &\#x27;Gauss&\#x27; 发布：新增图像与视频编解码器、Vulkan 编码支持](#item-tech-news-4) ⭐️ 8.0/10
5. [PHP 的 https 大小写错误导致 TLS 静默关闭，20 年漏洞](#item-tech-news-5) ⭐️ 8.0/10
6. [英国法庭裁定苹果胜诉，后门案须公开审理](#item-tech-news-6) ⭐️ 8.0/10
7. [近半年美批准 88 万颗 AI 芯片对华出口](#item-tech-news-7) ⭐️ 8.0/10
8. [AI 巨头引入第三方安检员，集体调整安全策略](#item-tech-news-8) ⭐️ 7.0/10
9. [美光总裁：2027 年 AI 存储供需将更加紧张](#item-tech-news-9) ⭐️ 7.0/10
10. [AI 能源缺口：储能与数据](#item-tech-news-10) ⭐️ 7.0/10
11. [淘天集团 KDD 2027 论文：大模型自动发现出价算法](#item-tech-news-11) ⭐️ 7.0/10
12. [知网 AI 检出率暴涨引争议](#item-tech-news-12) ⭐️ 7.0/10

**财经新闻**
1. [A 股连续七日超四千只个股下跌，宽基 ETF 尾盘放量](#item-finance-news-1) ⭐️ 8.0/10
2. [工商银行重夺 A 股市值冠军](#item-finance-news-2) ⭐️ 7.0/10
3. [百度实现 14 亿元盈利，人工智能收入占比过半](#item-finance-news-3) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Claude 解决两个黑洞物理开放问题](https://www.anthropic.com/research/claude-black-hole-physics) ⭐️ 9.0/10

Anthropic 的研究博客宣布，Claude 模型解决了两个黑洞物理中的开放问题：一个涉及复杂且易出错的计算，另一个则是在给定中心荷下证明了黑洞质量的上限，从而为一致的量子引力理论提供了约束。该成果以论文形式发布，但尚未经独立同行评审验证。

hackernews · cybermango · 11月19日 17:30 · [社区讨论](https://news.ycombinator.com/item?id=50563148)

**「核心背景：两个黑洞物理学开放问题」** Anthropic 宣称克劳德解决的两个开放问题均与黑洞和量子引力理论有关：一是涉及“bootstrap”方法的复杂计算，二是证明在给定中心电荷下黑洞质量存在上限，从而为自洽的量子引力理论提供关键约束。

**「影响」** 第二个结果给出了与中心荷相容的黑洞质量上界，超出该质量的理论不再被视为一致的量子引力理论，这为量子引力模型构建提供了一个具体的筛选条件，但其影响局限于该细分领域。

**「社区讨论」** 一位物理学家指出，理论物理学中“开放问题”数量庞大且高度专业化，该成果在其子领域内有意义，但不会引起整个物理学界的普遍关注。另一位评论者认为，相比第一个计算密集型问题，第二个证明质量上限的结果更具新意和深度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/research/claude-black-hole-physics">Claude solves two open problems in the physics of black holes</a></li>

</ul>
</details>

**标签**: `#ai`, `#physics`, `#black-holes`, `#claude`, `#scientific-research`

---

<a id="item-tech-news-2"></a>
### [PostgreSQL 19 发布：WAIT FOR LSN 实现读写一致性](https://simonwillison.net/2026/Nov/19/postgresql-19/) ⭐️ 9.0/10

PostgreSQL 19 已发布。该版本新增 WAIT FOR LSN 命令，允许应用在备用节点上等待特定日志序列号（LSN）被重放，从而在备用库上实现“读自己写”的一致性保证，并支持可选的超时参数。此次发布比 PostgreSQL 通常的年度九月发布推迟了约两个月，主要因团队需要处理大量由 AI 工具报告的漏洞。

rss · Simon Willison \(AI\) · 11月19日 20:43

**「背景」** PostgreSQL 通常每年九月推出新版本，但 19 版的发布因 AI 引发的漏洞报告而延迟。在读写分离的架构中，向主库写入后立即从备用库读取，可能因预写日志（WAL）重放延迟而看不到最新数据。此前一些应用（如 MediaWiki）需要通过保存主库的复制位置并等待备库追上来手动解决此问题。

**「影响」** 对于将读操作分配到备用节点的应用程序，WAIT FOR LSN 提供了原生的读写一致性机制，无需应用自行追踪复制进度和实现等待逻辑，可简化架构并降低用户遭遇旧数据的风险。

**标签**: `#postgresql`, `#databases`, `#release`, `#consistency`, `#open-source`

---

<a id="item-tech-news-3"></a>
### [Anthropic 登陆纳斯达克，AI IPO 创纪录](https://news.google.com/rss/articles/CBMi0AJBVV95cUxOa1JXZ2llZ3BVUXdmUEVWb1h6blRkOFNfaFgwNjFxS1B0RDZyUVA0b3Rkc1plVGJBYmlaQVo2QjJaWkVBMW9JMXp4YWZoUjFHVUttZUZqeE96WGs4dFk0SnEyZGNPUk9ZYmVTVktINmlqSFAzazVqN25Zc2hScXQyblRVRUJrQnB1VGVWTUswZGRSYW0tQlc5Z25JT211dVh3WVU3dmc0TlRMUmpXYjd4aDdhUEw2Tk1tX1NmLW9DQTd3UzNtMFVxQmdUanM1alkzZFcyUkRuMGxWU194eS15QTBFQ3Z0MWlyQXl4UUNCNTR5MkhOaENtTzJaOXpLQUxlVW50QVdoaFR3c19TalM5bHNtYk52U2xXWVlrakc2Vngwbkx6Q0E3WGEwMlZLT1JRYVhnendsWHgzdXVQaGtsUXI2aEZnOW5CWnVJSDdYM2c?oc=5) ⭐️ 9.0/10

人工智能公司 Anthropic 已正式在纳斯达克上市。其首次公开募股（IPO）据称为人工智能领域创纪录的发行，但报道未提供具体融资金额或估值细节。

rss · Google News AI · 11月19日 18:15

**「背景」** Anthropic 是人工智能助手 Claude 的开发商。该公司 IPO 定价每股 83 美元，募资 813 亿美元，开盘涨幅超 34%，超过了 SpaceX 今年 6 月的上市规模，成为史上最大的 IPO。其主要竞争对手 OpenAI 据报已将上市计划推迟至 2027 年。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.euronews.com/2026/11/19/anthropic-shares-open-34-above-ipo-price-in-nasdaq-debut-after-record-listing">Anthropic shares open 34% above IPO price in Nasdaq ... | Euronews</a></li>
<li><a href="https://www.france24.com/en/business/20261119-anthropic-begins-trading-1-5-trillion-company-biggest-ipo-record-ai">Anthropic blows past $2 trillion in Nasdaq debut, beating... - France 24</a></li>
<li><a href="https://www.dw.com/en/anthropic-trading-tests-investors-appetite-for-ai/a-79993163">Anthropic trading tests investors&#x27; appetite for AI</a></li>

</ul>
</details>

**标签**: `#artificial intelligence`, `#IPO`, `#Anthropic`, `#Nasdaq`, `#technology industry`

---

<a id="item-tech-news-4"></a>
### [FFmpeg 9.1 &\#x27;Gauss&\#x27; 发布：新增图像与视频编解码器、Vulkan 编码支持](https://ffmpeg.org/download.html#release_9.1) ⭐️ 8.0/10

FFmpeg 9.1“Gauss”正式发布，引入了 ASTC 图像编码和解码（通过 libastcenc，并配备.astc 与 KTX 1.0 封装/解封装器）、经深度改进的 AAC 编码器、APV Vulkan 视频编码器、LCEVC 载荷合并比特流过滤器，以及全新的基于图的比特流过滤 API。同时，新增 NVDEC CUARRAY 硬件加速、iTerm2 内联图像协议复用器、MVR 解复用器、latticepal 滤镜和 AMF 视频质量增强滤镜，libcurl 协议与 DVD-Audio LPCM 解码/解封装支持也一并加入。

hackernews · gyan · 11月20日 04:02 · [社区讨论](https://news.ycombinator.com/item?id=50569998)

**「背景」** FFmpeg 是广泛使用的开源跨平台多媒体框架，提供音视频录制、转换、流化等核心功能。9.1 版本代号“Gauss”，作为继 9.0 之后的主要更新，持续扩展编解码器与硬件加速支持，保持对现代多媒体工作流的适配能力。

**「影响」** 对于视频与音频处理应用的开发者而言，9.1 版本直接提供了对 ASTC 图像格式、LCEVC 分层视频编码、Vulkan GPU 编码等现代技术的集成能力，同时改进的 AAC 编码质量与多种硬件加速可提升转码效率与流媒体体验。

**标签**: `#open-source`, `#ffmpeg`, `#multimedia`, `#video-processing`, `#codecs`

---

<a id="item-tech-news-5"></a>
### [PHP 的 https 大小写错误导致 TLS 静默关闭，20 年漏洞](https://x.com/ljachowicz/status/2123477025268924514) ⭐️ 8.0/10

PHP 的 HTTP/FTP 流包装器在识别 URL scheme 时大小写不敏感，但仅当第五个字符为小写 s 时才启用 TLS。因此 HTTPS://、httpS:// 或 FTPS:// 等大写 S 的变体会被当作明文连接，导致令牌、Basic 认证、Cookie 等数据暴露。该漏洞编号 CVE-2026-128064，CVSS 4.0 评分 8.2，存在约 20 年，已在 PHP 8.2.36、8.3.37、8.4.28、8.5.13 和 8.6.0 中修复；8.1 及更早版本因终止支持不再修复，用户需将 URL scheme 统一转为小写。

telegram · zaihuapd · 11月20日 03:04

**「背景」** PHP 的 HTTP 和 FTP 流包装器（stream wrapper）允许开发者通过统一的文件操作函数（如 file\_get\_contents\(\)）访问远程资源。这些包装器在解析 URL schema 时原本采用大小写不敏感的比较方式，但实际启用 TLS 加密的条件仅检查 scheme 的第五个字符是否为小写的 &quot;s&quot;，导致大小写混写的变体（如 &quot;httpS://&quot;、&quot;HTTPS://&quot;）被当作明文连接处理。

**「影响」** 依赖 PHP 流包装器发起 HTTPS 请求的应用，若未将传入的 URL scheme 统一小写，或仍运行已终止支持的旧版 PHP，可能将认证凭据和敏感数据明文送出，在中间人攻击场景下面临直接的信息泄露风险。

**标签**: `#PHP`, `#security`, `#vulnerability`, `#TLS`, `#stream-wrapper`

---

<a id="item-tech-news-6"></a>
### [英国法庭裁定苹果胜诉，后门案须公开审理](https://appleinsider.com/articles/26/11/19/uk-cant-hide-that-it-tried-ordering-apple-to-allow-access-to-user-data) ⭐️ 8.0/10

英国调查权力法庭裁定苹果胜诉，要求英国内政部不得再秘密执行其向苹果发出的“技术能力通知（TCN）”，该通知旨在强制苹果为 iPhone 加密数据提供后门访问，案件大部分将公开审理。法庭认定内政部提出的国家安全保密理由“不切实际”，内政部事后确认了该通知的存在，但坚称仅出于打击犯罪目的。

telegram · zaihuapd · 11月20日 04:13

**「背景」** 英国《调查权力法案》赋予政府向科技公司秘密发出“技术能力通知”（TCN）的权力，强制其协助解密数据。英国内政部此前曾据此向苹果公司发出秘密命令，要求为 iPhone 加密数据设置后门，引发了苹果的法律挑战。

**「影响」** 该裁决将原本秘密进行的后门命令强制转为公开审理，可能形成先例，增加未来政府秘密要求加密后门的难度，并强化数字隐私保护的法律挑战空间。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/11/19/u-k-government-forced-to-disclose-secret-apple-backdoor-order/">UK government forced to disclose secret Apple backdoor order</a></li>
<li><a href="https://www.macrumors.com/2026/11/19/uk-loses-secrecy-fight-over-apple-backdoor-order/">UK Loses Secrecy Fight Over Apple &#x27;Backdoor&#x27; Order</a></li>

</ul>
</details>

**标签**: `#encryption`, `#privacy`, `#Apple`, `#government surveillance`, `#tech policy`

---

<a id="item-tech-news-7"></a>
### [近半年美批准 88 万颗 AI 芯片对华出口](https://foreignaffairs.house.gov/news/press-releases/chairman-brian-mast-exercises-legislative-authority-to-publicly-release-ai-chip-license-information-for-china) ⭐️ 8.0/10

美国众议院外交事务委员会公布的许可文件显示，2025 年 12 月至 2026 年 5 月，美国政府批准英伟达与 AMD 向中国出口 879,868 颗 AI 芯片，涉及 H200 和 MI325X 型号，企业申请总量达 344.4 万颗。获批企业包括腾讯、字节跳动（各获批 15 万颗）以及阿里、快手、滴滴（各获批 7.5 万颗）等。但截至 2026 年 5 月 11 日，所有许可下的芯片均未实际发货，获批数量不代表已交付。

telegram · zaihuapd · 11月20日 04:25

**「背景」** 此次数据源于美国众议院外交事务委员会对 AI 芯片出口许可审批的审查。美国持续限制向中国出口先进计算芯片，英伟达、AMD 等厂商对华销售特定性能的 AI 芯片需获得许可。委员会同时指出，阿里、腾讯、百度等获批企业此前已被列入所谓的中国军方关联企业名单，引发对审批合理性的质疑。

**「影响」** 截至 2026 年 5 月中旬，所有获批芯片仍未发货，意味着腾讯、字节跳动、阿里等企业并未因许可批准而获得实际 AI 算力补充，其模型训练与推理能力可能仍受限于现有库存或非受限替代方案。

**标签**: `#AI chips`, `#export controls`, `#US-China trade`, `#NVIDIA`, `#AMD`

---

<a id="item-tech-news-8"></a>
### [AI 巨头引入第三方安检员，集体调整安全策略](https://news.google.com/rss/articles/CBMijwFBVV95cUxPaHFUbnlDbnlGM2xidm5Vckw0N05pSGVyendyQzZXZWpnSlBjR211Q0lhWXp1ZDQtMVhfY3U1d2ZSTjNoMEtxZUM1Y1N1TzdVWmNZeml1T0h4QUItNVdHN1dDVFRQQmVmSVlrc25hRE5LMmNGT2tBMmZLOFpWbzJ0NWpHdTZkQURmZTdwTzF5aw?oc=5) ⭐️ 7.0/10

据 21 财经报道，多家头部 AI 公司正在集体调整内部安全策略，并开始允许第三方安全审查人员入驻办公场所。报道将此举描述为 AI 治理进入新阶段的信号，但未披露具体涉及的企业名称、安全调整措施的技术细节、第三方审查机构的资质以及入驻的时间安排与执行范围。目前信息仅限于标题与摘要，深度与确切规模仍不确定。

rss · Google News AI · 11月20日 08:24

**「事件背景」** 一个月前，Anthropic 已率先宣布与第三方安全机构合作，让外部人员进驻办公室，对前沿模型训练开展独立评估，并将其比喻为监管在银行派驻检查员。当地时间 11 月 18 日，OpenAI 发布《应对前沿 AI 风险：从训练到部署》安全说明，首次全面披露安全措施，并表示正在调整训练和模型发布速度。这两项举措构成了此次 AI 巨头集体引入第三方“安检员”的直接背景。

**「影响」** 若第三方安检入驻成为常态，AI 企业的内部研发流程与数据管理将面临外部合规审查，可能推动行业安全标准从自评转向独立验证。但当前缺乏具体案例与执行细则，实际影响尚无法评估。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cj.sina.com.cn/articles/view/1651428902/626ece2602001lwfc">AI巨头集体调整安全策略，第三方“安检员”开始入驻办公室_新浪财经</a></li>
<li><a href="https://guba.eastmoney.com/news,usant,1799347174.html">AI巨头集体调整安全策略 第三方“安检员”开始入驻办公室_Anthropic (us...</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#regulation`, `#industry news`, `#China`, `#third-party oversight`

---

<a id="item-tech-news-9"></a>
### [美光总裁：2027 年 AI 存储供需将更加紧张](https://news.google.com/rss/articles/CBMiSEFVX3lxTE9XR19jQmZvbE9lLTZBRzVWZmtMNl9jbWh0R1o4TnplaFRaUnY2MXpBVXpoNFVwQ2FmSWFQelNTMV9ER2JnaWxfXw?oc=5) ⭐️ 7.0/10

美光科技总裁警告称，人工智能存储的供需形势到 2027 年将比今年更为紧张。该声明暗示 AI 基础设施建设面临的硬件供应瓶颈短期内难以缓解。

rss · Google News AI · 11月20日 00:10

**「背景」** 自 2026 年中起，美光高层已多次就 AI 需求下的存储供应紧张发出预警。2026 年 6 月，CEO Sanjay Mehrotra 表示供应紧张状况将延续到 2027 年之后；10 月，他进一步指出 2027 和 2028 财年的供需将比 2026 年严峻得多。当前美光总裁的声明是这一系列预测的延续。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techspot.com/news/112894-micron-ceo-expects-memory-shortages-stretch-beyond-2027.html">Micron CEO expects memory shortages to stretch beyond 2027 as ...</a></li>
<li><a href="https://www.techpowerup.com/353296/micron-ceo-says-memory-supply-will-be-much-tighter-in-2027-and-2028-than-in-2026">Micron CEO Says Memory Supply Will Be Much Tighter in 2027 ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#storage`, `#hardware`, `#semiconductor`, `#supply chain`

---

<a id="item-tech-news-10"></a>
### [AI 能源缺口：储能与数据](https://news.google.com/rss/articles/CBMiSEFVX3lxTE9KNDJBLXNadjFEY0syS1YtRDkxMnlZUE9BeFhaeDdjTE9PdEZXeTI3NGdtM3F5UG9KZTJjd2NXOTIxc0xSZW1MRQ?oc=5) ⭐️ 7.0/10

财联社分析指出，近期密集出台的 AI 电力需求相关政策虽已逐步落地，但算力基础设施的能源配套仍面临储能和数据两大明显短板，政策驱动尚未弥补这些缺口。这意味着 AI 集群的规模化部署仍受限于电力供给链的完备性。

rss · Google News AI · 11月20日 01:00

**「背景」** 中国近年来已密集出台多项政策推动算力与电力协同发展，例如 2025 年发布的《算力电力协同发展研究报告》提出了六大关键举措，同期《中国新型储能发展报告》梳理了储能技术进展，而发改委与能源局联合发布的《关于推进“人工智能+”能源高质量发展的实施意见》则确立了“人工智能+”能源融合的顶层框架。这些政策为 AI 用能需求铺路，但储能设施和数据共享机制等关键环节仍待补足。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://fdi.mofcom.gov.cn/resource/pdf/2025/07/09/c45f080cb9064a219eb3629685190ba0.pdf">算力电力协同发展研究报告 (2025 年)</a></li>
<li><a href="https://www.nea.gov.cn/20250731/1d40d09f75714280a9218d5bea178fbd/c.html">《中国新型储能发展报告（2025）》-国家能源局</a></li>
<li><a href="https://www.gov.cn/zhengce/zhengceku/202509/content_7040253.htm">国家发展改革委 国家能源局关于推进“人工智能+”能源高质量发展的实施...</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#energy consumption`, `#policy`, `#data centers`, `#sustainability`

---

<a id="item-tech-news-11"></a>
### [淘天集团 KDD 2027 论文：大模型自动发现出价算法](https://news.google.com/rss/articles/CBMiSEFVX3lxTE52Vzh5NFQwaEltbzVwQzEtOGh6Y2tWQWJaTEktUkRRa19tQWpXR0JzN3Jqa1BtWUlJbEkyRmlLY29aRV8zbVNNSA?oc=5) ⭐️ 7.0/10

淘天集团在 KDD 2027 首轮有 7 篇论文被录用，其中一项研究提出了利用大语言模型自动发现电商广告出价算法的方法，另有多个新基准填补了相关领域评估的空白。这些论文目前处于学术录用阶段，尚未见其算法在实际系统中部署的说明。

rss · Google News AI · 11月20日 11:20

**「背景」** ACM SIGKDD 会议（KDD）是数据挖掘与知识发现领域的顶级学术会议，KDD 2027 计划于 2027 年 8 月在美国圣何塞举办，设有“数据集与基准”分论坛（Datasets and Benchmarks Track），专门接收评测基准相关论文。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://kdd2027.kdd.org/">KDD 2027 – KDD 2027 | San Jose</a></li>
<li><a href="https://www.myhuiban.com/conference/136">KDD 2027 (CCF A): ACM SIGKDD Conference on Knowledge Disc...</a></li>

</ul>
</details>

**标签**: `#KDD 2027`, `#algorithm discovery`, `#benchmark`, `#large language models`, `#e-commerce AI`

---

<a id="item-tech-news-12"></a>
### [知网 AI 检出率暴涨引争议](https://news.google.com/rss/articles/CBMiYEFVX3lxTFBFSm1YMi1ZekFQR2lTN2ZBTVZIajctVUlJRnYzWnlURU5FRl83NnJabzdBYndGLTNTazlyWlpiV0pobk1QcmtnV3Z4RVVKM2cwYjJmY3JsMWJsVnpQSzkzeA?oc=5) ⭐️ 7.0/10

中国知网的 AI 生成内容检测率近期出现显著上升，但其检测算法的准确性和可靠性遭到质疑，许多作者对检测结果感到困惑，并引发了对 AI 辅助思考与学术写作边界的讨论。

rss · Google News AI · 11月19日 23:46

**「知网 AI 检测的争议背景」** 中国知网（CNKI）作为国内高校和学术界广泛使用的学术不端检测平台，此前已上线专门针对 AI 生成文本的检测功能，用于辅助识别学位论文和期刊稿件中的疑似 AI 代写内容。近期该系统的 AI 生成内容检出率出现显著攀升，引发了对算法判定逻辑、误判风险以及如何界定“AI 辅助思考”与学术剽窃边界的集中质疑。

**标签**: `#AI detection`, `#academic integrity`, `#CNKI`, `#algorithms`, `#AI ethics`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [A 股连续七日超四千只个股下跌，宽基 ETF 尾盘放量](https://news.google.com/rss/articles/CBMiYkFVX3lxTE1IcHB6bzRheEdZaDhoTTl0RGxjTUJuM2xNdC1IX3pzb3ROX0V1aVJQcEN2ZDJQUGxGcXlvYjdfVVdnSzJWVjN2SVVqZkM5dTRLVGlfTjFsbDJTQXFwY043OC1n?oc=5) ⭐️ 8.0/10

A 股市场连续第七个交易日出现超过 4000 只个股下跌，同时追踪大盘指数的宽基 ETF 在收盘前成交量显著放大。

rss · Google News 财经 · 11月20日 09:26

**「背景」** A 股在此前六个交易日已连续出现超 4000 只个股下跌，市场情绪承压，本次下跌为这一趋势的延续。

**标签**: `#A-shares`, `#market decline`, `#ETF volumes`, `#market breadth`, `#Chinese stock market`

---

<a id="item-finance-news-2"></a>
### [工商银行重夺 A 股市值冠军](https://news.google.com/rss/articles/CBMiUEFVX3lxTE1iS0lDLUFTQmd2a3pTWUZfZjJNaGp5OEpUM3N1SUk4UHdFN1VaUUIyQkp3bm5Dc2tEZTVwNENBcjc4MFRxVFBYUU1Wd1VfTTct?oc=5) ⭐️ 7.0/10

据凤凰网财经报道，工商银行重新夺回了 A 股市场市值第一的位置。

rss · Google News 财经 · 11月20日 08:43

**「背景」** 此前在 2026 年 10 月，工商银行总市值曾一度突破 3 万亿元，反超半导体企业长鑫科技，重登 A 股上市公司市值榜首。

**「影响」** 这一变化反映出银行板块在市场中的相对强势，可能吸引投资者增配金融股。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.sina.com.cn/wm/2026-10-21/doc-inivyaau8019212.shtml">科技新贵让位老牌银行，工商银行总市值突破3万亿元杀回榜首，A股“一哥...</a></li>
<li><a href="https://www.thepaper.cn/newsDetail_forward_34282096">工商银行创历史新高，重回A股上市公司市值“一哥”，长鑫科技一度大跌超...</a></li>

</ul>
</details>

**标签**: `#ICBC`, `#A-share market`, `#market capitalization`, `#Chinese stocks`, `#banking`

---

<a id="item-finance-news-3"></a>
### [百度实现 14 亿元盈利，人工智能收入占比过半](https://news.google.com/rss/articles/CBMiZEFVX3lxTE9Bc3FzOUkxTUNtT1FHUlA1ZkdVV1E4QVhIZk9CX1c5LWZvTnNPWF82UHo0bWlUWld1QVhIdGpPdktSajhGWUtKWGNqZTM5TFJncldnOHM3d0trczB3SjF4M1dBdVI?oc=5) ⭐️ 7.0/10

百度发布最新财报，公司从上期亏损转为实现净利润 14 亿元，人工智能相关收入占总收入的比例首次超过一半。

rss · Google News 财经 · 11月20日 06:03

**「背景」** 这是百度将港交所上市地位变更为双重主要上市后公布的首份季报。此前，该公司 2026 年上半年总营收 634 亿元，其中 AI 业务收入 261 亿元。

**「影响」** 这一业绩标志着百度人工智能战略转型取得关键进展，可能增强市场对中国科技企业 AI 商业化能力的信心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.stockstar.com/SS2026112000020143.shtml">百度扭亏14亿，AI收入过半_财经频道_证券之星</a></li>
<li><a href="https://news.qq.com/rain/a/20260918A032GV00">百度发布年中财报：AI业务增势迅猛，收入同比增长36%</a></li>

</ul>
</details>

**标签**: `#Earnings`, `#Artificial Intelligence`, `#Chinese Stocks`, `#Technology`, `#Baidu`

---