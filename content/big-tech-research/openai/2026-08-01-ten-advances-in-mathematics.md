---
title: "Ten advances in mathematics and theoretical computer science"
date: 2026-08-01
draft: false
tags: ["big-tech-research", "openai"]
---

**[Ten advances in mathematics and theoretical computer science](https://openai.com/index/ten-advances-in-mathematics)** — _OpenAI · Aug 1_

**Main takeaway:** OpenAI shared ten new results, each resolving or making substantial progress on a long-standing open problem in math and theoretical CS, produced by an internal version of Astra (OpenAI's next major model) at a total token cost of roughly $2,000.

**Main methods:**
- **Model-generated proofs across ten problems.** Spans high-dimensional geometry, coding theory, arithmetic circuit complexity, group theory, operator algebras, quantum complexity, lattice cryptography, and extremal combinatorics.
- **Cheap to produce.** All ten solutions together would cost roughly $2,000 in token spend at Sol API rates.
- **Human + model pipeline.** Humans worked with the same model to turn its arguments into manuscripts, then the model formalized each proof as a Lean certificate.
- **Notable individual results.** Includes a disproof of Connes's rigidity conjecture, a superexponential lower bound for multicolor triangle Ramsey numbers (Erdős problem 183), and resolutions of Erdős problems 146 and 180 in extremal graph theory.
- **Follow-up to earlier math work.** Builds on a May disproof of the Erdős unit-distance conjecture, found while evaluating an unreleased model, which OpenAI says has already spurred further research.
- **Narrated reasoning released.** For each solution, OpenAI is publishing the model's own narration of its thinking process alongside the Lean-verified proof.

**[数学与理论计算机科学的十项新进展](https://openai.com/index/ten-advances-in-mathematics)** — _OpenAI · 8月1日_

**Main takeaway:** OpenAI 这次放出了十个结果，每一个都解决或者大幅推进了数学和理论计算机科学里一个悬而未决很久的难题，全部由他们下一代主力模型 Astra 的内部版本做出来的，十道题加起来按 Sol API 价格算，token 成本才两千美元左右。

**Main methods:**
- **十道题横跨多个数学分支。** 涵盖高维几何、编码理论、算术电路复杂度、群论、算子代数、量子复杂度、格密码学和极值组合数学。
- **成本低到离谱。** 十个解法加一起，按 Sol API 定价算下来大概只要 2,000 美元的 token 费用。
- **人和模型配合出稿。** 人类研究者和同一个模型一起把模型给出的论证整理成正式论文手稿，之后模型再把每个证明形式化成 Lean certificate。
- **几个亮点结果。** 包括推翻了 Connes's rigidity conjecture、给多色三角 Ramsey 数找到了超指数级下界（解决 Erdős problem 183），还解决了极值图论里的 Erdős problem 146 和 180。
- **接着五月的数学工作往下做。** 这次是接着五月那次"评估一个未发布模型时顺手推翻了 Erdős unit-distance conjecture"的工作继续做，OpenAI 说那次结果已经带动了数学界的后续研究。
- **连模型的思考过程都公开了。** 每道题除了 Lean 验证过的证明，OpenAI 还把模型自己叙述解题思路的内容一起放出来了。
