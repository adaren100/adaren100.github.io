---
title: "Gemini 4 Argon: our next era of frontier intelligence"
date: 2026-10-01
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Gemini 4 Argon: our next era of frontier intelligence](https://deepmind.google/blog/gemini-4-argon-our-next-era-of-frontier-intelligence/)** — _Google DeepMind · Oct 1_

**Main takeaway:** Google DeepMind announced Gemini 4 Argon, a frontier model built for long-horizon professional work across software engineering, legal and finance knowledge work, and defensive cybersecurity. Rather than a general launch, it is rolling out first to a set of trusted cyber defenders through the Fairwind Program, at an introductory $2 per million input tokens and $10 per million output tokens.

**Main methods:**
- **Built for sustained long-horizon reasoning.** A 1 million token limit backs deep multi-step problem solving, with the model aimed at coding, financial research, legal drafting, and autonomous cybersecurity vulnerability patching.
- **Quantum algorithmic optimization.** Argon helped Google's quantum computing researchers optimize the spacetime resources (qubits × gates) of subroutines that bottleneck important applications; in one case it beat the published baseline by 40% within minutes.
- **Fleet-wide memory optimization by agents.** A team of Argon agents read Google's fleet-wide profiling telemetry and autonomously identified and applied memory optimizations across its data centers, freeing over 300 TiB once rolled out, with an estimated 500 TiB to 1 PiB in total savings.
- **C/C++ to Rust migrations at scale.** Argon agents are migrating codebases across Google, from tens of thousands of lines in core libraries like re2 and libgav1 up to 800K+ lines for the Fuchsia Zircon kernel, with rigorous automated and manual auditing, emulation testing, and review before anything reaches production.
- **Already in Google's internal workflows.** Thousands of Googlers have been using it, flagging specialized coding tasks, deeper research, and writing quality as its strengths.
- **Staged release with external pre-release review.** Google is taking part in the U.S. government's voluntary process for pre-release model access and iterating on guardrails with feedback from early testers before opening Argon to developers, enterprises, and consumers.

**[Gemini 4 Argon：Google 的下一代 frontier 模型](https://deepmind.google/blog/gemini-4-argon-our-next-era-of-frontier-intelligence/)** — _Google DeepMind · 10月1日_

**Main takeaway:** Google DeepMind 发布了 Gemini 4 Argon，专门冲 long-horizon 的专业任务：软件工程、法律和金融这类企业知识工作，以及防御向的 cybersecurity。这次没有直接开放给所有人，而是先通过 Fairwind Program 发给一批可信的 cyber defender，价格是 input 每百万 token 2 美元、output 10 美元。

**Main methods:**
- **为长链条推理设计。** 1 million token 的上下文上限撑起多步问题求解，主打 coding、金融研究、法律文书起草，以及自动给安全漏洞打 patch。
- **帮量子团队做算法优化。** Argon 在帮 Google 量子计算的研究员优化那些卡住关键应用的子程序的 spacetime resource（qubits × gates），有一个例子里它几分钟就把已发表的 baseline 打下去 40%。
- **整个机群的内存优化交给 agent 跑。** 一组 Argon agent 读 Google fleet-wide 的 profiling telemetry，自己找出并应用了跨数据中心的内存优化，全量铺开后腾出 300 TiB 以上，估算总共能省下 500 TiB 到 1 PiB。
- **大规模把 C/C++ 迁到 Rust。** Argon agent 正在 Google 内部做迁移，从 re2、libgav1 这类核心库的几万行，一直做到 Fuchsia Zircon kernel 的 80 万行以上。因为这些系统太关键，重写过的代码要先过自动和人工审计、emulation 测试和 review 才能上生产。
- **内部已经在用了。** 几千个 Googler 用过之后反馈，它最强的地方是专门领域的 coding、更深的研究，以及写作质量。
- **分阶段放开，先过外部预审。** Google 参加了美国政府那个自愿的 pre-release 模型访问流程，一边收早期测试者的反馈一边调 guardrail，之后才会开放给开发者、企业和普通用户。
