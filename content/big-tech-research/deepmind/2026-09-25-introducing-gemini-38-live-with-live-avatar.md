---
title: "Introducing Gemini 3.8 Live with Live Avatar"
date: 2026-09-25
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Introducing Gemini 3.8 Live with Live Avatar](https://deepmind.google/blog/introducing-gemini-38-live-with-live-avatar/)** — _Google DeepMind · Sep 25_

**Main takeaway:** A week after the Gemini 3.8 Live launch, DeepMind is pairing the native live dialogue models with near real-time video generation, so an enterprise agent now answers with a visible, lip-synced persona instead of voice alone. It ships today in Gemini Enterprise.

**Main methods:**
- **Video generation coupled natively to speech.** Low-latency streaming video is generated alongside the audio rather than bolted on, which is what buys precise lip-syncing, facial expressions, and fluid turn-taking.
- **Simultaneous audio and visual input.** The model takes in what it sees and hears at the same time and responds with expressive audio and video, so the conversation stays multimodal in both directions.
- **Asynchronous tool calling keeps the dialogue alive.** The avatar can fire tool calls and fetch data in the background while still talking — the hotel check-in demo is the example DeepMind leads with — so complex tasks do not create dead air.
- **Multilingual speech-to-speech sync across 97 languages.** Lip-sync and expressions adapt dynamically and the avatar can switch languages mid-conversation without degrading video fidelity or introducing visual drift.
- **Custom avatars from a single reference image.** Developers can generate a fully animated, responsive avatar that preserves the reference likeness, brand styling, or character identity; there is also a preset library. Custom creation is gated behind enterprise allowlisting.
- **Safeguards framed around identity and disclosure.** DeepMind says the feature was built with strict safeguards designed to respect identity and keep AI-generated output transparent. The post's detail on how output is marked was cut off in the fetched body.

**[Gemini 3.8 Live 长出了脸：Live Avatar 上线](https://deepmind.google/blog/introducing-gemini-38-live-with-live-avatar/)** — _Google DeepMind · 9月25日_

**Main takeaway:** Gemini 3.8 Live 发布才一周，DeepMind 就把原生的 live dialogue 模型跟近实时视频生成拼到了一起，企业侧的 agent 现在不只是出声，还能顶着一张会对口型的脸跟你讲话。今天起在 Gemini Enterprise 里可以用。

**Main methods:**
- **视频是跟语音原生绑在一起生成的。** 低延迟的流式视频和音频一起出，不是事后贴上去的，所以口型、表情、还有轮流说话的节奏才能跟得这么准。
- **看和听同时进。** 模型把视觉和音频输入一起处理，再用有表情的音视频回你，等于来回两个方向都是多模态的。
- **异步 tool calling，话不会断。** Avatar 可以一边继续聊，一边在后台发 tool call 去取数据，DeepMind 举的例子是酒店前台给客人办入住这种活儿，好处是不会出现那种干等的冷场。
- **97 种语言的 speech-to-speech 同步。** 口型和表情会动态跟着调，聊到一半切语言也没问题，画面质量不掉，也不会出现视觉上的漂移。
- **一张参考图就能定制形象。** 开发者丢一张高质量参考图进去，就能生成一个能动能应答的 avatar，还保留原本的长相、品牌风格或角色设定；另外也有现成的预置形象库。定制这条路目前只对 enterprise allowlist 开放。
- **safeguard 主要围绕身份和标注。** DeepMind 说这套东西在做的时候加了比较严的 safeguard，一是尊重身份，二是让 AI 生成的内容保持可识别。不过抓到的正文在讲具体怎么标注的那句话被截断了。
