---
title: "Introducing Gemini 4 Hydrogen"
date: 2026-11-13
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Introducing Gemini 4 Hydrogen](https://deepmind.google/blog/introducing-gemini-4-hydrogen/)** — _Google DeepMind · Nov 13_

**Main takeaway:** A model release: Gemini 4 Hydrogen is the fast, efficient member of the Gemini 4 family, built for rapid execution across everyday coding and agentic workflows, and it already edges past the frontier Argon model on the Artificial Analysis Intelligence Index (51 vs. 50 at its default high thinking level, 54 at xhigh). It ships to every tier — all of Google AI Studio, the Gemini API, Gemini for business, the Gemini app, Google Search, and paid AI Pro and Ultra subscribers in Google Antigravity — at a flat $1.50 / $7.50 per million input / output tokens across the whole 1M-token context window.

**Main methods:**
- **Positioned as the execution engine, not the architect.** Carbon and Argon stay the models for deep, long-horizon reasoning — system design, subtle bugs — while Hydrogen handles the disciplined part of the loop: writing code, running tests, verifying changes, either standalone or paired with the frontier models.
- **Orchestrator in Google Antigravity.** Instead of one model from start to finish, Orchestrator switches between models like Carbon and Hydrogen inside a single session; on Terminal-Bench 4.0 it hit near-Carbon task success rates while using 24% less quota and finishing 19% faster on average.
- **Fan-out pattern for parallel agents.** Carbon acts as coordinator while Hydrogen powers the worker and verifier agents that build and test changes simultaneously across isolated workspaces — more throughput without the token bill of running a frontier model everywhere.
- **Big jump over Gemini 3.8 Flash.** At its high default setting Hydrogen finishes tasks 2.5× faster, more than triples Terminal-Bench 4.1 scores (57% vs. 18.2%), and cuts fabricated claims by more than 5×.
- **Better recovery behavior.** DeepMind specifically calls out that it adapts cleanly when a tool call fails or a search comes back empty, which is where lighter agentic models usually fall apart.
- **Thinking levels are a dial.** The same model spans speed-vs-intelligence settings from fast everyday help in the Gemini app and Search up to the xhigh setting used for its top benchmark number.

**[Gemini 4 Hydrogen 来了](https://deepmind.google/blog/introducing-gemini-4-hydrogen/)** — _Google DeepMind · 11月13日_

**Main takeaway:** 一次模型发布。Gemini 4 Hydrogen 是 Gemini 4 家族里主打快和省的那一档，专门拿来跑日常编码和各种 agentic 工作流，而且在 Artificial Analysis Intelligence Index 上已经反超了前沿档的 Argon（默认 high thinking 下 51 比 50，开到 xhigh 能到 54）。这次是真的铺给所有人：Google AI Studio 全部档位、Gemini API、Gemini for business、Gemini app、Google Search，还有 Google Antigravity 里付费的 AI Pro 和 Ultra 用户；整个 100 万 token 上下文统一价，输入每百万 token $1.50，输出 $7.50。

**Main methods:**
- **它的定位是执行层，不是设计层。** 系统架构设计、揪那种藏得很深的 bug，这些还是 Carbon 和 Argon 的活儿；Hydrogen 负责循环里最需要稳的部分，写代码、跑测试、验证改动，既能单独用，也能跟前沿模型搭着用。
- **Google Antigravity 里新加的 Orchestrator。** 不再是一个模型从头干到尾，Orchestrator 会在同一个 session 里动态切换 Carbon 和 Hydrogen 这类模型；Terminal-Bench 4.0 上它做到了接近 Carbon 的任务成功率，但平均少用 24% 的额度，还快了 19%。
- **并行 agent 的分工套路。** Carbon 当协调者，Hydrogen 去驱动一堆 worker 和 verifier agent，在各自隔离的 workspace 里同时改和测，吞吐上去了，又不用处处烧前沿模型的 token。
- **比 Gemini 3.8 Flash 提升挺猛。** 同样是默认的 high 档，任务完成速度快了 2.5 倍，Terminal-Bench 4.1 分数直接三倍多（57% 对 18.2%），编造内容的情况也少了 5 倍以上。
- **失败之后能接得住。** DeepMind 特别提到，tool call 挂了、搜索返回空结果的时候它能顺畅地改路子，这恰恰是轻量 agentic 模型最容易崩的地方。
- **thinking level 可以当旋钮用。** 同一个模型从 Gemini app 和 Search 里的快速日常问答，一直调到跑出最高分那档 xhigh，速度和智力自己权衡。
