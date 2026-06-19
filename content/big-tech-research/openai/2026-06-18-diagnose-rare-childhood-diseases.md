---
title: "Using AI to help physicians diagnose rare genetic diseases affecting children"
date: 2026-06-18
draft: false
tags: ["big-tech-research", "openai"]
---

**[Using AI to help physicians diagnose rare genetic diseases affecting children](https://openai.com/index/diagnose-rare-childhood-diseases)** — _OpenAI · Jun 18_

**Main takeaway:** In an NEJM AI study published June 18, 2026, researchers from Boston Children's Hospital's Manton Center, Harvard, and OpenAI used the o3 Deep Research reasoning model to reanalyze 376 previously unsolved rare-disease cases. After expert review and clinical confirmation, physicians established 18 new diagnoses — a 4.8% additional diagnostic yield on top of earlier specialist analysis.

**Main methods:**
- **The reanalysis premise.** Roughly half of rare-disease patients remain undiagnosed after extensive testing, but the underlying evidence — gene-disease links, variant reclassifications, new case reports — keeps growing, so old cases can become newly interpretable without new sequencing.
- **Cohort and model.** 376 de-identified previously analyzed but unsolved cases were fed to OpenAI o3 Deep Research, which produced evidence-linked candidate explanations for human review rather than diagnoses.
- **Human-in-the-loop workflow.** The model never diagnosed any patient or made clinical decisions; it surfaced testable hypotheses that specialists then evaluated, often with additional testing and confirmation in a clinical laboratory.
- **Diagnostic yield.** 18 cases received confirmed diagnoses after this process — a 4.8% incremental yield, on cases that had already evaded years of expert analysis.
- **Flexibility on variant identification.** The post highlights cases where the model demonstrated flexibility in surfacing variants and producing biologically coherent, testable hypotheses rather than just pattern-matching against existing labels.
- **Framing.** The authors position AI-assisted reanalysis as a scalability fix for a maintenance problem: the patient's genome is fixed, but the evidence around it changes continuously, and most labs cannot afford to revisit every old case manually.

**[OpenAI o3 帮医生在 376 个儿童罕见病疑难案例里多揪出 18 个诊断](https://openai.com/index/diagnose-rare-childhood-diseases)** — _OpenAI · 6月18日_

**Main takeaway:** Boston Children's Hospital 的 Manton Center、哈佛和 OpenAI 联合发的一篇 NEJM AI 研究（6月18日刊出），用 o3 Deep Research 这个 reasoning model 重新分析 376 例之前已经做过分析但一直没诊断出来的罕见病案例。经过专家复核和临床确认，physician 又确认了 18 个新诊断，相当于在原本已被专家分析过的基础上又多出 4.8% 的 diagnostic yield。

**Main methods:**
- **为什么值得重新分析。** 罕见病患者就算做了完整的基因检测，差不多一半还是没法明确诊断。但 gene-disease 的关联、variant 的重新分类、新的病例报告一直在累积，老案例其实可以在不重测的情况下被重新解读。
- **数据和模型。** 376 例去标识化的、之前分析过但没结果的案例丢给 OpenAI o3 Deep Research，模型输出的是带证据链的候选解释，给人类去审，不是直接出诊断。
- **整套流程都有 human-in-the-loop。** 模型从头到尾没"诊断"任何一个病人，也没做任何临床决策。它给出的是 specialist 可以验证的 hypothesis，必要时再做额外检测，最后在 clinical lab 里确认。
- **诊断结果。** 走完这套流程后，physician 在 18 个案例里确认了新诊断——4.8% 的额外 yield，而且这些都是被专家研究过好几年都没结论的硬骨头。
- **variant 识别上的灵活性。** 文章强调模型不是单纯 pattern match 现有标签，而是能在 variant 的识别上有点灵活度，输出生物学上自洽、可以拿去做实验验证的 hypothesis。
- **更大的命题。** 作者把这件事 frame 成一个 scalability 问题的解法：病人的 genome 是固定的，但围绕它的证据在不断更新，大部分实验室没人手定期 review 每个老案例，AI 可以补这个缺口。
