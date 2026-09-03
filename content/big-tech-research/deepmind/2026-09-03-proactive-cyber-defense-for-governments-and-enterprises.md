---
title: "Proactive cyber defense for governments and enterprises"
date: 2026-09-03
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Proactive cyber defense for governments and enterprises](https://deepmind.google/blog/proactive-cyber-defense-for-governments-and-enterprises/)** — _Google DeepMind · Sep 3_

**Main takeaway:** Google is launching the Fairwind Program, a limited-access program that puts Gemini 3.8 Flash Cyber plus the CodeMender harness in the hands of governments, critical-infrastructure operators, and Google Cloud security partners so they can autonomously find and patch vulnerabilities. More than 650 partners are already participating globally.

**Main methods:**
- **Gemini 3.8 Flash Cyber paired with the CodeMender harness.** The pitch is the full loop rather than just detection: find, verify, and fix at agentic scale, with the model writing and validating code fixes so defenders get verified, deployment-ready patches in minutes instead of weeks of manual work.
- **Framed against a cost/control dilemma.** Google's setup is that defenders previously had to choose between huge frontier models that are expensive to run and hard to control across enterprise codebases, or smaller open-weight models that struggle with real remediation and force teams to build their own tooling from scratch.
- **Runs inside the customer's own secure cloud environment.** Patch generation happens within the organization's environment, and Google stresses the specialized reasoning comes at a fraction of the operating cost of traditional frontier models.
- **Access is staged by societal criticality.** Three tiers named: governments and national cyber authorities hardening public-sector networks, critical-infrastructure operators across healthcare, telecoms, energy and finance, and core technology platforms whose security propagates to millions of downstream users.
- **Misuse controls are contractual, not technical.** Participants agree to strict operational standards: access limited to employees on internal cybersecurity, incident response, or penetration testing teams, plus protections like multi-factor authentication.
- **The "adaptation window" argument.** Google's stated rationale for restricted early access is giving trusted defenders time to harden systems before attackers reach comparable capability. Note that the post carries no benchmark numbers for Flash Cyber, and the partner list and partner quotes weren't captured in the extracted body.

**[Fairwind Program：把最强的攻防能力先发给防守方](https://deepmind.google/blog/proactive-cyber-defense-for-governments-and-enterprises/)** — _Google DeepMind · 9月3日_

**Main takeaway:** Google 推出 Fairwind Program，一个限量准入的项目，把 Gemini 3.8 Flash Cyber 加上 CodeMender harness 交给政府机构、关键基础设施运营方和 Google Cloud 的安全合作伙伴，让他们自己去自动挖漏洞、自动修。目前全球已经有 650 多家参与方。

**Main methods:**
- **Gemini 3.8 Flash Cyber 配 CodeMender harness。** 卖点不是"能扫出漏洞"，而是整条链路跑通：find、verify、fix 全部在 agentic 规模上做，模型自己写 patch 自己验证，原本要人肉修好几周的东西，几分钟就能拿到可直接上线的 patch。
- **对着一个成本和可控性的两难来讲故事。** Google 的铺垫是：防守方以前只有两个选择，要么上巨大的 frontier 模型，贵而且在企业级 codebase 里不好管；要么用小的 open-weight 模型，复杂漏洞修不动，工具链还得自己从零搭。
- **跑在客户自己的安全云环境里。** patch 生成整个过程留在组织内部环境，Google 特别强调这套专精 reasoning 的运行成本只有传统 frontier 模型的一个零头。
- **准入按"对社会有多关键"分批放。** 点名了三类：政府和国家级网络安全机构，负责加固公共部门网络和民生服务；医疗、电信、能源、金融这些关键基础设施运营方；以及底层技术平台，因为它们一加固，下游几百万用户跟着受益。
- **防滥用靠的是合同条款，不是技术手段。** 参与方要签一套严格的操作规范，比如只允许内部 cybersecurity、incident response、pen-testing 团队的员工使用，还得部署 multi-factor authentication 之类的保护。
- **所谓"适应窗口"的逻辑。** Google 给出的理由是先放给可信防守方，让他们在攻击者拿到同等能力之前把系统加固好。有一点要说，这篇没给 Flash Cyber 的任何 benchmark 数字，合作方名单和引述在抓取到的正文里也没体现出来。
