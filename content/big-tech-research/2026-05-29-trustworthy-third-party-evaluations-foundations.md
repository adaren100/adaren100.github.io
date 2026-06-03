---
title: "A shared playbook for trustworthy third party evaluations"
date: 2026-05-29
draft: false
tags: ["ai-digest", "research", "big-tech-research"]
source_org: "OpenAI"
source_url: "https://openai.com/index/trustworthy-third-party-evaluations-foundations"
---

**[A shared playbook for trustworthy third party evaluations](https://openai.com/index/trustworthy-third-party-evaluations-foundations)** — _OpenAI · May 29_

**Main takeaway:** OpenAI publishes a methodology guide for evaluating frontier AI models, arguing that modern models must be tested as tool-using, multi-step agents — not as chatbots — because performance depends heavily on the "harness" (execution environment and workflow setup) surrounding the model.

**Main methods:**
- **Beyond prompt-and-answer evaluation.** Today's frontier models use tools, maintain state across steps, and act within larger workflows; evaluation setups that prompt the model as a user miss critical capability signals.
- **Harness design as a first-class concern.** The harness — the scaffolding managing tool calls, context, and orchestration — can significantly alter benchmark scores, so OpenAI recommends evaluators publish full harness specs alongside results.
- **Capability vs. safety mitigations.** The guide distinguishes evaluating raw capabilities (what can the model do?) from evaluating mitigations (does the safeguard actually prevent misuse?), recommending different methodologies for each.
- **Ecological validity.** Tasks should reflect realistic attacker or user conditions, not idealized lab setups; the guide flags common validity-undermining mistakes like giving too many hints or using atypically clean environments.
- **Toward shared norms.** OpenAI frames the playbook as a contribution toward shared standards for third-party auditors — intended as input to the broader eval community, not an internal policy.

**[前沿模型第三方评估手册](https://openai.com/index/trustworthy-third-party-evaluations-foundations)** — _OpenAI · 5月29日_

**Main takeaway:** OpenAI 发了一篇方法论指南，专门讲怎么做前沿 AI 模型的第三方评估。核心论点：现在的模型是工具调用、多步推理的 agent，不是聊天机器人——用老方法评估会漏掉关键信号，因为模型表现严重依赖它运行的 "harness"（执行环境和工作流框架）。

**Main methods:**
- **超越"问答式"评估。** 今天的前沿模型会用工具、跨多步维护状态、嵌入更大的工作流——用"给它发消息看回答"这种方式会系统性地误估它的真实能力。
- **Harness 设计是一等公民。** Harness（管理工具调用、上下文、编排的脚手架）会显著影响 benchmark 分数，评估者应该把完整的 harness 规格跟结果一起公开发布。
- **能力评估 vs. 缓解措施评估。** 指南区分了两类：模型能做什么（能力上限）vs. 安全缓解措施是否真的挡住了滥用——两类的方法论不同，不能混用。
- **生态效度。** 任务设计要贴近真实的攻击者/用户条件，而不是理想化的实验室设置；指南列了常见的效度失效模式，比如给了太多提示、用了过于干净的环境。
- **迈向行业标准。** OpenAI 把这份 playbook 定位为对更广泛评估社区的贡献，推动第三方审计员之间形成共同规范。
