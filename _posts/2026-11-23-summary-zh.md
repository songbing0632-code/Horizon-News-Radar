---
layout: default
title: "Horizon Summary: 2026-11-23 (ZH)"
date: 2026-11-23
lang: zh
---

> 从 223 条内容中筛选出 7 条重要资讯。

---

**科技新闻**
1. [GLM-5.4：首款循环 Transformer 推动通用编码发展](#item-tech-news-1) ⭐️ 8.0/10
2. [Codex2api 疑似遭供应链攻击](#item-tech-news-2) ⭐️ 8.0/10
3. [利用互联网档案馆旧视频打造免费替代电视网络](#item-tech-news-3) ⭐️ 7.0/10
4. [1700 万行 Lean 代码的挑战](#item-tech-news-4) ⭐️ 7.0/10
5. [韩国首次成功使用人工智能人形机器人完成手术](#item-tech-news-5) ⭐️ 7.0/10

**财经新闻**
1. [摩根大通与现代卡测试无需人工参与的 AI 代理交易](#item-finance-news-1) ⭐️ 7.0/10
2. [A 股大幅反弹，机器人概念股领涨](#item-finance-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [GLM-5.4：首款循环 Transformer 推动通用编码发展](https://z.ai/blog/glm-5.4) ⭐️ 8.0/10

智谱发布了 GLM-5.4，引入了 Loop Transformer 技术，旨在提高大语言模型（LLM）推理效率，特别针对内存带宽瓶颈问题。该模型目前开源，并与即将发布的 GLM-5.5 形成连续的技术迭代，后者预计将在 12 月发布，参数规模达到 3 万亿。

hackernews · foohis · 11月23日 10:06 · [社区讨论](https://news.ycombinator.com/item?id=50609685)

**「背景介绍」** GLM-5.4 是智谱推出的新一代大语言模型，其核心创新在于引入了 Loop Transformer 架构，旨在优化大模型推理过程中的内存带宽瓶颈问题。此前的大模型通常采用标准 Transformer 架构，其中每一层权重在推理过程中需要频繁地在高带宽内存（HBM）和计算芯片之间移动，造成显著的性能限制。

**「社区讨论」** 社区对 GLM-5.4 的技术透明性表示赞赏，认为这是与西方公司封闭策略的鲜明对比。部分用户指出，尽管循环 Transformer 在理论上具有潜力，但实际推理效率仍需进一步验证。

**标签**: `#LLMs`, `#Transformer architecture`, `#inference optimization`, `#memory bandwidth`, `#AI systems`

---

<a id="item-tech-news-2"></a>
### [Codex2api 疑似遭供应链攻击](https://github.com/WormW/codex2api-incident-2026-11) ⭐️ 8.0/10

Codex2api 作者账号疑似被黑客入侵，攻击者绕过 main 分支推送 tag，导致构建出的 v3.1.11 版本存在后门。该版本移除了鉴权机制，允许无密码远程执行命令；同时，攻击者通过 workflow 泄露了 16 个 Actions secrets，影响至少 21 个仓库。建议用户立即停用 3.1.10–3.1.12 版本，回退至 3.1.9，并轮换相关密钥。

telegram · zaihuapd · 11月23日 11:21

**「背景信息」** 供应链攻击是一种通过篡改软件开发、分发过程中的组件来植入恶意代码的安全威胁。此类攻击通常影响广泛，因为被篡改的组件可能被集成到多个项目中，导致多层扩散。近期，与 AI 工具和开发组件相关的供应链安全事件频发，例如恶意 npm 包和被窃取的认证令牌，凸显了供应链安全在现代软件开发中的重要性。

**「影响」** 已安装或更新至 Codex2api 3.1.10–3.1.12 的用户面临远程代码执行和敏感信息泄露风险。建议用户立即停用受影响版本，并轮换 GitHub token、SSH key、数据库和 DeepSeek 等相关密钥以防止进一步损失。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/tanishqnaru_ai-is-the-next-attack-surface-activity-7470629198714281985-ypIt">AI Security: Supply Chain Attacks and Data Poisoning | LinkedIn</a></li>
<li><a href="https://www.bleuken.com/ai-agents-hacked-real-companies-this-week-and-the-attack-didnt-need-the-model/">AI Agents Hacked Real Companies This Week — and the Attack ...</a></li>
<li><a href="https://labs.cosmicbytez.ca/news/2026-06-01-openai-codex-authentication-tokens-stolen-in-codexui-android-npm-supply-chain-at">OpenAI Codex Authentication Tokens Stolen via... | CosmicBytez Labs</a></li>

</ul>
</details>

**标签**: `#security`, `#supply-chain`, `#vulnerability`, `#developer-tools`, `#incident`

---

<a id="item-tech-news-3"></a>
### [利用互联网档案馆旧视频打造免费替代电视网络](https://spelunkr.tv/) ⭐️ 7.0/10

一个流媒体平台正在重新利用来自互联网档案馆（Internet Archive）的旧视频，为用户提供怀旧且异步的电视观看体验。该项目并未带来技术上的突破，但通过重新利用公开的存档内容，为数字历史的访问与重构提供了新的视角。

hackernews · SockThief · 11月23日 01:13 · [社区讨论](https://news.ycombinator.com/item?id=50606192)

**「背景信息」** Spelunkr.tv 是一个利用互联网档案馆（Internet Archive）中被遗忘的视频构建的免费替代性电视网络，提供怀旧且异步的电视观看体验。这一项目将公开的存档内容重新利用，创造了一种新颖的流媒体体验。

**「影响」** Spelunkr TV 提供了一种怀旧的电视观看体验，可能会激发对数字历史重新利用的兴趣，但它并未引入重大的技术革新或广泛的行业影响。

**「社区讨论」** 一些用户对该项目表示赞赏，称其提供了独特的怀旧体验（如观看 1980 年代音乐视频和广告），但也有人提出担忧，例如直接从互联网档案馆流媒体播放可能带来的负载问题，以及是否影响其原有用户体验。另有建议认为可采用去中心化平台（如 PeerTube）来优化并发观看体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://spelunkr.tv/">SPELUNKR — Cable TV , but weirder</a></li>

</ul>
</details>

**标签**: `#streaming`, `#Internet Archive`, `#media curation`, `#nostalgia`, `#user experience`

---

<a id="item-tech-news-4"></a>
### [1700 万行 Lean 代码的挑战](https://micjm.com/blog/yes-17m-lines-of-lean-is-a-lot/) ⭐️ 7.0/10

这篇博客文章探讨了使用大型语言模型（LLMs）生成 1700 万行 Lean 代码所面临的挑战和影响。文章引发了关于 AI 在复杂软件工程任务中作用的讨论，特别是在代码的可读性、审查难度以及潜在隐藏问题方面的担忧。

hackernews · seizethecheese · 11月23日 05:00 · [社区讨论](https://news.ycombinator.com/item?id=50607668)

**「背景信息」** Lean 是一种开源编程语言和证明助手，旨在实现正确、可维护且经过形式验证的代码。此前，社区已在尝试使用大型语言模型（LLM）生成 Lean 代码，但 AI 生成的代码质量尚未达到数学库（如 Mathlib）的标准。2026 年 4 月的报道提到，管理数百万行 mathlib 代码已颇具挑战，而如今生成 1700 万行 Lean 代码更引发了关于可读性和审查可行性的讨论。

**「影响」** 随着 AI 辅助生成大量形式化代码，形式验证的重要性日益凸显。对于安全性和可靠性要求高的系统，形式化验证能够排除整类不安全行为，而不仅仅依赖测试结果。这种趋势可能会推动形式化方法在工业软件工程中的应用，使其逐渐成为主流技术。

**「社区讨论」** 社区评论指出，LLMs 在生成代码时往往缺乏对目标读者背景的理解，导致生成的代码难以阅读和审查。有评论提到，如此庞大的代码量让人类完全审查变得不现实，甚至可能隐藏额外信息。

<details><summary>参考链接</summary>
<ul>
<li>Lean Programming Language</li>
<li>Getting Started with Lean 4: Proofs as Code for Real Developers - Medium</li>
<li>Are we stuck with Lean? - MathOverflow</li>
<li><a href="https://www.prover.com/verification-validation/ai-makes-formal-verification-more-important-here-is-why/">AI makes formal verification more important. Here is why - Prover...</a></li>
<li><a href="https://martin.kleppmann.com/2025/12/08/ai-formal-verification.html">Prediction: AI will make formal verification go mainstream — Martin...</a></li>

</ul>
</details>

**标签**: `#AI-assisted coding`, `#formal verification`, `#LLMs`, `#software engineering`, `#code readability`

---

<a id="item-tech-news-5"></a>
### [韩国首次成功使用人工智能人形机器人完成手术](https://news.google.com/rss/articles/CBMiZEFVX3lxTFB6TUcwT1cwOVNESjRZRjg4RTFjbjB1MXJSazRqNi02WnBUaFVlQ1pXeDlMZGZfWEpQSll4SW5qZmdoSXl6MDBLa1M1UURCYXd5Wl9ESGppeUJOT0daVkJSQXBrVXU?oc=5) ⭐️ 7.0/10

韩国首次成功使用人工智能人形机器人执行手术，这标志着医疗机器人技术的重要进展。此次手术展示了人工智能与医疗技术结合的潜力，但尚未披露具体的技术细节或应用条件。

rss · Google News AI · 11月22日 20:00

**「背景信息」** 此前，人工智能在医疗领域的应用主要集中在辅助诊断和影像分析等方面。随着机器人技术和人工智能算法的进步，人形机器人开始被探索用于更复杂的医疗任务，如手术操作。

**「影响」** 这次成功手术可能推动医疗领域对手术机器人更广泛的研究和应用，尤其是在复杂操作中提高精准度和减少人为失误方面。

**标签**: `#Artificial Intelligence`, `#Robotics`, `#Healthcare Technology`, `#AI Applications`, `#Medical Innovation`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [摩根大通与现代卡测试无需人工参与的 AI 代理交易](https://www.cnbc.com/2026/11/18/jpmorgan-hyundai-card-ai-agents-payments.html) ⭐️ 7.0/10

摩根大通与韩国现代卡完成了首个基于区块链的 AI 代理自主交易测试，目标是在 2027 年上半年进行更复杂的多 AI 代理测试。

rss · CNBC Finance · 11月23日 06:06

**「背景」** 此次测试涉及现代卡的 AI 代理请求外汇交易以维持欧元流动性，属于企业资金管理的探索性应用。

**「影响」** 若成功推广，AI 代理交易可能改变企业资金管理方式，但目前仍受限于治理和安全风险。

**标签**: `#AI in Finance`, `#Corporate Treasury`, `#Financial Technology`, `#Blockchain`, `#AI Governance`

---

<a id="item-finance-news-2"></a>
### [A 股大幅反弹，机器人概念股领涨](https://news.google.com/rss/articles/CBMijwFBVV95cUxNQVBfVXM2dUtEZmlUaFRpbHl0UHZqQmFZb1JrYVhhSHJMQkNTMHVMTmRaOVpnNFIyNWhiODJDTEEtNUpWV0VhcmtqNEV3LVVoNlc5QXF0cEpRWmg2THFGYUYzMGFVa05pdFJHQjZnTDZyM3hDQ1lEWmFocWtWNFpfbXpuWk5Fc3lZTkNUQ1ZmRQ?oc=5) ⭐️ 7.0/10

2026 年 11 月 23 日，中国股市出现强劲反弹，超过百只股票涨停，机器人相关概念股表现尤为突出。

rss · Google News 财经 · 11月23日 08:55

**「背景」** 此前多个消息指出市场情绪回暖，包括政策支持和资金流入，推动超过 4600 只个股上涨。

**「影响」** 此次反弹增强了投资者信心，可能吸引更多资金进入市场，尤其是机器人等高科技领域。

**标签**: `#stock market`, `#China`, `#robotics`, `#market rebound`, `#investor sentiment`

---