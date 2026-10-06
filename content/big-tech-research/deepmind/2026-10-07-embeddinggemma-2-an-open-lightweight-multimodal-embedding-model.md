---
title: "EmbeddingGemma 2: an open, lightweight multimodal embedding model"
date: 2026-10-07
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[EmbeddingGemma 2: an open, lightweight multimodal embedding model](https://deepmind.google/blog/embeddinggemma-2-an-open-lightweight-multimodal-embedding-model/)** — _Google DeepMind · Oct 7_

**Main takeaway:** An open-weights model release: EmbeddingGemma 2 is a 740M-parameter, Apache 2.0 embedding model that natively maps text, code, images, audio, and video into one shared space on-device. Its headline gain is code retrieval, where MTEB Code jumps 9.92 points over EmbeddingGemma 1 (68.76 → 78.68).

**Main methods:**
- **Built on the Gemma 4 architecture.** Successor to last year's text-only EmbeddingGemma (20M+ downloads), sized at 740M parameters specifically for on-device inference, and sharing technology with the Gemini Embedding models.
- **Modular encoders.** Text-only workloads need as little as 270M parameters, with optional vision (170M) and audio (300M) encoders bolted on for full multimodal support.
- **Matryoshka Representation Learning for storage.** Output vectors can be truncated from 768 dimensions down to 512, 256, or 128, giving up to 6x less storage and memory for local vector databases.
- **Measured on-device footprint.** Quantized on a Google Pixel 11 Pro, it needs roughly 191MB active RAM for text-only weights and roughly 567MB for the full multimodal model.
- **8K context, 4x EmbeddingGemma 1.** That covers up to 5.5 minutes of audio, 29 images, or 58 video frames, including interleaved combinations, processed entirely on local hardware.
- **Quality-per-parameter claims.** Leading scores among sub-1B multimodal embedders on benchmarks like MTEB Code and MAEB, with multilingual text performance held steady and some specialist models more than twice its size beaten outright. Full numbers are in the model card.

**[EmbeddingGemma 2：740M 参数，把文字图片音视频塞进同一个 embedding 空间](https://deepmind.google/blog/embeddinggemma-2-an-open-lightweight-multimodal-embedding-model/)** — _Google DeepMind · 10月7日_

**Main takeaway:** 一次开源权重发布。EmbeddingGemma 2 只有 740M 参数，Apache 2.0 许可，原生就能把文本、代码、图片、音频、视频映射到同一个 embedding 空间，而且整个过程跑在端侧。最大的提升在代码检索，MTEB Code 从 68.76 涨到 78.68，差了 9.92 分。

**Main methods:**
- **架构基于 Gemma 4。** 去年那版只做文本的 EmbeddingGemma 下载量超过 2000 万，这次算是它的续作，740M 这个体量就是冲着端侧 inference 设计的，底层技术和 Gemini Embedding 系列同源。
- **encoder 是模块化的。** 只跑文本最少 270M 参数就够，想要完整多模态再挂上 vision（170M）和 audio（300M）两个 encoder。
- **用 Matryoshka Representation Learning 省空间。** 输出向量可以从 768 维直接截到 512、256 或者 128 维，本地 vector database 的存储和内存占用最多能省到六分之一。
- **端侧实测占用。** 做完 quantization 之后在 Google Pixel 11 Pro 上，纯文本权重大概吃 191MB active RAM，完整多模态版本大概 567MB。
- **context 拉到 8K，是上一代的 4 倍。** 折算下来一次能处理 5.5 分钟音频、29 张图或者 58 帧视频，混着交错输入也行，全都在本地硬件上跑。
- **主打每参数质量。** 在 MTEB Code、MAEB 这些 benchmark 上拿了 1B 以下多模态 embedder 里的第一，多语言文本能力和上一代持平，还把一些体量两倍多的专用模型给比下去了。详细数字在 model card 里。
