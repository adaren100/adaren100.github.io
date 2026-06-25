---
title: "Introducing computer use in Gemini 3.5 Flash"
date: 2026-06-25
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Introducing computer use in Gemini 3.5 Flash](https://deepmind.google/blog/introducing-computer-use-in-gemini-3-5-flash/)** — _Google DeepMind · Jun 24_

**Main takeaway:** Computer use is now a native, built-in tool in Gemini 3.5 Flash rather than a separate standalone model, giving developers Google's best-yet performance for agents that see, reason, and act across browser, mobile, and desktop environments.

**Main methods:**
- **Native integration, not a side model.** Computer use was previously only available as a standalone Gemini 2.5 computer use model; it's now folded directly into the main Gemini 3.5 Flash model alongside existing function calling and built-in tools like Search and Maps grounding.
- **Target use cases.** Pitched at long-horizon and enterprise automation tasks such as continuous software testing and cross-application knowledge work.
- **Demonstrated tasks.** Examples shown include 3.5 Flash analyzing the Gemini app to return a categorized feature list, and auditing its own documentation for accessibility issues.
- **Prompt-injection mitigation via training.** Targeted adversarial training is used specifically to harden computer use against prompt injection in live environments.
- **Two optional enterprise safeguards.** Enterprises can require explicit user confirmation for sensitive or irreversible actions, and can configure automatic task termination when an indirect prompt injection is detected.
- **Recommended defense-in-depth.** Google encourages pairing these safeguards with secure sandboxing, human-in-the-loop verification, and strict access controls; available now via the Gemini API and Gemini Enterprise Agent Platform, with a Browserbase-hosted demo.

**[Gemini 3.5 Flash 原生支持 computer use 了](https://deepmind.google/blog/introducing-computer-use-in-gemini-3-5-flash/)** — _Google DeepMind · 6月24日_

**Main takeaway:** Computer use 现在直接内置进了 Gemini 3.5 Flash，不再是单独拎出来的模型，agentic computer use 任务上拿到了 Google 目前最好的表现，开发者可以用它做能看、能推理、能跨浏览器/移动端/桌面环境动手操作的 agent。

**Main methods:**
- **从独立模型变成原生能力。** 之前 computer use 只在单独的 Gemini 2.5 computer use 模型里有，现在直接整合进了主力的 Gemini 3.5 Flash，跟已有的 function calling、Search、Maps grounding 这些内置工具放在一起用。
- **主打场景。** 瞄准的是 long-horizon 和企业级自动化任务，比如持续的软件测试、跨专业应用的知识工作。
- **实测案例。** 官方给的例子包括用 3.5 Flash 分析 Gemini app 然后输出分类好的功能列表，还有自己审计自家文档里的 accessibility 问题。
- **针对 prompt injection 做了专门训练。** 用 targeted adversarial training 来对抗 agent 在真实环境里跑的时候可能遇到的 prompt injection 风险。
- **两套可选的企业级 safeguard。** 一是对敏感或不可逆的操作要求用户明确确认，二是一旦检测到 indirect prompt injection 就自动停掉任务。
- **建议叠加多层防护。** Google 建议把这些 safeguard 跟 secure sandboxing、human-in-the-loop verification、严格的权限控制一起用；现在已经能通过 Gemini API 和 Gemini Enterprise Agent Platform 用上，Browserbase 那边也搭了个 demo 环境可以先试。
