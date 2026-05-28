+++
date = '2026-03-27T12:45:00+11:00'
draft = false
title = 'ACE: Let Models Write Their Own Playbook'
+++

![ACE Framework](/images/ace-framework.png)

## 主菜

ACE，全称 Agentic Context Engineering，是一个通过上下文积累而不是参数更新来改进模型表现的框架。

它的核心做法是让模型在完成任务的过程中，把有用的经验写进一份 `playbook`。

`playbook` 可以理解成一份持续演化的任务手册。模型在后续推理时会再次读取这份手册，因此新的经验可以被后面的样本复用。

整个流程分成三个角色：

- `Generator` 负责带着现有的 playbook 去回答问题。
- `Reflector` 负责回头看这一轮尝试，判断什么地方有帮助，什么地方出了错。
- `Curator` 负责把这次得到的经验整理成一条简短的笔记，放回 playbook。

因此，ACE 做的不是重新训练模型，而是通过 `生成 -> 反思 -> 整理` 的循环，让模型积累一份越来越有针对性的上下文知识。

## 例子

假设模型正在读一段财报，它看到这样一句话：

> Aggregate borrowings of $29.6 million were denominated in British pounds.

现在，它需要判断这个数字应该对应什么财务标签。

第一轮里，模型可能会答错，例如把这个金额误判成费用。

这时 Reflector 会分析这次错误，并提取出真正有用的线索。

例如，它可能会发现，模型过度关注了“这是一个金额”，却忽略了周围的关键词。像 `borrowings`、`debt`、`outstanding` 这样的词，更像是在描述债务本金，而不是费用。

Curator 随后会把这个经验写进 playbook，供后面的题继续使用。

## 初始 Playbook

在最开始的时候，playbook 几乎是空的。

它通常从几个栏目开始：

- `STRATEGIES & INSIGHTS`
- `FORMULAS & CALCULATIONS`
- `CODE SNIPPETS & TEMPLATES`
- `COMMON MISTAKES TO AVOID`
- `PROBLEM-SOLVING HEURISTICS`
- `CONTEXT CLUES & INDICATORS`
- `OTHERS`

这个时候，里面还没有真正的经验内容，只有分类结构。

后续新增的内容会被放到这些栏目中的某一个下面。

## 这个案例之后

经历了刚才那个 borrowing 的例子之后，playbook 就不再是空的了。

它里面可能会开始出现这样的笔记：

- 当句子里出现 `borrowings`、`debt` 或 `outstanding` 这些词时，更可能是在描述债务本金，而不是费用。
- 不要因为一个数字以金额形式出现，就默认它对应 expense。

这些内容会直接影响下一次类似问题的推理。

当模型以后再看到类似的句子时，Generator 会先读取 playbook，再基于这些经验作答。

这样，一次错误就不只是一次失败，而会被转化成后续可复用的结构化知识。

这也是 ACE 的核心：不是让模型“凭空变强”，而是让模型把经验沉淀成 playbook，并在后续任务中继续使用。

## Main Course

ACE, short for Agentic Context Engineering, is a framework that improves model performance through context accumulation rather than parameter updates.

Its core idea is to let the model write useful experience into a `playbook` while solving tasks.

The `playbook` is an evolving task manual. The model reads it again in later steps, so lessons from earlier cases can be reused on future ones.

The workflow has three roles:

- The `Generator` answers the current question using the existing playbook.
- The `Reflector` looks back at the attempt and judges what helped and what went wrong.
- The `Curator` turns that lesson into a short note and files it into the playbook.

So ACE does not improve the model by retraining it. It improves the task context through a `generate -> reflect -> curate` loop.

## Example

Imagine the model is reading a financial filing and sees a sentence like this:

> Aggregate borrowings of $29.6 million were denominated in British pounds.

The model needs to decide what financial tag should be assigned to that number.

In the first round, the model may answer incorrectly and treat the amount as an expense.

The Reflector then analyzes the error and extracts the useful signal behind it.

For example, it may find that the model focused too much on the fact that the sentence contains money, while ignoring surrounding words such as `borrowings`, `debt`, and `outstanding`, which are stronger signals for debt principal than expense.

The Curator then writes that lesson into the playbook for later reuse.

## Initial Playbook

At the beginning, the playbook is almost empty.

It starts with section headers such as:

- `STRATEGIES & INSIGHTS`
- `FORMULAS & CALCULATIONS`
- `CODE SNIPPETS & TEMPLATES`
- `COMMON MISTAKES TO AVOID`
- `PROBLEM-SOLVING HEURISTICS`
- `CONTEXT CLUES & INDICATORS`
- `OTHERS`

At this stage, there are no actual lessons yet, only a category structure.

New entries are added under one of these sections as the system processes more cases.

## After The Case

After the borrowing example, the playbook is no longer empty.

Now it may contain notes like these:

- When words like `borrowings`, `debt`, or `outstanding` appear, the sentence is more likely describing debt principal than expense.
- Do not classify a number as expense just because it is written as a dollar amount.

These entries directly affect future reasoning on similar cases.

When a similar sentence appears again, the Generator reads the playbook first and can use those stored lessons during inference.

In this way, one error becomes reusable structured knowledge.

That is the core of ACE: not making the model improve “by itself,” but letting it turn experience into a playbook and reuse that playbook later.
