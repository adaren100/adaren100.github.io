---
title: "Claude plays robotics"
date: 2026-07-09
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[Claude plays robotics](https://www.anthropic.com/research/claude-plays-robotics)** — _Anthropic · Jul 9_

**Main takeaway:** Anthropic gave language models control over a range of robot bodies — classic control toys, a simulated quadruped and humanoid, a robotic arm, and a real Unitree Go2 — and found their capability depends heavily on the control interface: driving joints directly mostly fails, but supervising a pretrained policy or using simple orientation tools lets models complete real navigation and manipulation tasks. A general-purpose chat model with no robotics training can already, on a good run, walk a quadruped through a maze or move a plate from counter to stove.

**Main methods:**
- **A range of embodiments.** Classic control toys, a simulated quadruped and humanoid, a robotic arm, and a real Unitree Go2 — the quadruped from Project Fetch.
- **A ladder of control abstraction.** From directly commanding motor torques, to writing controller code, to training a controller from scratch with reinforcement learning, to issuing high-level steering instructions to a pretrained robot policy.
- **Three task areas.** Classic control problems (like balancing a pendulum), locomotion and navigation (getting legged robots to balance, walk, and move through space), and manipulation (using a robotic arm to grasp and move objects).
- **The interface matters as much as the model.** The same model can look weak or strong depending on which control method it uses. For the hardest bodies — the humanoid in particular — today's models only get traction at high-abstraction interfaces where a pretrained policy handles the low-level physics.
- **Improvement is real but uneven.** The most consistent generational gains are on high-level interfaces; direct low-level control is also improving, but much less consistently.
- **Safety implications.** Frontier models can't control humanoids without a pretrained policy today, but newer models show real gains in direct manipulation and high-level policy control, and the reliability gap is closing with each model generation.

**[Claude 玩机器人：语言模型的能力能搬进物理世界吗](https://www.anthropic.com/research/claude-plays-robotics)** — _Anthropic · 7月9日_

**Main takeaway:** Anthropic 让几个语言模型去控制一批机器人身体，包括经典控制玩具、仿真的四足和人形机器人、机械臂，还有一台真的 Unitree Go2。结论是模型能不能干活，很大程度取决于它和机器人之间的控制接口：让它直接驱动关节基本都失败，但让它监督一个 pretrained policy 或者用简单的方向工具，就能真的完成导航和抓取任务。一个完全没受过 robotics 训练的通用 chat 模型，状态好的时候已经能把四足机器人慢慢带出迷宫，或者把盘子从台面挪到炉子上。

**Main methods:**
- **一整排 embodiment。** 经典控制玩具、仿真的四足和人形机器人、机械臂，外加一台真机 Unitree Go2，就是 Project Fetch 里那只四足。
- **从低到高的抽象接口。** 直接下 motor torque 指令、写 controller 代码、用 reinforcement learning 从头训一个 controller、给 pretrained policy（一个把高层指令转成协调关节动作的独立神经网络）下高层指令，几档抽象度都测了。
- **三类任务。** 经典控制问题（比如平衡倒立摆）、locomotion 和导航（让腿式机器人站稳、走路、穿过空间）、manipulation（用机械臂抓取和搬运物体）。
- **接口和身体跟模型本身一样重要。** 同一个模型换个控制方式，表现能从很弱变很强。最难控的人形机器人，目前的模型只有在高抽象接口下才玩得动，底层物理全靠 pretrained policy 兜着。
- **在进步，但不均匀。** 代际之间最稳定的提升出现在高层接口上；直接的底层控制也在进步，只是没那么稳定，有些新模型明显超过前代，有些则没有。
- **对安全的含义。** 今天的 frontier 模型离开 pretrained policy 还控不了人形机器人，但新一代模型在直接 manipulation 和高层 policy 控制上都有实打实的提升，可靠性差距每一代都在缩小。
