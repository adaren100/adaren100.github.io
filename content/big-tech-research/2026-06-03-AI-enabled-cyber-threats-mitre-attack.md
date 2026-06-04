---
title: "What we learned mapping a year's worth of AI-enabled cyber threats"
date: 2026-06-03
draft: false
tags: ["Anthropic", "research", "big-tech-research"]
source_org: "Anthropic"
source_url: "https://www.anthropic.com/news/AI-enabled-cyber-threats-mitre-attack"
---

**[What we learned mapping a year's worth of AI-enabled cyber threats](https://www.anthropic.com/news/AI-enabled-cyber-threats-mitre-attack)** — _Anthropic · Jun 2_

**Main takeaway:** Anthropic mapped 832 accounts banned for malicious cyber activity between March 2025 and March 2026 onto MITRE ATT&CK, and found attackers are pushing AI deeper into the attack life cycle — the share of actors scored medium-risk-or-higher jumped from 33% in the first six months to 56% in the second, a ~1.7× rise. They also argue MITRE ATT&CK no longer fully captures what makes AI-enabled attackers dangerous.

**Main methods:**
- **Dataset and mapping.** 832 banned-account cases with enough detail for thorough assessment were tagged against MITRE ATT&CK tactics and techniques; a subset of results was also published in Verizon's 2026 DBIR.
- **Where AI shows up in the kill chain.** 67.3% (560/832) of accounts used AI for malware writing and other prep work; a smaller 6.5% (54/832) used AI for lateral movement once inside a network — evidence that AI is moving past initial-access into post-compromise activity.
- **Shift from access to post-compromise.** AI-assisted account discovery (finding valid accounts inside a compromised env) rose 8.9% over the period, while AI-assisted phishing fell 8.6%, consistent with attackers applying AI deeper in operations.
- **Threat-level signals are breaking down.** Traditional risk signals — number of techniques used, sophistication of tools/interfaces — no longer correlate with actor skill, because AI now performs highly technical tasks on behalf of less-sophisticated operators.
- **Framework gap.** MITRE ATT&CK doesn't fully capture AI-specific tools and activities (e.g. agentic chaining of attack stages), which the report argues defenders need to start tracking explicitly.

**[Anthropic 用 MITRE ATT&CK 复盘了一年的 AI 网络攻击](https://www.anthropic.com/news/AI-enabled-cyber-threats-mitre-attack)** — _Anthropic · 6月2日_

**Main takeaway:** Anthropic 把 2025 年 3 月到 2026 年 3 月这一年里因为恶意网络活动被封的 832 个账号挨个映射到 MITRE ATT&CK 上，发现攻击者正在把 AI 用到攻击链更深的位置：被风险打分系统标成中高风险的比例，从前半年的 33% 涨到后半年的 56%，大概翻了 1.7 倍。他们还顺手指出，MITRE ATT&CK 已经盖不住 AI 攻击者真正危险的那部分能力了。

**Main methods:**
- **数据和映射方式。** 拿了 832 个 detail 足够多的被封账号，挨个打 MITRE ATT&CK 的 tactic/technique 标签，其中一部分结果还被收进了 Verizon 2026 年的 DBIR 报告。
- **AI 出现在攻击链的哪一段。** 67.3%（560/832）的账号是拿 AI 写 malware 和做攻击前准备；另外有 6.5%（54/832）已经在用 AI 做 lateral movement，也就是进到内网后横向走动，说明 AI 在往 post-compromise 阶段挪。
- **从拿初始访问转向拿内部立足。** 期间 AI 协助的 account discovery（在已攻陷环境里找有效账号）涨了 8.9%，AI 协助的 phishing 反而掉了 8.6%，能看出攻击者在把 AI 推到更靠后的环节。
- **判断 threat actor 等级的老办法失效了。** 过去看攻击者用了多少种 technique、工具有多花哨就大致能估出他的水平，但现在 AI 能替不太行的人干高技术含量的活，这套信号基本对不上号了。
- **框架本身有缺口。** MITRE ATT&CK 没有真正涵盖 AI 特有的工具和行为，比如 agentic 地把攻击各阶段串起来，报告认为 defender 得专门把这部分跟踪起来。
