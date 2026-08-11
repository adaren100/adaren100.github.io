---
title: "Responding to the next frontier of critical cyber capabilities"
date: 2026-08-08
draft: false
tags: ["big-tech-research", "openai"]
---

**[Responding to the next frontier of critical cyber capabilities](https://openai.com/index/responding-next-frontier-critical-cyber-capabilities)** — _OpenAI · Aug 8_

**Main takeaway:** Internal evals of Astra, an upcoming OpenAI model, show enough of a jump in agentic coding and cybersecurity that OpenAI says it cannot rule out the Critical cyber threshold under its Preparedness Framework — a step up from every prior model, including GPT-5.6 Sol, which were assessed at High.

**Main methods:**
- **What Critical means in the framework.** A model hits the Critical cyber threshold if it can identify and develop functional zero-day exploits of all severity levels in many hardened real-world critical systems without human intervention, or devise and execute end-to-end novel attack strategies against hardened targets given only a high-level goal.
- **The finding is preliminary.** Evaluations over the past few days plus expert assessment led OpenAI to conclude overnight that Critical can't be ruled out; benchmarking continues. The post explicitly notes Astra was not involved in exploiting Hugging Face.
- **Security controls scaled up.** Isolated testing environments, restricted network and tool access, enhanced model weight protections and encryption, additional monitoring and detection, and sandboxed execution.
- **Work paused where controls don't yet meet the bar.** OpenAI says it is pausing internal activities involving Astra that don't yet satisfy the strengthened security requirements.
- **Universal chain-of-thought monitoring.** All agentic applications of Astra, including training and evaluation, are monitored for risky actions and misalignment; monitors read the model's chain of thought and trigger a security response to review and interrupt high-risk activity.
- **External testing and shared controls.** OpenAI will work with relevant government agencies and select AI safety organizations to test the model, and will give recommended security controls to third-party testing partners running higher-risk evaluations and workloads.

**[Astra 的 cyber 能力可能已经踩到 Critical 线了](https://openai.com/index/responding-next-frontier-critical-cyber-capabilities)** — _OpenAI · 8月8日_

**Main takeaway:** OpenAI 在内部评测里发现，即将发布的模型 Astra 在 agentic coding 和网络安全上的提升幅度太大，按他们自己的 Preparedness Framework，已经没法排除它达到 Critical 这一档 cyber 能力。此前包括 GPT-5.6 Sol 在内的所有模型都只被评到 High。

**Main methods:**
- **Critical 这档的定义。** 按框架的说法，模型要是能在没有人介入的情况下，在大量加固过的真实关键系统里找出并写出各种严重级别的可用 zero-day exploit，或者只给一个高层目标就能自己设计并执行一整套针对硬目标的新型攻击方案，那就算踩到 Critical 了。
- **结论还是初步的。** 最近几天的评测加上专家判断，让他们在前一天晚上得出"排除不了 Critical"这个结论，benchmark 还在继续跑。文章还特意澄清了一句：Astra 跟 Hugging Face 那次被入侵没关系。
- **安全管控整个提了一档。** 隔离的测试环境、限制网络和工具访问、加强模型权重保护和加密、加装更多监控和检测、执行全部放进沙箱。
- **达不到新标准的活先停。** 内部涉及 Astra 但还没满足这套加强版安全要求的活动，OpenAI 说直接暂停。
- **全量上 chain-of-thought 监控。** Astra 所有 agentic 场景，包括训练和评测环节，都挂上了针对高风险行为和 misalignment 的监控；monitor 会读模型的 chain of thought，一旦触发就走安全响应流程，人工复核并中断高风险动作。
- **外部测试和管控外发。** 他们会拉上相关政府机构和一部分 AI 安全组织来测这个模型，同时把推荐的安全管控方案给到第三方测试伙伴，让他们跑高风险 eval 和 workload 时也有一套可依。
