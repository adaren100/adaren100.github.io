---
title: "Richpanel helps companies automate 50% of support in 30 days"
date: 2026-11-23
draft: false
tags: ["big-tech-research", "openai"]
---

**[Richpanel helps companies automate 50% of support in 30 days](https://openai.com/business/customer-stories/richpanel-ai-customer-support)** — _OpenAI · Nov 23_

**Main takeaway:** An OpenAI customer story: Richpanel guarantees clients a 50% support-automation rate within 30 days or their money back, and CEO Amit RG says it hit that bar across roughly 300 deployments completed in the six months before the October 2026 interview. The architectural point is model tiering — GPT‑6 Astra and GPT‑6.1 Sol to build the agents' tools and procedures, GPT‑6 Luna to run the conversations.

**Main methods:**
- **The stated bottleneck.** "The intelligence is no longer the bottleneck. It's everything around it." A human support agent may touch 20 or 30 tools per customer, and the procedures they follow were often never written down anywhere.
- **"Boss AI" replaces the forward-deployed engineer.** Deploying a support agent normally needs an engineer to wire it into the customer's systems and define its behavior; Richpanel built an AI manager to do that setup instead, which customers started calling Boss AI. It writes the procedures and defines how the frontline agent, copilot, and QA agent call their tools.
- **Accuracy tier for setup.** Boss AI runs on GPT‑6 Astra and GPT‑6.1 Sol, chosen for accuracy because everything the other agents do downstream follows from what it writes.
- **Cost tier for volume.** The frontline agent is built to handle hundreds of thousands of conversations, so per-interaction cost drives model choice: GPT‑6 Luna and other OpenAI models there, and the same reasoning applies to the copilot and QA agents.
- **The economic baseline is outsourced labour.** Richpanel's customers often already run low-cost outsourced support, so automation has to pencil out against that price, not against in-house headcount.
- **What made the split possible.** Amit credits OpenAI with shipping models that handle long context and longer tasks while staying cost efficient, letting Richpanel spend deeper reasoning on preparing agents and cheaper models on the conversations. He also claims the AI beat human agents on customer satisfaction in every one of those deployments — a vendor claim, with no methodology given.

**[Richpanel：30 天把 50% 的客服自动化掉](https://openai.com/business/customer-stories/richpanel-ai-customer-support)** — _OpenAI · 11月23日_

**Main takeaway:** 一篇 OpenAI 的客户案例：Richpanel 给客户的承诺是 30 天内把 50% 的客服工单自动化，做不到就退钱。CEO Amit RG 说截至 2026 年 10 月那次采访，前面半年做完的大约 300 个部署全都达标了。技术上值得看的是他们怎么分层用模型：GPT‑6 Astra 和 GPT‑6.1 Sol 负责把 agent 的工具和流程搭出来，GPT‑6 Luna 负责真正跟客户聊。

**Main methods:**
- **他们认为卡点在哪。** 原话是"intelligence 已经不是瓶颈了，瓶颈是它周围的一切"。一个人类客服服务一个客户可能要用上 20、30 个工具，而他们实际走的流程往往从来没被写下来过。
- **"Boss AI" 顶掉了 forward-deployed engineer 这个角色。** 平时上线一个客服 agent，得有工程师把它接进客户系统、再定义它该怎么干活。Richpanel 干脆做了个 AI manager 来干这件事，客户自己管它叫 Boss AI：流程由它写，前线 agent、copilot 和质检 agent 怎么调工具也由它定。
- **搭的时候用准确度那一档。** Boss AI 跑在 GPT‑6 Astra 和 GPT‑6.1 Sol 上，就是图准，因为下游几个 agent 的行为全都跟着它写出来的东西走。
- **跑量的时候换成便宜那一档。** 前线 agent 要扛几十万量级的对话，所以单次交互的成本直接决定选哪个模型，这块用的是 GPT‑6 Luna 和其他几个 OpenAI 模型；copilot 和质检 agent 也是同一套思路。
- **账是跟外包人力比的。** Richpanel 的客户本来很多就在用便宜的外包客服，所以自动化这笔账得跟那个价格比才算得过去，不是跟自建团队比。
- **这套分层能成立的前提。** Amit 把功劳给了 OpenAI 这边：模型能吃长 context、能做更长的任务，同时成本还压得住，他们才敢把重 reasoning 花在准备 agent 上、把便宜模型放到对话里。他还说这些部署里 AI 在客户满意度上都赢过人类客服，不过这是厂商自己的说法，文章没给任何评测方法。
