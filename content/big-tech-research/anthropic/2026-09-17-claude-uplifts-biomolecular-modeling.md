---
title: "How Claude is uplifting biomolecular modeling"
date: 2026-09-17
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[How Claude is uplifting biomolecular modeling](https://www.anthropic.com/research/claude-uplifts-biomolecular-modeling)** — _Anthropic · Sep 16_

**Main takeaway:** Working inside Claude Science, Claude optimized more than 30 open-source biomolecular models in just under four weeks, speeding them up roughly 4x on average and adding a low-memory mode that predicts systems larger than 10,000 tokens on a single NVIDIA GPU node. All the optimized code is being open-sourced, alongside a protein design competition with Adaptyv Bio backed by up to $1M in Claude credits.

**Main methods:**
- **Inference optimization, not retraining.** Claude rewrote inference paths for open-source models covering structure prediction, protein design, genomics, and protein language models — roughly 4x faster with minimal precision loss, and nearly 2x faster with bit-identical outputs.
- **Memory work unlocks bigger systems.** A new low-memory mode makes accurate prediction possible for biomolecular systems over 10,000 tokens (amino acids, nucleotides, and atoms from small molecules and ions) on one GPU node.
- **The cost problem it's solving.** The earlier de novo binder design result let Claude spend up to $10,000 per target on Modal, about 2,500 NVIDIA H100 GPU hours — out of reach for most protein designers.
- **Two orders of magnitude cheaper.** Combining these optimizations with simplifications to the earlier agentic protein design approach, Claude reached comparable in silico performance using ~100x fewer GPU hours.
- **Built on an earlier, smaller result.** Claude Mythos 5.1 had already accelerated seven open-source biology models by up to 2.5x; the 30+ model result came from an internal general-purpose research model.
- **Released to the community.** The optimized code is open-sourced with a technical report, and the Adaptyv Bio competition covers five frontier problems with up to $1M in Claude credits, $250K in Modal compute credits from Modal and Twist Bioscience, and wet lab validation for over 5,000 designs.

**[Claude 把 30 多个开源生物模型提速了 4 倍](https://www.anthropic.com/research/claude-uplifts-biomolecular-modeling)** — _Anthropic · 9月16日_

**Main takeaway:** Claude 在 Claude Science 里干了不到四周，把 30 多个科学家常用的开源生物分子模型优化了一遍，平均提速差不多 4 倍，还顺手做了个低显存模式，单个 NVIDIA GPU 节点就能准确预测超过 10,000 token 的生物分子体系。优化后的代码全部开源，同时和 Adaptyv Bio 一起办了个蛋白设计比赛，奖池是最高 100 万美元的 Claude credits。

**Main methods:**
- **动的是 inference，不是重新训练。** Claude 重写了这些开源模型的推理路径，涵盖结构预测、蛋白设计、基因组学和蛋白语言模型，精度基本不掉的情况下快了约 4 倍，要求输出完全一致的话也还有接近 2 倍。
- **显存这块的优化打开了更大的体系。** 新的 low-memory 模式让超过 10,000 token 的体系（氨基酸、核苷酸，以及小分子和离子里的原子）能在单个 GPU 节点上跑准。
- **它要解决的其实是成本。** 之前那个 de novo binder 设计的结果，Anthropic 允许 Claude 在 Modal 上每个靶点烧掉 1 万美元，大概相当于 2,500 个 NVIDIA H100 GPU 小时，绝大多数做蛋白设计的人根本用不起。
- **GPU 小时直接少了两个数量级。** 把这轮优化和之前那套 agentic 蛋白设计流程的简化合起来，Claude 用不到百分之一的 GPU 小时就做到了和之前差不多的 in silico 表现。
- **是在一个更小的结果上往前推的。** Claude Mythos 5.1 之前已经把七个开源生物模型加速到最高 2.5 倍，这次 30 多个模型的结果来自一个内部的通用研究模型。
- **东西都放出来了。** 优化代码今天全部开源，配了技术报告。和 Adaptyv Bio 合办的比赛选了五个当前能力边缘上的难题，Modal 和 Twist Bioscience 也掏了钱，一共最高 100 万美元 Claude credits、25 万美元 Modal 算力，外加给 5,000 多个设计做 wet lab 验证。
