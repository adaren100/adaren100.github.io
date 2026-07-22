---
title: "Introducing Gemini 3.5 Flash Cyber"
date: 2026-07-18
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Introducing Gemini 3.5 Flash Cyber](https://deepmind.google/blog/introducing-gemini-3-5-flash-cyber/)** — _Google DeepMind · Jul 18_

**Main takeaway:** Google DeepMind introduced Gemini 3.5 Flash Cyber, a lightweight cybersecurity model built on 3.5 Flash and fine-tuned to find, validate, and patch vulnerabilities, which in internal Big Sleep testing without safety guardrails significantly surpassed both mainline 3.5 Flash and 3.6 Flash on hard vulnerabilities in codebases like Chrome and Safari.

**Main methods:**
- **Lightweight model as the design choice.** Built on Flash rather than a large frontier model, aiming to offer a cost-efficient alternative to bigger, costlier cybersecurity models while remaining highly capable.
- **Solves the search-space bottleneck via repeated cheap calls.** Because 3.5 Flash Cyber is cheap to run, CodeMender invokes it multiple times (up to five, per the CyberGym setup) so sub-agents can explore far more code paths before producing one consolidated report.
- **Competitive on CyberGym.** Configured with up to five calls per final report, the CodeMender + 3.5 Flash Cyber combination achieved competitive performance against significantly larger models on the CyberGym benchmark (competitor scores are self-reported).
- **Stress-tested beyond the benchmark.** Google's Big Sleep team ran an independent evaluation targeting hard-to-find critical vulnerabilities in complex codebases (Chrome, Safari), where 3.5 Flash Cyber beat mainline 3.5 Flash and 3.6 Flash.
- **Limited-access, dual-use rollout.** Given the dual-use nature of a vulnerability-finding model, initial access is restricted to governments and trusted partners via CodeMender, expanding over time; CodeMender's broader capabilities are separately reaching customers through the Gemini Enterprise Agent Platform.

**[Google DeepMind 推出 Gemini 3.5 Flash Cyber](https://deepmind.google/blog/introducing-gemini-3-5-flash-cyber/)** — _Google DeepMind · 7月18日_

**Main takeaway:** Google DeepMind 推出了 Gemini 3.5 Flash Cyber，一个基于 3.5 Flash、专门微调来找漏洞、验证漏洞、修漏洞的轻量安全模型。在关掉安全防护的内部 Big Sleep 测试里，它在 Chrome、Safari 这类复杂代码库的高难度漏洞上，表现明显超过了主线的 3.5 Flash 和 3.6 Flash。

**Main methods:**
- **选轻量模型是有意为之的设计。** 没有用更大的 frontier 模型，而是基于 Flash 打造，目的是在保持强能力的同时，做出一个比又大又贵的安全模型更省钱的替代方案。
- **靠多次便宜调用解决搜索空间问题。** 因为 3.5 Flash Cyber 跑起来便宜，CodeMender 会多次调用它（CyberGym 的配置里最多五次），让 sub-agent 能探索多得多的代码路径，最后再汇总成一份报告。
- **CyberGym 上跑分能打。** 配置成每份最终报告最多调用五次之后，CodeMender 加 3.5 Flash Cyber 的组合在 CyberGym benchmark 上打出了和体量大得多的模型差不多的成绩（对手的分数是厂商自报的）。
- **跳出 benchmark 的压力测试。** Google 的 Big Sleep 团队另外做了一次评估，专门找 Chrome、Safari 这类复杂代码库里难找的严重漏洞，结果 3.5 Flash Cyber 比主线的 3.5 Flash 和 3.6 Flash 都强。
- **先小范围放开，因为是双刃剑。** 考虑到一个专门找漏洞的模型天生就是双刃剑，目前只通过 CodeMender 面向政府和可信合作伙伴开放，之后会逐步扩大；CodeMender 更基础的能力则另外通过 Gemini Enterprise Agent Platform 面向普通客户开放。
