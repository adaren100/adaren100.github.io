---
title: "Developing Enterprise Frontier Safeguards with our customers"
date: 2026-09-01
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[Developing Enterprise Frontier Safeguards with our customers](https://www.anthropic.com/news/enterprise-frontier-safeguards)** — _Anthropic · Sep 1_

**Main takeaway:** Anthropic is announcing Enterprise Frontier Safeguards (EFS), which pairs the privacy of zero data retention with the misuse detection that normally requires retaining data, by storing the data in cloud infrastructure the customer controls rather than Anthropic's. It rolls out in phases starting later this fall, and eligible customers keep ZDR on Fable 5 and Fable 5.1 until it's ready.

**Main methods:**
- **The dilemma EFS is built around.** Mythos-class models like Claude Fable 5.1 bring a large jump in intelligence and agentic capability, and with it more room for both misuse and autonomous misbehavior — including agents autonomously doing destructive things and attacks using stolen enterprise credentials, which are hard to spot without watching traffic for abnormal behavior.
- **Why per-interaction analysis isn't enough.** The most sophisticated misuse spreads tasks across many sessions and accounts, so data has to be held for a meaningful window to be correlated across time and accounts — analyzing each interaction and instantly discarding it can't catch it.
- **Retention was a safety decision, not a training one.** Anthropic introduced 30-day retention starting with Fable 5, and states it has never trained on enterprise data without explicit permission and never will.
- **Customer-controlled storage as the resolution.** Data lives in the customer's own cloud infrastructure, which is what lets EFS offer ZDR-grade privacy alongside cross-session monitoring — the sticking point for regulated industries that understood the safety case but couldn't adopt models with retention.
- **Designed with 100+ customers and the three major clouds.** Financial services, healthcare, manufacturing, telecom, law, retail and public sector, plus AWS, Google Cloud and Microsoft Azure. Feedback came from the security, product, compliance and delivery teams who'd actually operate it.
- **Who was in the room, and where it will run.** Partners included ARC (whose members are the CISOs of Goldman Sachs, Morgan Stanley, Citi, Bank of America and Wells Fargo) plus Comcast, KPMG, Mastercard, Salesforce and Visa — spanning a quarter of the Fortune 100. Support is planned for Claude Code, Claude Enterprise, the Claude Platform, Amazon Bedrock, Claude Platform on AWS, Google's Agent Platform and Microsoft Foundry. (The extracted body stops before the specific concerns and countermeasures are listed.)

**[Anthropic 推 Enterprise Frontier Safeguards：既要 ZDR，又要能查滥用](https://www.anthropic.com/news/enterprise-frontier-safeguards)** — _Anthropic · 9月1日_

**Main takeaway:** Anthropic announce 了 Enterprise Frontier Safeguards（EFS），想把 zero data retention 的隐私和"必须留数据才能做"的滥用检测同时拿到，办法是把数据存在客户自己控制的云上，而不是 Anthropic 手里。今年秋天晚些时候开始分批 rollout，在这之前符合条件的客户在 Fable 5 和 Fable 5.1 上继续享受 ZDR。

**Main methods:**
- **EFS 要解的那个两难。** Claude Fable 5.1 这种 Mythos 级别的模型，智能和 agentic 能力上了一大截，misuse 和自主乱来的空间也跟着变大，包括 agent 自己跑去做破坏性操作，以及拿偷来的企业 credential 发起的攻击。后面这类不盯着流量看异常行为，基本发现不了。
- **为什么单次交互分析不够用。** 真正老练的滥用会把任务拆散，铺在很多 session 和账号上，所以数据得留一段时间，才能跨时间、跨账号关联起来。每次交互单独分析完就立刻丢掉，这种玩法接不住。
- **留数据是出于安全，不是为了训练。** 从 Fable 5 开始 Anthropic 加了 30 天数据保留，他们特意强调：没有明确许可，Anthropic 从来没有拿企业数据训练过，以后也不会。
- **解法是把存储交给客户。** 数据放在客户自己的云基础设施里，这才让 ZDR 级别的隐私和跨 session 监控能共存。之前卡住的就是这一点，受监管行业其实认可安全上的道理，但带数据保留的模型他们真的用不了。
- **拉上 100 多家客户和三大云一起设计。** 金融、医疗、制造、电信、法律、零售、公共部门都有，云那边是 AWS、Google Cloud 和 Microsoft Azure。给意见的是真正每天要用它的人：安全、产品、合规、交付团队。
- **参与的都有谁，将来在哪儿能用。** 合作方里有 ARC（成员是 Goldman Sachs、Morgan Stanley、Citi、Bank of America、Wells Fargo 这些美国最大银行的 CISO），还有 Comcast、KPMG、Mastercard、Salesforce、Visa，聊过的公司覆盖了四分之一的 Fortune 100。支持范围计划包括 Claude Code、Claude Enterprise、Claude Platform、Amazon Bedrock、AWS 上的 Claude Platform、Google 的 Agent Platform 和 Microsoft Foundry。抓到的正文到"客户具体提了哪些顾虑、EFS 分别怎么应对"这里就断了。
