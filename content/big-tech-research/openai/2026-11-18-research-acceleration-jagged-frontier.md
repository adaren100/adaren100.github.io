---
title: "Research acceleration: The jagged frontier"
date: 2026-11-18
draft: false
tags: ["big-tech-research", "openai"]
---

**[Research acceleration: The jagged frontier](https://openai.com/index/research-acceleration-jagged-frontier)** — _OpenAI · Nov 18_

**Main takeaway:** OpenAI's second internal report on how much coding agents are accelerating its own AI research. Agents now autonomously complete nearly half of tasks estimated at two to four hours of human work — up from 23% in March to 46% in October — but the uplift is jagged, and humans remain central to the research loop.

**Main methods:**
- **Autonomous success by task length.** March → October, estimated success rose 23% → 46% on two-to-four-hour tasks and 13% → 35% on four-to-eight-hour tasks.
- **Jaggedness is the headline, not the average.** A task-level breakdown gives 79% autonomous success for monitoring training runs, 35% for launching training runs, and 25% for writing inference-and-serving-stack code.
- **Agent spend as a usage signal.** At API list prices, the median researcher's daily usage hit $2,400 in October, up 62% from September; the 90th percentile hit $23,000, up 105% — so the heaviest users are pulling further ahead.
- **Revealed preference via survey.** Asked what they would give up to keep frontier coding agents for three months, researchers' median answers were 30% of team compute, or 40% of team headcount in a separate question.
- **Human effort shifting to safety.** Safety and Alignment saw the largest absolute increase in documented research effort of any major OpenAI research area — documented workweeks up 77% from January to September, from both new hires and existing researchers switching in, with growth picking up after the response to the July 2026 Hugging Face incident.
- **Framed as RSI reporting, and explicitly partial.** The report extends OpenAI's September post and argues labs should be required to track and publicly report indicators of recursive self-improvement; the authors call the picture broader but still incomplete, measuring inputs, process, and outputs (lines of code changed, research experiments, OpenAI ECI).

**[研究加速报告：能力边界是锯齿状的](https://openai.com/index/research-acceleration-jagged-frontier)** — _OpenAI · 11月18日_

**Main takeaway:** OpenAI 的第二份内部报告，讲 coding agent 到底把他们自己的 AI 研究加速了多少。现在那种估计要人干两到四小时的任务，agent 自己能做成的接近一半：3 月是 23%，10 月到了 46%。但这个提升是锯齿状的，人还是研究 loop 里的核心。

**Main methods:**
- **按任务长度看自动完成率。** 3 月到 10 月，两到四小时的任务从 23% 涨到 46%，四到八小时的从 13% 涨到 35%。
- **重点是不均匀，不是那个平均数。** 拆到具体任务上：盯 training run 的成功率 79%，启动 training run 35%，写 inference 和 serving stack 的代码只有 25%。
- **用 agent 花了多少钱当使用强度的指标。** 按 API 标价算，中位数研究员 10 月每天用掉 2,400 美元，比 9 月涨 62%；90 分位到了 23,000 美元，涨 105%。重度用户正在越拉越开。
- **问他们愿意拿什么换。** 调查里问"要保住前沿 coding agent 再用三个月，你愿意付出什么"，中位数答案是让出团队 30% 的 compute，另一个问题里是让出 40% 的 headcount。
- **人力明显在往 safety 这边挪。** Safety and Alignment 是 OpenAI 所有主要研究方向里 documented research effort 绝对增幅最大的，1 月到 9 月 documented workweek 涨了 77%，既来自新招的人，也来自原有研究员转过来。2026 年 7 月应对 Hugging Face 事件之后这个增速明显加快。
- **这份报告是当 RSI 披露来写的，而且自己说不完整。** 它接着 9 月那篇写，主张应该强制要求实验室跟踪并公开 recursive self-improvement 的指标。作者自己说这次的图景更宽了但仍然是局部的，分 input、process、output 三层来量（output 包括改了多少行代码、跑了多少 research experiment、以及 OpenAI ECI）。
