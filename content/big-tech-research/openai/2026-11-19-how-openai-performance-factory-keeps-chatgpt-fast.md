---
title: "How OpenAI's Performance Factory keeps ChatGPT fast"
date: 2026-11-19
draft: false
tags: ["big-tech-research", "openai"]
---

**[How OpenAI's Performance Factory keeps ChatGPT fast](https://openai.com/index/how-openai-performance-factory-keeps-chatgpt-fast)** — _OpenAI · Nov 19_

**Main takeaway:** An engineering post by Okay Zed and Cyrus Forbes on the Performance Factory, an autonomous cloud system of Codex-powered workflows that finds and fixes ChatGPT performance regressions. In just over three months its first workflow tracked more than 1,700 investigations and root-caused over 600 cases — about 17 automated investigations a day.

**Main methods:**
- **Four-part architecture.** A task service with configurable workflows, a dispatch loop that assigns work, Codex running in the cloud, and subscriptions that wake the agent when something changes.
- **The Regression Workflow, end to end.** A performance alert opens a task; an agent investigates the slowdown, records findings in the task, and proposes a fix for an engineer to review; after deploy, another agent picks up the same task to check whether performance returned to baseline.
- **Adversarial review of the diagnosis.** A separate review step is used to strengthen the agent's root-cause claim rather than trusting the first investigation.
- **Fixing is harder than finding.** The post flags authoring the actual regression fix — not root-causing — as the hard part of the loop.
- **Engineers define the workflows, not the steps.** Teams write workflow definitions for recurring jobs plus instructions for the Codex agents that carry them out, which is how the team scaled from manual trace-and-log debugging (pre-Codex) to an agent factory.
- **Stated lessons.** Protect engineers' attention, evaluate changes to your agents, and turn recurring failures into self-repair. Next steps are broader applications and proactive monitoring instead of alert-driven response.

**[OpenAI 的 Performance Factory 是怎么把 ChatGPT 的速度盯住的](https://openai.com/index/how-openai-performance-factory-keeps-chatgpt-fast)** — _OpenAI · 11月19日_

**Main takeaway:** Okay Zed 和 Cyrus Forbes 写的一篇工程文章，讲他们搭的 Performance Factory：一套跑在云上的自动系统，用 Codex 驱动的 workflow 去找并修 ChatGPT 的性能回退。第一个 workflow 上线三个多月，跟了 1,700 多次调查，root cause 定下来的有 600 多个，平均一天 17 次自动调查。

**Main methods:**
- **整套东西分四块。** 一个能配 workflow 的 task service、一个负责派活的 dispatch loop、跑在云上的 Codex，再加上一套 subscription，环境一有变化就把 agent 叫起来。
- **Regression Workflow 从头到尾怎么走。** 性能 alert 一响就开一个 task，agent 去查这次变慢是怎么来的，把结论写回 task 里，再给出一个 fix 让工程师 review；部署完之后另一个 agent 接上同一个 task，确认性能是不是回到 baseline 了。
- **诊断结论要过一轮 adversarial review。** 不是第一份调查说什么就是什么，专门有一步用来挑刺，把 root cause 的结论夯实。
- **难的不是找，是修。** 文章自己说了，真正难的环节是把 regression 的 fix 写出来，而不是定位原因。
- **工程师定义的是 workflow，不是每一步。** 团队给常跑的活写 workflow 定义，再给执行的 Codex agent 写 instruction。他们就是这么从 Codex 之前那种手工翻 metric、翻 log、对 trace、上机器 debug，一路走到现在这种 agent factory 的。
- **他们总结的几条经验。** 保护工程师的注意力；改了 agent 要有 eval；反复出现的故障要变成能自愈的流程。下一步是往更多场景铺，以及从"等 alert"转成主动监控。
