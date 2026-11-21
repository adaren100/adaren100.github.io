---
title: "Can AI help scientists identify promising drug candidates?"
date: 2026-11-20
draft: false
tags: ["big-tech-research", "openai"]
---

**[Can AI help scientists identify promising drug candidates?](https://openai.com/index/introducing-medchembench)** — _OpenAI · Nov 20_

**Main takeaway:** OpenAI is releasing MedChemBench, a 99-problem benchmark on medicinal-chemistry reasoning: reading molecular structures, interpreting experimental results, and picking which compound to test next. At the xhigh reasoning setting GPT‑6.2 Astra earned 84.5% of available credit, against 83.3% for GPT‑6 Astra, 82.0% for GPT‑6.1 Sol, and 58.2% for GPT‑5.6 Sol.

**Main methods:**
- **The hard part it targets.** Improving one property of a molecule usually degrades another — a compound can bind a disease-related protein strongly but absorb poorly or break down too fast — so the benchmark is about reasoning through tradeoffs, not single-property prediction.
- **Sourced from real research programs.** 99 problems drawn from 117 papers and patents, covering 761 distinct molecular structures. Models get the context available at a chosen point in a program: the target, the researchers' goals, compounds studied so far, and selected experimental findings.
- **Four graded components.** Molecular structures (correct atom connections and specified stereochemistry), scientific reasoning (explanations supported by the supplied evidence), ranking and selection (choices meeting stated requirements), and property predictions (agreement with reported numerical values and categories).
- **Worked example on PRMT5.** Given structures and earlier results for cancer-relevant PRMT5 inhibitors, the model must predict cellular potency, cell-barrier permeability, and liver-enzyme breakdown rate for three related compounds — where withheld later experiments showed compound 23 more potent in cells while compound 24 permeated better and was more metabolically stable.
- **Where models are uneven.** GPT‑6 Astra was strongest at reconstructing molecular structures and explaining experimental evidence; selecting compounds and predicting numerical properties were harder for it.
- **Spatial reasoning gets its own section.** The benchmark separately probes spatial reasoning in medicinal chemistry, including assembling molecules from provided drawings and chemical groups.

**[MedChemBench：AI 能帮化学家挑出有戏的候选药吗](https://openai.com/index/introducing-medchembench)** — _OpenAI · 11月20日_

**Main takeaway:** OpenAI 放出了 MedChemBench，一个 99 道题的 benchmark，考的是药物化学里那套推理：看懂分子结构、读实验结果、决定下一步该做哪个化合物。在 xhigh reasoning 档位下，GPT‑6.2 Astra 拿到 84.5% 的可得分，GPT‑6 Astra 83.3%，GPT‑6.1 Sol 82.0%，GPT‑5.6 Sol 只有 58.2%。

**Main methods:**
- **它想考的难点在哪。** 分子这边改好一个性质，往那边常常就坏一个：可能对靶点蛋白结合得很强，但吸收差，或者在体内降解太快。所以这个 benchmark 考的是怎么在 tradeoff 里做判断，不是单测某个性质预测得准不准。
- **题目都是从真实研究里扒出来的。** 99 道题来自 117 篇论文和专利，涉及 761 个不同的分子结构。给模型的信息就是研究进行到某个时间点时手上有的东西：靶点、研究目标、已经做过的化合物、挑出来的几组实验结果。
- **分四块打分。** 分子结构（原子连接对不对、立体化学标没标对）、scientific reasoning（解释有没有被给的证据支撑）、排序和选择（选出来的化合物符不符合题目给的要求）、性质预测（跟原文报的数值和类别对不对得上）。
- **PRMT5 那道题可以看一下。** 给的是癌症药物研发里 PRMT5 抑制剂的结构和前期实验，让模型预测三个相关化合物在细胞里的抑制浓度、过细胞膜的难易、以及在肝酶 assay 里降解多快。后面那批没给模型看的实验结果显示确实有 tradeoff：化合物 23 在细胞里更低浓度就能起效，化合物 24 则更容易过膜、在肝酶 assay 里也更稳。
- **模型强弱很不均匀。** GPT‑6 Astra 最拿手的是把分子结构重建出来、把实验证据讲清楚；真要它挑化合物、报具体数值，就明显吃力。
- **空间推理单独拎出来测。** 其中一块专门考药物化学里的空间推理，包括照着给的结构式和基团把分子拼出来。
