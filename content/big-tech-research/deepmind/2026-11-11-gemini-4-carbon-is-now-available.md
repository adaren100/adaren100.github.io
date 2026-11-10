---
title: "Gemini 4 Carbon is now available"
date: 2026-11-11
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Gemini 4 Carbon is now available](https://deepmind.google/blog/gemini-4-carbon-is-now-available/)** — _Google DeepMind · Nov 11_

**Main takeaway:** A model release: Gemini 4 Carbon, DeepMind's strongest model for cybersecurity and long-horizon agentic work, is now open to all paying developers, enterprises, and Google AI Ultra subscribers at the same introductory price as Gemini 4 Argon ($2 / $10 per million input / output tokens). It ranks #1 on CursorBench 4.0, Perplexity's WANDR, and Zapier's AutomationBench at more than 2× lower cost per task than the next best external model.

**Main methods:**
- **Positioned above Argon, not replacing it.** Argon stays the default for most software engineering and knowledge work; Carbon is for tasks that test the limits of model intelligence — multi-step coding and debugging, open-ended scientific research — and deliberately spends more tokens to explore, reason, and run extended verification loops.
- **Staged rollout through defenders first.** Carbon went to a set of cybersecurity defenders via the Fairwind Program two weeks before this general release.
- **`/swarm` in Google Antigravity (preview).** Turns a single prompt into a coordinated, real-time-trackable team of agents: Carbon takes the deepest-reasoning roles (architectural design, coordination, auditing) while faster, lighter models run in parallel isolated workspaces alongside adversarial verifiers that test every change.
- **A new multimodal agent benchmark.** Because existing benchmarks don't capture agents reasoning natively over dense files with charts, blueprints, schematics, and tables, DeepMind partnered with Artificial Analysis on the Multimodal Knowledge Agent (MKA) benchmark; Carbon ranks #2 there at more than 6× lower average cost per task than the top performer.
- **Built for precision knowledge work.** Across legal, finance, and enterprise operations it pairs visual understanding with exhaustive retrieval over large dense document sets, and follows strict schemas and formatting to emit polished spreadsheets, presentations, and reports.
- **Wide surface availability.** API access through Google AI Studio and Gemini for business, plus rollout in Google Antigravity, the Gemini app, and AI Mode in Search.

**[Gemini 4 Carbon 正式开放](https://deepmind.google/blog/gemini-4-carbon-is-now-available/)** — _Google DeepMind · 11月11日_

**Main takeaway:** 一次模型发布。Gemini 4 Carbon 是 DeepMind 目前最强的一档，主打 cybersecurity 和长周期 agentic 任务，现在所有付费开发者、企业客户和 Google AI Ultra 订阅用户都能用，价格跟 Gemini 4 Argon 一样还是尝鲜价（输入每百万 token $2，输出 $10）。它在 CursorBench 4.0、Perplexity 的 WANDR 和 Zapier 的 AutomationBench 上都拿了第一，每个任务的成本还比第二名的外部模型低一半以上。

**Main methods:**
- **Carbon 不是来替掉 Argon 的。** 日常的软件工程和知识工作还是用 Argon 更合适；Carbon 是留给那些真正压榨模型智力上限的活儿，比如多步编码调试、开放式科研探索，它会故意比 Argon 烧更多 token，用来充分探索、深度 reasoning，还有跑很长的验证循环。
- **先给防守方试。** 两周前他们通过 Fairwind Program 把 Carbon 先放给了一批安全防守方，这次才正式开放。
- **Google Antigravity 里的 `/swarm`（预览）。** 一句 prompt 就能展开成一支能实时盯进度的 agent 团队：架构设计、协调、审计这类最吃 reasoning 的角色交给 Carbon，旁边配上跑在各自隔离 workspace 里的轻量模型，还有专门挑刺的 adversarial verifier，每个改动都要过一遍。
- **顺手推了个新的多模态 agent benchmark。** 现有 benchmark 测不出 agent 直接读带图表、蓝图、原理图和表格的密集文件时到底怎么推理，所以他们拉上 Artificial Analysis 做了 Multimodal Knowledge Agent（MKA）；Carbon 在上面排第二，但平均每任务成本比第一名低 6 倍以上。
- **冲着高精度知识工作做的。** 法律、金融、企业运营这些场景里，它把视觉理解和地毯式检索结合起来处理成堆的密集文档，还能严格照着给定的 schema 和格式产出能直接用的表格、演示文稿和报告。
- **铺开的面挺广。** API 走 Google AI Studio 和 Gemini for business，同时也上了 Google Antigravity、Gemini app 和 Search 里的 AI Mode。
