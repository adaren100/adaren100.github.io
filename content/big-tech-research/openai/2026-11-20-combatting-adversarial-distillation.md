---
title: "Combatting adversarial distillation"
date: 2026-11-20
draft: false
tags: ["big-tech-research", "openai"]
---

**[Combatting adversarial distillation](https://openai.com/index/combatting-adversarial-distillation)** — _OpenAI · Nov 20_

**Main takeaway:** OpenAI's writeup on defending against adversarial distillation — attackers using a frontier model's outputs to train a copy that inherits the capabilities but none of the safeguards. In an internal adaptive red-teaming eval, the average success rate for recovering protected reasoning fell from 54.0% against GPT‑6 Astra with its original safeguards to 0.2% against GPT‑6.2 Astra with the updated ones.

**Main methods:**
- **The threat model.** An adversary distills, say, a model's cyber capabilities into a second model, then deploys it without the refusals or safeguard layers that would have blocked the same requests on the original.
- **Chain-of-thought is the crown jewel.** Protected reasoning — the intermediate steps generated on the way to an answer — can contain information the final answer leaves out, which makes it unusually valuable as training data for someone else's model.
- **Layered defenses rather than one control.** Adversarial testing, model training, classifiers, and API-level protections, combined with investigations into coordinated extraction campaigns.
- **Promoted to bio/cyber tier.** The updated distillation safeguards are now aligned with the protections OpenAI already applies to biology and cybersecurity risks.
- **Two things being measured.** Resistance to reasoning extraction (the 54.0% → 0.2% adaptive-eval number) and campaign detection plus enforcement against coordinated actors.
- **Framed as an industry and national-security problem.** The post's closing sections argue adversarial distillation has national security implications and lays out how other labs can build on the approach.

**[怎么防住别人"偷蒸馏"自己的模型](https://openai.com/index/combatting-adversarial-distillation)** — _OpenAI · 11月20日_

**Main takeaway:** OpenAI 讲了他们怎么防 adversarial distillation，也就是有人拿前沿模型的输出去训自己的模型，能力抄过去了，safeguard 一个没带。他们自己做了一组自适应 red-teaming eval，测攻击者能不能把模型的 protected reasoning 掏出来：原来 GPT‑6 Astra 加旧 safeguard 的平均攻击成功率是 54.0%，换成 GPT‑6.2 Astra 加新 safeguard 之后降到 0.2%。

**Main methods:**
- **威胁模型长什么样。** 攻击者把模型的 cyber 能力蒸馏到第二个模型上，然后不带任何 refusal 和 safeguard 直接部署，原模型会拒答或者会被拦下来的请求，这个模型照做。
- **chain-of-thought 才是最值钱的那块。** 模型推理过程中产生的中间步骤，里面常常有最终答案里没写出来的信息，所以拿来当别人的训练数据特别好用，也就特别需要保护。
- **不靠单点防御，靠叠层。** adversarial testing、模型训练、classifier、API 层面的限制一起上，另外还会去查那些有组织地想把能力抽走的 campaign。
- **规格提到了 bio/cyber 那一档。** 这套新的蒸馏防护已经跟他们在生物和网络安全上用的保护级别对齐了。
- **他们盯两个指标。** 一个是抗 reasoning 提取的能力（就是 54.0% 降到 0.2% 那组自适应 eval），另一个是对有组织攻击者的检测和处置。
- **被当成行业问题和国家安全问题来写。** 文章后半专门谈了 adversarial distillation 的国家安全含义，也写了别的实验室可以怎么接着用这套做法。
