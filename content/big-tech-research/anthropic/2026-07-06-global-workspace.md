---
title: "A global workspace in language models"
date: 2026-07-06
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[A global workspace in language models](https://www.anthropic.com/research/global-workspace)** — _Anthropic · Jul 5_

**Main takeaway:** New interpretability research finds that Claude has developed a small set of internal neural patterns — dubbed the "J-space" — that function like a consciously-accessible mental workspace, distinct from the rest of the model's processing.

**Main methods:**
- **J-space discovery.** Found via a technique built on the Jacobian, this is a small collection of internal neural patterns, each linked to a particular word; when one lights up, it means the concept is "on the model's mind," not that the model is about to say it.
- **Distinct from chain-of-thought.** Unlike a written scratchpad, the J-space operates silently inside the model's internal activations, letting Claude think about a concept without writing it down — and it emerged on its own during training rather than being designed in.
- **Reportability.** Claude can accurately report what's currently active in its J-space when asked, whereas it's much worse at reporting on non-J-space internal representations.
- **On-demand modulation.** When asked to think about something or solve a problem silently, Claude lights up the corresponding J-space patterns; it struggles to deliberately modulate patterns outside the J-space.
- **Causal role in multi-step reasoning.** For problems requiring several steps, intermediate results light up in the J-space even when never stated aloud, and these patterns causally mediate task performance despite being smaller in magnitude than other representations.
- **Flexible, theory-inspired.** J-space content (e.g. "France") can be flexibly reused across tasks (recalling its capital, currency, continent), and blocking J-space use leaves fluent, grammatical speech intact but destroys higher-order cognitive function — echoing neuroscience's global workspace theory of consciousness.

**[语言模型里的"全局工作空间"](https://www.anthropic.com/research/global-workspace)** — _Anthropic · 7月5日_

**Main takeaway:** Anthropic 最新的可解释性研究发现，Claude 内部长出了一小撮神经模式——他们管它叫 "J-space"——功能上很像人类意识里那个可以被自己察觉、调用的"心理工作台"，跟模型其他部分的处理明显不一样。

**Main methods:**
- **J-space 是怎么找到的。** 用一种基于 Jacobian（雅可比矩阵）的技术找出来的一小撮内部神经模式，每个都和某个具体的词挂钩；某个模式亮起来，不代表模型马上要说这个词，只是说明这个概念"在它心里"。
- **跟 chain-of-thought 不是一回事。** 普通的草稿本是写出来的文字，J-space 不一样，它悄悄地在模型内部激活里运作，让 Claude 能想一个概念但不用写下来；而且这东西不是 Anthropic 设计出来的，是训练过程中自己长出来的。
- **可以被"汇报"。** 问 Claude 它在想什么，它能比较准确地说出 J-space 里正亮着的内容；但对 J-space 之外的内部表征，它汇报得就差很多。
- **可以按要求调用。** 让 Claude 去想某件事，或者在心里默默解题，它就会点亮对应的 J-space 模式；反过来，J-space 之外的模式它很难主动去调控。
- **在多步推理里起因果作用。** 做需要好几步的题目时，中间结果会在 J-space 里亮起来，哪怕从没说出口，而且这些模式对任务表现有因果性的影响，尽管它们的量级比其他表征要小。
- **用法灵活，还呼应了神经科学理论。** J-space 里的内容（比如"France"）可以灵活复用去做很多任务，比如接着推出它的首都、货币、所在大陆；如果把 J-space 屏蔽掉，Claude 说话还是流畅语法正确，但高阶认知功能就没了——这跟神经科学里解释意识的"全局工作空间理论"（global workspace theory）正好对上。
