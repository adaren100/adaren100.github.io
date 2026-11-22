---
title: "Perplexity and Intelligence"
date: 2026-11-22
draft: false
tags: ["big-tech-research", "openai"]
---

**[Perplexity and Intelligence](https://openai.com/index/perplexity-and-intelligence)** — _OpenAI · Nov 22_

**Main takeaway:** Chief Scientist Jakub Pachocki argues that perplexity (equivalently, cross-entropy loss) on a held-out dataset should become the shared cross-lab metric for tracking pretraining progress and informing safety standards, and publishes OpenAI's own internal perplexity curve from GPT‑3.5 onward as a first step. The log-perplexity milestones he cites on OpenAI's current main eval dataset: ~0.99 for GPT‑3.5, ~0.91 for GPT‑4, and now below 0.8.

**Main methods:**
- **The compressor framing.** Modern AI isn't assembled from capability-specific techniques; the capabilities come from training a compressor (equivalently, a next-token predictor) on a very large unstructured corpus, and everything else — prompting, finetuning, RL — is targeted elicitation of what's already latent in that model.
- **Separating creation from elicitation.** Pachocki splits development into building the "alien mind" with hard-to-predict emergent capabilities, then eliciting specific behaviors from it. Algorithmic progress blurs the training-phase boundaries but the conceptual split still holds.
- **Perplexity as the one metric that tracked it all.** OpenAI has measured progress on this "intelligence substrate" the same way for years — held-out perplexity — and the post maps capability jumps onto it: GPT‑2 set a perplexity SOTA on older datasets and was the first model to consistently write coherent paragraphs, GPT‑3 brought in-context learning, GPT‑3.5 (~0.99) fluent conversation and the original ChatGPT, GPT‑4 (~0.91) productive chain-of-thought.
- **Below 0.8 is where cyber and math showed up.** Now that losses have dropped under 0.8, transformative capabilities have emerged in cybersecurity and mathematics.
- **Thresholds weren't predictable in advance.** Pachocki is explicit that there was no a priori reason to expect those capabilities at those particular perplexity values; they are best read as emergent latent capabilities riding on one metric.
- **Why publish internal numbers at all.** Releasing the measurements gives competitors a clearer read on where OpenAI stands, but he judges that cost outweighed by the urgency of getting shared safety measures and a common scientific basis for pacing efforts across the industry.

**[为什么 OpenAI 想把 perplexity 立成行业通用标尺](https://openai.com/index/perplexity-and-intelligence)** — _OpenAI · 11月22日_

**Main takeaway:** 首席科学家 Jakub Pachocki 的观点是，held-out 数据集上的 perplexity（也就是 cross-entropy loss）应该成为各家实验室通用的那把尺子，用来跟踪 pretraining 的进展、也用来支撑共同的安全标准。作为第一步，他们直接把 OpenAI 从 GPT‑3.5 以来的内部 perplexity 曲线公开了：在他们现在的主评测集上，GPT‑3.5 的 log-perplexity 大约 0.99，GPT‑4 大约 0.91，现在已经跌到 0.8 以下。

**Main methods:**
- **先把"模型就是压缩器"这个框架摆出来。** 现在的 AI 不是靠一堆针对具体能力的技术拼出来的，能力其实都来自一件事：在超大规模无结构语料上训一个 compressor（等价于 next-token predictor）。prompting、finetuning、RL 这些后续手段，本质上只是把模型里已经有的东西引出来。
- **"造出来"和"引出来"要分开看。** Pachocki 把开发过程拆成两段：先造出那个带着难以预测的 emergent 能力的"alien mind"，再去做针对性的 elicitation。算法进步会让训练阶段的边界变模糊，但这个概念上的切分还是成立的。
- **一个指标居然串起了全部进展。** OpenAI 这些年衡量这层"intelligence substrate"的方式一直没变，就是看 held-out perplexity。文章顺手把能力跃迁一一挂到了这条曲线上：GPT‑2 在老数据集上刷了 perplexity SOTA，也是第一个能稳定写出连贯段落的模型；GPT‑3 带来了 in-context learning；GPT‑3.5（约 0.99）能流畅对话，撑起了最早那版 ChatGPT；GPT‑4（约 0.91）则能把 chain-of-thought 真正用起来。
- **跌破 0.8 之后，cyber 和数学才冒出来。** loss 压到 0.8 以下之后，他们看到网络安全和数学这两块出现了量级上的变化。
- **但这些门槛事前根本预测不了。** 他写得很清楚：没有任何先验理由说这些能力会刚好在那几个 perplexity 数值上出现，更应该理解成单一指标推进过程中自然浮出来的 emergent latent capability。
- **为什么愿意把内部数字摊开。** 公开这些测量等于让竞争对手更清楚 OpenAI 的位置，但他觉得这个代价比不上另一件事的紧迫性：整个行业需要共同的安全措施，也需要一个能谈 pacing 的共同科学基础。
