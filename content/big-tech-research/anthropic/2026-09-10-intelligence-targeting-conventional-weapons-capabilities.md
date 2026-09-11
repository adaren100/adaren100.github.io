---
title: "Measuring tactical intelligence targeting and conventional weapons capabilities of AI models"
date: 2026-09-10
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[Measuring tactical intelligence targeting and conventional weapons capabilities of AI models](https://www.anthropic.com/research/intelligence-targeting-conventional-weapons-capabilities)** — _Anthropic · Sep 10_

**Main takeaway:** Anthropic's Frontier Red Team built new evals for tactical intelligence targeting and conventional weapons development, and found that on some military and intelligence tasks, models can now do things that historically only a scarce set of highly-trained human experts could. Open-weights models from PRC developers trail the frontier but still showed concerning ability to identify and target adversaries and improve weapon performance.

**Main methods:**
- **Evals built around the kill chain.** Cyber and bio are the best-studied misuse domains, but most modern conflict is conventional, so the evals target steps of the "find, fix, track, target, engage, assess" kill chain — e.g. locating people from fragmentary information, or engineering drones to strike a moving target.
- **Expert-level on some tasks, steady gains overall.** For some military and intelligence tasks, models matched what only scarce, highly-trained experts could previously do, and models are making consistent progress across the simulated intelligence and weapons-development tasks.
- **Paired with real-world misuse evidence.** A companion report from Anthropic's Threat Intelligence Team documents instances of AI misuse in surveillance and conventional weapons development, showing threat actors already perceive a benefit.
- **Open-weights models aren't far behind.** The PRC-developed open-weights models tested typically landed between Sonnet and Mythos-class models in performance. Anthropic's conclusion: models well short of the frontier will still have intelligence and military applications.
- **New on-platform classifiers.** Anthropic says the results show why on-platform safety measures are necessary, and it has implemented new classifiers to block this kind of misuse.
- **No plateau in sight.** Anthropic expects AI could contribute to more novel, geostrategically consequential breakthroughs in these domains, which may change how models are trained, safeguarded, and released. The extracted body cuts off before the detailed per-eval results.

**[AI 能帮人找目标、改武器了吗？Anthropic Frontier Red Team 的新 eval](https://www.anthropic.com/research/intelligence-targeting-conventional-weapons-capabilities)** — _Anthropic · 9月10日_

**Main takeaway:** Anthropic 的 Frontier Red Team 专门做了一批新 eval，测 AI 在战术情报定位和常规武器研发上的能力，结论是在一部分军事和情报任务上，模型已经能干以前只有少数训练有素的专家才干得了的活。他们测的中国开发者的 open-weights 模型虽然落后前沿，但在识别、锁定对手和提升武器性能上也已经到了让人担心的水平。

**Main methods:**
- **沿着 kill chain 设计 eval。** cyber 和 bio 是研究得最多的 AI 滥用风险，但现代冲突大部分发生在常规领域，所以这批 eval 对准"find, fix, track, target, engage, assess"这条 kill chain，比如凭零碎信息找出一个人在哪，或者设计能打移动目标的无人机。
- **部分任务已到专家水平，整体稳步往上走。** 有些军事和情报任务过去只有稀缺的高水平专家做得了，现在模型也能做；在模拟的情报和武器研发任务上，模型能力一直在稳定提升。
- **和真实滥用案例对得上。** Anthropic 的 Threat Intelligence Team 同时出了一份报告，记录了有人拿 AI 做监控和常规武器研发的实际案例，说明 threat actor 已经尝到甜头了。
- **open-weights 模型也没差太远。** 测过的中国开发者 open-weights 模型，表现一般落在 Sonnet 和 Mythos 级别模型之间。Anthropic 的判断是，离前沿还差一截的模型照样会有情报和军事用途。
- **平台上加了新 classifier。** Anthropic 说这些结果正好说明平台侧的 safety 措施有必要，已经上线了新的 classifier 专门拦这类滥用。
- **不觉得能力会到平台期。** 他们预计 AI 还可能在情报和军事领域带来更新颖、地缘战略影响更大的突破，这会影响模型该怎么训练、怎么加 safeguard、怎么发布。抓到的正文到这儿就断了，每个 eval 的具体结果没拿到。
