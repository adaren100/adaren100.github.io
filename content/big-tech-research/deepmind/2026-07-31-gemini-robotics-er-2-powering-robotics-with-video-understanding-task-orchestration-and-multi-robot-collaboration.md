---
title: "Gemini Robotics ER 2: powering robotics with video understanding, task orchestration, and multi-robot collaboration"
date: 2026-07-31
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Gemini Robotics ER 2: powering robotics with video understanding, task orchestration, and multi-robot collaboration](https://deepmind.google/blog/gemini-robotics-er-2-powering-robotics-with-video-understanding-task-orchestration-and-multi-robot-collaboration/)** — _Google DeepMind · Jul 31_

**Main takeaway:** Google DeepMind launched Gemini Robotics ER 2, a "high-level brain" model for robots that does real-time spatial reasoning, multi-step task planning, and now multi-robot collaboration, handing off actual motor execution to a separate lower-level vision-language-action (VLA) model.

**Main methods:**
- **Separates thinking from moving.** ER 2 plans and reasons; it hands off motor execution to any given lower-level VLA model, and can "think" about the next step while the robot is still executing the current one.
- **Native tool calling.** Can call tools like Google Search or any user-defined function directly, not just plan robot actions.
- **Continuous video understanding.** By watching continuous video feeds, robots can track their own progress, notice when something's gone wrong, and know exactly when to move to the next step — a significant upgrade over ER 1.6.
- **New multi-robot collaboration.** Robots can now coordinate with each other in shared spaces to complete workflows a single robot couldn't handle alone.
- **Evaluated across three control modes.** Tested with real VLA models, simulated VLA models, and human tele-operation; ER 2 consistently outperforms ER 1.6 for tool orchestration in all three.
- **Availability.** Public via the Gemini API and Google AI Studio now; in private preview on the Gemini Enterprise Agent Platform.

**[Gemini Robotics ER 2：给机器人配上更强的"高层大脑"](https://deepmind.google/blog/gemini-robotics-er-2-powering-robotics-with-video-understanding-task-orchestration-and-multi-robot-collaboration/)** — _Google DeepMind · 7月31日_

**Main takeaway:** Google DeepMind 推出了 Gemini Robotics ER 2，一个专门给机器人当"高层大脑"的模型，负责实时空间推理、多步任务规划，这次还新加了多机协作能力，具体的运动执行则交给下面单独的 vision-language-action（VLA）模型去做。

**Main methods:**
- **思考和执行分开。** ER 2 只负责规划和推理，具体动作交给底层的 VLA 模型执行，而且它能在机器人还在执行当前动作的时候，就已经在"想"下一步该干什么了。
- **原生支持调用工具。** 除了规划机器人动作，还能直接调用 Google Search 之类的工具，或者任何用户自定义的 function。
- **能持续看视频理解进度。** 靠持续监看视频流，机器人能自己跟踪任务进度、发现哪里出岔子了、准确判断什么时候该进入下一步，这一点比 ER 1.6 有明显提升。
- **新增多机协作。** 现在多台机器人能在同一个空间里互相配合，完成单台机器人干不了的复杂流程。
- **在三种控制模式下都测过。** 分别在真实 VLA、仿真 VLA、人类远程操控这三种模式下评估，ER 2 在工具编排能力上全面超过 ER 1.6。
- **开放情况。** 现在已经能通过 Gemini API 和 Google AI Studio 公开使用，在 Gemini Enterprise Agent Platform 上还处于私有预览阶段。
