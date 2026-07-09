---
title: "Introducing GPT-Live"
date: 2026-07-08
draft: false
tags: ["big-tech-research", "openai"]
---

**[Introducing GPT-Live](https://openai.com/index/introducing-gpt-live)** — _OpenAI · Jul 8_

**Main takeaway:** OpenAI launched GPT-Live, a new full-duplex voice model family now powering ChatGPT Voice, replacing the old cascaded speech-to-text/LLM/text-to-speech pipeline with a single model that can listen and speak simultaneously.

**Main methods:**
- **Full-duplex architecture.** Unlike cascaded systems that process each turn sequentially, GPT-Live listens and speaks at the same time, letting it interject "mhmm"/"yeah", handle quick back-and-forth, or stay silent while the user thinks.
- **Delegates to a frontier model for hard queries.** For web search, deep reasoning, or complex tasks, GPT-Live hands off to a background frontier model (GPT-5.5 at launch) and keeps talking naturally while waiting for the result.
- **Fixes cascaded-system tradeoffs.** The original ChatGPT Voice chained three separate models (STT → LLM → TTS), which lost information across handoffs and produced slow, stilted responses; GPT-Live collapses this into one model.
- **Two size tiers shipping now.** GPT-Live-1 and GPT-Live-1 mini are rolling out to ChatGPT users globally today, with an API version planned and a signup form for developers/enterprises.
- **Framed as a stepping stone.** OpenAI positions this as unlocking longer-running, more agentic voice interactions over time, not just a chat-quality upgrade.

**[OpenAI 发布 GPT-Live,语音模型换代](https://openai.com/index/introducing-gpt-live)** — _OpenAI · 7月8日_

**Main takeaway:** OpenAI 推出新一代语音模型 GPT-Live,现在已经是 ChatGPT Voice 的底层引擎,用一个能同时听同时说的全双工模型,取代了原来那套语音转文字、LLM、文字转语音三段拼接的老流程。

**Main methods:**
- **全双工架构。** 跟老式级联系统一轮一轮处理不一样,GPT-Live 能一边听一边说,可以插一句"嗯嗯""对对"、快速接话,或者在用户思考的时候安静地等着。
- **遇到难题就丢给后台的前沿模型。** 需要网页搜索、深度推理或者复杂任务时,GPT-Live 会把活儿甩给后台的前沿模型(目前是 GPT-5.5),自己继续跟你自然地聊着,等结果回来了再接上。
- **解决了老架构的老毛病。** 最早的 ChatGPT Voice 是三个模型串联(语音转文字到 LLM 到文字转语音),信息在中间容易丢,响应也慢还生硬;GPT-Live 直接把这些合并成一个模型。
- **两个尺寸今天就上线。** GPT-Live-1 和 GPT-Live-1 mini 已经开始面向全球 ChatGPT 用户推送,API 版本也在计划中,开发者和企业可以填表等通知。
- **OpenAI 把这个定位成一个跳板。** 不只是聊天体验升级,他们说这套东西以后能撑起更长程、更 agentic 的语音交互。
