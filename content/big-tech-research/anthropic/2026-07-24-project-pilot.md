---
title: "Project Pilot: Can AI control a drone?"
date: 2026-07-24
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[Project Pilot: Can AI control a drone?](https://www.anthropic.com/research/project-pilot)** — _Anthropic · Jul 24_

**Main takeaway:** Anthropic and Andon Labs built Drone-Bench, a new benchmark plus live flight demonstrations testing whether AI models can autonomously pilot a quad-rotor drone to locate and follow a person indoors — a capability with both public-safety and surveillance/warfare dual-use implications.

**Main methods:**
- **Task design.** Models control a quad-rotor drone in an indoor office to find a specific person from a reference photo, follow them, and reacquire the target if they move out of frame.
- **Decomposed into sub-tasks.** The task breaks into command/control schema design, obstacle-aware indoor mapping and navigation, photo-based target identification, and continuous tracking — each individually solvable with known algorithms, but not trivial to integrate end-to-end as an AI-driven system.
- **Part of a broader physical-world series.** Follows Project Vend (AI running a small shop) and Project Fetch (robots retrieving objects), continuing Anthropic's track record of testing frontier models against real-world hardware tasks.
- **Framed as dual-use risk tracking.** Anthropic's Frontier Red Team uses this work to gauge how close AI is to autonomously piloting robots, citing both beneficial uses (search and rescue, disaster response) and risks (surveillance overreach, warfare).
- **Real flight demonstrations, not just simulation.** Combines actual drone flights with replicable evaluations so capability progress can be tracked over time.

**[Project Pilot：AI 能不能开无人机？](https://www.anthropic.com/research/project-pilot)** — _Anthropic · 7月24日_

**Main takeaway:** Anthropic 和 Andon Labs 一起做了个新 benchmark 叫 Drone-Bench，专门测 AI 模型能不能自主操控四旋翼无人机，在室内环境里找人并跟拍，这项能力既能用于搜救之类的公共安全场景，也有被滥用来监控甚至用于战争的风险。

**Main methods:**
- **任务设计。** 让模型操控一架四旋翼无人机，在室内办公环境里根据一张参考照片找到指定的人，跟着他们走，要是对方跑出画面还得重新找回来。
- **拆成几个子任务。** 整个任务被拆成控制指令schema设计、带避障的室内建图导航、照片比对找目标、以及持续跟踪这几块，每一块单独看都有现成算法，但要让AI模型端到端串起来跑通并不容易。
- **属于更大的物理世界系列研究。** 接着 Project Vend（AI 开小店）和 Project Fetch（机器人捡东西）继续做下去，Anthropic 一直在拿前沿模型去测真实硬件任务。
- **出发点是追踪dual-use风险。** Anthropic 的 Frontier Red Team 靠这类工作来判断AI离"能自主操控机器人"还有多远，既提到了搜救、灾害响应这类正面用途，也提到了监控越权、战争这类风险。
- **不只是仿真，是真实试飞。** 把实际飞行演示和可复现的eval结合起来，这样就能持续跟踪能力进展。
