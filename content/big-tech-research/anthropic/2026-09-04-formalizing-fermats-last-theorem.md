---
title: "Formalizing Fermat's Last Theorem"
date: 2026-09-04
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[Formalizing Fermat's Last Theorem](https://www.anthropic.com/research/formalizing-fermats-last-theorem)** — _Anthropic · Sep 4_

**Main takeaway:** Anthropic is releasing the first complete computer-checked proof of Fermat's Last Theorem, written in Lean by Claude working largely autonomously over 11 days. Along the way Claude produced 13 million lines of Lean and proved 29,500 intermediate theorems.

**Main methods:**
- **The novelty is verification, not new mathematics.** Anthropic explicitly contrasts this with recent AI-driven work on the Riemann hypothesis, which produced novel mathematics. Here the point is checking an existing proof the way you'd check an arithmetic computation with a calculator.
- **Lean as the target language.** The formalization encodes Wiles's reasoning into a form a computer can verify automatically, an idea proposed a decade after the 1995 proof by Dutch computer scientist Jan Bergstra.
- **It rides on an existing community effort.** Kevin Buzzard at Imperial College London kicked off a multi-year community formalization of FLT in Lean in 2024; mathematicians had been building up the encoding methods needed for a proof this complex ever since Bergstra's proposal.
- **Who ran it.** Tianyi Peng, an Anthropic researcher whose Columbia University group builds tools for AI formalization, set out only to test whether Claude could make progress on FLT. The result went further than expected.
- **Why the scale matters.** Wiles's 1995 proof ran to 129 pages and took months of painstaking human verification; understanding a novel result well enough to trust it can take months or years, and a single broken link invalidates everything downstream.
- **The failure mode this targets is real.** When Wiles presented the proof over three days of lectures in June 1993, two months into verification a reviewer's question exposed a critical gap that took him a year to fix. Buzzard's comment is that easy formalization could lighten the years-long burden of evaluating new results as AI produces more proofs. (The extracted body cuts off partway through the history, so the specifics of how Claude was scaffolded aren't available.)

**[Claude 花 11 天，把 Fermat 大定理的证明形式化跑通了](https://www.anthropic.com/research/formalizing-fermats-last-theorem)** — _Anthropic · 9月4日_

**Main takeaway:** Anthropic 放出了 Fermat 大定理第一份完整的、机器可验证的证明，用 Lean 写的，Claude 基本自己跑了 11 天做出来。中间它写了 1,300 万行 Lean，顺带证了 29,500 个中间定理。

**Main methods:**
- **新的地方是验证，不是新数学。** Anthropic 特意跟最近那波 AI 做 Riemann hypothesis 的工作划清界限，那边是产出了新数学，这边的重点是把一个已有的证明像用计算器核对算术那样查一遍。
- **落点选在 Lean。** 做的事情是把 Wiles 那套推理翻译成计算机能自动验证的形式。这个想法最早是荷兰计算机科学家 Jan Bergstra 提的，离 1995 年那份证明差不多隔了十年。
- **不是从零开始，是接在社区的活上。** Imperial College London 的 Kevin Buzzard 在 2024 年发起了一个用 Lean 形式化 FLT 的多年期社区项目。从 Bergstra 提议那会儿起，数学界就一直在攒编码这种复杂证明所需要的方法。
- **是谁在跑这件事。** Anthropic 研究员 Tianyi Peng，他在 Columbia University 的组本来就做 AI formalization 的工具。他最初只是想试试 Claude 在 FLT 上能推进到哪儿，结果比预想的走得远得多。
- **为什么这个体量值得说。** Wiles 1995 年那份证明有 129 页，人工验证花了好几个月。想把一个新结果吃透到敢说它没问题，动辄几个月甚至几年，而且逻辑链上断一环，后面全部可能作废。
- **它针对的是真实发生过的翻车。** 1993 年 6 月 Wiles 用三天讲完证明，验证进行到两个月的时候，一位审稿人一个问题就把一个关键漏洞捅出来了，Wiles 又花了一年才补上。Buzzard 的评价是，随着 AI 产出越来越多证明，形式化如果足够省事，就能把"评审一个新结果要耗好几年"这个负担卸掉不少。抓到的正文在讲历史的地方就断了，Claude 具体怎么搭的 harness 看不到。
