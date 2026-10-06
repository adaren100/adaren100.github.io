---
title: "Expanding the Cyber Verification Program"
date: 2026-10-06
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[Expanding the Cyber Verification Program](https://www.anthropic.com/news/cyber-verification-program)** — _Anthropic · Oct 6_

**Main takeaway:** A program announcement: Anthropic is folding Project Glasswing and the old Cyber Verification Program into one expanded CVP with three access tiers, each giving vetted security professionals reduced blocking classifiers plus Claude Opus 5.5, Claude Sonnet 5.5, and Claude Mythos 5.1. Verification requirements and security controls scale with the tier.

**Main methods:**
- **Two programs merged into one.** For the past six months Project Glasswing (Claude Mythos for organizations securing the most critical software) and the CVP (reduced safeguards on Opus and Sonnet for vetted security teams) ran separately; they are now a single tiered offering aimed at reaching more security organizations.
- **Why gating exists at all.** Cyber work is inherently dual use, so generally available models like Claude Opus 5.5, Claude Fable 5.1, and Claude Sonnet 5.5 keep conservative cyber safeguards that block most cyber work, while Anthropic keeps working to cut false positives for secure coding.
- **Defense Access tier.** Covers SOC and incident-response tasks, reverse-engineering malware, and analyzing and validating vulnerabilities. Eligible applicants include security teams at companies, nonprofits, universities and government bodies defending systems they own, critical-infrastructure operators of any size (regional hospitals, municipal utilities), smaller security firms, open-source maintainers, and individual researchers with a vulnerability-reporting track record; Anthropic aims to respond within a few days.
- **Red Team Access tier.** Adds authorized penetration testing and red-teaming for in-house, government, and commercial red teams, restricted to systems the applicant is authorized to test. Review takes a few weeks, applicants sit in Defense Access while they wait, and the tier is currently open to organizations only.
- **Hard blocks stay in place.** Even in the red-team tier, users still hit real-time blocks on actions that could cause physical harm or mass disruption, such as deploying ransomware, damaging physical systems, or pen testing high-risk safety systems.
- **Caveat on this summary.** The fetched article text cut off partway through the Red Team tier description, so details of the third access tier are not covered here; the application link is in the post.

**[Anthropic 把 Cyber Verification Program 扩成三档](https://www.anthropic.com/news/cyber-verification-program)** — _Anthropic · 10月6日_

**Main takeaway:** 一则项目公告。Anthropic 把 Project Glasswing 和原来的 Cyber Verification Program 合并成了一个扩容版 CVP，分三档接入，每一档都给过审的安全从业者放宽 blocking classifier，并开放 Claude Opus 5.5、Claude Sonnet 5.5 和 Claude Mythos 5.1。档位越高，verification 要求和安全管控也跟着加码。

**Main methods:**
- **两个项目并成一个。** 过去半年 Project Glasswing（给守着最关键软件的那批机构开 Claude Mythos）和 CVP（给过审的安全团队放宽 Opus、Sonnet 的 safeguard）是分开跑的，现在合成一套分档方案，想覆盖更多安全机构。
- **为什么要设门槛。** 网络安全天生就是 dual use，找漏洞和修漏洞用的是同一套能力，所以公开版模型比如 Claude Opus 5.5、Claude Fable 5.1、Claude Sonnet 5.5 都带着比较保守的 cyber safeguard，基本把大部分 cyber 工作都拦掉了，同时他们还在想办法降低 secure coding 场景的 false-positive rate。
- **Defense Access 档。** 对着防守侧的活儿：SOC 和 incident response、逆向分析 malware、分析和验证 vulnerability。能过的大致包括企业、非营利、高校和政府里守自己系统的安全团队，各种规模的关键基础设施运营方（小到地区医院、市政水电），小型安全公司，开源 maintainer，以及有漏洞上报记录的个人研究者。Anthropic 说这一档几天内就会回。
- **Red Team Access 档。** 在防守之外加上授权范围内的 pen-testing 和 red-teaming，面向企业自建红队、政府红队和做渗透测试的安全公司，但只能打自己有授权的系统。审核要几周，等的期间先放进 Defense Access，而且这一档目前只对机构开放。
- **该拦的还是拦。** 就算进了红队这一档，碰到可能造成人身伤害或者大范围瘫痪的操作还是会被实时拦下来，比如投放 ransomware、搞坏物理设备，或者去 pen test 高风险的安全系统。
- **这篇总结的一个 caveat。** 抓到的正文在 Red Team 那一档说明中间就断了，所以第三档的具体内容这里没写。申请入口在原文里。
