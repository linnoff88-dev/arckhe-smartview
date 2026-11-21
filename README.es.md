# SmartView — inteligencia visible

**🇧🇷 [Português](README.md) · 🇺🇸 [English](README.en.md) · 🇪🇸 [Español](README.es.md)**

[![SmartView — inteligencia visible](guia/assets/banner-es.jpg)](https://inematds.github.io/smartview/guia/es/)

## Qué es

SmartView es un modelo en texto, listo para copiar, que mide si un producto digital se explica solo. Sirve para quien crea sistemas, apps o sitios, con o sin agentes de IA. Lo usas de dos maneras: como **diagnóstico** de un sistema que ya existe, o como **sección del PRD** (el documento de requisitos) de un sistema que aún va a nacer. Al final sale una nota con número, letra y color, y una lista corta de lo que hay que corregir y de lo que hay que quitar. No necesitas instalar nada: basta leer y completar, o pedirle a Claude Code o a Codex que ejecute la skill.

## 📖 Guía de uso

Guía completa (landing + paso a paso + calculadora de nota): **https://inematds.github.io/smartview/guia/es/**

## Qué hay aquí

| Archivo | Para qué sirve |
|---------|----------------|
| [`modelo/rubrica.md`](modelo/rubrica.md) (en portugués) | Las 6 preguntas por elemento, las 10 pruebas de sistema y la nota (número + letra + color) |
| [`modelo/diagnostico.md`](modelo/diagnostico.md) (en portugués) | Modelo para auditar un sistema terminado |
| [`modelo/prd-secao.md`](modelo/prd-secao.md) (en portugués) | Bloque para pegar en el PRD/plan: 10 compuertas de oportunidad + requisitos de experiencia + criterio de terminado |
| [`exemplos/diagnostico-exemplo.md`](exemplos/diagnostico-exemplo.md) (en portugués) | Diagnóstico completado (sistema ficticio) |
| [`skill/smartview/SKILL.md`](skill/smartview/SKILL.md) (en portugués) | Skill para que Claude Code / Codex ejecute el diagnóstico o escriba la sección del PRD |

## Uso rápido

```bash
git clone https://github.com/inematds/smartview
cp -r smartview/skill/smartview ~/.claude/skills/   # Claude Code
cp -r smartview/skill/smartview ~/.agents/skills/   # Codex
```

Después, en el agente:

- `diagnóstico smartview de https://meusistema.com`
- `agrega la sección smartview al docs/PRD.md`

## La idea en una frase

> Si un extraño no dice qué hace tu producto en 5 segundos, ninguna cantidad de funciones lo salva.

---

Proyecto abierto de [INEMA.CLUB](https://inema.club). Licencia MIT.
