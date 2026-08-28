---
title: "Piloting the world's first double-blind AI evaluations"
date: 2026-08-27
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Piloting the world's first double-blind AI evaluations](https://deepmind.google/blog/piloting-the-worlds-first-double-blind-ai-evaluations/)** — _Google DeepMind · Aug 27_

**Main takeaway:** Google DeepMind ran what it calls the first double-blind evaluation of a proprietary, frontier-class model: a Gemini Flash Lite model tested against confidential external benchmarks inside a cryptographic enclave, so neither side ever sees the other's assets.

**Main methods:**
- **The problem is benchmark contamination.** If a model has seen the test prompts in advance, scores inflate and the benchmark stops meaning much; the post's analogy is a student who peeked at the exam before sitting it.
- **The old tradeoff being removed.** High-stakes external evals forced one of two disclosures — evaluators hand over their prompts, or the provider hands over model weights. Zero-logging protocols and contractual safeguards were the only guarantee on either side.
- **Confidential Space is the mechanism.** Running the eval inside Google Cloud's Confidential Computing portfolio lets both parties cryptographically verify that the evaluator never sees Gemini weights and Google never sees the evaluator's test prompts.
- **Who is in the pilot.** Partners are the Singapore AI Safety Institute, OpenMined, AVERI, and MLCommons; the model under test is a Gemini Flash Lite.
- **Where it matters most.** Framed for evals too sensitive to run in the open — cybersecurity testing and assessments run by government bodies — where data sovereignty concerns would otherwise block independent testing entirely.
- **Status and authors.** Written by William Isaac, Sol Messing, and Kristian Lum, and presented as a pilot they hope others build on rather than a finished program.

**[给前沿模型考试，双方都别看对方的底牌](https://deepmind.google/blog/piloting-the-worlds-first-double-blind-ai-evaluations/)** — _Google DeepMind · 8月27日_

**Main takeaway:** Google DeepMind 说这是业界第一次对闭源的前沿模型做 double-blind evaluation：把一个 Gemini Flash Lite 放进加密环境里，用外部机构保密的 benchmark 去测，两边谁也看不到对方的东西。

**Main methods:**
- **要解决的是 benchmark contamination。** 模型要是提前见过题，分数就是虚高的，这个 benchmark 也基本没意义了。原文打的比方是考生考前偷看了卷子。
- **以前只能二选一。** 高风险的外部评测，要么 evaluator 把题目交出去（模型方等于提前看到题），要么模型方把 weights 交出去（IP 就暴露了）。此前能依赖的只有合同条款和 zero-logging 协议。
- **靠 Confidential Space 落地。** 评测跑在 Google Cloud 的 Confidential Computing 里，两边都能用密码学手段验证：evaluator 摸不到 Gemini 的 weights，Google 也看不到对方的 prompt。
- **这次拉了谁一起。** 合作方是 Singapore AI Safety Institute、OpenMined、AVERI 和 MLCommons，被测的是 Gemini Flash Lite。
- **最吃这套的场景。** 那些敏感到没法公开跑的 eval，比如 cybersecurity 测试和政府主导的评估。以前卡在数据主权上，独立机构根本没法测。
- **作者和定位。** 文章署名 William Isaac、Sol Messing、Kristian Lum，他们自己也强调这只是 pilot，还不是成型的项目，希望别人能接着往下做。
