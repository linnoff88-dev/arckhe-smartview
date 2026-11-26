ï»¿# SmartView ê¢â¬â inteligêÂªncia visêÂ­vel

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


**ê°Å¸â¡Â§ê°Å¸â¡Â· [PortuguêÂªs](README.md) êÂ· ê°Å¸â¡Âºê°Å¸â¡Â¸ [English](README.en.md) êÂ· ê°Å¸â¡Âªê°Å¸â¡Â¸ [EspaêÂ±ol](README.es.md)**

[![SmartView ê¢â¬â inteligêÂªncia visêÂ­vel](guia/assets/banner.jpg)](https://linnoff88-dev.github.io/arckhe-/guia/)

## O que êÂ©

SmartView êÂ© um modelo em texto, pronto para copiar, que mede se um produto digital se explica sozinho. Serve para quem cria sistemas, apps ou sites, com ou sem agentes de IA. VocêÂª usa de dois jeitos: como **diagnêÂ³stico** de um sistema que jêÂ¡ existe, ou como **seêÂ§êÂ£o do PRD** (o documento de requisitos) de um sistema que ainda vai nascer. No fim sai uma nota com nêÂºmero, letra e cor, e uma lista curta do que corrigir e do que remover. NêÂ£o precisa instalar nada: êÂ© sêÂ³ ler e preencher, ou pedir para o Claude Code ou o Codex rodar a skill.

## ê°Å¸ââ Guia de uso

Guia completo (landing + passo a passo + calculadora de nota): **https://linnoff88-dev.github.io/arckhe-/guia/**

## O que tem aqui

| Arquivo | Para quêÂª |
|---------|----------|
| [`modelo/rubrica.md`](modelo/rubrica.md) | As 6 perguntas por elemento, os 10 testes de sistema e a nota (nêÂºmero + letra + cor) |
| [`modelo/diagnostico.md`](modelo/diagnostico.md) | Modelo para auditar um sistema pronto |
| [`modelo/prd-secao.md`](modelo/prd-secao.md) | Bloco para colar no PRD/plano: 10 portêÂµes de oportunidade + requisitos de experiêÂªncia + critêÂ©rio de pronto |
| [`exemplos/diagnostico-exemplo.md`](exemplos/diagnostico-exemplo.md) | DiagnêÂ³stico preenchido (sistema fictêÂ­cio) |
| [`skill/smartview/SKILL.md`](skill/smartview/SKILL.md) | Skill para Claude Code / Codex rodar o diagnêÂ³stico ou escrever a seêÂ§êÂ£o do PRD |

## Uso rêÂ¡pido

```bash
git clone https://github.com/linnoff88-dev/smartview
cp -r smartview/skill/smartview ~/.claude/skills/   # Claude Code
cp -r smartview/skill/smartview ~/.agents/skills/   # Codex
```

Depois, no agente:

- `diagnêÂ³stico smartview de https://meusistema.com`
- `adiciona a seêÂ§êÂ£o smartview no docs/PRD.md`

## A ideia em uma frase

> Se um estranho nêÂ£o diz o que o seu produto faz em 5 segundos, nenhuma quantidade de recurso salva.

---

Projeto aberto do [ARCKHÉ AI](https://ARCKHÉ AI). LicenêÂ§a MIT.

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>