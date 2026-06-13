---
title: "Claude Fable 5 and Claude Mythos 5"
date: 2026-06-09
draft: false
tags: ["Anthropic", "research", "big-tech-research"]
source_org: "Anthropic"
source_url: "https://www.anthropic.com/news/claude-fable-5-mythos-5"
---

**[Claude Fable 5 and Claude Mythos 5](https://www.anthropic.com/news/claude-fable-5-mythos-5)** — _Anthropic · Jun 8_

**Main takeaway:** Anthropic launched Claude Fable 5 — a Mythos-class model made safe for general use — alongside Claude Mythos 5 for a small group of cyber defenders. Fable 5 is state-of-the-art on nearly all tested capability benchmarks, priced at $10/$50 per million input/output tokens (less than half of Mythos Preview).

**Main methods:**
- **Two-tier launch.** Same underlying model: Fable 5 has safeguards on (queries on sensitive topics route to Opus 4.8 — triggers in under 5% of sessions); Mythos 5 has them lifted for select cyberdefender / infrastructure partners through Project Glasswing with US government collaboration.
- **Capability claims.** Top on most benchmarks; the longer and more complex the task, the larger Fable 5's lead — clearest in software engineering, knowledge work, vision, scientific research, life sciences.
- **Software-engineering proof points.** Stripe reports Fable 5 compressed months of engineering into days on a 50M-line Ruby codebase migration; top scorer on Cognition's FrontierCode evaluation at medium effort.
- **Conservative safeguards.** Tuned to occasionally catch harmless requests in favor of catching misuse; Anthropic explicitly plans to reduce false positives as next-gen models arrive.
- **Pricing shift.** $10 input / $50 output per million tokens — under half the price of Claude Mythos Preview, framed as bringing frontier capability to more users faster.
- **Caveat.** This model is the one the US government later directed Anthropic to suspend access to for foreign nationals — see the Jun 11 Fable-Mythos access statement.

**[Claude Fable 5 和 Claude Mythos 5 发布](https://www.anthropic.com/news/claude-fable-5-mythos-5)** — _Anthropic · 6月8日_

**Main takeaway:** Anthropic 发布了 Claude Fable 5——一个 Mythos 级别但做了通用安全处理的模型，同时为一小撮 cyber defender 发布了 Claude Mythos 5。Fable 5 在几乎所有能力 benchmark 上都是 SOTA，价格 \$10/\$50 每百万 input/output token，不到 Mythos Preview 的一半。

**Main methods:**
- **两档发布。** 底层是同一个模型：Fable 5 带 safeguard（敏感话题的 query 会被路由给 Opus 4.8 回答，平均在不到 5% 的 session 里触发）；Mythos 5 在部分领域放开了 safeguard，通过 Project Glasswing 给特定 cyberdefender 和基础设施伙伴用，并和美国政府合作。
- **能力。** 多数 benchmark 第一，任务越长越复杂 Fable 5 的优势越明显——软件工程、知识工作、视觉、科研、生命科学最突出。
- **软件工程的实证。** Stripe 反馈 Fable 5 在一个 5000 万行的 Ruby 代码库迁移上把几个月的工作压到几天；在 Cognition 的 FrontierCode eval 上 medium effort 就拿了第一。
- **保守的 safeguard。** 宁可偶尔误伤无害请求也要拦住误用；Anthropic 明确说下一代模型出来时会降低 false-positive rate。
- **价格大幅下调。** \$10 input / \$50 output 每百万 token，比 Mythos Preview 便宜一半多，定位是把前沿能力更快带给更多用户。
- **需要注意的 caveat。** 这就是几天后美国政府要求 Anthropic 对所有 foreign national 切断访问的那个模型，详见 6 月 11 日的 Fable-Mythos access 声明。
