---
title: "How Claude’s text watermark works"
date: 2026-08-14
draft: false
tags: ["big-tech-research", "anthropic"]
---

**[How Claude’s text watermark works](https://www.anthropic.com/news/claude-text-watermark)** — _Anthropic · Aug 14_

**Main takeaway:** Future Claude models will emit watermarked text — a statistical pattern in word choice that lets anyone holding the key assign a probability that Claude wrote a given passage. It's a compliance move for the EU AI Act, and other major developers who signed the same Code of Practice will ship their own watermarks.

**Main methods:**
- **The watermark rides on low-stakes word choices.** A model picks one word at a time from a list of candidates, and for something like "The weather today was cold and…" it doesn't much matter to the reader whether "overcast" or "grey" comes next. Normally that tie is settled by a random number; watermarking swaps out the source of that randomness.
- **The key plus preceding words decide the pick.** Instead of an arbitrary random number generator, the method combines a key with the few words that came before to settle the next word. Anyone with the key can then check whether the observed word sequence is consistent with the choices Claude would have made under that key, and assign a probability that Claude generated it.
- **Nothing is added to the text.** No hidden characters, no extra tokens, and no extra cost — the signal lives entirely in which of several roughly equally likely words gets selected.
- **No standing bias, no odd vocabulary.** The model isn't permanently tilted toward "overcast" or "grey"; which one appears still depends on the preceding words. The scheme also won't push Claude toward a word it wouldn't have considered anyway, Anthropic's example being the obscure synonym "nubilous".
- **The watermark carries no identifying information.** It can't be traced to a specific person, organization, or chat — it only speaks to whether Claude was involved in producing the text.
- **Why now, and who else.** As of August 2 the EU requires AI providers serving its market to mark AI-generated content, and other major model developers signed the same Code of Practice. Anthropic says output quality is unaffected and that a watermarked response is indistinguishable to a reader from an unwatermarked one.

**[Claude 的文字水印是怎么做的](https://www.anthropic.com/news/claude-text-watermark)** — _Anthropic · 8月14日_

**Main takeaway:** 以后的 Claude 模型吐出来的文字会带水印，本质是在选词上留下一个统计模式，手里有 key 的人可以据此算出这段话由 Claude 写出来的概率有多大。这么做是为了满足 EU AI Act，签了同一份 Code of Practice 的其他几家大厂也会各自上自己的水印。

**Main methods:**
- **水印藏在"选哪个词都行"的地方。** LLM 是一个词一个词往外蹦的，碰到 "The weather today was cold and…" 这种，接 overcast 还是 grey 对读者没什么差别，平时就靠一个随机数定下来。水印做的事情，就是把这个随机数的来源换掉。
- **改成用 key 加前文来决定选哪个词。** 不再用任意的随机数生成器，而是拿 key 和前面几个词一起算出这一步该选谁。这样有 key 的人回头把整段的词序列对一遍，看它跟"Claude 用这把 key 时会做的选择"对不对得上，就能给出一个概率。
- **文字本身没多加任何东西。** 没有隐藏字符，不额外吃 token，也不会更贵。整个水印就体现在几个概率差不多的词里最后挑了哪个。
- **不会固定偏向某个词，也不会蹦生僻词。** 模型不是从此就爱写 overcast 或者 grey，具体选哪个还是看前文。这套方法也不会逼 Claude 去选一个它本来压根不会考虑的词，Anthropic 举的例子是 nubilous 这种冷门同义词。
- **水印不带任何身份信息。** 它追不到具体是谁、哪家机构、哪一段对话，只能说明 Claude 有没有参与写这段文字。
- **为什么是现在，以及还有谁。** 8月2日起，EU 要求在其市场提供服务的 AI 厂商标记 AI 生成内容，其他几家主要模型厂商也签了同一份 Code of Practice。Anthropic 说输出质量不受影响，读者拿到带水印和不带水印的回答，是分不出区别的。
