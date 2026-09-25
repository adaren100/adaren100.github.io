---
title: "Project Swap: What happens when agents trade for us?"
date: 2026-09-24
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[Project Swap: What happens when agents trade for us?](https://www.anthropic.com/research/project-swap)** — _Anthropic · Sep 24_

**Main takeaway:** Anthropic built a miniature barter economy — 201 employees across six offices, each bringing a book to give away and sending a Claude-powered agent onto a trading floor to haggle on their behalf. After a five-minute chat, an agent's ranking of 10 books matched its person's on 61% of pairs, and the market's shortfall came mostly from what agents didn't know about their people, not from how they traded.

**Main methods:**
- **A controlled sequel to Project Deal.** Where the first experiment put agents into a marketplace loosely, Project Swap fixes the setting: one book in, one book out, a closed population, and a digital trading floor that runs until time expires.
- **Preference elicitation measured directly.** Participants separately ranked 10 books by interest, giving a ground truth to score the agent's own ranking against — 61% pairwise agreement from a single short conversation, which Anthropic calls surprisingly good.
- **The bottleneck is information, not negotiation.** On the floor the agents traded well; the efficiency losses trace back to the agent's incomplete picture of its participant rather than to bad bargaining.
- **Counterfactual re-runs of every floor.** Anthropic replayed each trading floor dozens of times while varying the underlying model and the agents' instructions. The model mattered more than the prompt, and stronger models produced more efficient markets.
- **Framed around deals that never happen.** The motivating cases are mundane search-and-negotiation failures — a patient who takes one unaffordable quote as final, a better-matched job neither side has time to find, shift swaps and carpools — where a round-the-clock agent might close the gap.
- **Open questions the design surfaces.** How do you know an agent has understood you, who writes the rules of engagement for a platform where many agents meet, who gets in, and what happens when a deal falls through. Participants said they'd hand Claude roughly a third of their yearly book budget.

**[Project Swap：让 agent 替我们上场交易，会发生什么](https://www.anthropic.com/research/project-swap)** — _Anthropic · 9月24日_

**Main takeaway:** Anthropic 搞了个迷你以物易物市场，六个办公室 201 号员工每人拿一本想送出去的书，然后放一个 Claude agent 上交易大厅替自己讨价还价。参与者只跟 agent 聊了五分钟，agent 对 10 本书的排序就跟本人对上了 61% 的两两比较；市场最后没跑到最优，主要卡在 agent 对自己主人了解得不够，而不是它不会谈。

**Main methods:**
- **这是 Project Deal 的加强控制版。** 上一次是把 agent 比较松地扔进市场里，这回条件收紧了：一人一本进、一本出，人群封闭，交易大厅开到时间结束为止。
- **偏好抓得准不准，直接量了。** 参与者另外按兴趣给 10 本书排了个序，正好拿来当 ground truth 对照 agent 自己的排序，结果一次短对话就能对上 61% 的两两比较，Anthropic 自己都觉得这个数好得有点意外。
- **瓶颈在信息，不在谈判。** 真上了交易大厅，agent 们谈得挺好，效率上的损失回溯过去基本都是因为 agent 没把人摸透，而不是价还得差。
- **每个交易大厅都重跑了几十遍。** 他们换模型、换 agent 的 instruction，把每场重放几十次，发现底层模型的影响比 prompt 怎么写更大，模型越强的市场跑得越有效率。
- **动机来自那些本该发生却没发生的交易。** 举的例子都挺日常：病人拿到一个付不起的报价就放弃治疗，其实还有更便宜的诊所；一份更合适的工作双方都没空找到对方；还有换班、拼车这种小事。有个全天候待命的 agent，这些也许就能撮合上。
- **这套设计逼出来的几个问题。** 你怎么知道 agent 真的听懂你了？一堆 agent 凑到一起，谁来定规则、谁有资格进场、谈崩了算谁的？另外参与者说，愿意把一年买书预算的三分之一左右交给 Claude 去花。
