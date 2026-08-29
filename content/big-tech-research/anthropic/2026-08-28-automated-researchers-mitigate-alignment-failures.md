---
title: "Automated researchers can reliably mitigate alignment failures"
date: 2026-08-28
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[Automated researchers can reliably mitigate alignment failures](https://www.anthropic.com/research/automated-researchers-mitigate-alignment-failures)** — _Anthropic · Aug 28_

**Main takeaway:** Anthropic had Claude autonomously run the full alignment-research loop against 10 categories of alignment failure, each scored on public benchmarks. For all 10, Claude found fixes that improved the target benchmarks without degrading the student model's general capabilities.

**Main methods:**
- **A closed research loop, one failure category at a time.** Claude searched the literature, proposed methods and training data, trained, then tested — repeating per category. For privacy violation, the targets were ConfAIde, PrivaCI-Bench, and PrivacyLens.
- **Scored by "percentage of safety gap closed."** Success was measured as how far a method moved the student model toward the theoretical perfect score, judged across the three to five benchmarks covering each alignment failure.
- **A monitoring agent enforced the constraints.** Methods that hurt general capabilities were excluded, and Claude was forbidden from distilling its own alignment directly into the target model; the monitor read every method before it was run.
- **Generalization held across held-out evals and model size.** The best methods still worked on alignment benchmarks Claude never saw during the loop, and on Petri (Anthropic's open-source tool that simulates adversarial multi-turn scenarios), and remained effective on models up to 4.7× larger than those they were optimized for.
- **Claude outscored 28 human safety researchers.** Given up to eight hours each, the humans lost on deception by 20% to Claude's best method. Anthropic flags this as not a clean comparison — the humans couldn't iterate — and frames the result as a workflow where Claude surfaces promising methods for humans to refine.
- **Next test: a weaker model aligning a stronger one.** They tasked Claude Sonnet 5, which trails Claude Opus 4.8 on the Epoch Capabilities Index, with post-training a production-grade model for better alignment; the extracted body cuts off before the results.

**[让 Claude 自己做 alignment 研究：10 类 alignment failure 全部修掉](https://www.anthropic.com/research/automated-researchers-mitigate-alignment-failures)** — _Anthropic · 8月28日_

**Main takeaway:** Anthropic 让 Claude 自己跑完整套 alignment 研究流程，去修 10 类 alignment failure，每一类都有公开 benchmark 打分。10 类全部拿下，Claude 找到的方法都把目标 benchmark 推上去了，而且没有把 student model 的通用能力弄坏。

**Main methods:**
- **一个闭环研究流程，一次只啃一类。** Claude 先查文献，再提方法和训练数据，然后训练、测试，一类一类循环。比如 privacy violation 这类，打的就是 ConfAIde、PrivaCI-Bench、PrivacyLens 这几个 benchmark。
- **打分方式是"safety gap 关掉了多少"。** 看方法把 student model 往理论满分推进了多远，每类 alignment failure 通常拿三到五个 benchmark 一起判。
- **拿一个 monitoring agent 卡规则。** 两条硬约束：伤通用能力的方法不算数，也不许 Claude 把自己的 alignment 直接 distill 进目标模型。每个方案跑之前都得先过 monitoring agent 这一关。
- **换没见过的 eval、换更大的模型，都还站得住。** 表现最好的那批方法在研究过程中完全没见过的 alignment benchmark 上照样有效，在 Petri（Anthropic 那个模拟多轮对抗场景测 misalignment 的开源工具）上也扛得住，模型尺寸放大到 4.7 倍效果依然在。
- **跟 28 位人类 safety researcher 比，Claude 赢了。** 人类那边每人最多有 8 小时想方案，deception 这一类上 Claude 最好的方法比人类最好的高 20%。不过 Anthropic 自己也说这不算公平对比，人类没机会迭代，更合适的理解是 Claude 负责海选出有潜力的方法，人再往下打磨。
- **下一步是弱模型去 align 强模型。** 他们让 Claude Sonnet 5（在 Epoch Capabilities Index 上不如 Claude Opus 4.8）去给一个 production 级别的模型做 post-training，可惜抓到的正文到这儿就断了，结果没拿到。
