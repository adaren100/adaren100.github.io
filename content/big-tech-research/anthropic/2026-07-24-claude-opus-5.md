---
title: "Introducing Claude Opus 5"
date: 2026-07-24
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[Introducing Claude Opus 5](https://www.anthropic.com/news/claude-opus-5)** — _Anthropic · Jul 24_

**Main takeaway:** Claude Opus 5, released today, reaches near-frontier intelligence (close to Fable 5) at half the price, setting new state-of-the-art on coding and knowledge-work evals like Frontier-Bench and GDPval-AA, while still trailing Mythos 5 on cybersecurity tasks. It's now the default model on Claude Max and the strongest model on Claude Pro.

**Main methods:**
- **Same cost, far higher performance.** Opus 5 costs the same as Opus 4.8 but more than doubles its Frontier-Bench v0.1 score at a lower cost per task.
- **Near-Fable performance at half the price.** On CursorBench 3.2 at max effort it lands within 0.5% of Fable 5's peak score at half the cost per task, and beats every model on cost-efficiency at high/xhigh/max effort settings.
- **Strong gains on novel-problem and agentic benchmarks.** Scores 3x the next-best model on ARC-AGI 3, and about 1.5x the pass rate of the next-best model on Zapier AutomationBench at equal cost — even its lowest effort setting beats every other model.
- **Computer-use leadership.** On OSWorld 2.0 it outperforms every model at any given cost, beating Fable 5's best result at just over a third of the cost.
- **Life-sciences gains.** Improves on Opus 4.8 across every internal life-sciences eval, with the largest jumps on organic chemistry (+10.2pp on inferring molecular structure from spectroscopy data) and protein-function prediction (+7.7pp).
- **Better self-verification and iteration.** Given a machine-part drawing but no way to directly view it, Opus 5 wrote its own computer-vision pipeline to extract geometry from raw pixels and rebuilt the part in FreeCAD — succeeding repeatedly where no competing model solved it in five attempts.

**[Claude Opus 5 正式发布](https://www.anthropic.com/news/claude-opus-5)** — _Anthropic · 7月24日_

**Main takeaway:** Anthropic 今天发布 Claude Opus 5，智能水平已经很接近 Fable 5 这个frontier档位，价格却只要一半。在 Frontier-Bench、GDPval-AA 这类coding和knowledge work的eval上它是新的SOTA，不过在cybersecurity任务上还是不如 Mythos 5。现在它是 Claude Max 的默认模型，也是 Claude Pro 里最强的选项。

**Main methods:**
- **同样的价格，性能翻倍不止。** Opus 5 定价和 Opus 4.8 一样，但在 Frontier-Bench v0.1 上的分数是 Opus 4.8 的两倍多，每个任务的成本还更低。
- **逼近 Fable 的水准，价格却砍半。** 在 CursorBench 3.2 上开 max effort，跑分离 Fable 5 的巅峰成绩只差 0.5%，但成本只要一半；在 high、xhigh、max 这几档 effort 上，它的性价比都超过所有其他模型。
- **新颖问题和agentic任务上进步明显。** ARC-AGI 3 上的分数是第二名的三倍；在 Zapier AutomationBench 上，同样成本下通过率大约是第二名的 1.5 倍，就算开最低 effort 也比其他所有模型强。
- **computer use 领跑。** 在 OSWorld 2.0 上，不管什么成本档位它都跑赢所有对手，用不到三分之一的成本就超过了 Fable 5 的最好成绩。
- **生命科学类任务全面提升。** 在所有内部 life sciences eval 上都比 Opus 4.8 强，涨幅最大的是有机化学（从光谱数据推断分子结构，提升 10.2 个百分点）和蛋白质功能预测（提升 7.7 个百分点）。
- **自我验证和迭代能力更强。** 给它一张机械零件的手绘图，却不让它直接"看"图，Opus 5 自己写了一套计算机视觉 pipeline 从像素里提取几何信息，再在 FreeCAD 里把零件重建出来，反复尝试都能成功，换其他模型跑五次都做不到。
