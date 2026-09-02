---
title: "Introducing agentic video understanding with Gemini"
date: 2026-09-02
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Introducing agentic video understanding with Gemini](https://deepmind.google/blog/introducing-agentic-video-in-gemini/)** — _Google DeepMind · Sep 2_

**Main takeaway:** Google shipped agentic video understanding on Gemini 3.7 Flash, 3.6 Flash and 3.5 Flash-Lite: instead of ingesting video at a fixed frame rate, the model decides what to watch and in which modality. Across standard video benchmarks it cuts token consumption by up to 88% and analysis cost by up to 66% while improving accuracy by up to 7%.

**Main methods:**
- **Agentic loop over native video tools.** The model pairs its core reasoning with Gemini's native video tools to search, scan and inspect specific segments across visual frames, audio and transcripts, fetching only the moments and signals it needs. This is the video analogue of agentic vision, which pairs code execution with native image understanding.
- **Replaces fixed-FPS static ingestion.** Current processing feeds the whole video in at a set frame rate (default 1 FPS, adjustable via API); agentic mode instead lets Gemini choose what to watch, at what speed, and through which modality.
- **Gains concentrate on long-form video.** From 10-minute how-to guides to 90-minute lectures and multi-hour recordings — exactly where static processing forces a choice between high token cost and sampling that drops critical details.
- **New capabilities, not just cheaper.** Sub-second moment retrieval, more accurate anomaly detection and precise counting all come out of the tool-driven approach.
- **Gemini 3.7 Flash sits on the pareto frontier.** All three models improve, but 3.7 Flash with agentic understanding gives both the best overall quality and the best quality-to-cost tradeoff among the models tested.
- **How to turn it on.** Set the API configuration to `agentic` in Google AI Studio or the Gemini Enterprise Agent Platform; it works today for both uploaded video and YouTube links.

**[Gemini 上线 agentic video：token 砍掉 88%，准确率还涨了](https://deepmind.google/blog/introducing-agentic-video-in-gemini/)** — _Google DeepMind · 9月2日_

**Main takeaway:** Google 给 Gemini 3.7 Flash、3.6 Flash 和 3.5 Flash-Lite 都开了 agentic video understanding。以前是按固定帧率把整段视频灌进去，现在换成模型自己决定看哪一段、用哪个模态去看。标准视频 benchmark 上跑下来，token 消耗最多降 88%，分析成本最多降 66%，准确率反而还涨了最多 7%。

**Main methods:**
- **一个 agentic loop 套在原生视频工具上。** 模型把自己的 reasoning 和 Gemini 原生的视频工具接起来，在画面帧、音频、transcript 之间去搜、去扫、去查具体片段，只把真正需要的那几个瞬间和信号取回来。思路跟之前的 agentic vision 是一套，那边是拿 code execution 配原生图像理解。
- **替掉固定 FPS 的静态处理。** 老做法是按设定帧率（默认 1 FPS，API 可调）把整段视频喂进去；agentic 模式下改成 Gemini 自己挑看什么、以多快的速度看、走哪个模态。
- **长视频上收益最明显。** 10 分钟的教程、90 分钟的讲座、几个小时的录像都算，恰恰是静态处理最难受的场景，要么 token 烧得很凶，要么抽帧的时候把关键细节漏掉。
- **不只是变便宜，还多了能力。** 亚秒级的 moment retrieval、更准的 anomaly detection、精确计数，都是靠这套工具调用做出来的。
- **Gemini 3.7 Flash 落在 pareto frontier 上。** 三个模型都有提升，但 3.7 Flash 开 agentic 之后质量最好，质量和成本的组合在测过的模型里也是最优的那个点。
- **怎么开。** 在 Google AI Studio 或 Gemini Enterprise Agent Platform 里把 API 配置设成 `agentic` 就行，上传的视频和 YouTube 链接现在都支持。
