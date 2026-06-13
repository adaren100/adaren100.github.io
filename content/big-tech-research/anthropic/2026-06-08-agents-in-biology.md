---
title: "Paving the way for agents in biology"
date: 2026-06-08
draft: false
tags: ["Anthropic", "research", "big-tech-research"]
source_org: "Anthropic"
source_url: "https://www.anthropic.com/research/agents-in-biology"
---

**[Paving the way for agents in biology](https://www.anthropic.com/research/agents-in-biology)** — _Anthropic · Jun 7_

**Main takeaway:** When tasked with retrieving sequence data from NCBI Virus, even the strongest scientific agents (Claude, Biomni OSS, Edison Analysis, GPT) failed to consistently meet the accuracy bar for reliable dataset construction — but accuracy jumped to nearly 100% once the team added gget virus, a deterministic retrieval layer. The lesson: biological data infrastructure needs to be redesigned with agents as first-class users.

**Main methods:**
- **The case study.** Multiple frontier scientific agents asked to pull virus sequence data from NCBI Virus (used by virologists for surveillance and diagnostic assay development). Top models still made errors that would invalidate downstream science.
- **Why the failures matter.** Biology errors compound: wrong genome build, mixing RefSeq with GenBank records, treating partial as complete genomes, mis-identifying segment names in segmented viruses, or missing records due to inconsistent metadata.
- **The fix: deterministic retrieval.** Adding gget virus, a deterministic retrieval tool, pushed accuracy to ~100%. The point isn't smarter agents alone — it's that scientific agent workflows need deterministic execution layers underneath reasoning.
- **Why biology is harder than software.** Software has clear APIs, package managers, version control, and testable outputs (e.g., resolving a GitHub issue with a passing patch). Biology has idiosyncratic file formats, scattered databases, one-off retrieval scripts, and few simple verifiable rewards.
- **The structural ask.** Biological databases need to be designed with agents in mind as scaled users — analogous to retrofitting an old city for cars vs. designing roads around them from the start.
- **Caveat.** Single-domain case study (NCBI Virus retrieval); broader claim about agent-friendly bio infrastructure is positioned as a research direction, not a benchmark result.

**[给生物领域的 agent 铺路](https://www.anthropic.com/research/agents-in-biology)** — _Anthropic · 6月7日_

**Main takeaway:** 让几个前沿科研 agent（Claude、Biomni OSS、Edison Analysis、GPT）从 NCBI Virus 拉病毒序列数据，结果即使是最强的模型也没法稳定达到可靠构建数据集所需的准确率——但只要给它套上 gget virus 这层确定性的 retrieval 工具，准确率立刻接近 100%。教训是：生物数据基础设施得重新设计，把 agent 当成一类正经用户。

**Main methods:**
- **case study。** 多个前沿科研 agent 被要求从 NCBI Virus 拉病毒序列数据（病毒学家做监测和诊断试剂开发都靠这个库）。最强的模型仍然会犯错，错了就会把下游研究污染掉。
- **为什么这些错很要命。** 生物里的错会累积：弄错了 genome build、把 RefSeq 和 GenBank 记录混着用、把部分基因组当完整基因组、segment 病毒里搞错 segment 名字、因为元数据字段不一致漏掉相关记录。
- **怎么修：确定性 retrieval。** 加一层 deterministic 检索工具 gget virus，准确率直接拉到 100% 附近。重点不是把 agent 做得更聪明，而是科研 agent workflow 需要在 reasoning 下面垫一层确定性执行层。
- **为什么生物比软件难。** 软件有清晰的 API、package manager、版本控制、可测试的输出（比如 GitHub issue 用过测试的 patch 解掉）；生物是各种古怪文件格式、零散数据库、一次性 retrieval 脚本，简单可验证的 reward 也少。
- **结构性的诉求。** 生物数据库需要把 agent 当作规模化用户来设计——就像给旧城改造让汽车通行，不如一开始就为汽车铺路。
- **需要注意的 caveat。** 单领域 case study（NCBI Virus 数据检索）；关于生物基础设施要为 agent 重新设计这个更大的论断，是研究方向的提议而不是 benchmark 结论。
