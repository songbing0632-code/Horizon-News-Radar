---
layout: default
title: "Horizon Summary: 2026-11-17 (ZH)"
date: 2026-11-17
lang: zh
---

> 从 234 条内容中筛选出 11 条重要资讯。

---

**科技新闻**
1. [卡内基梅隆大学在 YouTube 免费提供计算机科学课程](#item-tech-news-1) ⭐️ 8.0/10
2. [Optimizely 安全事件：Zoom 和 GitLab 等网站被植入恶意软件](#item-tech-news-2) ⭐️ 8.0/10
3. [研究分析称 66%的 ML 论文至少含一项无效改动](#item-tech-news-3) ⭐️ 8.0/10
4. [Jiff 1.0：一个用于 Rust 的新日期时间库](#item-tech-news-4) ⭐️ 7.0/10
5. [百度 AI 营收达 132 亿元，商业化加速重塑增长逻辑](#item-tech-news-5) ⭐️ 7.0/10
6. [深圳发布全国首个《人工智能工具应用商业秘密保护指引》](#item-tech-news-6) ⭐️ 7.0/10
7. [ICLR 2027 程序委员会对审稿进行 AI 检测](#item-tech-news-7) ⭐️ 7.0/10

**财经新闻**
1. [美国科技公司面临对华业务两难](#item-finance-news-1) ⭐️ 8.0/10
2. [伯克希尔增持达美航空并减持美国银行股份](#item-finance-news-2) ⭐️ 7.0/10
3. [美联储主席警告 AI 可能令人失望并导致失业](#item-finance-news-3) ⭐️ 7.0/10
4. [美股芯片出口管制升级，欧洲股市再度承压](#item-finance-news-4) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [卡内基梅隆大学在 YouTube 免费提供计算机科学课程](https://www.cs.cmu.edu/learn/) ⭐️ 8.0/10

卡内基梅隆大学（CMU）开始通过 YouTube 免费提供完整的计算机科学课程，涵盖多个主题，每天发布一门新课，首批课程已上线。这些课程由该校计算机科学系的教师授课，并由学生开发的自动化工具进行制作，以提高效率。此举为全球学习者提供了来自顶尖学府的高质量教育资源。

hackernews · pcompeau · 11月16日 20:43 · [社区讨论](https://news.ycombinator.com/item?id=50522980)

**「背景介绍」** 卡内基梅隆大学（CMU）通过 YouTube 平台免费开放其计算机科学课程，这些课程由该校格里芬计算机科学学院提供，并由学生团队制作和编辑。此举使得全球学习者可以自由获取真实课堂讲授内容，涵盖多个主题，每周发布一门新课程，首批课程已上线，更多课程将在 2027 年 1 月推出。此前，麻省理工学院（MIT）也曾在 25 年前开始类似尝试。

**「影响」** 对于希望自学或补充计算机科学知识的学习者而言，这提供了免费获取高质量课程内容的机会，有助于提升其专业技能和理论基础，从而增强在软件工程领域的竞争力。

**「社区讨论」** 部分评论指出课程音频质量存在不足，例如某门课程中教授使用麦克风不当导致声音失真；另一些评论则表达了对特定课程如机器学习系统、概率与计算等的兴趣，并呼吁提供更多课程资源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/@CMULearn">CS Learn at Carnegie Mellon - YouTube</a></li>
<li><a href="https://www.youtube.com/watch?v=TJ6qYAaGRZ8">CMU Machine Learning with Large Datasets (Fall 2026) - YouTube</a></li>
<li><a href="https://news.ycombinator.com/item?id=50522980">Carnegie Mellon is putting computer science courses on YouTube for...</a></li>

</ul>
</details>

**标签**: `#education`, `#open-source`, `#software-engineering`

---

<a id="item-tech-news-2"></a>
### [Optimizely 安全事件：Zoom 和 GitLab 等网站被植入恶意软件](https://blog.report-uri.com/worlds-largest-brands-infected-with-malware-via-optimizely/) ⭐️ 8.0/10

安全公司 Report URI 发现，Optimizely 平台在 2026 年 11 月被黑客攻击，导致其脚本被篡改，并通过 Zoom、GitLab 等大型网站向用户分发恶意软件。该事件影响了包括 CNN、BBC 在内的多个拥有大量用户的网站，暴露了第三方脚本管理中的严重安全隐患。

hackernews · kristjansson · 11月16日 23:00 · [社区讨论](https://news.ycombinator.com/item?id=50524767)

**「背景」** Optimizely 是一个提供网站优化和 A/B 测试服务的平台，其脚本被黑客攻击后被用于在多个大型网站上分发恶意软件。此次事件影响了包括 Zoom、GitLab、CNN、BBC 在内的超过 178 家组织，这些网站的访客可能因此受到恶意代码感染。攻击者利用了 Optimizely 平台的信任机制，将恶意脚本部署到合作方网站上，从而绕过了常规安全防护措施。

**「行业问责缺失与第三方脚本系统性风险」** 社区讨论指出，此次事件暴露了供应商和大型网站双方的安全责任缺失。评论认为 Optimizely 应实施发布冷却期、分阶段 rollout 和自动安全检查等防护机制；而 CNN、BBC 等拥有海量用户的网站更应自行托管脚本而非直接引用第三方供应商代码，否则用户面临恶意脚本攻击风险的事件将持续发生。

**「Community Discussion」** 社区成员指出，此类事件反映了网站脚本管理机制的缺陷，特别是营销团队被授权直接修改网页脚本的做法增加了安全风险。有评论建议应加强内部审核流程和自动安全检查机制，并质疑大型媒体网站为何允许此类高风险脚本运行。另有观点认为这凸显了浏览器安全策略的重要性，以及使用 NoScript 等工具减少潜在威胁的必要性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/optimizely-supply-chain-attack-delivers-malware-to-cnn-fox-news-bbc-salesforce-sites/">Optimizely hack infected CNN, Fox News, BBC, Salesforce sites ...</a></li>
<li><a href="https://cybernews.com/security/178-company-websites-infected-malware/">Optimizely script attack hit 178 major websites | Cybernews</a></li>
<li><a href="https://news.ycombinator.com/item?id=50524767">Optimizely compromised, served malware on Zoom , GitLab</a></li>

</ul>
</details>

**标签**: `#security`, `#web-development`, `#vendor-vulnerability`

---

<a id="item-tech-news-3"></a>
### [研究分析称 66%的 ML 论文至少含一项无效改动](https://www.reddit.com/r/MachineLearning/comments/1xybvju/we_logged_621k_changes_from_127k_papers_ablations/) ⭐️ 8.0/10

Latentic Labs 分析了 2016 至 2026 年间 ICML、NeurIPS、ICLR、CVPR 等顶会的 126,758 篇论文，提取了 621,064 项实验改动及其效果报告。结果显示：69%的改动有帮助，10%效果不明显，16%反而更差，5%混合。66%的论文至少报告了一项无效改动。ML 会议中 31%的改动报告 null 或负面结果，而视觉会议为 22%。最常见的无效改动包括：提高采样温度（52%的 122 篇论文）、增大 LoRA rank（46%）、增大学习率（46%）。最少无效的是添加对比损失（仅 4%的 1,317 篇论文）。

reddit · r/MachineLearning · /u/latenticlabs · 11月17日 05:11

**「机器学习研究中的实验变更有效性分析」** 一项针对 2016 至 2026 年间发表在 ICML、NeurIPS、ICLR、CVPR、AAAI、ICCV、ECCV、TPAMI、IJCV 和 JMLR 等会议与期刊上的 126,758 篇论文的分析显示，研究人员记录了总计 621,064 项实验变更，并评估其效果。结果显示，69%的变更对模型性能有帮助，10%无明显影响，而 16%的变更（其中 5%为混合结果）反而降低了性能。此外，66%的论文报告至少有一项无效的实验变更。该研究还发现，在视觉领域，约 22%的变更未带来积极效果，而在整体机器学习领域则为 31%。

**「实际影响」** 该分析为 ML 研究者提供了基于大规模实证数据的改动效果参考，可帮助优先尝试更可能有效的技术（如对比损失），避免常见陷阱（如盲目增大学习率或 LoRA rank），同时表明 ML 文献中存在大量未报告的负面结果，研究浪费问题值得重视。

**标签**: `#machine learning`, `#research methodology`, `#reproducibility`, `#empirical analysis`, `#software engineering`

---

<a id="item-tech-news-4"></a>
### [Jiff 1.0：一个用于 Rust 的新日期时间库](https://burntsushi.net/jiff/) ⭐️ 7.0/10

Jiff 1.0 是一个为 Rust 设计的新日期时间库，旨在改进现有解决方案如 chrono 的 API。它提供了更简洁、直观的接口，并在设计上更加注重易用性和一致性。该库已经发布并获得社区关注，其作者 burntsushi 表示希望它能被更广泛的生态系统采用以取代 chrono。

hackernews · burntsushi · 11月16日 16:53 · [社区讨论](https://news.ycombinator.com/item?id=50519744)

**「背景介绍」** Jiff 1.0 是一个为 Rust 语言设计的新日期时间库，旨在改进现有解决方案如 chrono 的 API 设计。Chrono 是 Rust 社区中广泛使用的日期时间处理库，但其 API 被一些开发者认为存在不足之处，这促使了 Jiff 的开发。Jiff 试图通过提供更清晰、更现代的接口来解决这些问题，并且在设计上更加注重实用性和易用性。

**「对开发者的影响」** 对于需要处理日期时间逻辑的 Rust 开发者来说，Jiff 提供了一个新的选择，可能减少因旧版库（如 chrono）API 复杂而导致的开发负担。然而，由于其与现有代码库的兼容性问题，迁移可能需要一定成本。

**「社区讨论摘要」** 社区成员对 Jiff 的设计理念表示赞赏，尤其是它承认自身并非适用于所有场景的态度。同时有用户询问了关于时间尺度的支持情况，例如 TAI 和 UT1 等，显示出对其扩展性的兴趣。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.rs/chrono/latest/chrono/">Chrono : Date and Time for Rust</a></li>
<li><a href="https://github.com/polyfractal/rust-chrono/blob/master/README.md">rust - chrono /README.md at master · polyfractal/ rust - chrono · GitHub</a></li>

</ul>
</details>

**标签**: `#rust`, `#datetime`, `#software-engineering`

---

<a id="item-tech-news-5"></a>
### [百度 AI 营收达 132 亿元，商业化加速重塑增长逻辑](https://news.google.com/rss/articles/CBMijwFBVV95cUxQNlhucWRWc2ZUenhsZXBuVUo1Q3NfQncwdXJwNnJMZDBIWkxyakJyV0p3M0VBRlU0OU9xbWlqSk1jN08tcFZBUDdodS1BZEpwUFhfQUpINF93MTdWR0tEc2gxdVhUYnEzeXZ1LWxfYy1WMjYzRllKUVQtc2hUZkx4TENMLTdhOFBqajRBN2NsSQ?oc=5) ⭐️ 7.0/10

百度 AI 营收增长至 132 亿元人民币，表明其人工智能商业化进程取得显著进展。这一增长反映了 AI 技术在企业层面的广泛应用和价值实现，正在改变百度的增长路径。该营收数据标志着百度从技术驱动向商业变现转型的重要一步。

rss · Google News AI · 11月17日 07:37

**「背景」** 百度在 2026 年第三季度实现了 132 亿元人民币的 AI 业务收入，占其一般性业务收入的 53%。这一数字同比增长 37%，显示出 AI 商业化已逐渐成为公司核心增长动力。此前，百度的财报显示其总营收为 308.1 亿元，尽管广告业务仍在下滑，但 AI 相关的新业务表现强劲，表明公司在业务转型中正逐步摆脱传统业务的压力。

**「实际影响」** 对于百度而言，AI 营收的显著增长意味着其在人工智能领域的商业化策略已初见成效，有助于提升整体盈利能力并巩固其在中国人工智能市场的地位。这可能促使更多科技公司加大对 AI 商业化路径的投入，推动整个行业向更注重实际应用和变现的方向发展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.toutiao.com/article/7708705765695865407/">百度Q3财报出炉！AI收入132亿，广告还在掉，到底走到哪一步了？</a></li>
<li><a href="https://news.qq.com/rain/a/20261116A0EKI700">AI收入132亿、占比53%，百度的“智能组织”走到哪一步？</a></li>
<li><a href="https://original.ifeng.com/c/8y6Sm4wc7an">百度第三季度营收308.1亿元 核心AI新业务收入132亿元_凤凰网</a></li>

</ul>
</details>

**标签**: `#AI商业化`, `#百度`, `#中国科技公司`, `#营收增长`, `#人工智能市场`

---

<a id="item-tech-news-6"></a>
### [深圳发布全国首个《人工智能工具应用商业秘密保护指引》](https://news.google.com/rss/articles/CBMiWEFVX3lxTFBzbFdmZnNsZlU0aVdLVk5jM21IZkQ0Qk5VWjdOODZaMGV5WWhhWkhFZFJRRUdPR3RCRWRDWDQ5V1owOWpGUVBzVkQ0WEg2d1k2XzNzTDA1RjM?oc=5) ⭐️ 7.0/10

深圳市发布了全国首个《人工智能工具应用商业秘密保护指引》，这是中国首个针对 AI 工具应用场景下商业秘密保护的指导性文件。该指引旨在为企业使用 AI 工具过程中的知识产权保护提供规范依据。

rss · Google News AI · 11月17日 02:58

**「背景」** 深圳市市场监督管理局近日发布了全国首个专门针对人工智能工具应用的商业秘密保护指引，旨在为企业在使用 AI 工具时提供商业秘密保护的操作指南。该指引是继今年 6 月深圳推出多个行业商业秘密保护工作指引之后，在 AI 领域的一项具体监管举措，反映了地方对新兴技术中知识产权保护问题的关注和制度建设的推进。

**「影响分析」** 该指引的发布意味着企业在商业场景中使用 AI 工具时，将有明确的商业秘密保护规范可循，有助于降低因 AI 工具应用导致的知识产权风险，可能为其他地区提供参考模板。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sznews.com/news/content/2026-11/03/content_32206531.htm">sznews.com/news/content/2026-11/03/content_32206531.htm</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#intellectual property`, `#commercial secrets`, `#China tech policy`, `#AI governance`

---

<a id="item-tech-news-7"></a>
### [ICLR 2027 程序委员会对审稿进行 AI 检测](https://www.reddit.com/r/MachineLearning/comments/1xyf1tq/iclr_2027_pcs_ran_an_ai_detector_on_reviews_peer/) ⭐️ 7.0/10

ICLR 2027 程序委员会（PC）在审稿过程中使用 AI 检测工具，发现大量审稿人未披露其使用 AI 的情况。尽管允许使用 AI 辅助审稿，但要求必须明确说明使用情况。大多数审稿人未按要求披露 AI 使用情况，导致程序委员会要求相关审稿人更新其审稿内容并补充说明 AI 使用细节。此举引发了关于学术诚信和研究评价透明度的讨论。

reddit · r/MachineLearning · /u/otsukarekun · 11月17日 08:22

**「ICLR 2027 允许审稿使用 AI 但须披露」** ICLR 2027 会议制定了审稿人 AI 使用政策，允许有限且负责任地使用 AI 工具辅助撰写审稿意见，但强制要求披露使用情况，审稿表格中设有专门的 AI 使用披露字段。程序委员会主席此次通过 AI 检测器主动检查审稿内容，验证该政策的实际执行效果。

**「影响」** 该事件可能促使未来学术会议和期刊在审稿流程中加强 AI 使用的规范与审查，要求所有参与者必须明确披露其在评审过程中的 AI 使用情况，以维护学术诚信。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://iclr.cc/Conferences/2027/AIPolicyForReviewers">ICLR 2027 Policy on LLM use for writing reviews or meta reviews</a></li>
<li><a href="https://iclr.cc/Conferences/2027/ReviewerGuidelines">ICLR 2027 Reviewer Guidelines</a></li>

</ul>
</details>

**标签**: `#AI ethics`, `#academic publishing`, `#peer review`, `#research integrity`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美国科技公司面临对华业务两难](https://www.cnbc.com/2026/11/17/us-tech-firms-china-ties-political-pressure.html) ⭐️ 8.0/10

美国科技公司如英伟达和苹果正面临在华业务的两难境地，因中美政治与经济紧张局势加剧，以及美国对中国芯片出口的新限制。

rss · CNBC Finance · 11月17日 08:52

**「背景」** 美国政府收紧对华芯片出口管制，限制中国公司通过海外数据中心远程使用先进 AI 芯片，引发美国科技企业在中国市场战略的争议与调整。此前英伟达 CEO 黄仁勋因个人丑闻辞职，进一步加剧了外界对公司如何平衡中美关系的担忧。

**「影响」** 美国科技公司如苹果和英伟达在中国市场面临战略两难，因为中美政治紧张局势加剧及美国对先进芯片的出口管制，可能导致其供应链和市场准入受到威胁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bbc.com/news/live/c6zjry11v8w1t">Huang agrees to appear before Congress, US lawmakers... - BBC News</a></li>
<li><a href="https://corbettreport.com/from-jensen-huang-to-wwiii/">Episode 511 - From Jensen Huang to WWIII... | The Corbett Report</a></li>
<li><a href="https://www.cnbc.com/2026/11/16/nvidia-stock-price-jensen-huang.html">Nvidia stock slides as investors weigh Jensen Huang resignation</a></li>
<li><a href="https://www.cnbc.com/2026/11/17/nvidia-china-cloud-ai-chip-access.html">Nvidia warns chip buyers of legal risks tied to China access: sources</a></li>
<li><a href="https://reason.com/2026/11/16/trumps-new-chip-export-rule-targets-china-but-exempts-tiktoks-parent-company/">Trump’ s new chip export rule exempts TikTok’ s parent company</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-16/us-moves-to-limit-remote-access-to-advanced-ai-chips">US Moves to Curb China ’ s Remote Access to Nvidia’ s AI Chips</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_supply_chain">Apple supply chain - Wikipedia</a></li>
<li><a href="https://aei.org/wp-content/uploads/2025/06/RPT_Miller_Apple-Supply-Chain_June-2025.pdf">Apple&#x27;s Supply Chain: Economic and Geopolitical Implications</a></li>

</ul>
</details>

**标签**: `#geopolitics`, `#technology`, `#supply chains`, `#regulation`, `#corporate strategy`

---

<a id="item-finance-news-2"></a>
### [伯克希尔增持达美航空并减持美国银行股份](https://www.cnbc.com/2026/11/16/berkshire-hathaway-raised-its-stake-in-delta-air-in-the-third-quarter.html) ⭐️ 7.0/10

伯克希尔·哈撒韦在第三季度将其在达美航空的持股比例提高了 12%，同时减持了美国银行近 6%的股份。

rss · CNBC Finance · 11月16日 23:01

**「背景」** 由于燃油成本上升和美联储加息，美国航空业在第三季度面临压力，Delta Air Lines 股价下跌。与此同时，Berkshire Hathaway 在第三季度增持了 Delta 的股份，并减持了 Bank of America 的持股。

**「影响」** 此举可能对伯克希尔的股东和投资者产生直接影响，因其战略调整反映了对航空业和银行业在经济波动中前景的不同判断。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.delta.com/sites/default/files/2026-10/delta-air-lines-announces-september-quarter-2026-results.pdf">Delta Air Lines Announces September Quarter 2026 Financial ...</a></li>
<li><a href="https://ir.delta.com/news/news-details/2026/Delta-Air-Lines-Announces-June-Quarter-2026-Financial-Results/default.aspx">Delta Air Lines Announces June Quarter 2026 Financial Results</a></li>
<li><a href="https://www.reuters.com/business/energy/delta-air-lines-cuts-profit-outlook-fuel-costs-outpace-fare-gains-2026-10-09/">Delta warns of more airline capacity restraint as fuel shock ...</a></li>
<li><a href="https://www.cnbc.com/2026/09/16/fed-rate-decision-september-2026.html">Fed rate decision September 2026 : Rates rise to 3.75%-4%</a></li>

</ul>
</details>

**标签**: `#Investing`, `#Corporate Actions`, `#Economic Trends`, `#Market Analysis`

---

<a id="item-finance-news-3"></a>
### [美联储主席警告 AI 可能令人失望并导致失业](https://www.cnbc.com/2026/11/16/fed-ai-task-force-kevin-warsh.html) ⭐️ 7.0/10

美联储主席凯文·沃什强调人工智能对经济的重要影响，但警告称该技术可能导致大规模失业或无法实现预期效果。

rss · CNBC Finance · 11月16日 18:46

**「背景」** 美联储主席凯文·沃什在旧金山召开会议，强调人工智能（AI）对经济的重要影响，并警告其可能带来的就业冲击或未能达到预期效果。此次会议是其为研究 AI 对生产力和就业影响而设立的专项工作组首次听证会。

**「对经济和就业的潜在影响」** 人工智能可能带来生产力提升、维持高就业率，但也可能导致自动化失业或回报不及预期，从而引发经济放缓和失业率上升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.federalreserve.gov/monetarypolicy/productivity-and-jobs-task-force.htm">Federal Reserve Board - Productivity and Jobs</a></li>
<li><a href="https://finance.yahoo.com/economy/policy/article/warsh-kicks-off-first-task-force-hearing-on-how-ai-could-fuel-growth-or-disrupt-jobs-171720426.html?fr=sycsrp_catchall">Warsh kicks off first task force hearing on how AI could fuel ...</a></li>
<li><a href="https://www.sciencedirect.com/org/science/article/pii/S0953481426000588">A systematic analysis of the impact of artificial ...</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S2773032824000154">AI-induced job impact: Complementary or substitution ...</a></li>
<li><a href="https://www.oecd.org/en/publications/the-impact-of-artificial-intelligence-on-productivity-distribution-and-growth_8d900037-en.html">The impact of Artificial Intelligence on productivity ... - OECD</a></li>

</ul>
</details>

**标签**: `#AI`, `#monetary policy`, `#economy`, `#employment`

---

<a id="item-finance-news-4"></a>
### [美股芯片出口管制升级，欧洲股市再度承压](https://news.google.com/rss/articles/CBMicEFVX3lxTE5fRTQ2aUFMaVdBSV9oZkFraG1kMHBsdWpvRjhTMl9zbWJnYW5aQ2VwQkxNa3hvSEJLZUxpTXRMaGpleS1qUmhfdzZWZnJZMnZnRlU1X3k4M1pwNDlyMGJOdF9nNmthaWV3RVhXajBGeWM?oc=5) ⭐️ 7.0/10

美国升级芯片出口管制措施，对欧洲股市造成压力。

rss · Google News 财经 · 11月17日 08:04

**「背景」** 美国在 2026 年 11 月进一步收紧了对华芯片出口管制，要求企业出口人工智能芯片时需获得许可，以防止向中国等受限制国家提供计算能力。此举延续了自 2022 年以来逐步加强的政策趋势，旨在限制中国获取先进芯片技术。

**「影响」** 由于美国加强对芯片的出口管制，欧洲股市受到压力，主要因为市场担心人工智能领域的贸易限制会影响相关企业业绩。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/11/16/us-tightens-ai-chip-export-controls-to-deter-chinese-companies-from-accessing-compute-remotely/">US tightens AI chip export controls to deter Chinese ...</a></li>
<li><a href="https://eccnfinder.com/guides/ai-chip-export-controls-2026/">AI Chip Export Controls: 2026 EAR Rules Explained</a></li>
<li><a href="https://finance.yahoo.com/technology/articles/european-shares-slip-fresh-u-083821310.html?fr=sycsrp_catchall">European shares slip on fresh U.S. chip curbs - Yahoo Finance</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-17/european-stocks-fall-as-us-chip-curbs-ignite-fresh-ai-selloff">European Stocks Fall as US Chip Curbs Ignite Fresh AI Selloff</a></li>

</ul>
</details>

**标签**: `#regulation`, `#markets`, `#technology`, `#international trade`

---