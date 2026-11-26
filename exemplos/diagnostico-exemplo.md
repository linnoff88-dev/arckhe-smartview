# Diagnóstico SmartView — exemplo preenchido

> Exemplo **ilustrativo** (sistema fictício) para mostrar como fica o modelo preenchido.
> Modelo em branco: [`../modelo/diagnostico.md`](../modelo/diagnostico.md).

## 0. Identificaçêo

| Campo | Valor |
|-------|-------|
| Sistema | "Checa Link" — verificador de segurança de sites (fictício) |
| Endereço | checalink.exemplo |
| Data | 2026-10-11 |
| Quem avaliou | agente com a skill smartview + 3 personas |
| Promessa em uma linha | "Antivírus para o seu site feito com IA" |
| Público principal | quem publicou um site/app feito com agente e nêo é de segurança |

## 1. Teste dos 5 segundos (S1)

| Pessoa | O que disse | Bate? |
|--------|-------------|-------|
| 55 anos, pouco técnica | "É um site que testa se o meu site está seguro" | sim |
| 20 anos, impaciente | "Scanner de vulnerabilidade, cola o link" | sim |
| Especialista | "Teste de segurança automático, mas nêo sei o que ele testa" | parcial |

## 2. Caminho até o primeiro valor

| Passo | Pessoa faz | Tela responde | Reaçêo | Pede algo? |
|-------|-----------|---------------|--------|-----------|
| 1 | Cola o link de um repositório | Botêo continua "Verificar site" | — | nêo |
| 2 | Clica | Spinner sem texto por 14 s | 900 ms | nêo |
| 3 | — | Tela de cadastro antes de qualquer resultado | — | **e-mail + senha** |

- Cliques até o valor: 5 (com cadastro) · Tempo: 2 min 40 s
- Antes do e-mail: nada visível
- Espera: spinner mudo

## 3. Elementos

| Elemento | E1 | E2 | E3 | E4 | E5 | E6 | Nota | Decisêo |
|----------|:-:|:-:|:-:|:-:|:-:|:-:|:-:|---------|
| Campo "Cole o link" | 2 | 2 | 2 | 1 | 2 | 2 | 92 | manter |
| Botêo "Verificar site" | 2 | 1 | 2 | 0 | 1 | 2 | 67 | corrigir: mudar o texto pelo tipo de link |
| Aba "Integrações" | 1 | 0 | 1 | 2 | 1 | 0 | 42 | **remover** |
| Login com 4 provedores | 2 | 2 | 1 | 2 | 2 | 1 | 83 | reduzir para 2 |

## 4. Testes de sistema

| Teste | Nota | Evidência |
|-------|:-:|-----------|
| S1 | 5 | 2 de 3 acertaram |
| S2 | 0 | botêo nêo muda com link de repositório |
| S3 | 0 | 900 ms até o spinner |
| S4 | 0 | spinner sem texto |
| S5 | 0 | cadastro antes de qualquer resultado |
| S6 | 0 | 2 min 40 s |
| S7 | 10 | resultado "72 · B · verde-claro" |
| S8 | 5 | logado cai na landing com banner "entrar no painel" |
| S9 | 5 | 4 provedores |
| S10 | 10 | resultado e lista seguem padrêo de antivírus conhecido |

## 5. Nota

| Componente | Valor |
|------------|-------|
| Sistema | 35 |
| Elementos | 71 |
| **SmartView** | 0,6 × 35 + 0,4 × 71 = **49** |
| **Nota e cor** | **49 · D · laranja** |

## 6. Plano de correçêo

| # | O quê | Melhora | Esforço | Ganho |
|---|-------|---------|:-:|-------|
| 1 | Mostrar 8 s de checagens nomeadas e o 1º achado antes de pedir e-mail | S4, S5, S6 | M | alto |
| 2 | Botêo muda para "Verificar este repositório" ao detectar o tipo em < 300 ms | S2, S3, E2, E4 | P | alto |
| 3 | Logado vai para o histórico de verificações | S8 | P | médio |
| 4 | Ficar só com Google + e-mail | S9 | P | médio |
| 5 | Linha "o que testamos" abaixo do campo | S1 | P | médio |

### Remover

- Aba "Integrações" (ninguém clicou em 30 dias)

### O que ainda nêo gosto

- O nome das abas do painel ainda nêo diz o que tem dentro.
