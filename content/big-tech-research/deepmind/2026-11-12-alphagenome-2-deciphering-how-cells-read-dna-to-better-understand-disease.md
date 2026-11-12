---
title: "AlphaGenome 2: Deciphering how cells read DNA to better understand disease"
date: 2026-11-12
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[AlphaGenome 2: Deciphering how cells read DNA to better understand disease](https://deepmind.google/blog/alphagenome-2-deciphering-how-cells-read-dna-to-better-understand-disease/)** — _Google DeepMind · Nov 12_

**Main takeaway:** A model release: AlphaGenome 2 predicts how DNA sequences and their variants affect hundreds of specific human cell types and states rather than broad tissue averages, and it identifies nearly twice as many expression-changing variants as DeepMind's previous state-of-the-art model. It was trained on more than 100 million individual cell profiles across 68 tissues and is available today for non-commercial research through the AlphaGenome API, with commercial research in private preview.

**Main methods:**
- **From parallel outputs to a conditional model.** AlphaGenome 1 took a 1-million-letter DNA sequence and predicted thousands of experiments across many tissues all at once, which spread model capacity thin; AlphaGenome 2 predicts one condition — a tissue, cell type, or cell state — at a time, feeding that condition in alongside the sequence at every stage of the architecture.
- **A cell encoder for unseen conditions.** The target condition can come from a reference catalog of cell types or be generated on the fly from a scientist's own single-cell experiment, which is what lets the model make predictions for cell and disease states it never saw in training.
- **Single-cell atlases as training signal.** Training on 100M+ individual cell profiles across 68 tissues turns static cell atlases — the kind the Human Cell Atlas is building — into a predictive engine for human genetics.
- **Why cell-type resolution matters.** Every cell carries the same DNA but switches different genes on and off; variant effects in disease-relevant cells get averaged away in broad-tissue models, which is exactly the signal AlphaGenome 2 is after.
- **Builds on the AlphaGenome Atlas.** The earlier release precomputed effects for all 9 billion possible single-letter changes in the human genome, already used to prioritize and interpret variants in rare disease and complex-trait work.

**[AlphaGenome 2：细胞到底怎么读 DNA](https://deepmind.google/blog/alphagenome-2-deciphering-how-cells-read-dna-to-better-understand-disease/)** — _Google DeepMind · 11月12日_

**Main takeaway:** 一次模型发布。AlphaGenome 2 不再只给组织层面的平均值，而是能预测 DNA 序列和它的变异在几百种具体人类细胞类型和细胞状态里的影响，能找出来的"会改变基因表达的变异"比他们上一代 SOTA 多了将近一倍。模型用 68 种组织、超过 1 亿条单细胞数据训出来，今天起非商业研究可以通过 AlphaGenome API 直接用，商业研究还在私有预览。

**Main methods:**
- **从并行输出改成条件模型。** AlphaGenome 1 是喂进 100 万字母的 DNA 序列，一次性把几千个实验、好多组织的结果全预测出来，结果模型容量被摊得太薄；AlphaGenome 2 改成一次只预测一个 condition，也就是一种组织、细胞类型或者细胞状态，并且把这个 condition 和序列一起，在架构的每一层都喂进去。
- **用 cell encoder 覆盖没见过的情况。** 目标 condition 既可以从现成的细胞类型目录里挑，也可以拿研究者自己做的单细胞实验当场生成，所以哪怕是训练里压根没出现过的细胞状态和疾病状态，它也能给出预测。
- **把单细胞图谱变成训练信号。** 68 种组织、1 亿多条单细胞 profile 喂进去之后，像 Human Cell Atlas 那种原本静态的细胞图谱，就变成了能用来做人类遗传学预测的引擎。
- **为什么非要做到细胞类型这一级。** 每个细胞带的 DNA 都一样，但开关的基因不同；真正跟疾病相关的那些细胞里的变异效应，在组织级模型里会被平均掉，而这恰恰是 AlphaGenome 2 要抓的信号。
- **接着 AlphaGenome Atlas 往下做。** 之前那个平台已经把人类基因组里全部 90 亿种单字母改动的效应算了一遍，研究者拿它来筛和解释变异，在罕见病和复杂性状上已经出了一些发现。
