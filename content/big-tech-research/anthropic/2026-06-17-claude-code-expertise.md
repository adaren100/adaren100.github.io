---
title: "Agentic coding and persistent returns to expertise"
date: 2026-06-17
draft: false
tags: ["Anthropic", "research", "big-tech-research"]
source_org: "Anthropic"
source_url: "https://www.anthropic.com/research/claude-code-expertise"
---

**[Agentic coding and persistent returns to expertise](https://www.anthropic.com/research/claude-code-expertise)** — _Anthropic · Jun 16_

**Main takeaway:** A privacy-preserving analysis of ~400,000 Claude Code sessions from ~235,000 users (Oct 2025–Apr 2026) finds a stable division of labor — people decide *what* to build, Claude decides *how* — and that domain expertise (not coding proficiency) is what amplifies effective use. Over the seven months, debugging's share of sessions roughly halved while end-to-end agentic use grew, and the estimated value of a typical task rose ~25%.

**Main methods:**
- **Framework for studying interactive agentic coding.** Categorizes each session by composition of tasks, who makes planning vs. execution decisions, and whether the session ends in verifiable success (passing tests, committed work, etc.). Covers CLI, Claude.ai, and Claude Code desktop usage.
- **Division of labor finding.** Users typically own planning decisions, Claude owns execution; the higher a user's domain expertise, the more work Claude does per instruction.
- **Cross-occupation success rates.** On coding tasks, every major occupation succeeds at nearly the same rate as software engineers on average, suggesting the tool is broadly usable beyond formal coders.
- **Expertise gap is modest.** Domain experts succeed more often and recover from errors more easily than intermediates, but the gap between intermediate and expert is small — proficiency, not deep mastery, is enough.
- **Usage shift over seven months.** Debugging share of sessions fell by nearly half; usage moved toward end-to-end agentic work — deploying and running code, analyzing data, writing non-code documents.
- **Task value rose ~25%.** Estimated by comparison to freelance job postings; the value of the typical task rose in almost every kind of work over the observation window. Claude Code users now average 20 hours/week with the tool, and the share of GitHub projects with coding-agent activity has more than doubled since late 2025.

**[Agentic coding 的回报，正在向"领域专家"倾斜](https://www.anthropic.com/research/claude-code-expertise)** — _Anthropic · 6月16日_

**Main takeaway:** Anthropic 用 privacy-preserving 的方式分析了 2025 年 10 月到 2026 年 4 月之间约 40 万次 Claude Code session（约 23.5 万用户），发现一个挺稳定的分工：人决定"做什么"，Claude 决定"怎么做"。真正放大工具效用的是 domain expertise，而不是写代码本身的熟练度。七个月里，debugging 占 session 的比例几乎砍了一半，end-to-end 的 agentic 用法上来了，典型任务的估算价值也涨了大概 25%。

**Main methods:**
- **一套研究 interactive agentic coding 的框架。** 按任务构成、planning 和 execution 谁来拍板、以及 session 是否以 verifiable 的成功收尾（跑通测试、提交代码等）来分类。覆盖 CLI、Claude.ai 和 Claude Code 桌面端。
- **分工模式很清楚。** 用户主要管 planning，Claude 主要管 execution；用户在该领域越懂行，Claude 每条指令能做的活就越多。
- **跨职业的成功率。** 在 coding 任务上，几乎所有主要职业的成功率跟软件工程师差不多，说明这个工具对非正式 coder 也已经能用得起来。
- **expert 和 intermediate 的差距不大。** domain expert 成功率更高，遇到错误也更容易救回来；但跟 intermediate 用户的 gap 其实挺小——熟悉这个领域就够用了，不必是顶尖专家。
- **七个月里使用方式的变化。** debugging 占比几乎减半，重心转向 end-to-end 的 agentic 用法——部署和运行代码、做数据分析、写非代码文档都明显多了。
- **任务价值大约涨了 25%。** 通过对照 freelance 招聘的报价估算，几乎每一类工作的典型任务价值都涨了。Claude Code 用户现在平均每周用 20 小时，有 coding agent 活动的 GitHub 项目占比也比 2025 年底翻了一倍多。
