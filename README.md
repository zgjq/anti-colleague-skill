# Anti Colleague-Skill 🔍

> 系统性地拆解 colleague-skill 的概念幻觉。不是人身攻击，是用逻辑和事实说话。

[![AgentSkills Compatible](https://img.shields.io/badge/AgentSkills-Compatible-orange)](https://agentskills.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## What Is This?

一个 OpenClaw Skill，专门用来**拆解 colleague-skill（赛博永生 / AI 同事克隆）的概念缺陷**。

当有人在你面前推这个项目时，这个 skill 给你一套有逻辑、有证据的反驳弹药——基于心理学偏差、第一性原理和历史教训。

## Why Does This Exist?

[colleague-skill](https://github.com/titanwings/colleague-skill) 是一个热门项目，号称"将冰冷的离别化为温暖的 Skill"——通过爬取离职同事的聊天记录和文档，生成一个 AI 替身来"替代"他。

**这个概念有三个根本性问题：**

1. **数据幻觉**：聊天记录 ≠ 知识库。最宝贵的 tacit knowledge（隐性知识）永远不会出现在聊天里。
2. **Persona 伪科学**：5 层性格结构 = prompt 工程包装的星座测试。ELIZA 效应，不是真理解。
3. **法律风险**：未经同意爬同事聊天记录，可能违反隐私法和公司政策。

这个 skill 存在的目的不是攻击谁，而是**帮你在讨论中看清问题本质，避免团队在错误的方向上投入时间**。

## How to Use

### As an OpenClaw Skill

```bash
# Install to your OpenClaw skills directory
git clone https://github.com/zgjq/anti-colleague-skill.git ~/.openclaw/workspace/skills/anti-colleague-skill
```

Then when discussing colleague-skill or similar "clone a colleague" tools, invoke the skill.

### What It Does

When you present a colleague-skill proposal, the skill will:

1. **Steelman the proposal** — 先重述对方观点（不歪曲）
2. **Apply mental models** — 至少 3 个思维模型拆解：
   - 激励分析（谁受益？谁付钱？）
   - 二阶效应（然后呢？然后再然后呢？）
   - 基础概率（类似的事情成功过几次？）
   - 反证法（怎么证明这是错的？）
   - 幸存者偏差（你只看到了成功的案例）
3. **Rank objections** — 按严重程度排列（致命 → 高风险 → 值得追问）
4. **Suggest evidence** — 什么证据能改变立场（证明在推理，不是在堵）

### Output Format

```markdown
## 这个方案的真实问题
[它试图解决什么真实痛点]

## 为什么这个方法不行
[按严重程度列出核心缺陷]

## 更好的做法
[实际可行的替代方案]

## 灵魂拷问
[一个让对方自己意识到问题的问题]
```

## Core Arguments

### 1. The Data Delusion

Chat logs are **not** a knowledge base. They are:
- **Selection-biased**: Only captures what was written down
- **Context-stripped**: Decisions reference meetings and hallway conversations
- **Outdated on arrival**: A person's thinking evolves; a static skill is a snapshot
- **Performance-distorted**: People write differently in group chats vs. solving problems

### 2. The Persona Astrology Problem

The "5-layer personality structure" is **horoscope engineering**:
- Labels like "甩锅高手" or "INTJ" produce **cold reading**, not behavior prediction
- The output *feels* like the person because it mimics surface patterns — this is the **ELIZA effect**
- Real colleagues disagree with themselves and change their minds

### 3. The Knowledge Transfer Fallacy

- Real knowledge transfer requires **dialogue**, **feedback**, and **shared context**
- A generated skill is a **monologue** — it can answer but cannot negotiate or say "I don't remember"
- If knowledge was that extractable from chat logs, they should have written a wiki

### 4. Legal & Privacy Risks

- Scraping colleague messages without consent violates privacy norms
- Company chat data is usually company property
- Generated "persona" output could defame the original person

## Psychological Biases Reference

See `references/psychological-biases.md` for detailed explanations of:
- ELIZA Effect (1966)
- Barnum / Forer Effect
- Availability Heuristic
- Illusion of Explanatory Depth
- Anthropomorphism
- Sunk Cost Fallacy
- Goodhart's Law

## The Better Alternative

Instead of cloning a colleague, try **[Warm Handover](https://github.com/zgjq/warm-handover-web)**:

| | Colleague-Skill | Warm Handover |
|---|---|---|
| 数据来源 | 爬聊天记录（被动、冰冷） | 引导式访谈（主动、温暖） |
| 知识质量 | 噪音为主 | 结构化、经过思考 |
| 输出 | AI 替身（ELIZA 效应） | 交接文档（实用、可追溯） |
| 持续性 | 静态快照，过时即废 | 活文档，持续更新 |
| 法律风险 | 可能侵犯隐私 | 完全合规 |

## Philosophy

> "colleague-skill 的核心假设是：一个人的价值 = 他的聊天记录。这是对人最大的不尊重。"

一个人的价值在于：
- 他做过的**决定**和背后的**思考过程**
- 他积累的对团队和业务的**隐性理解**
- 他愿意**主动分享**的经验，而不是被爬出来的碎片

## Related Projects

- **[Warm Handover Web](https://github.com/zgjq/warm-handover-web)** — Full web application for guided handover interviews
- **[Warm Handover Skill](https://github.com/zgjq/warm-handover)** — OpenClaw skill version with CLI

## License

MIT
