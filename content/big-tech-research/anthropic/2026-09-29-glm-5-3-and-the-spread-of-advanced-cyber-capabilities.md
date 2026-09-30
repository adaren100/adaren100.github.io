---
title: "GLM-5.3 and the spread of advanced cyber capabilities"
date: 2026-09-29
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[GLM-5.3 and the spread of advanced cyber capabilities](https://www.anthropic.com/research/glm-5-3-and-the-spread-of-advanced-cyber-capabilities)** — _Anthropic · Sep 29_

**Main takeaway:** Anthropic's evaluation of Zhipu AI's GLM-5.3 finds it can autonomously build end-to-end cyber exploits at roughly Claude Mythos Preview's rate, but shipped without meaningful misuse safeguards: simple techniques bypassed its safeguards 64–100% of the time in simulated tests, while the same attacks failed against safeguarded Claude models.

**Main methods:**
- **Safeguard-bypass testing is the new contribution.** Anthropic's capability numbers broadly match NIST CAISI's Sept. 17 assessment, which called GLM-5.3 "the most cyber-capable open-weight model released to date" and about four months behind the US frontier on an aggregate of CAISI's cyber benchmarks. This post adds how easily GLM-5.3's safeguards can be bypassed or removed.
- **ExploitBench, end-to-end only.** On ExploitBench, which measures exploiting known vulnerabilities in Chrome's V8 engine, GLM-5.3 produced working end-to-end exploits in 50 of 410 attempts, against 56 of 410 for Claude Mythos Preview. They score end-to-end success specifically because that's what matters to an attacker.
- **Two evaluation modes, sandboxed.** Automated benchmarks plus human-in-the-loop workflows, with every tested model confined to isolated sandboxes attacking only offline targets Anthropic set up. An internal Binary Exploitation benchmark tests finding plus exploiting vulnerabilities, not just exploiting known ones.
- **The access asymmetry.** CAISI compared US models with cyber safeguards disabled where applicable, and its US frontier includes models released only to vetted users, which attackers can't readily get. Anyone can download GLM-5.3.
- **Why Mythos Preview was gated.** Anthropic released it narrowly through Project Glasswing, where trusted defenders found more than 10,000 vulnerabilities in critical software, on the bet that comparable capability would proliferate and defenders should get a head start. The post's premise is that those models have now arrived.
- **Dual-use, acknowledged.** Anthropic assesses GLM-5.3's lax safeguards as significantly expanding what malicious actors can do, while noting the same capabilities help defenders secure their own systems.

**[GLM-5.3：能自己写出完整 exploit，却几乎没配 safeguard](https://www.anthropic.com/research/glm-5-3-and-the-spread-of-advanced-cyber-capabilities)** — _Anthropic · 9月29日_

**Main takeaway:** Anthropic 实测了智谱（Zhipu AI，海外叫 Z.ai）的 GLM-5.3，发现它自主写出端到端 exploit 的水平跟 Claude Mythos Preview 差不多，但发布时基本没带能拦住滥用的 safeguard：在模拟测试里用很简单的手法就能绕过，成功率 64% 到 100%，同一批攻击打在带 safeguard 的 Claude 上一次都没成。

**Main methods:**
- **这篇真正补上的是绕过测试。** 能力数据上 Anthropic 跟 NIST CAISI 9 月 17 日那份评估大体一致，CAISI 说 GLM-5.3 是"迄今最强的 open-weight 网络攻击模型"，在他们整套 cyber benchmark 的综合成绩上落后美国 frontier 大约四个月。Anthropic 这篇加的是：它的 safeguard 有多容易被绕过或者直接拆掉。
- **ExploitBench 只看端到端。** ExploitBench 测的是能不能利用 Chrome V8 引擎里已知的漏洞，GLM-5.3 在 410 次尝试里写出 50 个能跑通的完整 exploit，Claude Mythos Preview 是 410 次里 56 个。他们专门只算端到端成功，因为对攻击者来说这才是有用的那一档。
- **两套评测，全程沙箱。** 自动化 benchmark 加上 human-in-the-loop 流程，所有被测模型都关在隔离沙箱里，只能打 Anthropic 自己搭的离线目标。另外还有一个内部的 Binary Exploitation benchmark，考的是自己找漏洞再利用，不只是利用已知漏洞。
- **不对等的地方在获取难度。** CAISI 那份对比里，美国模型是在关掉 cyber safeguard 的状态下测的，而且所谓美国 frontier 包含了只对审核过的用户开放的版本，攻击者拿不到。GLM-5.3 谁都能下载。
- **当初 Mythos Preview 为什么要限流。** Anthropic 只通过 Project Glasswing 小范围放出去，让可信的防守方在关键软件里找出了一万多个漏洞，赌的就是同等能力迟早会扩散，得先让防守方抢一段时间。这篇的前提是：那批模型现在到了。
- **dual-use 他们也承认。** Anthropic 判断 GLM-5.3 这种松散的 safeguard 明显抬高了恶意行为者手上的能力，同时也说同一套能力对想加固自己系统的防守方一样有用。
