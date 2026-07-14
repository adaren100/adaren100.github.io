---
title: "Claude's values across models and languages"
date: 2026-07-13
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[Claude's values across models and languages](https://www.anthropic.com/research/claude-values-models-languages)** — _Anthropic · Jul 13_

**Main takeaway:** Anthropic analyzed 300,000 real Claude.ai conversations and compressed the thousands of values Claude expresses into four interpretable axes — Deference vs. Caution, Warmth vs. Rigor, Depth vs. Brevity, and Candor vs. Execution — which together capture 15% of the variation in Claude's values. The resulting value profiles match perceived model character (Sonnet 4.6 warm, Opus 4.7 rigorous) and vary measurably across the top 20 languages on Claude.ai.

**Main methods:**
- **Compressing 3,000+ values into axes.** Prior work identified more than 3,000 distinct values in 700,000 anonymized conversations — too many to reason about. Here each axis is a number line between two opposing groups of values, and where Claude falls on the line shows which group it leans toward.
- **Four key axes.** Deference vs. Caution (accommodate the user vs. guard against risk), Warmth vs. Rigor (positivity and care vs. accuracy and precision), Depth vs. Brevity (explain in depth vs. do only what was asked), Candor vs. Execution (foreground uncertainty vs. deliver a polished, confident answer).
- **Profiles match model reputations.** Sonnet 4.6 is regarded as particularly warm, Opus 4.7 as rigorous — and their measured profiles mirror this: Sonnet 4.6 leans toward deference and emotional warmth, Opus 4.7 toward accuracy, precision, and guarding against misuse.
- **Values shift across languages.** The largest variation is on the Warmth vs. Rigor axis: Claude leans most toward warmth-related values in Arabic and Hindi, and most toward rigor-related values in English and Russian.
- **Connecting values to training.** Because the axes quantify differences between models, the approach may eventually let Anthropic tie variation in expressed values back to specific character-training and fine-tuning decisions.

**[Claude 的价值观：跨模型、跨语言实测](https://www.anthropic.com/research/claude-values-models-languages)** — _Anthropic · 7月13日_

**Main takeaway:** Anthropic 分析了 30 万条真实的 Claude.ai 对话，把 Claude 表达出来的几千种价值观压缩成四条可解释的轴：Deference vs. Caution、Warmth vs. Rigor、Depth vs. Brevity、Candor vs. Execution，这四条轴加起来解释了 Claude 价值观里 15% 的变化。测出来的价值观画像和大家对各模型性格的印象对得上（Sonnet 4.6 偏暖，Opus 4.7 偏严谨），在 Claude.ai 上最常用的 20 种语言之间也有可测量的差异。

**Main methods:**
- **把 3,000 多种价值观压成几条轴。** 之前的工作在 70 万条匿名对话里识别出 3,000 多种价值观，数量太大没法直接分析。这次每条轴是一根数轴，两端各是一组相对的价值观，Claude 落在哪一边就说明它偏向哪组。
- **四条关键的轴。** Deference vs. Caution（顺着用户的需求，还是防范风险和伤害）、Warmth vs. Rigor（表达关心和正面情绪，还是强调准确和精确）、Depth vs. Brevity（讲深讲透，还是只做被要求的事）、Candor vs. Execution（主动摆出自己的不确定性，还是给一个更完整自信的答案）。
- **画像和模型的口碑对得上。** Sonnet 4.6 一直被认为特别暖，Opus 4.7 以严谨著称。实测下来 Sonnet 4.6 确实更偏 deference 和情感上的 warmth，Opus 4.7 更强调准确、精确，也更注意防 misuse。
- **不同语言差别不小。** 差异最大的是 Warmth vs. Rigor 这条轴：Claude 在阿拉伯语和印地语里最暖，在英语和俄语里最偏严谨。
- **往训练决策上挂钩。** 这套轴能量化模型之间的差异，以后可能把价值观表达上的变化跟具体的 character training 和 fine-tuning 决策联系起来。
