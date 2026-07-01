---
title: "Introducing GeneBench-Pro"
date: 2026-06-30
draft: false
tags: ["big-tech-research", "openai"]
---

**[Introducing GeneBench-Pro](https://openai.com/index/introducing-genebench-pro)** — _OpenAI · Jun 30_

**Main takeaway:** OpenAI introduced GeneBench-Pro, a 129-question research-level benchmark testing AI agents' ability to make scientific judgment calls in computational biology — not just execute predefined workflows, but choose the right analysis path, revise assumptions mid-analysis, and decide when a result is ready to act on.

**Main methods:**
- **"Research taste" as the target capability.** GeneBench-Pro operationalizes higher-order scientific judgment: deciding which questions a dataset can actually support, updating the analysis plan when early diagnostics change the estimand, and knowing when a result is decision-ready.
- **129 problems across 10 domains.** Covers statistical genetics (17), population genetics (21), quantitative genetics (17), regulatory omics (17), functional genomics (9), clinical/PGx/diagnostics (26), cancer genomics (10), microbial genomics (3), and forensic genetics (2) — all using realistic, messy datasets.
- **Iterative task format.** Each problem provides a dataset, brief experimental context, and a target estimand tied to a downstream decision; the model must explore the data, choose an analysis approach, iterate, and deliver a final answer — mirroring real research workflows rather than step-by-step scripts.
- **Designed to avoid contamination.** GeneBench-Pro avoids constructing multi-step problems from existing papers (where training data could contain the answer); synthetic datasets are used where necessary.
- **The bottleneck GeneBench-Pro targets.** Gene sequencing costs have fallen far enough that downstream analysis, not sample collection, is now the limiting factor in biology; the benchmark measures AI's capacity to close that gap.

**[OpenAI 推出 GeneBench-Pro](https://openai.com/index/introducing-genebench-pro)** — _OpenAI · 6月30日_

**Main takeaway:** OpenAI 推出了 GeneBench-Pro，一个 129 题的研究级 benchmark，专门测 AI agent 在计算生物学里做判断的能力——不只是跑固定流程，而是要看出数据能回答什么问题、中途能不能更新分析方案、什么时候结果可以用了。

**Main methods:**
- **"Research taste" 是核心考点。** GeneBench-Pro 想量化的是高阶判断力：数据实际能支持哪些问题、早期诊断信号出来后怎么调整分析目标、最终结果什么时候算"够了可以用"。
- **129 题覆盖 10 个领域。** 包括统计遗传学（17 题）、群体遗传学（21）、数量遗传学（17）、调控组学（17）、功能基因组学（9）、临床/PGx/诊断（26）、癌症基因组学（10）、微生物基因组学（3）、法医遗传学（2），数据都是真实且"脏"的。
- **任务格式强调迭代。** 每题给一个数据集加目标估计量，模型得自己探索数据、选分析路径、反复实验，最后给出答案，模拟真实科研节奏，不是照着步骤走。
- **刻意规避 benchmark 污染。** 专门设计来避免"从已有论文拆步骤"的构题方式——那样训练集里可能已经有答案；必要时使用合成数据集。
- **指向真正的瓶颈。** 基因测序成本已经足够低，数据分析才是科研的限速步骤；GeneBench-Pro 衡量的就是 AI 能不能解开这个瓶颈。
