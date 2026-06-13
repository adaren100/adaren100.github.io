---
title: "Fluid, natural voice translation with Gemini 3.5 Live Translate"
date: 2026-06-10
draft: false
tags: ["Google DeepMind", "research", "big-tech-research"]
source_org: "Google DeepMind"
source_url: "https://deepmind.google/blog/fluid-natural-voice-translation-with-gemini-35-live-translate/"
---

**[Fluid, natural voice translation with Gemini 3.5 Live Translate](https://deepmind.google/blog/fluid-natural-voice-translation-with-gemini-35-live-translate/)** — _Google DeepMind · Jun 9_

**Main takeaway:** Gemini 3.5 Live Translate is a new audio model doing near-real-time speech-to-speech translation across 70+ languages, generating continuous translated speech that stays a few seconds behind the speaker while preserving intonation, pacing, and pitch.

**Main methods:**
- **Streaming, not turn-taking.** The model emits speech continuously rather than waiting for the speaker to stop, trading off some context for sync with the live conversation.
- **Auto language detection.** 70+ languages detected without manual configuration; designed to be noise-robust for messy real-world environments.
- **Preserves prosody.** Output keeps the original speaker's intonation, pacing, and pitch, avoiding the flat TTS feel of older systems.
- **Distribution.** Rolling out today: developers via the Gemini Live API and Google AI Studio (public preview), enterprises via Google Meet (private preview), consumers via Google Translate on Android and iOS.
- **Partners and integrations.** Agora, Fishjam, LiveKit, Pipecat, and Vision Agents handle the real-time media plumbing; Grab is piloting it for driver-passenger calls (10M+ voice calls/month); Meet will expand from 5 to 70+ languages and from English-only pairs to 2,000+ language combos.

**[Gemini 3.5 Live Translate 做实时语音翻译](https://deepmind.google/blog/fluid-natural-voice-translation-with-gemini-35-live-translate/)** — _Google DeepMind · 6月9日_

**Main takeaway:** Gemini 3.5 Live Translate 是一个新的 audio 模型，做 70 多种语言之间的近实时 speech-to-speech 翻译，输出是连续的翻译语音，比说话人滞后几秒，同时保留原说话人的语调、节奏和音高。

**Main methods:**
- **流式输出而不是轮流说。** 模型一边收一边吐，不等说话人说完——拿一点上下文的代价换和现场对话的同步。
- **自动识别语言。** 70 多种语言不用手动配置；专门针对嘈杂的真实环境做了 noise robust。
- **保留 prosody。** 输出保留原说话人的语调、节奏和音高，没有老 TTS 那种平板感。
- **分发渠道。** 今天开始铺：开发者通过 Gemini Live API 和 Google AI Studio（公开 preview），企业走 Google Meet（私有 preview），普通用户走 Android 和 iOS 上的 Google Translate。
- **合作方和集成。** Agora、Fishjam、LiveKit、Pipecat、Vision Agents 帮忙搞定实时媒体管道；Grab 在司机和乘客通话里试（每月 1000 万通语音）；Meet 从原来 5 种语言扩到 70+，从只能和英语互译扩到 2000+ 语言对。
