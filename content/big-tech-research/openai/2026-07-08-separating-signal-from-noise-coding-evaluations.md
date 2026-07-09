---
title: "Separating signal from noise in coding evaluations"
date: 2026-07-08
draft: false
tags: ["big-tech-research", "openai"]
---

**[Separating signal from noise in coding evaluations](https://openai.com/index/separating-signal-from-noise-coding-evaluations)** — _OpenAI · Jul 8_

**Main takeaway:** OpenAI audited SWE-Bench Pro, the coding benchmark it previously recommended as a SWE-bench Verified replacement, and estimates ~30% of its tasks are broken — echoing the contamination issues that killed SWE-bench Verified's usefulness.

**Main methods:**
- **Two-pass audit pipeline.** A datapoint analysis pipeline reviewed model attempts, task metadata, and failure traces to flag likely evaluation flaws, then each flagged task got multiple investigator-agent passes plus independent review by five experienced software engineers.
- **Convergent numbers from two methods.** The automated pipeline flagged 200 tasks (27.4%) as broken, while a separate human annotation campaign flagged 249 (34.1%) — landing OpenAI on a ~30% overall estimate.
- **Four failure categories.** Overly strict tests that enforce unstated implementation details, underspecified prompts that omit requirements hidden tests still check, low-coverage tests that let incomplete fixes pass, and misleading prompts that contradict what the tests require.
- **Context from SWE-bench Verified.** OpenAI previously found that benchmark's design and contamination issues had already made it useless as a capability signal, and had pushed the community toward SWE-Bench Pro as the fix.
- **Reported pass-rate jump.** On the 731-task public split, frontier model pass rates rose from 23.3% to 80.3% in eight months — a trajectory OpenAI now says is partly an artifact of broken tasks rather than pure capability gain.
- **Takeaway for the field.** Curating hard-but-fair benchmarks is genuinely difficult, and agents are becoming a scalable way to do systematic data-quality audits on eval sets.

**[SWE-Bench Pro 也翻车了,OpenAI 审计发现三成任务有问题](https://openai.com/index/separating-signal-from-noise-coding-evaluations)** — _OpenAI · 7月8日_

**Main takeaway:** OpenAI 之前把 SWE-Bench Pro 推荐为 SWE-bench Verified 的替代品,结果自己审计一遍下来发现,这个 benchmark 大概三成任务都是有问题的,跟当年拖垮 SWE-bench Verified 的污染问题如出一辙。

**Main methods:**
- **两轮审计流程。** 先用一套 datapoint analysis pipeline 检查模型的答题记录、任务元数据和失败轨迹,标出可能有问题的任务,再让 investigator agent 多轮复核,最后交给五位有经验的软件工程师独立审。
- **两条路径的数字对得上。** 自动化 pipeline 标出 200 个(27.4%)问题任务,人工标注这边单独标出 249 个(34.1%),两边一综合,OpenAI 给出大约 30% 的总体估计。
- **四类典型问题。** 测试过严(要求 prompt 里根本没写的具体实现细节)、prompt 描述不全(隐藏测试要求的东西压根没在题目里说清楚)、测试覆盖率太低(功能没做完也能过)、prompt 本身就带偏方向(跟测试要求对不上)。
- **和 SWE-bench Verified 的前情。** OpenAI 之前就发现那个 benchmark 设计缺陷加数据污染,已经测不出真实的软件开发能力,当时还专门建议大家转去用 SWE-Bench Pro。
- **通过率涨得有点可疑。** 在 731 个任务的公开集上,前沿模型八个月内通过率从 23.3% 涨到 80.3%,现在看这里面有一部分可能就是题目本身有问题,不完全是模型真变强了。
- **给整个行业的启示。** 做一个又难又公平的 benchmark 真的很难,而用 agent 来做大规模的数据质量审计,正在变成一个越来越靠谱的办法。
