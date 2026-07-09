---
title: "An off switch for dual use knowledge in AI models"
date: 2026-07-08
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[An off switch for dual use knowledge in AI models](https://www.anthropic.com/research/off-switch-dual-use)** — _Anthropic · Jul 7_

**Main takeaway:** Anthropic and AE Studio present GRAM (Gradient-Routed Auxiliary Modules), a preliminary method for confining dual-use knowledge (e.g. virology, cybersecurity) to removable compartments within a single trained model, instead of needing separate models for restricted vs. vetted users.

**Main methods:**
- **Dedicated removable modules per category.** GRAM adds extra neurons to every transformer layer, grouped into modules, one per dual-use knowledge category (e.g. virology).
- **Selective gradient routing during training.** On general text, the whole model learns normally; on dual-use category text, only that category's module updates while the rest of the network's weights stay frozen.
- **Deletion removes the capability.** Because dual-use knowledge accumulates in its dedicated module rather than diffusing through the network, deleting the module after training removes that capability specifically.
- **Motivated by filtering's limits.** Prior work filtered CBRN content out of pretraining data and confined dual-use knowledge to a removable weight slice, but that approach yields one fixed-capability model — serving both a restricted public version and a fuller version for vetted labs would mean training two separate frontier models, which is prohibitively expensive.
- **Goal: three-way balance.** The method aims to limit dangerous capability access surgically, still let trusted/vetted users access it for legitimate purposes, and avoid degrading performance on unrelated tasks.
- **Explicitly preliminary.** Anthropic states GRAM hasn't been applied to any production model and isn't confirmed to ever be — this is early-stage research, not a shipped safeguard.

**[给 AI 模型的双用途知识装一个"开关"](https://www.anthropic.com/research/off-switch-dual-use)** — _Anthropic · 7月7日_

**Main takeaway:** Anthropic 和 AE Studio 合作搞出一个叫 GRAM(Gradient-Routed Auxiliary Modules)的方法,能把病毒学、网络安全这类双刃剑知识关进模型里一个可以整体删掉的隔间,不用再为受限用户和 vetted 用户分别训练两个模型。

**Main methods:**
- **每类知识配一个专属可删除模块。** GRAM 在 transformer 每一层都加了一批额外神经元,按双用途知识类别分组,比如病毒学单独一个模块。
- **训练时做选择性梯度路由。** 碰到普通文本,整个模型正常学习;碰到某个双用途类别的文本(比如病毒学),只有对应模块会更新,其余权重保持冻结。
- **删掉模块就等于删掉能力。** 因为双用途知识都攒在专属模块里,不会扩散到整个网络,训练完之后直接删掉那个模块,对应能力也就没了。
- **动机是过滤法的局限。** 之前的做法是从预训练数据里过滤掉 CBRN 相关内容,把双用途知识关进一小块可删除的权重里,但这样只能得到一个能力固定的模型,想同时给公众一个受限版、给 vetted 实验室一个完整版,就得单独训练两个前沿模型,成本高到不现实。
- **目标是三头兼顾。** 既要尽量精准地限制危险能力的访问,又要让可信、经过审核的用户还能拿来做正当用途,同时不能拖累模型在其他任务上的表现。
- **明确说了还是早期阶段。** Anthropic 说 GRAM 目前还没用在任何正式发布的模型上,以后会不会用也不确定,这是早期研究,还不是已经上线的安全机制。
