# 摸摸头 (PatPat) | AI Co-Regulation Skill for Kids

[![GitHub license](https://img.shields.io/github/license/gglinux/patpat-skill)](https://github.com/gglinux/patpat-skill/blob/main/LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/gglinux/patpat-skill)](https://github.com/gglinux/patpat-skill/stargazers)

**PatPat (摸摸头)** is an AI-powered interactive storybook skill for kids aged 3-8. It transforms negative emotional moments into magical, choice-based narratives that focus on **Co-regulation** and **Interoception**.

「摸摸头 (PatPat)」是一款面向 3-8 岁儿童的 AI 互动绘本技能书。它将负面情绪时刻转化为基于选择的魔法故事，核心关注**共同调节 (Co-regulation)** 与**躯体觉察 (Interoception)**。

---

## ✨ Key Features | 核心特性

- **Externalization (叙事外化)**: Emotions are personified as "Emotion Creatures" (e.g., Sparky the Fire 🔥).
- **Interoception Mapping (躯体映射)**: Connecting abstract feelings to physical sensations (e.g., hot palms, tight tummy).
- **Co-regulation (共同调节)**: Empowering parents to be the regulator for the child, providing specific sync actions.
- **De-stigmatization (去道德化)**: Validating natural impulses while guiding towards adaptive behaviors.

---

## 🛠️ Repository Structure | 仓库结构

- `SKILL.md`: The core logic and instructions for AI Agents (English Optimized).
- `logic/story-engine.md`: JSON Schema and narrative rules for interactive stories.
- `logic/emotion-creatures.md`: Mapping of emotions to physical sensations and visual states.
- `logic/parent-coach.md`: Scaffolding guide for parents (Self-rescue & Sync actions).

---

## 🤖 Usage | 如何使用

This skill is designed to be ingested by advanced LLMs (like GPT-4, DeepSeek, Claude). It provides a structured brain for generating emotional regulation content.

该技能旨在被大语言模型吸收，为生成情绪调节内容提供结构化的“大脑”。

1.  **Ingest** the `SKILL.md` into your Agent's system prompt.
2.  **Refer** to the `logic/` folder for specific protocol constraints.
3.  **Generate** JSON output for front-end rendering (Web/Mini Program).

---

## 📄 License | 开源协议

MIT License. Copyright (c) 2026 gglinux.
