---
title: "Introducing Gemini 3.7 Flash"
date: 2026-08-14
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Introducing Gemini 3.7 Flash](https://deepmind.google/blog/introducing-gemini-3-7-flash/)** — _Google DeepMind · Aug 14_

**Main takeaway:** Gemini 3.7 Flash lands just three weeks after 3.6 Flash as DeepMind's "most intelligent workhorse model yet for coding and agents," with FrontierCode 1.1 Main climbing to 43.6% from 34.4% and DeepSWE v1.1 to 65.3% from 49.0%. It ships at an introductory $0.75/1M input and $3.75/1M output tokens — half the original 3.6 Flash price.

**Main methods:**
- **Coding is the headline.** Gains over 3.6 Flash on debugging and issue resolution, higher first-pass code accuracy, and better production-ready code: FrontierCode 1.1 Main 43.6% vs 34.4%, DeepSWE v1.1 65.3% vs 49.0%.
- **Web dev and UI generation.** Elo 1588 vs 1538 on Arena.ai's WebDev Arena, more functional layouts and feature-complete apps in fewer prompts, and high design adherence when handed a reference — a screenshot, an image, or a full design system.
- **Knowledge-dense domains.** For finance, law, and biosciences, it hits 34.0% vs 22.0% on the GDP.pdf benchmark (complex document processing) and 30.4% vs 17.0% on AutomationBench (real-world business workflows).
- **Agentic discipline, not just scores.** DeepMind claims it adapts better to roadblocks, clarifies intent when needed, follows instructions more faithfully, and puts more effort into multi-step planning and tool calls — meaning less manual oversight and fewer retries.
- **Demos are multi-model orchestration.** A playable 3D game with Nano Banana generating characters, items, and textures in real time; one-shot interactive landing pages where 3.7 Flash orchestrates sub-agents and Gemini Omni builds the parallax; a robotics model trained in a 3-agent graph loop; and a static PDF turned into an interactive data story with live charts.
- **Caveats.** The $0.75/$3.75 pricing is introductory and only runs through the end of the year, and the post credits "developer feedback and algorithmic innovations" without disclosing any architecture or training detail.

**[Gemini 3.7 Flash 发布：coding 主力升级，价格砍一半](https://deepmind.google/blog/introducing-gemini-3-7-flash/)** — _Google DeepMind · 8月14日_

**Main takeaway:** 距离 3.6 Flash 才三周，Gemini 3.7 Flash 就上了，DeepMind 把它定位成"目前最聪明的 coding 和 agent 主力机"。FrontierCode 1.1 Main 从 34.4% 提到 43.6%，DeepSWE v1.1 从 49.0% 提到 65.3%，而 introductory 价格是每百万 token 输入 $0.75、输出 $3.75，正好是当初 3.6 Flash 的一半。

**Main methods:**
- **主打还是写代码。** debug 和 issue resolution 这类活比 3.6 Flash 明显强，第一次就写对的比例更高，产出的代码也更接近能直接上线的状态：FrontierCode 1.1 Main 43.6% 对 34.4%，DeepSWE v1.1 65.3% 对 49.0%。
- **前端和 UI 生成。** 在 Arena.ai 的 WebDev Arena 上 Elo 1588 对 1538，用更少的 prompt 就能做出布局能用、功能齐全的应用。给它一张截图、一张图或者一整套 design system 当参考，还原度都不错。
- **知识密集的领域也补了。** 金融、法律、生命科学这些方向，GDP.pdf 这个专门测复杂文档处理的 benchmark 上 34.0% 对 22.0%，AutomationBench（真实业务流程）30.4% 对 17.0%。
- **比分数更值得看的是 agent 表现。** DeepMind 说它碰到卡点会自己调整路线，该问的时候会先问清楚意图，instruction following 更稳，多步规划和 tool call 上也更肯下功夫，实际用起来就是少盯着它、少重试几轮。
- **demo 全是多模型串起来玩的。** 一句话生成能玩的 3D 游戏，角色、道具、贴图由 Nano Banana 实时生成；一次成型的交互式落地页，3.7 Flash 负责调度 sub-agent，Gemini Omni 做 parallax 组件；机器人模型放在一个三 agent 的 graph loop 里训练；还有把静态 PDF 年报直接变成带实时图表的交互式数据故事。
- **有两点要说。** $0.75/$3.75 是 introductory 价，只到年底；另外这篇只提了"developer feedback 加算法改进"，架构和训练细节一个字没给。
