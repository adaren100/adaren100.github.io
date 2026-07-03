---
title: "More details on Fable 5's cyber safeguards and our jailbreak framework"
date: 2026-07-03
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[More details on Fable 5's cyber safeguards and our jailbreak framework](https://www.anthropic.com/news/fable-safeguards-jailbreak-framework)** — _Anthropic · Jul 1_

**Main takeaway:** With Claude Fable 5 re-deployed and available globally again, Anthropic published a detailed list of what its cyber safety classifiers do and don't block, plus an early draft of a jailbreak severity framework developed with Project Glasswing partners — intended to give AI developers and governments a consistent vocabulary for how dangerous a given jailbreak is.

**Main methods:**
- **Four-category classifier taxonomy.** Rather than blocking all cybersecurity activity, Fable 5's classifiers are trained to discern between four categories of cyber use, from the most clearly potentially dangerous to the most clearly potentially benign — because the domain is dual use (codebase vulnerability scanning helps defenders but could also be an attack precursor).
- **A deliberately enlarged safety margin.** The low-risk dual-use category overlaps heavily with the "safety margin" from the redeployment post: benign uses Anthropic would prefer to allow but blocks out of caution. A request has to look very clearly safe to avoid triggering the classifier, and for Fable 5 this margin was made larger than for previous models.
- **Jailbreak severity framework (first draft).** Jailbreaks range from unblocking minor undesirable behaviors to unblocking wide ranges of harmful outputs, yet no agreed-upon severity standard exists. The proposed framework would let AI developers and governments discuss each jailbreak's risk in consistent terms.
- **Open call for feedback.** The framework is explicitly a discussion starter across academia, industry, civil society, and government; critique is welcomed at cyber-safeguards@anthropic.com.
- **HackerOne program.** Security researchers can now submit potential cyber jailbreaks they discover in Fable 5 for Anthropic's review.
- **Classifiers are one layer of several.** Alongside classifiers, Anthropic uses access controls, model safety training, and offline monitoring as additional safeguards.

**[Fable 5 的 cyber safeguard 细节和 jailbreak 严重度框架初稿](https://www.anthropic.com/news/fable-safeguards-jailbreak-framework)** — _Anthropic · 7月1日_

**Main takeaway:** Claude Fable 5 重新上线、全球恢复访问之后，Anthropic 顺势公布了两样东西：一份详细清单，说明他们的 cyber safety classifier 到底拦什么、不拦什么；还有一份和 Project Glasswing 合作方一起起草的 jailbreak 严重度框架初稿，目标是让 AI 开发者和政府在谈论某个 jailbreak 有多危险时，能用上一套统一的语言。

**Main methods:**
- **classifier 按四档分类。** Fable 5 并不是一刀切把所有网络安全相关的活动全拦掉，而是把 cyber 用途分成四档来判断，从最明显危险到最明显无害。原因是这个领域天然 dual use：扫代码库找 vulnerability 对防守方是刚需，落到坏人手里却可能是攻击的前奏。
- **safety margin 刻意加大了。** 低风险 dual use 这一档和之前重新上线那篇文章里讲的 safety margin 高度重叠：很多本来无害、Anthropic 也愿意放行的用途，出于谨慎还是先拦下。一个请求得看起来非常明确地安全，才不会触发 classifier；Fable 5 的这道 margin 比以前的模型都更宽。
- **jailbreak 严重度框架（初稿）。** jailbreak 的危害差别很大，有的只是解锁一些小毛病，有的能放开一大片有害输出，但业界至今没有一套公认的严重度标准。这个框架就是想补上这个空缺，让开发者和政府能用统一的等级来沟通每个 jailbreak 的风险。
- **公开征求意见。** Anthropic 明说这只是当前思路，希望学界、业界、civil society 和政府一起来讨论这些线该怎么划，反馈可以发到 cyber-safeguards@anthropic.com。
- **HackerOne 项目。** 安全研究人员现在可以把在 Fable 5 上发现的潜在 cyber jailbreak 提交给 Anthropic 审核。
- **classifier 只是其中一层。** 除了 classifier，Anthropic 还叠加了 access control、模型安全训练和离线监控这几道 safeguard。
