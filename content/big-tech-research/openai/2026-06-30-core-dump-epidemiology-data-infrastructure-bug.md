---
title: "Core dump epidemiology: fixing an 18-year-old bug"
date: 2026-06-30
draft: false
tags: ["big-tech-research", "openai"]
---

**[Core dump epidemiology: fixing an 18-year-old bug](https://openai.com/index/core-dump-epidemiology-data-infrastructure-bug)** — _OpenAI · Jun 30_

**Main takeaway:** OpenAI engineers used population-level "epidemiology" analysis of crash dumps to debug impossible-looking crashes in ChatGPT's Rockset data infrastructure, uncovering two completely unrelated bugs: silent CPU math corruption on one Azure host, and an 18-year-old race condition in the widely used GNU libunwind library.

**Main methods:**
- **Population-level diagnosis over case-by-case.** Instead of deeply examining a few core dumps (the "doctor" approach), the team built a high-quality dataset of the entire crash population and analyzed patterns across all of them — revealing what individual case examination missed.
- **The Rockset context.** Crashes occurred in Rockset, a C++ data service for ChatGPT that handles search connectors and conversation history search; C++'s lack of memory safety allowed subtle bugs to produce intermittent crashes.
- **Bug #1: silent hardware corruption.** One Azure host's CPU was silently computing math incorrectly; crashes only appeared when that specific host was involved, making the failures seem random and impossible to reproduce.
- **Bug #2: an 18-year-old libunwind race window.** GNU libunwind has a single-instruction race: when a C++ exception fires at exactly the wrong moment, it corrupts the %rsp stack pointer register, causing the function to return to a garbage address. This bug went undetected for ~18 years in a widely used open-source library.
- **Why both bugs appeared now.** The scale increase in ChatGPT's data infrastructure made previously theoretical race conditions observable in production for the first time.

**[用流行病学方法修掉一个 18 年的老 bug](https://openai.com/index/core-dump-epidemiology-data-infrastructure-bug)** — _OpenAI · 6月30日_

**Main takeaway:** OpenAI 工程师用"流行病学"思路，从整批 core dump 里找规律，破解了 ChatGPT 数据基础设施 Rockset 里一组看起来不可能发生的崩溃，最终发现是两个完全无关的 bug：一台 Azure 机器 CPU 悄悄算错了数，加上 GNU libunwind 里藏了 18 年的 race condition。

**Main methods:**
- **换思路：群体分析而不是逐案精读。** 不是把几个 crash 挨个深挖（"医生模式"），而是把所有崩溃攒成一个高质量数据集，在整个群体里找规律——这才看出了个案分析看不到的东西。
- **背景：Rockset 是什么。** Rockset 是 ChatGPT 数据基础设施里一套 C++ 搜索服务，负责 sync connector 和对话历史搜索；C++ 没有内存安全保障，偶发 bug 才能悄悄崩出来。
- **Bug #1：CPU 悄悄算错了。** 一台 Azure 机器的 CPU 在某些运算时会静默给出错误结果，只有这台机器参与时才会崩溃，所以复现极其随机。
- **Bug #2：libunwind 里藏了 18 年的 race window。** GNU libunwind 有一个单条指令的 race：C++ 异常恰好在错误时机触发，会破坏 %rsp 寄存器，导致函数返回到垃圾地址。这个 bug 在被广泛使用的开源库里藏了约 18 年没被发现。
- **为什么现在才暴露。** ChatGPT 数据基础设施的流量规模上来之后，原本只在理论上存在的 race 才第一次在生产环境里稳定可观测到。
