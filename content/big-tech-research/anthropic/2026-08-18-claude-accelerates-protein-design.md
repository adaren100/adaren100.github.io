---
title: "How Claude is accelerating protein design and analytical chemistry"
date: 2026-08-18
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[How Claude is accelerating protein design and analytical chemistry](https://www.anthropic.com/research/Claude-accelerates-protein-design)** — _Anthropic · Aug 18_

**Main takeaway:** Two life-science results. Claude (Mythos Preview and Opus 4.8) designed protein binders from scratch against 15 targets and succeeded on 14, with 22–35% of individual designs binding versus the 10–15% typical of protein design campaigns today. Separately, Claude Opus 5 read a contract lab's raw NMR and LC-MS files from a two-sentence prompt and returned finished analyses in 23 and 19 minutes, matching the lab on hydrogen counts and purity (96.4% vs 96.33%).

**Main methods:**
- **Protein binder design as the benchmark task.** Designing binders against a target is an early-stage drug design step that has historically taken a specialist weeks to months per target; Claude was run against 15 targets and hit 14.
- **Hit rate beat the field, and so did affinity.** Depending on setup, 22–35% of individual designs bound successfully against a typical 10–15% baseline, and some of Claude's strongest designs bound several times more tightly than the best previously published result.
- **Analytical chemistry with almost no scaffolding.** Opus 5 was handed only the contract lab's raw files and a two-sentence prompt — no pipeline, no tooling described — and produced finished results in 23 and 19 minutes that matched the lab's own hydrogen counts and purity figure to within 0.07 points.
- **The generally available model did the chemistry.** Anthropic emphasizes that the chemistry result used Opus 5, which anyone can access, while the protein work needed Mythos Preview and Opus 4.8 — the point being that routine, time-intensive research work is already reachable with shipped models.
- **Access caveat.** Life science research tasks are currently blocked in Anthropic's most capable model; launching an access program for scientists is stated as one of their highest priorities, with Opus 5 the best generally available option until then.
- **Scope caveat.** Anthropic notes these two tasks sit only in the early stages of drug development, and that speeding up the pipeline end-to-end depends more on policy and operational bottlenecks than on core scientific capability. Context given for pace: Erdős problems are now falling at several a month, and Claude recently improved a longstanding lower bound on the Riemann zeta function.

**[Claude 开始给蛋白质设计和分析化学提速](https://www.anthropic.com/research/Claude-accelerates-protein-design)** — _Anthropic · 8月18日_

**Main takeaway:** 两个生命科学方向的结果。第一个是从零设计 protein binder，Claude（Mythos Preview 和 Opus 4.8）对 15 个 target 出手，14 个成了，单个设计的成功结合率在 22% 到 35% 之间，而现在业界做 protein design campaign 一般也就 10% 到 15%。第二个是 Claude Opus 5 拿到一家外包实验室的 NMR 和 LC-MS 原始文件，配一句两句话的 prompt，23 分钟和 19 分钟各出一份完整分析，氢原子计数和纯度都和实验室自己的结果对得上（96.4% 对 96.33%）。

**Main methods:**
- **为什么拿 protein binder 设计当题目。** 针对一个 target 设计 binder 是药物设计早期很典型的一步，以前专家做一个 target 要花几周到几个月。这次一口气上了 15 个 target，成了 14 个。
- **命中率和亲和力都压过现有水平。** 按不同设置，单个设计的成功结合率落在 22% 到 35%，对照的基线是 10% 到 15%。而且其中最好的几个设计，结合强度比此前公开发表的最佳结果还要高好几倍。
- **分析化学这边几乎没搭什么架子。** 给 Opus 5 的就是外包实验室的原始文件加两句话的 prompt，没有 pipeline，也没提什么专门工具，23 分钟和 19 分钟出结果，氢原子计数对上了，纯度差 0.07 个点。
- **化学那一半用的是人人能用的模型。** Anthropic 特意点明化学结果跑在 Opus 5 上，谁都能用；蛋白质那部分才需要 Mythos Preview 和 Opus 4.8。言下之意是那些又琐碎又耗时的常规科研工作，现在已经能用发布出来的模型接住了。
- **一个需要注意的点：能力还锁着。** 生命科学类研究任务在他们最强的模型上目前是被限制的。Anthropic 说给科学家开一个 access program 是当前最高优先级之一，在那之前 Opus 5 就是公开可用里最能打的。
- **另一个点：别把范围想大了。** 这两个任务都只落在药物开发的前段，Anthropic 自己说整条链路要提速，卡点更多在政策和运营层面，而不是核心科学能力。文章顺带给了个节奏参照：Erdős 问题现在一个月能倒下好几个，Claude 前不久还把 Riemann zeta 函数一个长期未破的下界往前推了一截。
