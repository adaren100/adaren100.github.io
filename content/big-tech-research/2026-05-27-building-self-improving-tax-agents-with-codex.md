---
title: "Building self-improving tax agents with Codex"
date: 2026-05-27
draft: false
tags: ["OpenAI", "research", "big-tech-research"]
source_org: "OpenAI"
source_url: "https://openai.com/index/building-self-improving-tax-agents-with-codex"
---

**[Building self-improving tax agents with Codex](https://openai.com/index/building-self-improving-tax-agents-with-codex)** — _OpenAI · May 27_

**Main takeaway:** OpenAI and Thrive Holdings describe a six-month co-development effort to build a self-improving tax agent for Crete accountants, where Codex-driven eval infrastructure automates the feedback loop from production failures to prompt and code improvements — replacing the manual engineer-in-the-loop update cycle.

**Main methods:**
- **Self-improvement via eval infrastructure.** The core insight: with good eval harnesses and access to real practitioner environments, you can build agents that detect their own production failures and improve without manual engineer intervention each cycle.
- **Practitioner-in-the-loop data generation.** Tax domain expertise was embedded by pairing engineers with Crete's accountants to generate realistic edge cases and ground-truth annotations that pure synthetic data misses.
- **Codex as meta-level optimizer.** Codex was used not just as the agent itself but as the optimizer — rewriting prompts and code based on eval failures, closing the loop between production behavior and model instructions.
- **Forward deployment model.** OpenAI engineers embedded directly with the customer team for six months, enabling rapid iteration that a remote API relationship wouldn't support.

**[用 Codex 构建自我改进的税务 agent](https://openai.com/index/building-self-improving-tax-agents-with-codex)** — _OpenAI · 5月27日_

**Main takeaway:** OpenAI 和 Thrive Holdings 花六个月为 Crete 税务会计师联合开发了一个自我改进税务 agent，核心方法是用 Codex 驱动的 eval 基础设施，把"生产环境报错→改进提示词和代码"这个反馈循环自动化，替代了之前靠工程师手动推进的瓶颈。

**Main methods:**
- **靠 eval 基础设施实现自我改进。** 关键洞察：有了完善的 eval harness 和真实从业者环境的访问权限，可以构建能自动检测生产故障并自我改进的 agent，不需要工程师手动介入每次迭代。
- **从业者参与生成数据。** 把税务领域专业知识嵌进来的方式：让工程师和 Crete 的会计师配对工作，生成纯合成数据覆盖不到的真实边缘案例和 ground-truth 标注。
- **Codex 同时是 agent 本身和元层面优化器。** Codex 不只是跑任务的 agent，还被用来根据 eval 失败重写提示词和代码——把生产行为和模型指令之间的反馈环闭合。
- **前置部署模式。** OpenAI 工程师直接嵌入客户团队工作了六个月，这种深度配合支撑了快速迭代，远程 API 关系做不到。
