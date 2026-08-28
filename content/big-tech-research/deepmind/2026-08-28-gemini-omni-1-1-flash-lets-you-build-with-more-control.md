---
title: "Gemini Omni 1.1 Flash lets you build with more control"
date: 2026-08-28
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Gemini Omni 1.1 Flash lets you build with more control](https://deepmind.google/blog/gemini-omni-1-1-flash-lets-you-build-with-more-control/)** — _Google DeepMind · Aug 28_

**Main takeaway:** A developer-facing update to Gemini Omni, positioned as production-ready for generative video through the Gemini API: scenes can now be extended in 10-second increments up to 40 seconds total, with start/end frame control and 4K upscaling.

**Main methods:**
- **Scene extension now reads 10 seconds of prior context.** Earlier models referenced only the final second of a clip before continuing it; Omni 1.1 analyzes up to 10 seconds, which Google credits for the improved visual consistency and narrative adherence. Extensions come in 10-second increments to a cumulative 40 seconds.
- **First and last frame interpolation.** You set a start frame and an end frame and the model generates the transition between them, pitched as a way to get deliberate camera moves instead of whatever the prompt happens to produce.
- **360p previews as the cost and iteration lever.** Draft at low resolution while you are still working out the shot, then upscale the final cut to 4K for delivery.
- **Where it runs.** Available through the Gemini API in Google AI Studio and the Gemini Enterprise Agent Platform, aimed at generative video workflows, creative tools, and media editing software.
- **Camera work stays in the prompt.** The post's own examples drive shots with plain instructions like "continue the video, execute a cinematic optical dolly-zoom shot," rather than exposing a separate control surface for camera movement.

**[Gemini Omni 1.1 Flash：生成视频这回给了你更多控制权](https://deepmind.google/blog/gemini-omni-1-1-flash-lets-you-build-with-more-control/)** — _Google DeepMind · 8月28日_

**Main takeaway:** Gemini Omni 面向开发者的一次更新，官方口径是生成视频到这一版才算 production-ready：可以按 10 秒一段往后接，累计最长 40 秒，还能指定首尾帧、把成片升到 4K。

**Main methods:**
- **续写场景时能往回看 10 秒。** 之前的模型接着往下生成时只参考最后 1 秒，Omni 1.1 能吃进最多 10 秒上下文，Google 把画面一致性和叙事连贯性的提升就归在这一点上。每次续 10 秒，累计最多接到 40 秒。
- **首尾帧插值。** 你给定起始帧和结束帧，模型负责把中间那段补出来，卖点是运镜可以是你想要的样子，而不是 prompt 抽到什么算什么。
- **360p 预览用来省钱省时间。** 镜头还没想清楚的时候先出低分辨率草稿，定了稿再升到 4K 交付。
- **在哪儿用。** 通过 Google AI Studio 里的 Gemini API 和 Gemini Enterprise Agent Platform 接入，主要面向做生成视频流程、创作工具和剪辑软件的开发者。
- **运镜还是拿自然语言 prompt 指挥。** 官方给的例子就是直接写"continue the video，来一个 cinematic 的 dolly-zoom"这种话，没有另外做一套控制面板。
