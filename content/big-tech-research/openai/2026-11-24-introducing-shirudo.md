---
title: "OpenAI and Cisco introduce Shirudo"
date: 2026-11-24
draft: false
tags: ["big-tech-research", "openai"]
---

**[OpenAI and Cisco introduce Shirudo](https://openai.com/index/introducing-shirudo)** — _OpenAI · Nov 24_

**Main takeaway:** OpenAI and Cisco are launching Shirudo, an open-source eBPF runtime that lets operators protect running Linux systems during the window before a patch lands, with no restart. In a controlled test, a Codex-generated shield blocked a Java4Shell exploit attempt against a live Elasticsearch service while the service kept serving traffic.

**Main methods:**
- **The gap it targets.** Testing and deploying a patch still takes days or weeks, and an exploit often rides on the same Linux operation as a legitimate request, so blocking that operation outright would take the service down.
- **"Shields" as temporary, testable safeguards.** A shield is a targeted block on the behavior that exposes the vulnerability; teams can first observe how a proposed shield would affect the application, and deploy it only after an operator approves, without stopping the service.
- **eBPF as the insertion point.** Shirudo leans on eBPF, which runs small programs at specific points inside the kernel, to both observe suspicious activity and apply protections to already-running systems.
- **Agents in the loop, humans on the trigger.** OpenAI and Cisco are designing programmable controls so agents can investigate a vulnerability, write a targeted shield, and validate it against exploits and real workloads — but security teams decide what actually gets deployed.
- **Two layers of trust.** Shields are cryptographically signed and verified before loading, with Linux's eBPF verifier and kernel security controls on top; a TPM keeps a verifiable record of which protections were loaded or removed, as evidence for compliance checks.
- **The Java4Shell walkthrough.** Codex generated a shield that added an input check to Java's Base64 decoder and attached it to a running Elasticsearch process; the malicious input was rejected while Elasticsearch stayed up. A technical walkthrough from the Linux Plumbers Conference is public, and the project is open to outside developers, security researchers, and infrastructure operators.

**[OpenAI 和 Cisco 开源 Shirudo：补丁没到之前先给系统套个盾](https://openai.com/index/introducing-shirudo)** — _OpenAI · 11月24日_

**Main takeaway:** OpenAI 和 Cisco 一起开源了 Shirudo，一个基于 eBPF 的 runtime，专门管补丁还没打上那段空窗期：不用重启就能护住正在跑的 Linux 系统。他们做了个受控实验，让 Codex 生成一个 shield，直接挡住了针对线上 Elasticsearch 的 Java4Shell exploit，而 Elasticsearch 自己照常对外服务。

**Main methods:**
- **补的是哪个窟窿。** 一个 patch 从测试到上线还是要几天甚至几周，更麻烦的是 exploit 走的 Linux 操作往往和正常请求是同一个，你要是把这个操作一刀切掉，服务就跟着挂了。
- **shield 是临时的，而且可以先试。** 所谓 shield 就是只拦住暴露这个 vulnerability 的那一小段行为。团队可以先观察这个 shield 上去之后会怎么影响应用，等 operator 点头了再部署，期间服务不用停。
- **为什么选 eBPF。** eBPF 能在内核内部的特定位置跑小程序，所以既能盯住可疑行为，也能把保护直接打到已经在跑的系统上。
- **agent 干活，人按按钮。** 他们在设计一套可编程的接口，让 agent 自己去查 vulnerability、写出针对性的 shield，再拿 exploit 和真实流量去验证效果。但最后部署什么，还是安全团队说了算。
- **信任链做了两层。** shield 加载前要过 cryptographic 签名和校验，再叠上 Linux 自带的 eBPF verifier 和内核安全控制；另外用 TPM 记一份可验证的账，哪个保护什么时候加载、什么时候撤掉都有据可查，正好能拿去应付合规检查。
- **Java4Shell 那个 demo。** Codex 生成的 shield 在 Java 的 Base64 decoder 上加了一道输入检查，然后挂到正在跑的 Elasticsearch 进程上，恶意输入被挡掉，Elasticsearch 没受影响。Linux Plumbers Conference 上的技术 walkthrough 已经公开，项目也欢迎外部开发者、安全研究员和基础设施运维一起参与。
