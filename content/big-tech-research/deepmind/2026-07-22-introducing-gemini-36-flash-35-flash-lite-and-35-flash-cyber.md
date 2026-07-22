---
title: "Introducing Gemini 3.6 Flash, 3.5 Flash-Lite, and 3.5 Flash Cyber"
date: 2026-07-22
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Introducing Gemini 3.6 Flash, 3.5 Flash-Lite, and 3.5 Flash Cyber](https://deepmind.google/blog/introducing-gemini-36-flash-35-flash-lite-and-35-flash-cyber/)** — _Google DeepMind · Jul 22_

**Main takeaway:** Google DeepMind released Gemini 3.6 Flash, 3.5 Flash-Lite, and 3.5 Flash Cyber, with 3.6 Flash cutting output token usage 17% versus 3.5 Flash on the Artificial Analysis Index (up to 65% on DeepSWE) at a lower cost per output token, while pre-training has begun on Gemini 4.

**Main methods:**
- **3.6 Flash as the workhorse upgrade.** Improves coding, knowledge work, and multimodal performance over 3.5 Flash while using fewer reasoning steps and tool calls per task, priced at $1.50/1M input and $7.50/1M output tokens.
- **Benchmark gains alongside efficiency.** DeepSWE improves from 37% to 49%, MLE Bench from 49.7% to 63.9%, OSWorld-Verified (computer use) from 78.4% to 83.0%, and GDPval-AA v2 from 1349 to 1421.
- **Computer use goes native.** Computer use is now a built-in client-side tool in the Gemini API and Gemini Enterprise rather than a bolt-on capability.
- **3.5 Flash-Lite for cost/speed-sensitive agents.** The fastest, most cost-effective 3.5-class model, delivering 350 output tokens/second per the Artificial Analysis Index and outperforming prior Flash-Lite generations on agentic workflows.
- **3.5 Flash Cyber paired with CodeMender.** A new specialized cyber-focused model combined with Google's CodeMender code security agent, aimed at competitive frontier performance for vulnerability work.
- **Gemini 4 teased.** Google says it has started its most ambitious pre-training run yet for Gemini 4, alongside Gemini 3.5 Pro currently testing with partners ahead of broader release.

**[Google DeepMind 发布 Gemini 3.6 Flash、3.5 Flash-Lite 和 3.5 Flash Cyber](https://deepmind.google/blog/introducing-gemini-36-flash-35-flash-lite-and-35-flash-cyber/)** — _Google DeepMind · 7月22日_

**Main takeaway:** Google DeepMind 一口气发了 Gemini 3.6 Flash、3.5 Flash-Lite 和 3.5 Flash Cyber 三个模型，3.6 Flash 在 Artificial Analysis Index 上比 3.5 Flash 少耗 17% 的 output token（DeepSWE 上最多能到 65%），单价还更便宜，与此同时 Gemini 4 的 pre-training 已经跑起来了。

**Main methods:**
- **3.6 Flash 是主力型号升级。** 相比 3.5 Flash，coding、知识型工作和多模态表现都有提升，完成任务需要的 reasoning 步骤和 tool call 也更少，定价是 $1.50/1M input、$7.50/1M output token。
- **效率提升的同时跑分也涨了。** DeepSWE 从 37% 涨到 49%，MLE Bench 从 49.7% 涨到 63.9%，OSWorld-Verified（computer use）从 78.4% 涨到 83.0%，GDPval-AA v2 从 1349 涨到 1421。
- **computer use 变成原生能力。** 现在 Gemini API 和 Gemini Enterprise 里 computer use 是内置的 client side tool，不再是外挂能力。
- **3.5 Flash-Lite 主打省钱和快。** 3.5 档位里最快、最省钱的型号，Artificial Analysis Index 测出来能跑到 350 output tokens/秒，agentic workflow 上也比之前的 Flash-Lite 系列强不少。
- **3.5 Flash Cyber 配合 CodeMender 一起用。** 一个新的专精网络安全的模型，和 Google 的 CodeMender 代码安全 agent 搭配，目标是在漏洞相关工作上做到 frontier 级别的竞争力。
- **顺带预告了 Gemini 4。** Google 说已经启动了迄今为止最有野心的一次 pre-training run，就是给 Gemini 4 用的；同时 Gemini 3.5 Pro 正在和合作伙伴测试，准备更广泛发布。
