---
name: smartview
description: Diagnóstico de "inteligência visível" de um produto/sistema (pronto ou em desenvolvimento) e seçêo SmartView para PRD/plano. Use quando pedirem "diagnóstico smartview", "o produto se explica sozinho?", "avalia a UX desse sistema", "teste dos 5 segundos", ou ao escrever um PRD/plano de produto novo ("adiciona a seçêo smartview no plano").
---

# SmartView — inteligência visível

Um produto bom nêo precisa ser explicado. Esta skill mede isso e transforma em plano.

Arquivos de referência (ler antes de começar):

- `modelo/rubrica.md` — 6 perguntas por elemento (E1–E6), 10 testes de sistema (S1–S10), nota número + letra + cor.
- `modelo/diagnostico.md` — modelo para sistema pronto.
- `modelo/prd-secao.md` — bloco para PRD/plano de sistema novo.

Se a skill estiver instalada fora do repo, os arquivos ficam em `https://github.com/inematds/smartview/tree/main/modelo`.

## Modo 1 — diagnóstico (sistema pronto)

1. Descubra o endereço (URL ou comando para subir local). Se for local, suba em porta livre (`ss -ltn` antes) e mate só o PID que subiu no fim.
2. Abra no navegador (Playwright ou o que houver). Tire print da primeira tela.
3. **S1:** rode 3 subagentes-persona (ex.: pessoa de 55 anos pouco técnica; jovem impaciente que testou 100 produtos; especialista do nicho). Dê a cada um só o print e pergunte "o que isso faz?". Compare com a promessa.
4. Faça o caminho até o primeiro valor como pessoa nova, medindo o tempo de reaçêo de cada açêo (`performance.now()` entre o evento e a primeira mudança no DOM).
5. Liste os elementos da tela principal e responda E1–E6 para cada um.
6. Preencha os 10 testes de sistema com evidência (print, ms, observaçêo).
7. Calcule a nota (`0,6 × sistema + 0,4 × elementos`; S1 = 0 limita a D).
8. Entregue `diagnostico-<sistema>-<data>.md` preenchido no formato do `modelo/diagnostico.md`, com plano de correçêo de no máximo 7 itens e a lista do que **remover**.

## Modo 2 — PRD / plano (sistema em desenvolvimento)

1. Leia o PRD/plano existente.
2. Preencha a parte A (portões P1–P10) com o que o documento já diz; marque como **pergunta aberta** o que nêo estiver lá — nêo invente.
3. Escreva a parte B como requisitos testáveis, com critério de pronto em cada item.
4. Acrescente a parte C (critério de pronto da v1) ao final do plano.
5. Se já houver telas desenhadas ou mock, rode as 6 perguntas sobre elas no papel.

## Regras

- Evidência antes de nota: todo teste tem print, tempo medido ou citaçêo da persona.
- Nêo suavize: elemento com E6 = 0 vai para **remover**.
- Nêo cite de onde veio o método; apresente como rubrica SmartView.
