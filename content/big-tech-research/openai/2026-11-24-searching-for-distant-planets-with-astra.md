---
title: "Searching for distant planets with Astra"
date: 2026-11-24
draft: false
tags: ["big-tech-research", "openai"]
---

**[Searching for distant planets with Astra](https://openai.com/index/searching-for-distant-planets-with-astra)** — _OpenAI · Nov 24_

**Main takeaway:** A user story: two amateur astronomers used Codex and Astra to hunt for exoplanet transits in public Kepler and TESS data, and both produced candidates that professional astronomers are now checking. An astronomer at the SETI Institute independently recovered two of one searcher's Kepler signals, and one of the other's strongest candidates is queued for further TESS analysis.

**Main methods:**
- **Transit detection framed as a coding problem.** A planet crossing in front of its star dips the measured brightness; find a dip that recurs at regular intervals in the light curve and you have a candidate. Astronomers have published methods for pulling faint recurring dips out of years of measurements, so the work is largely about implementing and tuning them.
- **Kevin Bond's Codex search.** Bond, an engineer at OpenAI who came to astronomy through night-sky photography, used Codex to compare published detection methods, combine them into one search program, and test whether code changes actually improved the search — then ran it over observations of roughly 100,000 Kepler stars (mission ran 2009–2018).
- **Ethan Byrd's Astra search.** Byrd, founder of the email-infrastructure start-up Primitive, worked independently and tried several AI models before settling on Astra to analyze telescope data covering about 19 million stars.
- **Both handed results to professionals rather than claiming discoveries.** Bond went to a SETI Institute astronomer, whose independent search turned up two of the same Kepler signals. Byrd sent a top candidate to researchers on NASA's TESS mission, where it is in line for further analysis, with two more candidates awaiting submission.
- **Prior art this builds on.** In 2017, researchers trained a neural network on 15,000 already-vetted Kepler signals to learn which starlight patterns most likely came from a planet; applied to weaker signals, it led them to an eighth planet around Kepler-90.
- **Why the leftovers matter.** More than 6,400 exoplanets have been confirmed since 1992, and amateurs have long been part of that search — these tools aim them at datasets whose obvious signals have already been harvested.

**[两个业余天文爱好者用 Codex 和 Astra 翻公开数据找系外行星](https://openai.com/index/searching-for-distant-planets-with-astra)** — _OpenAI · 11月24日_

**Main takeaway:** 这是篇用户故事：两个业余天文爱好者分别用 Codex 和 Astra，在 Kepler 和 TESS 的公开数据里找系外行星的 transit 信号，各自都挖出了候选目标，现在交给专业天文学家在核。SETI Institute 的一位天文学家独立搜了一遍，把其中一人在 Kepler 数据里找到的两个信号也找了出来；另一人最强的那个候选已经排队等 TESS 那边进一步分析。

**Main methods:**
- **找 transit 说到底是个编程问题。** 行星从恒星前面过去的时候，测到的亮度会掉一点点；如果 light curve 上这个凹坑按固定间隔反复出现，就是个候选。怎么从好几年的观测里把这种微弱又重复的凹坑捞出来，天文学界已经有公开的方法，所以活儿主要落在实现和调参上。
- **Kevin Bond 这边用 Codex。** 他是 OpenAI 的工程师，因为爱拍星空入了天文的坑。他让 Codex 把已发表的几种检测方法横向比了一遍，拼成一个搜索程序，还逐版验证改代码到底有没有让搜索变好，最后扫了 Kepler 大约 10 万颗恒星的观测数据（Kepler 这个任务跑了 2009 到 2018 年）。
- **Ethan Byrd 这边用 Astra。** 他是邮件基础设施创业公司 Primitive 的创始人，跟 Bond 互不相干，试了好几个模型之后选了 Astra，处理的望远镜数据覆盖约 1,900 万颗恒星。
- **两人都没自己宣布发现，而是把结果交出去。** Bond 找了 SETI Institute 的天文学家，对方独立搜了一遍，在 Kepler 数据里也命中了同样的两个信号。Byrd 把一个最强的候选发给了 NASA TESS 任务的研究人员，已经在排队做进一步分析，另外两个候选还没提交。
- **这事儿之前就有先例。** 2017 年有人拿 15,000 个天文学家已经看过的 Kepler 信号训了个神经网络，让它学哪种亮度变化最像行星；再拿去看那些更弱的信号，结果顺着查到了 Kepler-90 的第八颗行星。
- **为什么值得在"别人剩下的数据"里翻。** 1992 年以来已经确认了 6,400 多颗系外行星，业余爱好者一直是这场搜索的一部分。这类工具正好让他们去啃那些明显信号早被收割完的数据集。
