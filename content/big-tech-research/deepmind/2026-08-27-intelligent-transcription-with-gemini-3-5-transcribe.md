---
title: "Intelligent transcription with Gemini 3.5 Transcribe"
date: 2026-08-27
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Intelligent transcription with Gemini 3.5 Transcribe](https://deepmind.google/blog/intelligent-transcription-with-gemini-3-5-transcribe/)** — _Google DeepMind · Aug 27_

**Main takeaway:** Google DeepMind released Gemini 3.5 Transcribe, a speech-to-text model reporting an average Word Error Rate of 4.0% for streaming and 2.6% for non-streaming as measured by Artificial Analysis, now available to developers through the Gemini API.

**Main methods:**
- **Two APIs for two shapes of workload.** `gemini-3.5-transcribe-live` runs continuous bidirectional streaming with sub-second latency through the Live API for interactive voice apps; `gemini-3.5-transcribe` handles pre-recorded audio through the Interactions API with speaker attribution and word-level timestamps.
- **Transcription that edits as it listens.** The model resolves self-corrections ("let's meet Tuesday—no, Wednesday"), strips filler words, and auto-formats the output rather than emitting raw recognition text.
- **Function calling from inside transcription.** It can delegate tasks like image generation and file analysis to other Gemini models via function calls, currently only in the Gemini macOS app.
- **Custom vocabulary and 85+ languages.** Adapts to a supplied jargon list and unusual spellings, auto-detects and transcribes over 85 languages, and is claimed to hold up in noisy real-world environments including alphanumeric entities like postal codes and order IDs.
- **Speaker separation caps at three.** Multi-speaker attribution on pre-recorded audio is accurate for up to three speakers; support beyond three is labelled experimental.
- **Already shipping in consumer products.** The same model powers Rambler on Android and voice in the Gemini app on macOS, so this developer release follows deployment rather than preceding it.

**[Gemini 3.5 Transcribe：转文字的时候顺手把话也理顺了](https://deepmind.google/blog/intelligent-transcription-with-gemini-3-5-transcribe/)** — _Google DeepMind · 8月27日_

**Main takeaway:** Google DeepMind 放出 Gemini 3.5 Transcribe，按 Artificial Analysis 的测法，streaming 场景平均 WER 4.0%，非 streaming 2.6%，现在开发者可以直接通过 Gemini API 调。

**Main methods:**
- **两个 API 对两类活。** `gemini-3.5-transcribe-live` 走 Live API，双向流式、亚秒级 latency，给交互式语音应用用；`gemini-3.5-transcribe` 走 Interactions API 处理录好的音频，带说话人归属和词级时间戳。
- **一边听一边把话理顺。** 说话人自己改口（"周二吧，不对，周三"）它能处理掉，"嗯""啊"这类语气词直接删，还顺手排版，而不是把识别的原始结果丢给你。
- **转写过程里能 function calling。** 生成图片、分析文件这类活，模型可以通过 function call 交给别的 Gemini 模型，目前只在 macOS 版 Gemini app 里能用。
- **自定义词表加 85 种以上语言。** 你给一份专业术语和特殊拼写它就能适配，自动识别并转写 85 种以上语言，口音重、环境吵的场景官方说也扛得住，邮编、订单号这种字母数字混排的能听准。
- **说话人最多分到 3 个。** 录播音频的多说话人归属在 3 人以内准确，再多就标成 experimental 了。
- **消费端其实已经在跑了。** Android 上的 Rambler 和 macOS 版 Gemini app 的语音功能用的就是它，这次是先上产品，再开放给开发者。
