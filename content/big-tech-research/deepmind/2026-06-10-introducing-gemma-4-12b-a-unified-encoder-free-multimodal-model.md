---
title: "Introducing Gemma 4 12B: a unified, encoder-free multimodal model"
date: 2026-06-10
draft: false
tags: ["Google DeepMind", "research", "big-tech-research"]
source_org: "Google DeepMind"
source_url: "https://deepmind.google/blog/introducing-gemma-4-12b-a-unified-encoder-free-multimodal-model/"
---

**[Introducing Gemma 4 12B: a unified, encoder-free multimodal model](https://deepmind.google/blog/introducing-gemma-4-12b-a-unified-encoder-free-multimodal-model/)** — _Google DeepMind · Jun 9_

**Main takeaway:** Gemma 4 12B is a mid-sized, encoder-free multimodal model that runs locally on a laptop with 16GB of RAM, reaches benchmark performance near the 26B MoE, and is the first mid-sized Gemma to take native audio input.

**Main methods:**
- **Encoder-free architecture.** No separate vision or audio encoder — visual inputs go through a single matmul + positional embedding + normalization into the LLM backbone; raw audio is projected directly into the text-token dimensional space.
- **Sized for laptops.** 12B parameters, runs locally in 16GB VRAM/unified memory; designed to bridge the gap between edge-friendly E4B and the larger 26B MoE.
- **Performance.** Approaches the 26B MoE on standard benchmarks at less than half the memory footprint, while supporting multi-step reasoning and agentic workflows.
- **Native audio inputs.** First mid-sized Gemma with raw audio, not just a text+vision stack.
- **MTP drafters built in.** Ships with Multi-Token Prediction drafters to reduce inference latency.
- **Open and reachable.** Apache 2.0; weights on Hugging Face and Kaggle; works in LM Studio, Ollama, Google AI Edge Gallery, Eloquent, and the LiteRT-LM CLI.

**[Gemma 4 12B：统一架构、不要 encoder 的多模态模型](https://deepmind.google/blog/introducing-gemma-4-12b-a-unified-encoder-free-multimodal-model/)** — _Google DeepMind · 6月9日_

**Main takeaway:** Gemma 4 12B 是一个中等大小、去掉 encoder 的多模态模型，16GB 内存的笔记本就能本地跑，benchmark 直逼 26B MoE，还是 Gemma 系列里第一个吃 raw audio 的中型模型。

**Main methods:**
- **不要 encoder 的架构。** 没有单独的 vision 或 audio encoder——图像输入只过一次 matmul 加位置编码加 normalization 就进 LLM 主干；音频直接投到文本 token 的维度空间。
- **奔笔记本来的。** 12B 参数，16GB 显存/统一内存就跑得动；定位是衔接 edge 端的 E4B 和上层的 26B MoE。
- **性能。** 在标准 benchmark 上接近 26B MoE，但内存占用不到一半，同时支持多步推理和 agentic workflow。
- **原生音频输入。** Gemma 中型模型里第一个直接吃 raw audio 的，不再是 text+vision 那套。
- **自带 MTP drafter。** 内置 Multi-Token Prediction drafter 降低推理延迟。
- **完全开放。** Apache 2.0；权重在 Hugging Face 和 Kaggle；LM Studio、Ollama、Google AI Edge Gallery、Eloquent、LiteRT-LM CLI 都能直接跑。
