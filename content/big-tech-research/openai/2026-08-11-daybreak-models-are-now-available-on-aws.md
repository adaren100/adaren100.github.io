---
title: "Daybreak models are now available on AWS"
date: 2026-08-11
draft: false
tags: ["big-tech-research", "openai"]
---

**[Daybreak models are now available on AWS](https://openai.com/index/daybreak-models-are-now-available-on-aws)** — _OpenAI · Aug 11_

**Main takeaway:** OpenAI is making its Daybreak cyber capabilities available through Amazon Bedrock, with both the Daybreak Blue and Daybreak Red access levels live on AWS. This is a distribution and procurement move — the same models, reachable from inside the AWS environments enterprises already operate.

**Main methods:**
- **Two access levels, both on AWS.** Daybreak Blue gives access to frontier general-purpose models, including GPT‑5.6 Sol, with safeguards tailored to authorized defensive security work. Daybreak Red gives access to the purpose-trained cybersecurity models for authorized vulnerability research, exploit validation, and security testing.
- **Workflows targeted end to end.** The models are pitched at vulnerability research, detection engineering, and incident response — from initial discovery through to a validated fix — plus harder workflows like exploit reproduction and mitigation development.
- **The stated blocker was never model quality.** OpenAI argues enterprise adoption of specialized cyber capabilities also needs security review, governance, procurement, access controls, and an operating model teams can actually support.
- **Bedrock is the answer to that blocker.** Routing through Amazon Bedrock lets eligible customers apply the models via familiar AWS security, governance, and operational workflows, in the environments where they already build, secure, and run software.
- **Access is gated and endpoint-specific.** Daybreak Red and Daybreak Blue both require enrollment in Daybreak Access; once approved, you reach the model through the Amazon Bedrock console or the Responses API using the `bedrock-mantle` endpoint.
- **Builds on an earlier AWS step.** Earlier this year OpenAI frontier models and Codex became generally available on AWS; the post frames Daybreak on Bedrock as the next installment of that partnership.

**[Daybreak 上 AWS 了](https://openai.com/index/daybreak-models-are-now-available-on-aws)** — _OpenAI · 8月11日_

**Main takeaway:** OpenAI 把 Daybreak 那套安全能力搬到了 Amazon Bedrock 上，Daybreak Blue 和 Daybreak Red 两档权限在 AWS 都能用了。这篇讲的是渠道和采购路径，模型本身没变，只是现在能从企业本来就在跑的 AWS 环境里直接调。

**Main methods:**
- **两档权限，AWS 上都有。** Daybreak Blue 给的是前沿通用模型，包括 GPT‑5.6 Sol，safeguard 是按授权过的防守方工作调的。Daybreak Red 给的是他们专门训过的安全模型，面向获得授权的 vulnerability research、exploit 验证和安全测试。
- **想覆盖的是整条链路。** 从最开始的发现一直到确认修好，vulnerability research、detection engineering、incident response 都算在内，还包括 exploit 复现和写 mitigation 这类更难的活。
- **卡住企业的从来不是模型好不好。** OpenAI 的说法是，企业要用上这类专门的安全能力，还得过 security review、治理、采购、权限控制这些关，最后团队得真的运维得起来。
- **Bedrock 就是冲着这个来的。** 走 Amazon Bedrock 之后，符合条件的客户可以沿用自己熟悉的 AWS 安全、治理和运维流程，在本来就用来开发、防护、运行软件的环境里把模型接进去。
- **权限是审核制，endpoint 也是专用的。** Daybreak Red 和 Blue 都要先申请 Daybreak Access，批下来之后从 Amazon Bedrock 控制台或者 Responses API 走 `bedrock-mantle` endpoint 调。
- **接着今年早些时候那步走。** OpenAI 的前沿模型和 Codex 今年早些时候就已经在 AWS 全面开放了，这次 Daybreak 上 Bedrock 被摆在同一条合作线的下一步。
