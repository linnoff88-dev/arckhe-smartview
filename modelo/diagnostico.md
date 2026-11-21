# Diagnóstico SmartView — sistema pronto

> Use quando o sistema já existe (no ar ou rodando local). Preencha de cima para baixo.
> Regras e pesos: [`rubrica.md`](rubrica.md).

## 0. Identificação

| Campo | Valor |
|-------|-------|
| Sistema | |
| Endereço / pasta | |
| Data | |
| Quem avaliou | (pessoa ou agente) |
| Promessa em uma linha | ("antivírus para apps feitos com IA" é melhor que "o Uber de X") |
| Público principal | |

## 1. Teste dos 5 segundos (S1)

Mostre a primeira tela por 5 s a 3 pessoas de fora (ou 3 personas simuladas).

| Pessoa | O que ela disse que o produto faz | Bate com a promessa? |
|--------|-----------------------------------|----------------------|
| 1 | | sim / parcial / não |
| 2 | | |
| 3 | | |

## 2. Caminho até o primeiro valor (S3, S4, S5, S6)

Faça o caminho como uma pessoa nova. Anote cada passo.

| Passo | O que a pessoa faz | O que a tela responde | Tempo até reagir | Pede algo? (e-mail, login, cartão) |
|-------|--------------------|-----------------------|------------------|-------------------------------------|
| 1 | | | ms | |
| 2 | | | | |
| 3 | | | | |

- Cliques até o primeiro valor real: **___**
- Tempo total até o valor: **___ s** (meta < 120 s)
- O que a pessoa recebe **antes** de pedir o e-mail: ___
- A espera mostra atividade legível ou só um spinner? ___

## 3. Inventário de elementos (E1–E6)

Liste os elementos da tela principal (botões, campos, abas, avisos). 2 = sim, 1 = mais ou menos, 0 = não.

| Elemento | E1 nome | E2 ação | E3 padrão | E4 reage | E5 cai onde prometeu | E6 faria falta | Nota (÷12×100) | Decisão |
|----------|:-:|:-:|:-:|:-:|:-:|:-:|:-:|---------|
| | | | | | | | | manter / corrigir / **remover** |
| | | | | | | | | |
| | | | | | | | | |

> E6 = 0 → **remover**, não melhorar.

## 4. Testes de sistema (S1–S10)

| Teste | Resultado (10 / 5 / 0) | Evidência (print, tempo, observação) |
|-------|:-:|------|
| S1 5 segundos | | |
| S2 entende o que recebeu | | |
| S3 reação < 300 ms | | |
| S4 espera legível | | |
| S5 prova antes do pedido | | |
| S6 valor em 2 min | | |
| S7 número + nota + cor | | |
| S8 logado cai no saguão | | |
| S9 caminhos de login mínimos | | |
| S10 padrão emprestado | | |

## 5. Nota

| Componente | Valor |
|------------|-------|
| Média dos testes de sistema (×10 → 0–100) | |
| Média das notas de elemento | |
| **SmartView** (0,6 × sistema + 0,4 × elementos) | |
| Trava S1 = 0 → máximo D? | sim / não |
| **Nota e cor** | ex.: **68 · C · âmbar** |

## 6. Plano de correção (máximo 7 itens, ordem de impacto)

| # | O quê | Teste/elemento que melhora | Esforço (P/M/G) | Ganho esperado |
|---|-------|----------------------------|-----------------|----------------|
| 1 | | | | |
| 2 | | | | |
| 3 | | | | |

### Remover (somar subtraindo)

- 

### O que ainda não gosto (honestidade registrada)

- 
