---
title: "Learning more about Claude's mathematical capabilities"
date: 2026-08-10
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[Learning more about Claude's mathematical capabilities](https://www.anthropic.com/research/riemann-zeta)** — _Anthropic · Aug 10_

**Main takeaway:** An unreleased research version of Claude, asked to take a real stab at the Riemann hypothesis, didn't crack it — but along the way it improved a longstanding lower bound on the fraction of Riemann zeta zeros satisfying the hypothesis, from 41.6% to 67.2%.

**Main methods:**
- **What the bound measures.** It's the minimum proportion of the zeta function's zeros known to lie on the critical line; decades of incremental work had pushed it to 41.6%, and Claude's argument takes it to 67.2%.
- **Combining two separate lines of work.** Claude found that the Baluyot–Goldston–Suriajaya–Turnage-Butterbaugh results, which let Montgomery's 1973 techniques run without assuming the hypothesis, can be combined with a 2000 paper of Bombieri to beat the previous state of the art.
- **The shape of the proof.** Claude builds a suitable space of functions with a quadratic form induced by Weil, where zeros on the line give positive-definite subspaces and zeros off it give negative-definite ones, then writes down an inequality on the rank of that quadratic form in terms of first- and second-moment estimates.
- **Two-track verification.** Two mathematicians at Anthropic studied and validated the paper and wrote an informal note stating the proof concisely for experts; Claude also produced a formally verifiable version of the result, and Brian Conrey and Dan Goldston examined the paper on short notice.
- **Honest limitation.** Anthropic does not expect these techniques to lead to a proof of the Riemann hypothesis itself; the claim is about the pace of progress in models' mathematical capability, not about the hypothesis falling.
- **The prompt was just an unreasonable challenge.** The result came out of an Anthropic staff member telling Claude to attempt the full hypothesis, not from a project targeting the lower bound.

**[Claude 顺手把 Riemann zeta 零点的下界从 41.6% 推到了 67.2%](https://www.anthropic.com/research/riemann-zeta)** — _Anthropic · 8月10日_

**Main takeaway:** Anthropic 的人给一个还没发布的研究版 Claude 出了道离谱的题：认真去攻 Riemann 猜想。猜想当然没证出来，但在过程中它把"有多少比例的 zeta 零点落在临界线上"这个沿用多年的下界从 41.6% 提到了 67.2%。

**Main methods:**
- **这个下界是什么。** 它衡量的是已知落在临界线上的零点占比下限，几十年里数学家一点点把它推到 41.6%，Claude 这套论证直接推到 67.2%。
- **关键是把两条独立的线接上了。** Baluyot、Goldston、Suriajaya、Turnage-Butterbaugh 那一系列工作，让 Montgomery 1973 年的技术不用预设猜想成立也能用；Claude 发现把这些结果跟 Bombieri 2000 年的一篇论文拼起来，就能越过原来的 41.6%。
- **证明大致长什么样。** Claude 先构造一个合适的函数空间，配上由 Weil 诱导的二次型，线上的零点对应正定子空间、线外的对应负定子空间，然后写出一个用一阶和二阶矩估计来卡这个二次型秩的不等式。
- **验证走了两条路。** Anthropic 内部两位数学家把论文读完并验证过，还写了份给专家看的简版说明；Claude 自己也产出了一份可形式化验证的证明。领域内的 Brian Conrey 和 Dan Goldston 也在很短的时间里帮忙看了这篇论文。
- **需要注意的 caveat。** Anthropic 自己说，这套技术并不会顺着往下就把 Riemann 猜想证出来。这篇想说的是模型数学能力推进的速度，不是猜想要倒了。
- **起点只是一句随口的挑战。** 这个结果不是某个专门冲下界去的项目，就是有同事让 Claude 认真试试整个猜想，试出来的副产品。
