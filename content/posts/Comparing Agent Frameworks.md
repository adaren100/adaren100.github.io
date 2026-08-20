---
title: "Comparing Agent Frameworks: OpenClaw, Hermes, and DeepSeek"
date: 2026-08-19
draft: false
tags:
---

## Key components

### OpenClaw

 OpenClaw has two layers:
- **The workspace** contains persona, user context, operating rules, memories, daily notes, skills, and project files.
- **The state** directory contains runtime configuration, credentials, per-agent state, session stores, transcripts, logs, and trajectory exports.

**OpenClaw Architecture:**

```text
├── Workspace
│   ├── SOUL.md
│   ├── USER.md
│   ├── AGENTS.md
│   ├── MEMORY.md
│   ├── memory/YYYY-MM-DD.md
│   └── skills/
│
└── State directory
    ├── config
    ├── credentials
    ├── agent state
    ├── sessions
    ├── transcripts
    ├── logs
    └── trajectory exports
```

OpenClaw defines its roles, tones, and personality by using SOUL, USER, AGENTS, accompanied by daily memory, long-term memory, and state. This setup enables it behave like a considerate personal assistant. 

Compared to Hermes, OpenClaw emphasizes the importance of memory. It includes daily notes (memory) and long-term memory. 
https://docs.openclaw.ai/concepts/memory

### Hermes

Hermes emphasizes the importance of skills. It has a mechanism to **create, patch, edit, and delete skills**, along with writing and removing supporting a skill's supporting files. 

They also have a token efficient way to retrieve skills.

```text
Level 0: skills_list()           → [{name, description, category}, ...]   (~3k tokens)
Level 1: skill_view(name)        → Full content + metadata                (varies)
Level 2: skill_view(name, path)  → Specific reference file                (varies)
```


**Hermes architecture**:

```text
~/.hermes/
├── SOUL.md
├── memories/
│   ├── MEMORY.md
│   └── USER.md
├── skills/
├── sessions/
├── state.db
├── cron/
├── logs/
├── workspace/
├── home/
├── config.yaml
├── .env
└── auth.json
```


**Hermes skills**

```text
~/.hermes/skills/
├── category/
│   └── skill-name/
│       ├── SKILL.md
│       ├── references/
│       ├── templates/
│       ├── scripts/
│       ├── examples/
│       └── assets/
├── .hub/
└── .bundled_manifest
```


After execution of each task, Hermes runs a post-task review, and then writes the facts into Memory and workflows into skills.

### DeepSeek Harness

```text
Model
+ Agent Loop
+ Tools
+ Skills
+ Sessions
+ Storage / Memory
+ Sandbox
+ Scheduler
+ UI
= Agent Runtime
```

DeepSeek harness was released after the others. It is natural to introduce more flexible assembling paradigms. Developers can choose which components to include, based on questions such as:
- How the **agent loop** plans, calls tools, retries, and terminates, and whether to add a review agent, verifier, or memory writer? 
- Whether **memory** should use Markdown, a database, a vector store, or custom storage.
- Whether **skills** should be static documents, dynamically generated modules, or versioned code.
- **Session and Workspace**: How **sessions** are stored and resumed, and how tools and code are isolated through **sandboxes**.

 It could implement a workspace-memory design similar to OpenClaw or a task-review and skill-distillation loop similar to Hermes.

### Conclusion

**OpenClaw**

```text
= Workspace + Memory + Session + Trajectory
  with a strong personal-assistant continuity model
```

**Hermes**

```text
= Memory + Session + Agent Loop + Skill Learning
  with a strong experience-distillation model
```

**DeepSeek Harness**

```text
= Pluggable Session + Storage + Memory + Tools + Loops + Skills
  with a strong runtime-composability model
```

所以简单来说， OpenClaw 通过workspace 和 memory 记住你们曾经的所有对话，所以act like a personal assistant。 就是让人觉得是那种悟性比较好的，说一次就记住的好助理。
Hermes就像那种学霸，不停的维护ta的错题本和答案本。
DeepSeek Harness 是lego，是工程化抽象化的工厂，可以组装定制各自想要的流程。
