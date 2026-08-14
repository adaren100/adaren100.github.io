---
title: "Previewing Ultrafast mode: GPT-5.6 Sol at up to 14X the speed"
date: 2026-08-13
draft: false
tags: ["big-tech-research", "openai"]
---

**[Previewing Ultrafast mode: GPT-5.6 Sol at up to 14X the speed](https://openai.com/index/previewing-ultrafast)** — _OpenAI · Aug 13_

**Main takeaway:** OpenAI is previewing Ultrafast, a new API service tier that runs GPT‑5.6 Sol up to 14× faster than Standard processing at up to 750 output tokens per second, powered by Cerebras. The pitch is that you no longer drop to a smaller model to get real-time speed.

**Main methods:**
- **A service tier, not a new model.** Ultrafast runs the same frontier model — GPT‑5.6 Sol — and launches first in the OpenAI API. OpenAI frames the goal as "more useful work per second" rather than trading intelligence away for latency.
- **Cerebras is the hardware story.** The tier is powered by Cerebras and generates up to 750 output tokens per second; OpenAI credits efficiency work "across every layer of our stack" under GPT‑5.6 for making the economics work.
- **Target workloads are time-boxed ones.** Incident response (analyzing logs, recent code changes, and engineer reports while the outage is still unfolding), financial research and fraud detection on moving conditions, real-time voice and support, and commerce answers delivered before a shopper abandons checkout.
- **The research-loop use case.** OpenAI singles out turning an overnight experiment run into an interactive working session — test an idea, read the results, adjust, rerun — without the team losing flow.
- **Limited preview, deliberately.** An initial cohort across coding, commerce, financial research, and support is being studied in real production environments so findings can guide deployment as capacity grows; everyone else joins a notify list.
- **Caveats.** The post gives no Ultrafast pricing, no general-availability date, and no evals showing output quality holds at Ultrafast speed. The 14× and 750 tok/s figures are OpenAI's own, and the only side-by-side shown is a demo building a 3D warehouse simulator from one prompt.

**[Ultrafast 预览：GPT‑5.6 Sol 最高快 14 倍](https://openai.com/index/previewing-ultrafast)** — _OpenAI · 8月13日_

**Main takeaway:** OpenAI 放出了 Ultrafast 的预览，这是 API 上新增的一档 service tier，跑的还是 GPT‑5.6 Sol，但比 Standard 快最多 14 倍，输出能到每秒 750 个 token，底层由 Cerebras 支撑。卖点很直接：想要实时速度，不用再退回小模型了。

**Main methods:**
- **这是一档 tier，不是新模型。** 跑的就是 GPT‑5.6 Sol 本身，先在 OpenAI API 上线。OpenAI 的说法是目标不在于"牺牲智能换延迟"，而是每秒能干出更多有用的活。
- **硬件是 Cerebras。** 这一档由 Cerebras 提供算力，输出速度最高每秒 750 个 token。OpenAI 说 GPT‑5.6 这一代在整个 stack 每一层做的效率优化，才让这个账算得过来。
- **瞄的都是有时间窗口的场景。** 故障响应（系统挂的时候一边看 log、最近的代码改动和工程师报告，一边把可能原因和修法先备好）、市场信号和可疑交易分析、实时语音和客服、以及在用户还没放弃购物车之前就把商品问题、库存、推荐和结账问题解决掉。
- **还有一个做研究的用法。** OpenAI 专门点了这个：以前得跑一晚上的实验，现在能变成一次交互式的工作会话，试个想法、看结果、调方向、再跑一轮，中间不用断。
- **preview 阶段是刻意收着的。** 先跟 coding、commerce、金融研究、客服这几类客户在真实生产环境里跑，看清楚"快一个数量级"到底在哪儿最值钱，再随着算力扩容往外放，其他人先登记等通知。
- **需要注意的点。** 这篇没给 Ultrafast 的价格，没给正式开放时间，也没有任何 eval 证明这个速度下输出质量不掉。14 倍和每秒 750 token 都是 OpenAI 自己的数字，唯一的对比只有一个 demo：同一句 prompt 下 Ultrafast 和 Standard 各做一个 3D 仓库模拟器。
