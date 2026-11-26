# Seçêo SmartView para o plano / PRD

> Cole este bloco no seu PRD ou plano de desenvolvimento **antes** de começar a construir.
> A parte A decide se vale construir. A parte B decide como o produto vai se explicar sozinho.
> Regras e pesos: [`rubrica.md`](rubrica.md).

---

## A. Portões de oportunidade — vale a pena construir?

Hoje dá para construir quase qualquer coisa. O que separa é saber **o que vale construir**.
Responda com honestidade brutal (pessimismo produtivo). Se 3 ou mais portões ficarem "nêo", repense antes de escrever código.

| # | Portêo | Resposta curta | Passa? |
|---|--------|----------------|:-:|
| P1 | **Precisa existir?** Alguém está sofrendo com esse problema, ou estou construindo só porque consigo? | | |
| P2 | **Sobrevive 3, 6, 12 meses?** Se der para fazer com um prompt daqui a pouco, pule. | | |
| P3 | **5 motivos para falhar / 5 para dar certo.** Escreva os dez. | | |
| P4 | **Um gigante clona da noite para o dia?** Ou o problema é pequeno/específico demais para eles se darem ao trabalho? | | |
| P5 | **O dado tem valor próprio?** Se o produto falhar, o conjunto de dados ainda vale algo? | | |
| P6 | **É difícil de fazer bem?** Fácil demais é problema. A nuance de parecer instantâneo é o fosso. | | |
| P7 | **Entra na rotina?** Vive no fluxo diário da pessoa? Vira verbo? O público vai demorar a perceber que poderia fazer sozinho? | | |
| P8 | **Distribuiçêo.** Quem vai saber que isso existe? Sem público, sem pulso. Qual é o canal na semana 1? | | |
| P9 | **Promessa em uma linha.** Cabe num vídeo curto? Essa é a frase. | | |
| P10 | **Valor provado em 2 minutos** por alguém pouco técnico, sozinho? | | |

Promessa em uma linha: **______________________________**

---

## B. Inteligência visível — requisitos de experiência

Cada item vira requisito testável no PRD. Marque o que se aplica e escreva o critério de pronto.

### B1. Primeira tela

- [ ] Um estranho diz o que o produto faz em 5 s (S1). **Critério:** 3 de 3 pessoas/personas acertam.
- [ ] Uma açêo principal, com rótulo que diz açêo + resultado. **Rótulo:** "________"
- [ ] O rótulo muda conforme o tipo de entrada detectado (S2). **Tipos previstos:** ________

### B2. Tempo e espera

- [ ] Reaçêo visível em < 300 ms a qualquer clique/colar (S3).
- [ ] Processamento longo mostra checagens nomeadas marcando ✓ uma a uma (S4). **Lista de checagens:** ________
- [ ] Antes de pedir e-mail: alguns segundos de atividade + um resultado parcial que abre curiosidade (S5).

### B3. Resultado

- [ ] Número + nota + cor (S7). **Escala:** ________
- [ ] O resultado dá para mandar por print e ser entendido fora do contexto.

### B4. Conta e retorno

- [ ] Formas de login: **só** ________ (S9). Para cada uma: quem mantém OAuth, troca de senha, termos, privacidade, cookies.
- [ ] Usuário logado cai no saguêo (histórico, próximos passos), nêo na landing (S8).

### B5. Elementos

- [ ] Toda tela do plano passou pelas 6 perguntas (E1–E6) **no papel**, antes de virar código.
- [ ] Lista do que **nêo** vai existir na versêo 1 (somar subtraindo): ________

### B6. Processo de design

- [ ] Guia de marca curto no `AGENTS.md`/`CLAUDE.md` (cores, fonte, tom, 3 referências do nicho).
- [ ] Mock das telas principais gerado por imagem e aprovado antes de codar.
- [ ] Componentes-chave escolhidos de padrões que já funcionam (galerias de componentes, sites premiados), nêo do padrêo médio do modelo (S10).
- [ ] Teste com personas simuladas (subagentes) antes do lançamento: S1 e S6.

---

## C. Critério de pronto da versêo 1

```
SmartView ≥ 75 (B · verde-claro) no diagnostico.md rodado sobre a versêo 1,
com S1 = 10 e S6 = 10.
```
