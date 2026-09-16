---
title: "Introducing Gemini 3.8 Live and 3.8 Live Extended Thinking"
date: 2026-09-16
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Introducing Gemini 3.8 Live and 3.8 Live Extended Thinking](https://deepmind.google/blog/introducing-gemini-3-8-live-and-3-8-live-extended-thinking/)** — _Google DeepMind · Sep 15_

**Main takeaway:** Google DeepMind released two live dialogue models for voice agents, and the bigger one — Gemini 3.8 Live Extended Thinking — takes the #1 overall spot on Artificial Analysis' Speech to Speech Quality Index at 82.6, plus 68.6% on τ-Voice and 97.7% on Big Bench Audio. The smaller Gemini 3.8 Live targets scale and cost, landing second in the Speech Agent Arena.

**Main methods:**
- **Two models, split by cost vs. complexity.** Gemini 3.8 Live is built for scale and cost efficiency, pairing conversational intelligence with fluid dialogue and visual grounding; 3.8 Live Extended Thinking is for high-complexity tasks with more intelligence and multi-step reasoning.
- **Parallel reasoning while the conversation keeps going.** The models run tool calls and background task execution without interrupting the dialogue, which is what makes the "think while you talk" behavior work.
- **Agentic voice benchmarks.** Extended Thinking leads agentic task completion with 68.6% on τ-Voice and 35.1% on Sierra's τ-Voice-banking benchmark, and scores 97.7% on Big Bench Audio for reasoning — at what DeepMind calls a competitive price point against other frontier models.
- **Real-time visual context and language switching.** Both models take real-time visual context alongside speech, and handle interruptions and mid-conversation language switching.
- **Shipping surfaces.** Available now through the Gemini API, the Gemini app, Google Workspace, and Search — positioned as production-ready building blocks for developers and enterprises building voice agents.
- **Caveat on the extract.** The post also cites ServiceNow's EVA-Bench, but the fetched body cuts off mid-sentence there, so those numbers aren't available here.

**[Gemini 3.8 Live 和 3.8 Live Extended Thinking 来了](https://deepmind.google/blog/introducing-gemini-3-8-live-and-3-8-live-extended-thinking/)** — _Google DeepMind · 9月15日_

**Main takeaway:** Google DeepMind 一口气放出两个做 voice agent 的实时对话模型。大的那个 Gemini 3.8 Live Extended Thinking 在 Artificial Analysis 的 Speech to Speech Quality Index 上拿了总榜第一，82.6 分，τ-Voice 68.6%，Big Bench Audio 97.7%。小的 Gemini 3.8 Live 主打便宜和跑量，在 Speech Agent Arena 排第二。

**Main methods:**
- **两个型号，按成本和复杂度分工。** Gemini 3.8 Live 是冲规模和成本效率去的，对话流畅度加上 visual grounding；Extended Thinking 那个专门啃高复杂度任务，智能更高，能做多步 reasoning。
- **一边聊一边并行推理。** 模型会在后台调工具、跑任务，同时对话不中断，所谓"边想边说"就是这么实现的。
- **agentic 语音 benchmark 上的成绩。** Extended Thinking 在 agentic task completion 这块领先，τ-Voice 68.6%、Sierra 的 τ-Voice-banking 35.1%，reasoning 那边 Big Bench Audio 97.7%，DeepMind 说价格相比其他 frontier 模型还挺能打。
- **实时看得见，还能中途换语言。** 两个模型都能接实时视觉输入，用户打断、说着说着切换语言，它都接得住。
- **上线的入口。** 现在 Gemini API、Gemini app、Google Workspace 和 Search 都能用，定位就是给开发者和企业拿来直接搭 voice agent 的现成积木。
- **抓取上的一个 caveat。** 原文还提到了 ServiceNow 的 EVA-Bench，但正文抓到那句就断了，具体数字这边看不到。
