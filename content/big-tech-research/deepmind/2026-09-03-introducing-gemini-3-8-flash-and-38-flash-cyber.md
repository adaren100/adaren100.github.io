---
title: "Introducing Gemini 3.8 Flash and 3.8 Flash Cyber"
date: 2026-09-03
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Introducing Gemini 3.8 Flash and 3.8 Flash Cyber](https://deepmind.google/blog/introducing-gemini-3-8-flash-and-38-flash-cyber/)** — _Google DeepMind · Sep 3_

**Main takeaway:** Google's third Flash release in six weeks ships two variants off one core: Gemini 3.8 Flash, billed as its best reasoning and coding model yet at 3.7 Flash's speed and price ($0.75/M input, $3.75/M output) and scoring 54.9% on HLE-Verified, and Gemini 3.8 Flash Cyber, a cybersecurity-specialized version released only to trusted defenders through the new Fairwind Program.

**Main methods:**
- **One foundational core, two deployment targets.** Both variants are powered by the same underlying intelligence; Google credits much of the shared coding and reasoning gain to rigorous training in the demanding domain of cybersecurity, then packages it differently for general developers versus vetted defenders.
- **Long-running agentic loops in the training stack.** Both releases are described as "further accelerated by long-running agentic loops designed to recursively evaluate and refine the underlying models" — the model improvement process is itself agentic rather than a single post-training pass.
- **Benchmark claims skew agentic and professional.** On DeepSWE v1.1 (long-horizon software engineering), 3.8 Flash beats most larger frontier models at solving engineering problems end to end at a fraction of the cost; it also tops 3.7 Flash and other frontier models on Vals Finance Agent V2 and Harvey's Legal Agent Benchmark, plus 54.9% on HLE-Verified.
- **The gains come from "working harder," explicitly.** Google names the design choice: on complex tasks the model executes extra reasoning steps and calls tools iteratively, and may burn more tokens to maximize performance, especially at higher effort levels.
- **Cost is the honest caveat, with an escape hatch.** For compute-constrained applications Google tells developers to drop the effort level or stay on 3.7 Flash, which remains fully supported for efficiency-first workloads — an unusual admission that the new model isn't a drop-in win on price.
- **Demos lean on single-prompt agentic builds.** The post's showcases are all built in Google Antigravity from one prompt with a looping instruction: a 3D wizard-castle puzzle game with Nano Banana textures, and a playable DOS-style Google Maps with directions and Street View.

**[Gemini 3.8 Flash 和 3.8 Flash Cyber 一起来了](https://deepmind.google/blog/introducing-gemini-3-8-flash-and-38-flash-cyber/)** — _Google DeepMind · 9月3日_

**Main takeaway:** 六周内的第三个 Flash，同一个底座出两个版本：Gemini 3.8 Flash 是他们目前最强的 reasoning 和 coding 模型，速度和价格跟 3.7 Flash 持平（输入 $0.75/M，输出 $3.75/M），HLE-Verified 拿到 54.9%；Gemini 3.8 Flash Cyber 则是安全专精版，只通过新的 Fairwind Program 发给可信的防守方。

**Main methods:**
- **一个底座，两个投放口。** 两个版本共用同一份 foundational intelligence，Google 说这轮 coding 和 reasoning 的提升有很大一部分要归功于在 cybersecurity 这个高强度领域里的硬训练，然后再分别打包给普通开发者和经过审核的防守方。
- **训练环节里塞了 long-running agentic loop。** 官方描述是用长跑的 agentic loop 去递归地评估和打磨底层模型，也就是说模型迭代这件事本身已经是 agent 在做，不再是一轮 post-training 就收工。
- **benchmark 全押在 agentic 和专业场景上。** DeepSWE v1.1 这种长周期软件工程任务里，3.8 Flash 端到端解题的表现超过大多数体量更大的 frontier 模型，成本却低一截；Vals Finance Agent V2、Harvey's Legal Agent Benchmark 上也压过 3.7 Flash 和其他 frontier 模型，HLE-Verified 54.9%。
- **提升是"更卖力"换来的，这点写得很直白。** Google 自己点名了这个设计取舍：碰到复杂任务它会多走几步 reasoning、反复调工具，effort level 调高的时候还会多烧 token。
- **成本是真 caveat，好在留了后门。** 对算力敏感的场景，官方建议直接把 effort level 调低，或者继续用 3.7 Flash，那个版本仍然全面支持。承认新模型在价格上不是无脑升级，这话说得挺少见。
- **demo 全是一句 prompt 跑出来的。** 展示的东西都在 Google Antigravity 里用一条带循环指令的 prompt 生成：一个用 Nano Banana 贴图的 3D 巫师城堡解谜关卡，还有一个能查地点、看路线、逛 Street View 的 DOS 风格 Google Maps。
