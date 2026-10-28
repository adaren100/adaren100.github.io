---
title: "Gemini 4 Carbon: Our next frontier model"
date: 2026-10-29
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Gemini 4 Carbon: Our next frontier model](https://deepmind.google/blog/gemini-4-carbon-our-next-frontier-model/)** — _Google DeepMind · Oct 29_

**Main takeaway:** Google DeepMind announced Gemini 4 Carbon, a frontier model aimed at cybersecurity defense and long-horizon agentic work, which ranks #1 on v5.0 of the Artificial Analysis Intelligence Index at 59. It leads SEC-bench Pro (88.2%) for vulnerability finding, ExploitGym (54.8%) for exploitation, and CWE-bench (71.0%) for patching.

**Main methods:**
- **Full cyberdefense lifecycle, not just detection.** Carbon claims state-of-the-art across vulnerability detection, validation, and remediation, with the three external benchmark scores evaluated without guardrails in place.
- **Internal secure-coding uplift.** On internal benchmarks Carbon more than doubles the success rate for generating secure code over Gemini 4 Argon, and in live coding environments with Google's own teams it shows reduced misalignment and fabrication rates.
- **Partner validation.** The Chrome team reported Carbon performing 10×+ better than another lab's large frontier model at generating high-quality patches, and cloud security platform Wiz sees it leading web pen-testing benchmarks for its Scan for Good initiative.
- **Built for multi-day agentic runs.** Internal teams have had Carbon run for days, pushing through dead ends on multi-step engineering tasks like root-causing and patching subtle bugs across large codebases and low-level systems.
- **Broader quality gains.** Web development output quality improved enough to jump +89 elo to #4 (1768) on WebDev Arena, alongside gains in coding, agentic, scientific, and multimodal tasks.
- **Staged, government-engaged rollout.** Google is in the U.S. government's voluntary pre-release testing process; access starts this week with a subset of cyber defenders, then phases out to trusted partners via the Fairwind Program before general availability. Pricing matches Argon's introductory $2 / $10 per million input / output tokens, with cached input 95% off.

**[Gemini 4 Carbon：安全能力拉满的下一代前沿模型](https://deepmind.google/blog/gemini-4-carbon-our-next-frontier-model/)** — _Google DeepMind · 10月29日_

**Main takeaway:** Google DeepMind 放出了 Gemini 4 Carbon，主打 cybersecurity 防御和超长时间跨度的 agentic 任务，在最新 v5.0 的 Artificial Analysis Intelligence Index 上以 59 分排第一。三条安全线也都是第一：找漏洞的 SEC-bench Pro 88.2%，做 exploitation 的 ExploitGym 54.8%，打补丁的 CWE-bench 71.0%。

**Main methods:**
- **覆盖整条 cyberdefense 链路。** 不只是检测，detection、validation、remediation 三段都说是 state-of-the-art，上面那三个外部 benchmark 的分数是在不加 guardrail 的情况下测的。
- **内部实测安全代码写得更稳。** 内部 benchmark 上生成安全代码的成功率比 Gemini 4 Argon 翻了一倍多，在 Google 自己团队真实的 coding 环境里，misalignment 和瞎编（fabrication）的比例也降了。
- **合作方那边也对得上。** Chrome 团队说在生成高质量 patch 这件事上，Carbon 比另一家实验室的大模型好 10 倍以上；云安全平台 Wiz 也看到它在 web pen-testing 的 benchmark 上领先，这正是他们 Scan for Good 计划的核心能力。
- **就是为跑好几天设计的。** 内部团队让它连着跑好几天，在大型 codebase 和底层系统里一步步定位并修掉那些很隐晦的 bug，撞进死路也能自己退出来接着试。
- **通用能力顺手也涨了。** web 开发的产出质量提升明显，WebDev Arena 上直接涨了 89 elo，到 1768 分排第四；coding、agentic、科学任务和多模态理解也都有进步。
- **发布节奏刻意放慢。** Google 正在参与美国政府那套自愿的发布前模型测试流程，这周先给一小批 cyber defender 用，再通过 Fairwind Program 逐步放给更多信任的合作方，之后才会进产品面向开发者和普通用户。价格跟 Argon 的首发价一样，每百万 input token 2 美元、output 10 美元，cached input token 在此基础上再便宜 95%。
