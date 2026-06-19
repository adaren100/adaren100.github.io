---
title: "Introducing LifeSciBench"
date: 2026-06-18
draft: false
tags: ["OpenAI", "research", "big-tech-research"]
source_org: "OpenAI"
source_url: "https://openai.com/index/introducing-life-sci-bench"
---

**[Introducing LifeSciBench](https://openai.com/index/introducing-life-sci-bench)** — _OpenAI · Jun 17_

**Main takeaway:** OpenAI is releasing LifeSciBench, a 750-task expert-authored benchmark for evaluating whether AI systems can support real-world life science research — interpreting evidence, designing experiments, troubleshooting assays, and reasoning under uncertainty — rather than just answering biology trivia.

**Main methods:**
- **Taxonomy grounded in practitioner surveys.** Tasks span seven workflows (evidence handling, analysis, design and optimization, scientific reasoning, validation and operations, translation, scientific communication) across seven biological domains, derived from surveying practicing life scientists about the work they actually do.
- **Free-response with expert rubrics.** Each task is framed like a request to a knowledgeable collaborator — scientific prompt, context or artifacts, free-response answer — and graded by expert-written rubrics that check correctness, justification, caveats, and formatting.
- **Multi-step reasoning is the norm.** 79% of tasks require multiple reasoning or decision-making steps, averaging four steps per task; this is explicitly designed to go beyond clean fact-recall benchmarks.
- **Artifact-heavy.** Includes 1,062 attached artifacts spanning figures, PDFs, tables, sequence files, structure or chemical files, and web references; 53% of tasks require interpreting or synthesizing at least one artifact.
- **Author pool.** 173 expert scientists with Ph.D.-level training and biotech or pharmaceutical industry experience authored the tasks, with unbounded revision rounds before acceptance.
- **Caveat.** The fetched body cuts off before any model-vs-model leaderboard numbers, so this writeup doesn't capture how current frontier models actually score on LifeSciBench.

**[OpenAI 发布 LifeSciBench：一个真要干生命科学研究的 benchmark](https://openai.com/index/introducing-life-sci-bench)** — _OpenAI · 6月17日_

**Main takeaway:** OpenAI 推出了 LifeSciBench，一个 750 道题、由领域专家写、专家审的 benchmark，专门考 AI 能不能干真实的生命科学研究——解读证据、设计实验、调 assay、在不确定下做判断，而不是回答生物常识题。

**Main methods:**
- **任务分类直接来自从业者调研。** 七大 workflow（证据处理、分析、design and optimization、scientific reasoning、validation and operations、translation、scientific communication）配七个生物学方向，taxonomy 是先调研一线生命科学家平时都在干什么再归类出来的。
- **自由回答 + 专家 rubric 打分。** 每道题做成"研究员给一个懂行 collaborator 发任务"的样子：scientific prompt、相关 context 或 artifact、然后自由作答，由专家写的 rubric 来评判答案对不对、论证够不够、caveat 有没有、格式符不符合预期。
- **多步推理是常态。** 79% 的任务都需要多步推理或决策，平均一题要走 4 步，刻意拉开和那种 clean fact-recall benchmark 的距离。
- **大量 artifact。** 一共 1,062 个附件，涵盖图、PDF、表、序列文件、结构 / 化学文件、网页链接；53% 的题要求模型从至少一个 artifact 里提取或综合信息。
- **出题人阵容。** 173 位有 Ph.D. 训练、又有 biotech 或药企产业经验的专家出题，每道题可以无上限地反复修订直到收录。
- **需要注意的 caveat。** 抓到的正文在出 model-vs-model 排行榜之前就截断了，所以这里没法告诉你各家 frontier model 在 LifeSciBench 上实际得分多少。
