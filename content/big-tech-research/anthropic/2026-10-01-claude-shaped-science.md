---
title: "Claude-shaped science"
date: 2026-10-01
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[Claude-shaped science](https://www.anthropic.com/research/claude-shaped-science)** — _Anthropic · Oct 1_

**Main takeaway:** In a guest post following up on Vibe Physics, Prof. Matthew Schwartz describes stopping the fight to make Claude work like a human scientist and instead hunting for "Claude-shaped" problems — ones that suit what current LLM tools actually do well. That shift produced BootLoops, an open-source toolkit for exact calculations in quantitative science that turned out to apply far outside high-energy theory.

**Main methods:**
- **Name the real failure mode: impedance mismatch.** Schwartz argues the models are brilliant but are not scientists — working like a human scientist is not what current LLMs do best, so most of what a researcher puts in never gets through. The fix is to look for problems where that mismatch is less acute rather than to push harder.
- **Why the headlines feel distant.** Most AI-for-science wins so far have been well-scoped applications of existing techniques, and many are in mathematics, the one field where a problem can be stated completely and an answer checked absolutely. Most of science is not like that.
- **BootLoops as a harness, not a model.** It started as an accessible suite of tools for mathematical physics that Claude built, then grew into software plus scientific protocols. Schwartz frames it as a harness for the LLM in the same sense that Claude Code or Claude Science is a harness for Claude, or Codex is for GPT, and it is open-source so it runs with whatever model you like.
- **"Claude-shaped" problems defined.** Once it had BootLoops, Claude kept spotting the same pattern: many fields have problems a known technique from mathematics, physics, or computer science would solve outright if anyone there knew it existed.
- **Followed the pattern out of his own field.** Schwartz took it from high-energy theoretical physics into geology, biology, economics, and linguistics, including connections to ecology and population genetics.
- **Domain experts were the missing piece.** The cross-field results were often technically correct but scientifically unremarkable at first, so he worked with domain experts to steer BootLoops toward questions those fields actually care about.

**[Claude 擅长什么形状的科学问题](https://www.anthropic.com/research/claude-shaped-science)** — _Anthropic · 10月1日_

**Main takeaway:** 这是 Matthew Schwartz 教授继 Vibe Physics 之后的第二篇客座文章。他说自己不再硬掰着让 Claude 按人类科学家的方式工作，转而去找那些"Claude 形状"的问题，也就是刚好配得上现在这代 LLM 长处的问题。顺着这条路他做出了 BootLoops，一个开源的、做精确计算的量化科学工具包，结果它能用的范围远远超出高能理论本身。

**Main methods:**
- **先把症结叫出名字：impedance mismatch。** 他的看法是模型很聪明，但它们不是科学家。按人类科学家那套方式干活并不是现在的 LLM 最擅长的事，所以研究者投进去的东西大半传不过去。解法不是更使劲推，而是去找 mismatch 没那么严重的问题。
- **为什么头条看着离自己很远。** 到目前为止 AI 做科学的成果大多是把已有技术用在界定清楚的问题上，而且很多集中在数学，因为数学是唯一能把问题完整写清楚、答案也能被绝对验证的领域。科学里大部分事情不长这样。
- **BootLoops 是个 harness，不是模型。** 一开始只是他让 Claude 搭的一套好上手的数学物理工具，后来长成了软件加科研流程。他的比喻是，BootLoops 对 LLM 来说就像 Claude Code 或 Claude Science 对 Claude、Codex 对 GPT 那样是个 harness。它开源，想配哪个模型都行。
- **"Claude 形状"的问题指什么。** 有了 BootLoops 之后，Claude 反复撞见同一个模式：很多领域里有些问题，数学、物理或计算机里现成的某个技术拿过来就能直接解决，只是那个领域里没人知道它存在。
- **顺着这个模式走出自己的地盘。** 他从高能理论物理一路走到地质、生物、经济和语言学，中间还牵出 ecology 和 population genetics 的联系。
- **缺的那一环是领域专家。** 跨领域出来的结果一开始常常是技术上没错但科学上不值一提，所以他拉上各领域的专家一起，把 BootLoops 往这些领域真正关心的问题上掰。
