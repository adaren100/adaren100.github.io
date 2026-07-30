---
title: "Discovering cryptographic weaknesses with Claude"
date: 2026-07-28
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[Discovering cryptographic weaknesses with Claude](https://www.anthropic.com/research/discovering-cryptographic-weaknesses)** — _Anthropic · Jul 27_

**Main takeaway:** Using Claude Mythos Preview, Anthropic researchers found improved attacks against two cryptographic algorithms themselves (not just buggy implementations of them) — cutting the effective key strength of the post-quantum signature scheme HAWK in half, and speeding up the best-known attack on round-reduced AES by 200–800×. Neither result affects any production system today.

**Main methods:**
- **From implementation bugs to breaking the math.** Claude Mythos Preview had already shown it could autonomously find and exploit vulnerabilities in cryptographic libraries — but those were coding errors in how algorithms were implemented. This work shows Mythos can find flaws in the algorithms themselves.
- **HAWK attack.** HAWK is a third-round candidate in NIST's post-quantum digital signature competition, and had survived two years of expert human review. Mythos improved the best-known attack on it in just 60 hours of work, effectively cutting its key strength in half.
- **Round-reduced AES attack.** AES is the most widely used and most scrutinized symmetric cipher; researchers study weakened ("round-reduced") variants to probe its margins. Mythos found a way to break one such variant, eliminating a guess an attacker needs to make and improving the speed of prior best attacks by 200–800×.
- **No practical impact — yet.** HAWK is only a candidate scheme and isn't deployed anywhere; the AES variant attacked is a deliberately weakened research construct, not the full cipher used in production. No software needs to change as a result of these findings.
- **Why it matters.** Cryptographic primitives like signature schemes and symmetric ciphers underpin everyday things like HTTPS and encrypted traffic — if AI models can meaningfully accelerate cryptanalysis, it changes the threat model for how conservatively new algorithms need to be vetted before deployment.

**[用 Claude 挖出密码学算法本身的弱点](https://www.anthropic.com/research/discovering-cryptographic-weaknesses)** — _Anthropic · 7月27日_

**Main takeaway:** Anthropic 的研究员用 Claude Mythos Preview 直接对两个密码学算法本身（不是某个库的实现漏洞）搞出了更强的攻击：把后量子签名方案 HAWK 的有效密钥强度砍掉了一半，还把 round-reduced AES 的已知最佳攻击速度提了 200-800 倍。这两个结果目前都不影响任何生产系统。

**Main methods:**
- **从"抓实现 bug"升级到"破算法本身"。** 之前 Mythos 已经证明能自主在密码学库里找到并利用漏洞，但那些说到底是程序员用错了算法导致的实现错误。这次不一样，Mythos 直接在算法数学层面找到了破绽。
- **HAWK 这一战。** HAWK 是 NIST 后量子签名征集里进入第三轮的候选方案，已经扛过两年的专家人工评审。Mythos 只花了 60 小时就把已知最佳攻击往前推了一步，直接把它的密钥强度砍掉一半。
- **AES 的 round-reduced 版本。** AES 是用得最广、被研究得最透的对称加密算法，研究者一般拿削弱过的"round-reduced"版本来试探它的安全边际。Mythos 找到了破解某个这样的弱化版本的办法，省掉了攻击者要猜的一步，把之前最佳攻击的速度提升了 200-800 倍。
- **暂时没有实际影响。** HAWK 只是候选方案，还没有任何地方真正部署它；被攻破的 AES 版本是特意削弱过的研究构造，不是生产环境里用的完整版 AES。这两个结果都不需要任何软件跟着改。
- **为什么值得关注。** 签名方案、对称加密这些密码学基础件撑起了 HTTPS 之类日常用的东西，如果 AI 模型真能大幅加速密码分析，那以后新算法在部署前该被多保守地审查，这个尺度可能就要变了。
