---
title: "DiffusionGemma: 4x faster text generation"
date: 2026-06-11
draft: false
tags: ["Google DeepMind", "research", "big-tech-research"]
source_org: "Google DeepMind"
source_url: "https://deepmind.google/blog/diffusiongemma-4x-faster-text-generation/"
---

**[DiffusionGemma: 4x faster text generation](https://deepmind.google/blog/diffusiongemma-4x-faster-text-generation/)** — _Google DeepMind · Jun 10_

**Main takeaway:** DiffusionGemma is an Apache 2.0 open experimental 26B MoE that uses text diffusion instead of autoregressive decoding, delivering up to 4× faster generation on dedicated GPUs (1000+ tok/s on H100, 700+ on RTX 5090) — at the cost of lower overall quality than standard Gemma 4.

**Main methods:**
- **Diffusion head on a Gemma 4 backbone.** Generates 256 tokens per forward pass in parallel rather than one-at-a-time, shifting the decode bottleneck from memory bandwidth to compute.
- **Hardware footprint.** 26B total MoE but only 3.8B activated per inference; fits inside 18GB VRAM when quantized — usable on a high-end consumer GPU.
- **Bi-directional attention.** Every token attends to every other token in the block, which helps non-linear tasks (in-line editing, code infilling, amino-acid sequences, math graphs) — Unsloth fine-tuned it to play Sudoku, a task autoregressive models struggle with because tokens depend on future tokens.
- **Iterative self-correction.** The model refines the whole 256-token block across diffusion steps, fixing earlier mistakes mid-generation.
- **Where to use it (and not).** For maximum quality on production tasks, DeepMind still recommends standard autoregressive Gemma 4; DiffusionGemma is positioned for speed-critical local/interactive workflows.

**[DiffusionGemma：文本生成快 4 倍](https://deepmind.google/blog/diffusiongemma-4x-faster-text-generation/)** — _Google DeepMind · 6月10日_

**Main takeaway:** DiffusionGemma 是一个 Apache 2.0 的实验性开源模型，26B MoE，用 text diffusion 替代 autoregressive 解码，在专用 GPU 上推理快到 4 倍（H100 上 1000+ tok/s，RTX 5090 上 700+），代价是整体输出质量比标准 Gemma 4 低。

**Main methods:**
- **Gemma 4 主干上接 diffusion head。** 一次 forward 并行生成 256 个 token，不再一个一个吐，把解码瓶颈从 memory bandwidth 挪到 compute。
- **硬件门槛。** 总参数 26B 的 MoE，实际推理只激活 3.8B；量化后能塞进 18GB 显存，高端消费级 GPU 跑得动。
- **双向 attention。** block 里每个 token 都能 attend 到其他所有 token，对 in-line editing、code infilling、氨基酸序列、数学图这类非线性任务特别有利——Unsloth 已经 fine-tune 它来解数独，autoregressive 模型在这种 token 依赖未来的任务上一直吃亏。
- **迭代自我修正。** 模型在 diffusion 步里反复 refine 整个 256-token block，可以在生成途中改掉之前的错。
- **什么时候用，什么时候别用。** 追求质量的生产场景，DeepMind 还是推荐标准 autoregressive 的 Gemma 4；DiffusionGemma 定位是速度优先的本地/交互式 workflow。
