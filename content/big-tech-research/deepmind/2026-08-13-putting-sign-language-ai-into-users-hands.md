---
title: "Putting sign language AI into users' hands"
date: 2026-08-13
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Putting sign language AI into users' hands](https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/)** — _Google DeepMind · Aug 13_

**Main takeaway:** Google DeepMind is shipping SL2T, a massively multilingual sign-language-to-text translation model, into consumer products for the first time: it powers sign-to-text dictation in Gboard and Live Transcribe on Pixel 11, starting with American Sign Language to English.

**Main methods:**
- **What actually ships.** Deaf users can sign anywhere they'd normally type — searching the web, drafting messages and documents, asking Gemini to answer a query or run a task — and in Live Transcribe they can sign responses mid-conversation instead of typing back and forth. Testers report signing in ASL is faster and more natural than typing English.
- **Translation, not transcription.** Speech-to-text is a sequential mapping from sound to text within one language, whereas sign languages are independent natural languages with their own grammars and lexicons, so the model has to do true machine translation rather than sign-to-word substitution.
- **The perception problem.** Meaning is carried by simultaneous movements of the hands, arms, torso, head, and face, so the model must track fine-grained whole-body motion at high frame rates — a difficult and computationally demanding computer vision task.
- **Why earlier attempts were limited.** Devices like sign language gloves were fundamentally constrained because sign languages aren't "English on the hands"; capturing hand shape alone misses most of the signal.
- **The gap it targets.** Decades of progress in spoken-language AI have left out the world's 200+ sign languages and the estimated 70 million Deaf and hard of hearing people who use them.
- **Rollout caveat.** Today it's ASL to English on Pixel 11 only; DeepMind says more devices are coming soon and additional languages will follow, without giving a timeline.

**[手语 AI 第一次装进手机：SL2T 上线 Pixel 11](https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/)** — _Google DeepMind · 8月13日_

**Main takeaway:** Google DeepMind 放出了 SL2T，一个覆盖多种手语的 sign-language-to-text 翻译模型，并且第一次把手语 AI 装进了消费级产品：Pixel 11 上 Gboard 和 Live Transcribe 的手语转文字就是它在跑，第一版做的是 ASL 转英文。

**Main methods:**
- **实际能拿来干什么。** 以前要打字的地方现在都能直接比手语：搜网页、写消息和文档、让 Gemini 查东西或者执行任务。Live Transcribe 里也能直接用手语回话，不用来回打字。测试用户说比打英文更快、也更自然。
- **这是 translation，不是 transcription。** 语音转文字只是在同一种语言里把声音顺着映射成文字，而手语是有自己语法和词汇的独立语言，所以模型得做真正的 machine translation，不能一个手势换一个词。
- **难点在"看懂"。** 手语的意思是手、胳膊、躯干、头和面部同时动出来的，模型要在高帧率下把这些细节全跟住，computer vision 这块的开销很大。
- **早年那些方案为什么不行。** 手语手套之类的东西天生受限，因为手语根本不是"把英语打在手上"，只抓手型会漏掉绝大部分信息。
- **这个空白有多大。** 语音那边的 AI 已经推进了几十年，全世界 200 多种手语、大约 7000 万使用手语的 Deaf 和听障人群基本没被覆盖到。
- **不过有一点要说。** 目前只有 Pixel 11 上的 ASL 转英文，官方说更多设备很快跟上、更多语言后面会加，但没给时间表。
