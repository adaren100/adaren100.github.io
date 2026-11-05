---
title: "Gemini Omni 1.2 Flash: Fast and cost-effective with longer clips"
date: 2026-11-06
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Gemini Omni 1.2 Flash: Fast and cost-effective with longer clips](https://deepmind.google/blog/gemini-omni-12-flash-fast-and-cost-effective-with-longer-clips/)** — _Google DeepMind · Nov 6_

**Main takeaway:** A model release: Gemini Omni 1.2 Flash is now generally available on the Gemini API and Gemini for business, pushing native video generation from 10 to 15 seconds while cutting the price 30% from Omni 1.1 to $0.07 per second of 720p video.

**Main methods:**
- **Longer native clips with per-second control.** Generates and edits up to 15 seconds natively, and duration can be set in one-second increments from 3 to 15 seconds — enough for a product explainer or a full social ad spot in one generation.
- **Multi-turn conversational editing.** Clips can be fixed through follow-up turns instead of re-generating from scratch, which is where much of the cost saving comes from in practice.
- **Draft-cheap-then-upscale workflow.** The recommended pipeline is to draft at 360p or 720p, patch details with an edit, then upscale only the keepers to 1080p or 4K.
- **Richer reference conditioning.** Generation can be guided by character, product, or style images, motion clips up to three seconds, and audio cues; faces, garments, packaging typography, and brand colors are held across camera angles.
- **Less drift across a shot.** Character, object, and scene consistency holds from first to last frame with less morphing through motion and camera transitions, including when interpolating between keyframes or extending a clip.
- **Worked example given.** One model photo plus front-and-back shots of three outfits produced a 15-second virtual try-on sequence with 360-degree turns and match cuts, keeping identity and each garment's cut and drape intact.

**[Gemini Omni 1.2 Flash：片子更长了，价格还降了 30%](https://deepmind.google/blog/gemini-omni-12-flash-fast-and-cost-effective-with-longer-clips/)** — _Google DeepMind · 11月6日_

**Main takeaway:** 一次模型发布。Gemini Omni 1.2 Flash 在 Gemini API 和 Gemini for business 上正式 GA，原生视频长度从 10 秒拉到 15 秒，价格比 Omni 1.1 又降了 30%，720p 现在是每秒 $0.07。

**Main methods:**
- **原生长片，还能按秒指定。** 生成和编辑都能直接做到 15 秒，时长可以 3 到 15 秒按一秒一档来调，一次生成就够出一条产品讲解或者一整条社交广告。
- **多轮对话式编辑。** 哪里不对就接着聊、接着改，不用整条重新生成，省钱其实主要省在这儿。
- **先糙后精的工作流。** 官方推荐的做法是先用 360p 或 720p 快速打草稿，有细节问题就补一次 edit，最后只把满意的几条 upscale 到 1080p 或 4K。
- **reference 条件给得更足。** 可以同时拿角色图、产品图、风格图、最长 3 秒的动态片段和音频提示去引导生成，人脸、衣服、包装上的字体、品牌色这些换机位也还在。
- **一镜之内不容易漂。** 角色、物体、场景从第一帧到最后一帧的一致性更稳，运镜和转场时不太会 morph，首尾关键帧插值或者接着往后延长片段也一样。
- **官方给了个实例。** 一张模特照加三套衣服的正反面产品图，直接出了一段 15 秒的虚拟试穿，中间有 360 度转身和 match cut，模特的身份和每套衣服的版型、垂感都没跑。
