---
title: "Previewing the Model Hardware Standard"
date: 2026-08-27
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[Previewing the Model Hardware Standard](https://www.anthropic.com/news/model-hardware-standard-research-preview)** — _Anthropic · Aug 27_

**Main takeaway:** Anthropic opened a research preview of the Model Hardware Standard (MHS), a shared specification that lets AI agents discover and safely drive physical lab and factory instruments — microscopes, liquid handlers, robotic arms — in parallel, and claims it cuts hardware integration work from weeks or months down to hours or minutes.

**Main methods:**
- **A standardized driver built on read/write primitives.** MHS defines a driver layer translating between the operating system and the device using commands as simple as "read" (get temperature) and "write" (set temperature), which any programmable device can act on.
- **Devices announce themselves.** Each device is made discoverable in a standard format so devices and agents find each other across networks, replacing the bespoke translator programs labs currently write for each pair of instruments.
- **Natural-language tags carry the tacit knowledge.** The driver holds tags where a user writes machine characteristics not discernable from code — the post's example is the weight of a robot arm, which an agent needs in order to manipulate it safely. Users fill these in directly or by chatting with an agent that interviews them about the setup, and the driver then generates a device reference file.
- **Model-agnostic and harness-agnostic.** MHS works with any device that has a programmable interface, and any agent harness can reach it over standard protocols such as the Model Context Protocol.
- **Origin and who gets it first.** Development began as a collaboration between Anthropic and HHMI Janelia Research Campus; the preview goes to scientific research labs and advanced manufacturers across science, robotics, electronics, and manufacturing.
- **Safety evals come before open-sourcing.** Anthropic says it is sharing the early version specifically to co-develop safety evaluations and best practices for AI systems operating physical equipment, ahead of releasing the standard as open source.

**[Model Hardware Standard 预览版：让 agent 直接上手实验室设备](https://www.anthropic.com/news/model-hardware-standard-research-preview)** — _Anthropic · 8月27日_

**Main takeaway:** Anthropic 开放 Model Hardware Standard（MHS）的 research preview，这是一套让 AI agent 发现并安全操作物理设备的通用规范，显微镜、liquid handler、机械臂都能同时管，官方说法是把原本要花几周甚至几个月的硬件对接压缩到几小时甚至几分钟。

**Main methods:**
- **一层标准化 driver，只有读和写两类原语。** MHS 定义的 driver 负责在操作系统和设备之间做翻译，命令简单到就是"read"（比如读温度）和"write"（比如设温度），任何有可编程接口的设备都能听懂。
- **设备自己会报到。** 每台设备按统一格式暴露出来，设备和 agent 在网络上互相就能找到，不用再像现在这样每两台机器之间手写一个转换程序。
- **拿自然语言 tag 把隐性知识写进去。** driver 里留了 tag，让人把光看代码看不出来的机器特性写清楚，原文举的例子是机械臂的重量，agent 得知道这个才能安全地操作它。这些信息可以自己填，也可以跟一个 agent 聊，让它把你的硬件配置问出来，之后 driver 自动生成设备的参考文件。
- **不绑模型，也不绑 harness。** 只要设备有可编程接口就能接，任何 agent harness 都能通过 Model Context Protocol 这类标准协议访问。
- **从哪儿来，先给谁用。** 这套东西最早是 Anthropic 和 HHMI Janelia Research Campus 合作做起来的，preview 阶段先给科研实验室和先进制造企业，覆盖科学、机器人、电子和制造几个方向。
- **先把 safety 那块做完再开源。** Anthropic 说提前放出早期版本就是为了跟合作方一起搭 AI 操作物理设备的 safety evaluation 和最佳实践，之后才会把标准正式开源。
