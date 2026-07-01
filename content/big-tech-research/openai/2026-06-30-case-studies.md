---
title: "Inside Genebench-Pro"
date: 2026-06-30
draft: false
tags: ["big-tech-research", "openai"]
---

**[Inside Genebench-Pro](https://openai.com/index/genebench-pro/case-studies)** — _OpenAI · Jun 30_

**Main takeaway:** This companion page to the GeneBench-Pro announcement presents 10 representative benchmark problems with their full prompts, datasets, and supporting materials; the featured somatic oncology problem requires recovering a structural-variant-defined tumor subgroup from multi-modal evidence before estimating treatment benefit-risk.

**Main methods:**
- **Ten sample problems across domains.** Case studies span somatic oncology, functional genomics (CRISPR target validation), statistical genetics (protein drug target prioritization), clinical genomics (carrier screening), single-cell genomics (eQTL), structural genetics, regulatory genomics, and population genetics.
- **Somatic oncology showcase.** The highlighted problem asks models to estimate the marginal benefit-risk of a TXR1-directed inhibitor in SV-activated tumors, requiring integration of long-read sequencing, expression, tumor-quality, and pharmacogenomic data before computing net clinical utility = benefit − 0.35 × toxicity, then making a treatment decision.
- **Synthetic benchmark labels used.** TXR1, TXR1i, DLR1, and star-allele labels are all synthetic, preventing models from directly looking up real drug data as a shortcut.

**[深入 GeneBench-Pro 案例](https://openai.com/index/genebench-pro/case-studies)** — _OpenAI · 6月30日_

**Main takeaway:** GeneBench-Pro 正式发布的配套案例展示页，给出 10 道代表题，附完整 prompt 和数据集；重点展示的肿瘤学题目要求模型先从多模态证据中挖出结构变异定义的靶向亚群，再估算 TXR1 抑制剂的获益-风险并做出治疗决策。

**Main methods:**
- **10 道样题覆盖多个子领域。** 涉及肿瘤学、功能基因组（CRISPR 靶点验证）、统计遗传学（蛋白药物靶点优先级）、临床基因组（携带者筛查）、单细胞基因组（eQTL）、结构遗传学、调控基因组学和群体遗传学。
- **肿瘤学例题。** 要求模型估算 SV 激活 TXR1 肿瘤亚群里 TXR1 抑制剂的边际获益-风险差，需要整合长读长测序、表达量、肿瘤质量和药物基因组学数据，计算净临床效用（获益差 − 0.35 × 毒性风险），最终给出是否推荐 TXR1i 的决策。
- **全用合成标签。** TXR1、TXR1i、DLR1 等都是合成 benchmark 标签，防止模型直接查真实药物数据走捷径。
