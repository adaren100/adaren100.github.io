---
title: "Gemini Robotics 2 brings whole body intelligence to robots"
date: 2026-07-28
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Gemini Robotics 2 brings whole body intelligence to robots](https://deepmind.google/blog/gemini-robotics-2-brings-whole-body-intelligence-to-robots/)** — _Google DeepMind · Jul 28_

**Main takeaway:** Google DeepMind launched Gemini Robotics 2, a three-model system that gives humanoid robots "whole body intelligence" — full-body control from feet to fingertips, advanced dexterity, and multi-robot collaboration.

**Main methods:**
- **Three specialized models.** Gemini Robotics 2 (VLA) converts vision and language input into motor control across a full humanoid body, including 22-degree-of-freedom hands; Gemini Robotics ER 2 is the high-level embodied-reasoning planner for multi-step tasks; Gemini Robotics On-Device 2 runs locally without network latency.
- **Tested on real hardware.** Evaluated on Apptronik Apollo 2 with SharpaWave hands, Apollo 2 with Inspire hands, and Franka Duo grippers.
- **Fast embodiment adaptation.** The on-device model adapts to new bi-arm robot bodies via "motion transfer" in just a few hours, typically using fewer than 200 examples.
- **Long-horizon task planning.** ER 2 handles tasks spanning several minutes and hundreds of decisions, with improved event detection and task-boundary recognition.
- **Reported task success rates.** Whole-body pick-from-shelf hit 76.3%, unscrewing a bulb hit 92%, precise insertion tasks hit 89.6% — though tasks like screwing in a bulb (36%) and tying a trash bag (44%) remain hard.
- **New safety benchmark.** Introduced "ASIMOV-Agentic" to evaluate whether agents refuse unsafe tool calls and proactively ask humans to step in.

**[Gemini Robotics 2：给机器人装上"全身智能"](https://deepmind.google/blog/gemini-robotics-2-brings-whole-body-intelligence-to-robots/)** — _Google DeepMind · 7月28日_

**Main takeaway:** Google DeepMind 发布了 Gemini Robotics 2，一套由三个模型组成的系统，让人形机器人拥有从脚到手指的全身控制能力、更精细的灵巧操作，还能多机协作。

**Main methods:**
- **三个专门模型分工协作。** Gemini Robotics 2 (VLA) 负责把视觉和语言输入转成运动控制，能操控整个身体，包括 22 自由度的灵巧手；Gemini Robotics ER 2 是负责多步任务规划的高层 embodied reasoning 模型；Gemini Robotics On-Device 2 则跑在本地，不用担心网络延迟。
- **真机上测过。** 在 Apptronik Apollo 2（配 SharpaWave 手和 Inspire 手两个版本）以及 Franka Duo 夹爪上都做了实测。
- **能很快适配新机型。** On-device 模型靠"motion transfer"技术，通常只需要几个小时、不到 200 个示例，就能适配一个新的双臂机器人本体。
- **能规划长程任务。** ER 2 能处理持续几分钟、涉及上百个决策的任务，事件检测和任务边界识别的能力都有提升。
- **实测成功率。** 从货架上取物达到 76.3%，拧下灯泡 92%，精密插装任务 89.6%；不过拧上灯泡（36%）和系垃圾袋（44%）这类任务还是比较难。
- **新增了安全 benchmark。** 推出了 ASIMOV-Agentic，专门评估 agent 会不会拒绝执行不安全的工具调用，以及会不会主动请求人类介入。
