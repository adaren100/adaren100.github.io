---
title: "Project Fetch: Phase two"
date: 2026-06-18
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[Project Fetch: Phase two](https://www.anthropic.com/research/project-fetch-phase-two)** — _Anthropic · Jun 17_

**Main takeaway:** Anthropic re-ran its August 2025 robodog experiment with a newer model and found that Claude Opus 4.7, operating without any human assistance, was about 20× faster than the fastest human team at all tasks completed by participants less than a year ago — and at least 10× faster on every individual task any human team had completed.

**Main methods:**
- **What the original Project Fetch tested.** Teams of non-roboticist Anthropic employees, randomly assigned with or without Claude Opus 4.1, had to operate an off-the-shelf robotic quadruped, connect to its video and lidar sensors, write a manual control program, monitor its path, detect a beach ball, and finally retrieve it autonomously.
- **Baseline finding from August 2025.** Opus 4.1 *helped* humans substantially but could not do the tasks itself — it got stuck on the preliminary step of connecting to the robot. That phase established the "models help humans" rung of the ladder.
- **Phase two setup.** Three trials of Opus 4.7 in Claude Code with adaptive thinking at maximum effort. The researcher only plugged in the laptop, entered the initial prompt, approved commands, and approved transitions between tasks — no debugging help.
- **Speed result.** On every task at least one human team had completed in August, Opus 4.7 finished at least 10× faster. On the four tasks both human teams completed, Opus 4.7 was on average >37× faster than the no-Claude team and >18× faster than the Claude-assisted team.
- **What it still cannot do.** The model still struggled with the "fetching" itself — precisely moving the beach ball with the robot — and the experiment doesn't touch low-level robotic control like learning an actuation policy.
- **Framing.** Anthropic reads this as the familiar progression — first models help humans, then humans help models, then models largely do it themselves — now appearing at the AI/physical-world interface, just as it did earlier in cybersecurity.

**[Project Fetch 第二阶段：Opus 4.7 自己上手，比去年最快的人类队还快 20 倍](https://www.anthropic.com/research/project-fetch-phase-two)** — _Anthropic · 6月17日_

**Main takeaway:** Anthropic 把 2025 年 8 月那个机器狗实验重新跑了一遍，换上新模型。结果是 Claude Opus 4.7 不靠人类协助、自己一路干下来，在所有去年人类参与者完成过的任务上，平均比当时最快的人类队还快 20 倍左右；单看每个任务，至少都快了 10 倍。

**Main methods:**
- **原版 Project Fetch 在测什么。** 一群不懂机器人的 Anthropic 员工，被随机分成"有 Claude Opus 4.1"和"没 Claude"两队，要去操作一只市售的四足机器狗：连上它的视频和 lidar、写手动控制程序、监控它的路径、检测沙滩球，最后把球自动叼回来。
- **去年 8 月的 baseline。** Opus 4.1 帮人类队效果挺明显，但自己 standalone 干完全做不到——卡在第一步"怎么连上机器狗"上就过不去了。那一轮验证的是"模型帮人"这一档。
- **这次的实验设置。** 在 Claude Code 里跑了三轮 Opus 4.7，adaptive thinking 开到最大档。研究员的角色就是把 laptop 插进机器狗、输入初始 prompt、approve 命令、approve 任务之间的切换——没有 debug 协助。
- **速度结果。** 去年人类至少有一队完成过的每个任务，Opus 4.7 都至少快 10 倍。两队人类都完成的那四个任务里，Opus 4.7 平均比无 Claude 队快 37 倍以上、比 Claude 加持队快 18 倍以上。
- **还做不到的地方。** "fetching" 本身——精确控制机器狗去推沙滩球——模型还是不太行。而且这一系列任务都没碰更底层的 actuation policy 之类的 robotic control 难题。
- **Anthropic 怎么解读。** 跟 cybersecurity 一样的曲线又出现了：先是模型帮人，再是人帮模型，最后模型基本能自己干。现在这条曲线开始在 AI 跟物理世界的交界处复现。
