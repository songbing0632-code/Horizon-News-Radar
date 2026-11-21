---
layout: default
title: "Horizon Summary: 2026-11-21 (ZH)"
date: 2026-11-21
lang: zh
---

> 从 186 条内容中筛选出 14 条重要资讯。

---

**科技新闻**
1. [陶哲轩宣布 Navier-Stokes 奇点与广义黎曼假设的潜在证明](#item-tech-news-1) ⭐️ 10.0/10
2. [数学家急发 GRH 草稿以回应 AI 突破](#item-tech-news-2) ⭐️ 9.0/10
3. [Levent Alpöge 宣布用 AI 辅助的 Lean 证明广义黎曼猜想](#item-tech-news-3) ⭐️ 9.0/10
4. [Anthropic 数学家声称用 Claude 证明黎曼猜想](#item-tech-news-4) ⭐️ 9.0/10
5. [浙大首次在真机上实现量子随机存储器 QRAM](#item-tech-news-5) ⭐️ 9.0/10
6. [美院报 88 万 AI 芯输华军企](#item-tech-news-6) ⭐️ 8.0/10
7. [为规避 AI 误判，学术论文被迫降至“学生作文水平”](#item-tech-news-7) ⭐️ 7.0/10
8. [谷歌论文称实现 AI 递归自我改进](#item-tech-news-8) ⭐️ 7.0/10

**财经新闻**
1. [美股、黄金、比特币同时暴跌，纳指抹去年内所有涨幅](#item-finance-news-1) ⭐️ 10.0/10
2. [纳斯达克指数暴跌逾 10%，恐慌指数飙升](#item-finance-news-2) ⭐️ 9.0/10
3. [美联储主席沃什回避前瞻指引，其他官员发言量创 2025 年来新高](#item-finance-news-3) ⭐️ 8.0/10
4. [美国企业由回购转向大规模股票发行，牛市面临供应压力](#item-finance-news-4) ⭐️ 8.0/10
5. [阿根廷政府批准该国史上最大投资项目](#item-finance-news-5) ⭐️ 7.0/10
6. [A 股公司因财务造假面临 3400 万元罚款，年内股价下跌超 70%](#item-finance-news-6) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [陶哲轩宣布 Navier-Stokes 奇点与广义黎曼假设的潜在证明](https://terrytao.wordpress.com/2026/11/20/unforced-euler-singularity-unforced-navier-stokes-singularity-and-the-generalized-riemann-hypothesis/) ⭐️ 10.0/10

2026 年 11 月 20 日，数学家陶哲轩宣布了一项潜在证明，将 Navier-Stokes 方程奇点的存在性问题与广义黎曼假设联系起来，并通过包含约 1500 万行代码的 Lean 形式化验证工具完成验证。该证明声称使用了朗兰兹纲领和算术几何的现代成果，但正式声明中仍强调其为潜在证明，尚需同行审查。独立验证者确认两个独立内核接受了该结果，降低了内核漏洞的可能性，但仍有专家质疑形式化代码是否精确捕捉了原始数学问题的表述。

hackernews · archon1410 · 11月20日 17:21 · [社区讨论](https://news.ycombinator.com/item?id=50578358)

**「研究背景」** 纳维-斯托克斯方程的存在性与光滑性是克雷数学研究所悬赏的千禧年难题之一，要求证明三维不可压缩流体方程在给定光滑初始条件下是否必然存在光滑解。2016 年，陶哲轩曾证明一个平均化版本的三维纳维-斯托克斯方程会出现有限时间爆破，揭示了原始方程的可能奇异性。广义黎曼假设则是关于狄利克雷 L 函数零点分布的核心猜想，深刻影响着解析数论的诸多方向。

**「影响」** 若该证明经过审查被确证，它将同时解决 Navier-Stokes 方程光滑解存在性与广义黎曼假设这两个悬而未决的重大数学问题，但当前形式化验证的可靠性取决于 Lean 代码中对原始问题的精确建模，数学家需核实形式化表述与原始猜想的等价性。

**「社区讨论」** 社区评论中，部分用户表达了兴奋与恐惧交织的情绪，担忧 AI 已经超越人类智能，影响科学家职业生涯；技术层面，有人质疑 1500 万行 Lean 代码是否确实证明了所声称的数学定理，而非仅仅是形式化了一个无关的平凡命题，但另有评论指出两个独立内核的一致通过减少了内核级漏洞的风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Navier%E2%80%93Stokes_existence_and_smoothness">Navier – Stokes existence and smoothness - Wikipedia</a></li>

</ul>
</details>

**标签**: `#mathematics`, `#formal-verification`, `#AI`, `#Navier-Stokes`, `#Riemann-Hypothesis`

---

<a id="item-tech-news-2"></a>
### [数学家急发 GRH 草稿以回应 AI 突破](https://math216.wordpress.com/2026/11/20/hurried-announcement-alessandro-masullo-grh/) ⭐️ 9.0/10

2026 年 11 月 20 日，在人工智能公司 Anthropic 宣称其 AI 求解广义黎曼假设（GRH）后数小时内，数学家亚历山德罗·马苏洛（Alessandro Masullo）匆忙发布了一份长达 940 页的 GRH 证明草稿，试图确立优先权。该草稿尚不完整，第 1.1.1 节为空，且未经过同行评议，其正确性待定。此事件凸显了人类与 AI 在重大数学难题上竞赛时，优先权与验证流程面临的挑战。

hackernews · jasondavies · 11月20日 18:33 · [社区讨论](https://news.ycombinator.com/item?id=50579568)

**「背景」** 2026 年 11 月 20 日早些时候，Anthropic 员工 Levent Alpöge 发布了一项由 Claude 生成的证明，声称解决了数学界最著名的未解难题黎曼假设。这一声明直接促使数学家 Alessandro Masullo 通过 AMS 主席 Ravi Vakil 紧急公开了他长达 940 页、耗时约 12 年完成的广义黎曼假设证明草案，以争取发现的优先权。

**「影响」** 马苏洛的匆忙发布使其与 Anthropic 的优先权之争进入公开阶段，但草稿中明显的空白章节令其证明的有效性受到广泛质疑，双方成果均须通过数学界的严格审查才能获得认可。

**「社区讨论」** 有评论者推测，Anthropic 的 AI 可能无意中接触了该证明的早期片段（如通过相关数学家上传），要求对其进行数据审查；同时，手稿的空章节等问题引发了对证明完成度的质疑，凸显了悬而未决的优先权争议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.scientificamerican.com/article/dueling-claims-of-riemann-hypothesis-proofs-emerge/">Dueling claims of Riemann hypothesis proofs emerge</a></li>
<li><a href="https://xenospectrum.com/en/masullo-riemann-proof-draft-release/">Draft Proof of the Generalized Riemann Hypothesis, 12 Years ...</a></li>

</ul>
</details>

**标签**: `#mathematics`, `#ai`, `#research-ethics`, `#open-science`, `#academic-culture`

---

<a id="item-tech-news-3"></a>
### [Levent Alpöge 宣布用 AI 辅助的 Lean 证明广义黎曼猜想](https://alpo.ge/remark.pdf) ⭐️ 9.0/10

数学家 Levent Alpöge 于 2026 年 11 月 20 日发布了一份用 Lean 证明助手形式化的广义黎曼猜想（GRH）证明，并声称该证明获得了 AI 的辅助。该形式化文件体积达 1.3GB、约 1500 万行 Lean 代码，可通过其个人网站获取。目前该证明尚未经过同行评审或独立验证，其正确性仍待确认。

hackernews · iamronaldo · 11月20日 14:16 · [社区讨论](https://news.ycombinator.com/item?id=50574968)

**「背景」** Levent Alpöge 是立足于人工智能公司 Anthropic 的数学家，以在 Lean 中形式化重大定理而闻名，包括 2025 年与合作者给出的希尔伯特第十问题不可判定性的第二个证明。这一背景为理解他此次发布一个体积达 1.3 GB、约 1500 万行代码的广义黎曼假设 Lean 形式化证明提供了直接前提。

**「社区讨论」** 社区评论中，部分用户对 AI 能够辅助攻克如此困难的猜想表示震惊，并指出科幻作品曾对此持怀疑态度；另有用户关注证明的技术规模，提供了下载和统计该 1.3GB、约 1500 万行 Lean 代码的命令行方法，凸显了此类形式化证明的庞大体量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Levent_Alp%C3%B6ge">Levent Alpöge - Wikipedia</a></li>

</ul>
</details>

**标签**: `#mathematics`, `#formal-verification`, `#ai`, `#research`, `#lean`

---

<a id="item-tech-news-4"></a>
### [Anthropic 数学家声称用 Claude 证明黎曼猜想](https://www.scientificamerican.com/article/anthropic-mathematician-claims-to-prove-riemann-hypothesis-most-famous-problem-in-all-of-math/) ⭐️ 9.0/10

11 月 20 日，Anthropic 的数学家 Levent Alpöge 声称借助公司 AI 模型 Claude 证明了黎曼猜想，并发布了以可验证数学正确性的 Lean 语言编码的证明文稿，篇幅超过 25 万页。该声称还涵盖了广义黎曼猜想的证明，但尚未经过同行或独立验证。

telegram · zaihuapd · 11月20日 15:29

**「黎曼猜想简介」** 黎曼猜想由德国数学家伯恩哈德·黎曼于 1859 年提出，它描述了素数在自然数中的分布规律，是数学史上最著名的未解难题之一。该猜想的一个更广泛形式——广义黎曼猜想——此前也未被证明。如果声称的证明通过验证，将对数论及相关领域产生重大影响。

**标签**: `#anthropic`, `#claude`, `#riemann-hypothesis`, `#lean`, `#formal-verification`, `#ai-mathematics`

---

<a id="item-tech-news-5"></a>
### [浙大首次在真机上实现量子随机存储器 QRAM](https://finance.sina.com.cn/stock/2026-11-21/doc-iniznhsk3530826.shtml) ⭐️ 9.0/10

浙江大学团队在自主制备的超导量子芯片“天目 2 号”上，全球首次真机实现了量子随机存储器（QRAM），成果发表于《自然·物理》。该原型成功运行了 4 位和 8 位数据调取，准确率分别为 80.9%和 60.4%，线路深度较未优化方案降低 30%以上，并首次验证了该架构具有局部抗噪特性。

telegram · zaihuapd · 11月21日 08:31

**「量子随机存储器（QRAM）背景」** 量子随机存储器（QRAM）是量子计算机的关键组件，能以叠加态并行读取经典或量子数据，为许多量子算法（如量子机器学习、量子线性代数）提供数据访问支持。此前 QRAM 主要停留在理论方案或经典仿真阶段，在真实量子芯片上实现受限于噪声和保真度。浙江大学团队此次基于自研超导量子芯片“天目 2 号”，首次在物理量子比特上运行 QRAM 原型，验证了该架构的硬件可行性。

**标签**: `#quantum-computing`, `#QRAM`, `#quantum-memory`, `#superconducting-qubit`, `#research`

---

<a id="item-tech-news-6"></a>
### [美院报 88 万 AI 芯输华军企](https://news.google.com/rss/articles/CBMi5gNBVV95cUxPdFdPMWhPN3duNG5mNzd5T293WlhzRnZFaWVGa1cxa3dnbng5WU92eVY1LWd5WW9JRE1JRmJRZkI3UE90XzhlRHlTazRRMVMyVnk5X2xsRlpUS1E1dE8zVW8wZGozWDh4RXo2MV8tekVvaW90Y0d0OXl3aE1Fb1F1cHZOb2xMTUFCTTJFNDZDdVRCdTNDNGlZZlJRRTlaZEZNMDhNTmEyZEdGS3QxalNUUnB6NWIyZ3VMSlZYSHlrcG4ydDhUZnc1SGwzUjA1M0VWc1NrM1RHc3NHTWFrT09kYW53SUhhU1MzMW5ESlRwRjR3MkFiUU4tT0hzR0EwUGtiYkVfd1UyM1htNk9JcHRndE5aSEhHZElpSnN0enRfb05Idkp1NGJzVDhRcWNMYkxBZnppQjJnMVlxVjV4b0dFNUNEZE83RVZhUlpkbWpKcFRPWWFrZGpUNm94OWx2SGJqSzlycTBzZGZEVkJER0gzeC1PTkhsMTl3aVRDNDN5TGdfVmxXTnpTVkxic2N0MEt0RS1RbGYydXFxVHBhU3RzUmtCNFIwdXpGVTVwMmN2ckowVHlWZzJlNEJ4NXJUeFpYOWdCN2xSbHVHVVJQbEpCd1hqbzJCMnp4MnJ6andKelRrVlcwNFE?oc=5) ⭐️ 8.0/10

美国众议院最新披露的数据显示，近 88 万枚先进人工智能（AI）芯片已获批出口至中国。这批芯片的接收方中包括被美国国防部明确认定为“军工企业”的实体。该情况暴露出在对华半导体出口管制框架下，受限制的军事终端用户仍能通过许可程序获取关键硬件。

rss · Google News AI · 11月20日 11:40

**「美国对华 AI 芯片出口管制背景」** 美国近年来持续收紧对华先进 AI 芯片出口管制，要求相关芯片须获得商务部发放的出口许可证。这些限制至今仍被视为中国发展人工智能的主要障碍之一（《纽约时报》2026 年 11 月 3 日报道）。

**「潜在影响」** 此次披露揭露了出口管制执行层面的显著漏洞，原本被列入黑名单的中国军工企业仍可获取美国 AI 芯片。此举可能推动美国国会加速立法，要求国防部对涉军实体的许可申请拥有更直接的审查或否决权限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cn.nytimes.com/china/20261103/chinas-message-to-its-rivals-you-need-what-we-make/">中 国 技术 出 口 管制升级：利用 工 业 优势构建经济武器库 - 纽约时报 中 文网</a></li>

</ul>
</details>

**标签**: `#AI chips`, `#export controls`, `#China`, `#technology policy`, `#hardware`

---

<a id="item-tech-news-7"></a>
### [为规避 AI 误判，学术论文被迫降至“学生作文水平”](https://news.google.com/rss/articles/CBMiZkFVX3lxTE53Q3ViRHAyWjhaODdTV2hGTWNVXzl6NnlMdDc2Q0JIeHdvRm9IcWFQc3JUelpOeW41c3VEbUdnU3RQRjg5ZFdrQmttX2d5M3htaDB0WXJzQ0ZRdkRVTEw4aXR6dm1rZw?oc=5) ⭐️ 7.0/10

学术研究人员正面临 AI 检测工具带来的自证困局。为避免被误判为 AI 生成内容，他们不得不将论文修改至缺乏专业性的“学生作文水平”，导致学术严谨性受损。该报道指出，此类工具的高误报率正在迫使作者牺牲学术表达以换取低检出率。

rss · Google News AI · 11月21日 05:08

**「背景」** 近年来，学术期刊与高校越来越多地采用 AI 内容检测工具来识别可能由生成式 AI 撰写的文本，但这类工具在学术写作场景下的可靠性备受质疑。2026 年发表于《AI and Ethics》与《Discover Education》的研究指出，检测器存在系统性误报风险，尤其是对非英语母语作者的流畅表达或经过 AI 润色的文本容易做出错误判定，这种假阳性问题正迫使作者为规避误判而刻意简化语言，削弱论文的学术性。

**「影响」** 研究者因规避误判而过度简化写作，直接牺牲了论文的学术深度和专业术语准确性，从而削弱了学术出版的严谨性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://link.springer.com/article/10.1007/s43681-026-01376-w">The pitfalls of AI detection in academic writing: bias, false ...</a></li>
<li><a href="https://link.springer.com/article/10.1007/s44217-026-02307-x">AI content detection in student text assignments, false ...</a></li>

</ul>
</details>

**标签**: `#ai detection`, `#academic integrity`, `#nlp`, `#education technology`, `#ai ethics`

---

<a id="item-tech-news-8"></a>
### [谷歌论文称实现 AI 递归自我改进](https://news.google.com/rss/articles/CBMiTkFVX3lxTE5SOTdmTjhkWXJpemhxbzZPWFppSnd1Q0dfRnZaSmlmaGRHUzJUdnp1VEM5MXYxWXhGa3NoZDNxNEJSdmQ5RzV1Um5Tc0QwUQ?oc=5) ⭐️ 7.0/10

36Kr 报道称，谷歌一篇未详细公开的论文显示其内部已实现递归自我改进（RSI），并将 Anthropic 的 Opus 模型经验迁移至 Gemini，AI 获得了可延续的“进化记忆”。但报道未提供论文原文、具体版本或能力验证细节，因此这些成果目前仅为媒体转述的声称。

rss · Google News AI · 11月21日 04:12

**「背景信息」** 递归自我改进（RSI）是一种假设性过程，其中人工智能（AI）系统迭代设计出更强大的后续系统（tool-1-1）。此前有报道称，谷歌联合创始人谢尔盖·布林（Sergey Brin）曾表示，谷歌的 AI 正在接近实现这一目标，并以 Gemini 4 之前的 Flash 模型发布作为证据（tool-1-2）。此外，谷歌的 Dream RSI 论文曾被提及，据称其通过模拟过去的 AI 研究来寻找更优的发现路径（tool-1-3）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self - improvement - Wikipedia</a></li>
<li><a href="https://www.businessinsider.com/sergey-brin-google-gemini-ai-argon-recursive-self-improvement-rsi-2026-10">Sergey Brin Says Google &#x27;s AI Is Approaching... - Business Insider</a></li>
<li><a href="https://www.mindstudio.ai/blog/google-dream-rsi-recursive-self-improvement">What Is Dream RSI ? Google &#x27;s Recursive Self - Improvement , Explained</a></li>

</ul>
</details>

**标签**: `#artificial-intelligence`, `#recursive-self-improvement`, `#google`, `#gemini`, `#large-language-models`, `#research`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美股、黄金、比特币同时暴跌，纳指抹去年内所有涨幅](https://news.google.com/rss/articles/CBMicEFVX3lxTE5ybEZqVEZ6Q3lIbF9OdEZqUFdTZXdRdW9PYl9zLUFLa1RBNTVjbFdwcTNCUDRya3RPaGpMOEYyaFVNUGtZT1hjZ1BkNzRicUI0SXFkbWhfT3Ita2RYNFk1X3ZlWGxOWlFES1BIOUdYYlU?oc=5) ⭐️ 10.0/10

隔夜市场出现了股票、黄金和比特币无差别的同步暴跌，CBOE 波动率指数（VIX）一度飙升至 40 点，纳斯达克综合指数抹去了今年以来的全部涨幅。

rss · Google News 财经 · 11月20日 23:00

**「背景」** 此次全面抛售的直接触发因素是人工智能（AI）概念股及科技板块遭遇的猛烈获利了结，其中英伟达股价单日暴跌 14%，拖累主要股指进入技术回调区间。

**「影响」** 恐慌情绪的急剧升温导致跨资产持有人普遍受损，重仓科技股的投资者以及黄金、比特币多头均面临较大的账面损失，市场对未来经济前景的疑虑进一步加深。

**标签**: `#market turmoil`, `#VIX spike`, `#equity selloff`, `#bitcoin crash`, `#systemic risk`

---

<a id="item-finance-news-2"></a>
### [纳斯达克指数暴跌逾 10%，恐慌指数飙升](https://news.google.com/rss/articles/CBMiiAFBVV95cUxPYkRJbU5aVlVneUlhUG5ySU9TMHBTQ0R3TGt6dy1Qbm9VSFFQRDdaU19lT1FRV2J3Nlc3ZjNtSzdKeVBrWXJDRWlPbFNJYk5pYWpyTWd2R1R6ck5hNVZWT1F2dWI5ZHZMU0g4R3QtUnlPend3dWJQbmltUUlHRXplZFdTcFplRktX?oc=5) ⭐️ 9.0/10

纳斯达克指数单日暴跌超过 10%，同时被称为“恐慌指数”的 VIX 波动率指标大幅飙升。华尔街分析师警告，此轮抛售可能尚未结束（来源：Sohu 报道）。

rss · Google News 财经 · 11月21日 08:30

**「背景」** 被称为“恐慌指数”的标普 500 波动率指数（VIX）在 11 月 20 日收涨 26.2%至 35.89 点，盘中一度触及 40.03，为 2025 年 4 月以来最高水平。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://qhweb.eastmoney.com/news/202611213936813054.html">恐慌指数飙升：纳指狂泻逾10%，华尔街警告抛售“未完待续”</a></li>

</ul>
</details>

**标签**: `#美股`, `#纳斯达克`, `#恐慌指数`, `#抛售`, `#市场波动`

---

<a id="item-finance-news-3"></a>
### [美联储主席沃什回避前瞻指引，其他官员发言量创 2025 年来新高](https://www.cnbc.com/2026/11/20/warsh-fed-forward-guidance-rate-hikes.html) ⭐️ 8.0/10

美联储主席沃什拒绝就未来利率路径提供前瞻指引，导致其他联邦公开市场委员会成员频繁公开发言。据美国银行分析，过去两周的“联储讲话”量创下 2025 年初以来新高。

rss · CNBC Finance · 11月20日 21:10

**「背景」** 沃什认为前瞻指引会束缚决策者，因此拒绝暗示利率方向，这迫使其他官员通过密集讲话来表明立场。

**「影响」** 分析师警告，内部沟通分歧公开化可能加剧利率市场波动，并削弱美联储后续加息行动的可信度。

**标签**: `#Federal Reserve`, `#monetary policy`, `#forward guidance`, `#interest rates`, `#FOMC communications`

---

<a id="item-finance-news-4"></a>
### [美国企业由回购转向大规模股票发行，牛市面临供应压力](https://www.cnbc.com/2026/11/20/equity-issuance-bull-market-problem.html) ⭐️ 8.0/10

美国企业已从股票回购转向大规模发行股票，据 Acadian 资产管理公司分析，净新增发行量占总市值的 3.1%，可能给持续四年的牛市带来压力。

rss · CNBC Finance · 11月20日 14:15

**「背景」** 此前数年，企业通过净回购减少了市场流通股数，助推股价和每股收益上升。

**「影响」** 本周 Anthropic 的 IPO 募资 810 亿美元，但其股价上市后下跌并拖累大盘，凸显股票供应激增对市场的压力。

**标签**: `#equity issuance`, `#stock buybacks`, `#bull market`, `#capital allocation`, `#market trends`

---

<a id="item-finance-news-5"></a>
### [阿根廷政府批准该国史上最大投资项目](https://news.google.com/rss/articles/CBMiZ0FVX3lxTE1oTTJ4b1NBbWZIMXBGZ1E4cjg5R2prS3pYNlhHdEhGSWZld1g0am5xRWVDQ3VxYmo0RWxFUlk4eEFzN2JpR21IRDJCTlhFMlJacHotdDRnaHNJVTkyMExVbzhsY1NXdG8?oc=5) ⭐️ 7.0/10

阿根廷政府批准了该国迄今为止规模最大的投资项目，但官方尚未披露具体投资金额与行业细节。

rss · Google News 财经 · 11月21日 01:37

**「背景」** 阿根廷正面临高通胀和外汇储备压力，政府致力于通过大型项目吸引外国投资以稳定经济。

**「潜在影响」** 该大型投资项目一旦落地，可能为阿根廷创造大量就业岗位并带动相关产业发展，但具体经济拉动效应取决于后续公布的行业与资金规模。

**标签**: `#Argentina`, `#investment project`, `#government approval`, `#economic development`, `#foreign investment`

---

<a id="item-finance-news-6"></a>
### [A 股公司因财务造假面临 3400 万元罚款，年内股价下跌超 70%](https://news.google.com/rss/articles/CBMiY0FVX3lxTE9Hb0NGLWxKUV9hWUg2Zy1uZTB4c1dpZjRCeThWa1F4QmxLMEtWYXU2d29vWUdjdVVuTGpFeW1ka1YtZW10eTVEeHRHZFRueTFkV3FiLUhxVWpVS0tfUElqRXhrZw?oc=5) ⭐️ 7.0/10

中国监管机构计划对一家 A 股公司因财务造假处以 3400 万元人民币罚款，该公司股价今年已下跌超过 70%。

rss · Google News 财经 · 11月20日 18:35

**「背景信息」** 此前类似财务造假案件中，监管机构曾对公司及责任人合计拟处罚约 870 万元，其中包括公司罚款 180 万元，实际控制人及前董事长罚款 500 万元，其他责任人合计罚款约 190 万元。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://stock.10jqka.com.cn/20260531/c677103234.shtml">stock.10jqka.com.cn/20260531/c677103234.shtml</a></li>
<li><a href="https://finance.sina.cn/stock/ggyj/2026-05-31/detail-inhzurim9208298.d.html?vt=4">finance.sina.cn/stock/ggyj/ 2026 -05-31/detail-inhzurim9208298.d.html?...</a></li>

</ul>
</details>

**标签**: `#financial fraud`, `#regulatory penalty`, `#A-shares`, `#stock decline`, `#China`

---