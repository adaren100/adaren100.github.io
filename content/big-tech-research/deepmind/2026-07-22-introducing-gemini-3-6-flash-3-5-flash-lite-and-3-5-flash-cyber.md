---
title: "Introducing Gemini 3.6 Flash, 3.5 Flash-Lite, and 3.5 Flash Cyber"
date: 2026-07-22
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Introducing Gemini 3.6 Flash, 3.5 Flash-Lite, and 3.5 Flash Cyber](https://deepmind.google/blog/introducing-gemini-3-6-flash-3-5-flash-lite-and-3-5-flash-cyber/)** — _Google DeepMind · Jul 21_

**Main takeaway:** Google DeepMind introduced three new Gemini models — 3.6 Flash, 3.5 Flash-Lite, and 3.5 Flash Cyber — with 3.6 Flash cutting output token usage by 17% versus 3.5 Flash (up to 65% on DeepSWE) while improving coding, agentic, and multimodal performance at a lower price.

**Main methods:**
- **3.6 Flash: efficiency + quality gains.** Consumes 17% fewer output tokens than 3.5 Flash on the Artificial Analysis Index (up to 65% on DeepSWE by Datacurve), and takes fewer reasoning steps and tool calls per task, at a lower price of $1.50/1M input and $7.50/1M output tokens.
- **Benchmark deltas.** DeepSWE precision rose from 37% to 49%, MLE-Bench (ML research) jumped from 49.7% to 63.9%, OSWorld-Verified (computer use) improved from 78.4% to 83.0%, and GDPval-AA v2 (knowledge work) rose from 1349 to 1421.
- **Computer use now built-in.** Computer use is now a native client-side tool via the Gemini API and Gemini Enterprise, rather than a bolt-on capability.
- **3.5 Flash-Lite: speed-optimized.** The fastest, most cost-effective 3.5-class model, hitting 350 output tokens/second per the Artificial Analysis Index, with notable gains over prior Flash-Lite generations on agentic workflows.
- **3.5 Flash Cyber + CodeMender.** A new specialized cyber-focused model paired with the CodeMender code-security agent, aimed at frontier-competitive performance for cybersecurity applications specifically.
- **What's next.** Gemini 3.5 Pro is in partner testing ahead of broader release, and the team has begun its most ambitious pre-training run yet, for Gemini 4.

**[Gemini 3.6 Flash、3.5 Flash-Lite 和 3.5 Flash Cyber 发布](https://deepmind.google/blog/introducing-gemini-3-6-flash-3-5-flash-lite-and-3-5-flash-cyber/)** — _Google DeepMind · 7月21日_

**Main takeaway:** Google DeepMind 一口气放出三个新 Gemini 模型——3.6 Flash、3.5 Flash-Lite 和 3.5 Flash Cyber，其中 3.6 Flash 在 Artificial Analysis Index 上比 3.5 Flash 省 17% 的输出 token（DeepSWE 上最多能省到 65%），编码、agentic 和多模态表现都更好，价格反而更低。

**Main methods:**
- **3.6 Flash：又快又好又省。** 在 Artificial Analysis Index 上比 3.5 Flash 少耗 17% 的输出 token（Datacurve 的 DeepSWE 上最多省 65%），完成多步任务用的推理步数和工具调用也更少，价格还降到了每百万输入 token 1.50 美元、输出 token 7.50 美元。
- **跑分实测。** DeepSWE 精度从 37% 提到 49%，MLE-Bench（机器学习研究能力）从 49.7% 冲到 63.9%，OSWorld-Verified（computer use）从 78.4% 提到 83.0%，知识工作类的 GDPval-AA v2 从 1349 涨到 1421。
- **Computer use 变成原生功能。** Computer use 现在是 Gemini API 和 Gemini Enterprise 里内置的 client-side 工具，不再是外挂能力。
- **3.5 Flash-Lite：专攻速度。** 3.5 系列里最快、最便宜的一款，Artificial Analysis Index 上跑到每秒 350 个输出 token，agentic workflow 上比上一代 Flash-Lite 强不少。
- **3.5 Flash Cyber 搭配 CodeMender。** 一个专门做网络安全的高效模型，配合 CodeMender 这个代码安全 agent 一起用，目标是在网络安全场景里做到 frontier 级别的表现。
- **接下来的计划。** Gemini 3.5 Pro 正在和合作伙伴测试，准备更大范围开放；团队已经启动了迄今为止最雄心勃勃的一次预训练，也就是 Gemini 4。
