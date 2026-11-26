# SmartView — visible intelligence

**🇧🇷 [Português](README.md) · 🇺🇸 [English](README.en.md) · 🇪🇸 [Español](README.es.md)**

[![SmartView — visible intelligence](guia/assets/banner-en.jpg)](https://linnoff88-dev.github.io/arckhe-/guia/en/)

## What it is

SmartView is a ready-to-copy text model that measures whether a digital product explains itself. It is for people who build systems, apps or websites, with or without AI agents. You can use it in two ways: as an **audit** of a system that already exists, or as a **PRD section** (the requirements document) for a system that is yet to be born. In the end you get a score with a number, a letter and a color, plus a short list of what to fix and what to remove. Nothing to install: just read and fill it in, or ask Claude Code or Codex to run the skill.

## 📖 User guide

Full guide (landing + step by step + score calculator): **https://linnoff88-dev.github.io/arckhe-/guia/en/**

## What's in here

| File | Purpose |
|------|---------|
| [`modelo/rubrica.md`](modelo/rubrica.md) (in Portuguese) | The 6 questions per element, the 10 system tests and the score (number + letter + color) |
| [`modelo/diagnostico.md`](modelo/diagnostico.md) (in Portuguese) | Template for auditing a finished system |
| [`modelo/prd-secao.md`](modelo/prd-secao.md) (in Portuguese) | Block to paste into the PRD/plan: 10 opportunity gates + experience requirements + done criterion |
| [`exemplos/diagnostico-exemplo.md`](exemplos/diagnostico-exemplo.md) (in Portuguese) | A filled-in audit (fictional system) |
| [`skill/smartview/SKILL.md`](skill/smartview/SKILL.md) | Skill for Claude Code / Codex to run the audit or write the PRD section |

## Quick start

```bash
git clone https://github.com/linnoff88-dev/smartview
cp -r smartview/skill/smartview ~/.claude/skills/   # Claude Code
cp -r smartview/skill/smartview ~/.agents/skills/   # Codex
```

Then, in the agent:

- `smartview audit of https://meusistema.com`
- `add the smartview section to docs/PRD.md`

## The idea in one sentence

> If a stranger can't say what your product does in 5 seconds, no amount of features will save it.

---

An open project of [ARCKHÉ AI](https://ARCKHÉ AI). MIT License.
