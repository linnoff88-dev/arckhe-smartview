# SmartView â€” inteligÃªncia visÃ­vel

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


**ðŸ‡§ðŸ‡· [PortuguÃªs](README.md) Â· ðŸ‡ºðŸ‡¸ [English](README.en.md) Â· ðŸ‡ªðŸ‡¸ [EspaÃ±ol](README.es.md)**

[![SmartView â€” inteligÃªncia visÃ­vel](guia/assets/banner.jpg)](https://inematds.github.io/smartview/guia/)

## O que Ã©

SmartView Ã© um modelo em texto, pronto para copiar, que mede se um produto digital se explica sozinho. Serve para quem cria sistemas, apps ou sites, com ou sem agentes de IA. VocÃª usa de dois jeitos: como **diagnÃ³stico** de um sistema que jÃ¡ existe, ou como **seÃ§Ã£o do PRD** (o documento de requisitos) de um sistema que ainda vai nascer. No fim sai uma nota com nÃºmero, letra e cor, e uma lista curta do que corrigir e do que remover. NÃ£o precisa instalar nada: Ã© sÃ³ ler e preencher, ou pedir para o Claude Code ou o Codex rodar a skill.

## ðŸ“– Guia de uso

Guia completo (landing + passo a passo + calculadora de nota): **https://inematds.github.io/smartview/guia/**

## O que tem aqui

| Arquivo | Para quÃª |
|---------|----------|
| [`modelo/rubrica.md`](modelo/rubrica.md) | As 6 perguntas por elemento, os 10 testes de sistema e a nota (nÃºmero + letra + cor) |
| [`modelo/diagnostico.md`](modelo/diagnostico.md) | Modelo para auditar um sistema pronto |
| [`modelo/prd-secao.md`](modelo/prd-secao.md) | Bloco para colar no PRD/plano: 10 portÃµes de oportunidade + requisitos de experiÃªncia + critÃ©rio de pronto |
| [`exemplos/diagnostico-exemplo.md`](exemplos/diagnostico-exemplo.md) | DiagnÃ³stico preenchido (sistema fictÃ­cio) |
| [`skill/smartview/SKILL.md`](skill/smartview/SKILL.md) | Skill para Claude Code / Codex rodar o diagnÃ³stico ou escrever a seÃ§Ã£o do PRD |

## Uso rÃ¡pido

```bash
git clone https://github.com/inematds/smartview
cp -r smartview/skill/smartview ~/.claude/skills/   # Claude Code
cp -r smartview/skill/smartview ~/.agents/skills/   # Codex
```

Depois, no agente:

- `diagnÃ³stico smartview de https://meusistema.com`
- `adiciona a seÃ§Ã£o smartview no docs/PRD.md`

## A ideia em uma frase

> Se um estranho nÃ£o diz o que o seu produto faz em 5 segundos, nenhuma quantidade de recurso salva.

---

Projeto aberto do [INEMA.CLUB](https://inema.club). LicenÃ§a MIT.

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>