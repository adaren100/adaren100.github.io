---
title: "Expanding Daybreak as the Cyber Defense Window Narrows"
date: 2026-08-10
draft: false
tags: ["big-tech-research", "openai"]
---

**[Expanding Daybreak as the Cyber Defense Window Narrows](https://openai.com/index/expanding-daybreak-as-the-cyber-defense-window-narrows)** — _OpenAI · Aug 10_

**Main takeaway:** OpenAI is splitting its Daybreak security program into two access tiers and shipping GPT-5.6-Cyber, a cybersecurity-specific model built on GPT-5.6 Sol that completes 95.0% of requests on an internal refusal eval versus 1.5% for stock GPT-5.6 Sol.

**Main methods:**
- **Two access tiers.** Daybreak Blue gives approved defenders frontier general-purpose models including GPT-5.6 Sol with the production cyber screening removed — pitched as the starting point for vulnerability discovery, secure code review, malware analysis, incident response, and patch validation. Daybreak Red adds purpose-trained cyber models for authorized vulnerability research, exploit validation, and security testing.
- **GPT-5.6-Cyber.** Built on GPT-5.6 Sol and trained both to do better on specialized tasks (finding zero-day vulnerabilities, developing exploit chains) and to refuse less on higher-risk dual-use cyber work.
- **Advanced Cybersecurity Completion Rate.** An internal eval measuring how often a model answers requests involving exploit-chain development, authentication bypass, privilege escalation, and similar scenarios. GPT-5.6-Cyber completes 95.0%, GPT-5.5-Cyber 57.3%, GPT-5.6 Sol on Daybreak Blue 2.0%, and stock GPT-5.6 Sol 1.5%.
- **Guardrails were blocking real work.** OpenAI says its production system-level screening of cyber requests also blocks legitimate defensive work, which is exactly what Blue removes; even without those guardrails Sol still refuses hard dual-use prompts like pentesting production systems, which is what Red addresses.
- **The 57.3% number is a response to researcher feedback.** GPT-5.5-Cyber's persistent refusals were a complaint from security researchers, and the new model's completion rate is presented as the fix.
- **Framing: a narrowing defense window.** The stated rationale is getting frontier capability to trusted defenders before attackers deploy offensive AI at scale, including fully autonomous attacks. The post shows the same prompts (e.g. a macOS tool that bypasses Keychain prompts and decrypts Chrome cookies) answered across all four configurations.

**[Daybreak 扩容，顺带放出专做安全的 GPT-5.6-Cyber](https://openai.com/index/expanding-daybreak-as-the-cyber-defense-window-narrows)** — _OpenAI · 8月10日_

**Main takeaway:** OpenAI 把 Daybreak 这个安全项目拆成了两档权限，同时发了 GPT-5.6-Cyber：一个基于 GPT-5.6 Sol 训的安全专用模型，在内部那套测拒答率的 eval 上完成了 95.0% 的请求，而原版 GPT-5.6 Sol 只有 1.5%。

**Main methods:**
- **两档权限。** Daybreak Blue 给通过审核的防守方开放前沿通用模型（包括 GPT-5.6 Sol），把线上那层安全类请求的筛查拿掉，官方推荐大多数人从这档开始，覆盖漏洞挖掘、secure code review、恶意样本分析、incident response、patch 验证。Daybreak Red 再往上，给的是专门训过的安全模型，用于授权范围内的 vulnerability research、exploit 验证和安全测试。
- **GPT-5.6-Cyber。** 底子是 GPT-5.6 Sol，一方面把找 zero-day、写 exploit chain 这类专项能力练上去，另一方面专门降低高风险 dual-use 场景下的拒答。
- **Advanced Cybersecurity Completion Rate。** 内部自建的 eval，测模型面对 exploit chain 开发、认证绕过、提权这类请求时到底肯不肯答。GPT-5.6-Cyber 完成 95.0%，GPT-5.5-Cyber 57.3%，走 Daybreak Blue 的 GPT-5.6 Sol 只有 2.0%，原版 Sol 1.5%。
- **guardrail 确实误伤了正经活。** OpenAI 自己承认，线上那套安全请求筛查在防滥用的同时也拦掉了不少合法的防守工作，Blue 这档就是为了把它拿掉。但就算没有系统层 guardrail，Sol 碰上"给生产系统做 pen-testing"这种硬 dual-use 请求照样会拒，所以才有了 Red。
- **57.3% 这个数字是回应研究员的抱怨。** 之前不少安全研究员反馈 GPT-5.5-Cyber 老是拒答，新模型的完成率就是拿来对照的答复。
- **叙事是"防守窗口在收窄"。** 官方的逻辑是趁攻击方还没大规模用上进攻型 AI（包括全自动攻击）之前，先把前沿能力交到可信的防守方手里。文章里还并排展示了同一批安全 prompt（比如"写个绕过 macOS Keychain 弹窗、解密 Chrome cookie 的工具"）在四种配置下分别怎么答。
