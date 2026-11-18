---
title: "Introducing Gemini 4 Neon"
date: 2026-11-19
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Introducing Gemini 4 Neon](https://deepmind.google/blog/introducing-gemini-4-neon/)** — _Google DeepMind · Nov 19_

**Main takeaway:** A model release: Gemini 4 Neon is pitched as frontier-level intelligence with fast end-to-end task completion across software engineering, knowledge work, and science, scoring 61 on the Artificial Analysis Intelligence Index at its xhigh thinking level — #3 overall, behind only larger and slower models. It ships today at $3 / $15 per million input / output tokens with a 1M-token context window.

**Main methods:**
- **Positioned on the speed-vs-frontier Pareto frontier.** Neon ranks #2 on the Vals Index and lands on that index's Pareto frontier, i.e. DeepMind is selling it as the best intelligence you can get at its latency and price rather than the outright top score.
- **Steerability treated as a first-class metric.** Neon is #2 on steerability on the new Agent Arena Index — specifically adapting cleanly to mid-task user corrections — and DeepMind pairs that with its lowest fabrication rate yet in internal Google Antigravity testing.
- **Multimodal enterprise synthesis in one context.** Spreadsheets, PDFs, charts, audio, and video go into a single 1M-token window and come back out as structured deliverables; it scores 70.9% on the Vals Index and takes #1 on both Legal Research Bench and Tax Agent Bench.
- **Long-horizon agent benchmarks.** #1 overall on Zapier's AutomationBench (56.3%) and on Andon Labs' Vending-Bench 2 ($16,843, a long-horizon simulation of running a business), plus a #2 global debut at 1336 on Arena's Agent Arena Index across 4,200+ real-world agent sessions.
- **Science and math scores.** Best in class on Terminal-Bench Science (70.5%), RiemannBench (84.0%), and HLE-Diamond (71.3%); 73.5% on Chartography for reading dense professional charts and 75.8% on Agents' Last Exam v1.1.
- **Aggressive cache pricing.** Cached input tokens are $0.15 per million — a 95% discount — which is the lever for the long-running, repeatedly-re-read agent workflows the post is targeting.

**[Gemini 4 Neon 来了](https://deepmind.google/blog/introducing-gemini-4-neon/)** — _Google DeepMind · 11月19日_

**Main takeaway:** 一次模型发布。Gemini 4 Neon 主打的是前沿水平的智力加上"快"，软件工程、知识工作、科研这几类任务都能端到端跑完；在 Artificial Analysis Intelligence Index 上开到 xhigh thinking 拿了 61 分，总榜第三，前面只剩那些更大更慢的模型。今天就上线，输入每百万 token $3，输出 $15，上下文 100 万 token。

**Main methods:**
- **它站的是速度和前沿之间的 Pareto frontier。** Vals Index 上排第二，而且正好落在那条 Pareto frontier 上；DeepMind 卖的点不是绝对最高分，而是"同样的延迟和价格里智力最高"。
- **steerability 被当成正经指标。** 新的 Agent Arena Index 里 Neon 的 steerability 排第二，看的就是任务中途你改主意、它能不能干净地跟上；配套的还有他们内部在 Google Antigravity 上测出来的历史最低 fabrication rate。
- **企业数据一个 context 里全吃下。** 表格、PDF、图表、音频、视频塞进同一个 100 万 token 窗口，出来的是能直接用的结构化交付物；Vals Index 上 70.9%，Legal Research Bench 和 Tax Agent Bench 两个都是第一。
- **长周期 agent benchmark 表现。** Zapier 的 AutomationBench 总榜第一（56.3%），Andon Labs 的 Vending-Bench 2 也是第一（$16,843，这个是模拟长期经营一门生意）；Arena 新出的 Agent Arena Index 上首次亮相就是全球第二，1336 分，背后是 4,200 多个真实 agent session。
- **科学和数学这块。** Terminal-Bench Science（70.5%）、RiemannBench（84.0%）、HLE-Diamond（71.3%）都是同档最好；读那种信息密集的专业图表 Chartography 拿了 73.5%，Agents' Last Exam v1.1 是 75.8%，跟头部模型打平。
- **cached input 的价格给得很狠。** 缓存输入每百万 token 只要 $0.15，直接打了 95% 折，这正是给文中那种反复重读上下文的长时间 agent workflow 准备的。
