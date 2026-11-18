---
title: "Inside the Codex sandbox"
date: 2026-11-18
draft: false
tags: ["big-tech-research", "openai"]
---

**[Inside the Codex sandbox](https://openai.com/index/inside-the-codex-sandbox)** — _OpenAI · Nov 18_

**Main takeaway:** An engineering post on Codex's local execution model: it walks through how Codex runs commands on your own machine while enforcing the filesystem and network limits you set, across macOS, Linux, and Windows. Only the listing summary was available (the article body returned HTTP 403), so the per-OS sandboxing primitives, the default policy, and the escape-hatch behavior are not covered here.

**[Codex 的 sandbox 是怎么做的](https://openai.com/index/inside-the-codex-sandbox)** — _OpenAI · 11月18日_

**Main takeaway:** 一篇工程向的文章，讲 Codex 在本地怎么执行命令：命令跑在你自己的机器上，但文件系统和网络的边界由你设定，macOS、Linux、Windows 三个平台都是这套。这篇只拿到列表页简介，正文返回 HTTP 403，所以三个系统各自用的是什么 sandbox 机制、默认策略怎么定、需要放开权限的时候是什么行为，这里都没有。
