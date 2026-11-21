# Rubrica SmartView — inteligência visível

> Um bom produto é como uma boa piada: não precisa ser explicado.
> O trabalho inteiro é **encurtar a distância entre o pensamento da pessoa e o resultado**.

A rubrica tem duas camadas que se usam juntas:

1. **Elemento** — as 6 perguntas, aplicadas a cada botão, campo, tela, aviso.
2. **Sistema** — 10 testes que olham o produto como um todo.

Ela serve igual para **diagnosticar um sistema pronto** (`diagnostico.md`) e para **escrever o plano/PRD** de um sistema novo (`prd-secao.md`).

---

## Camada 1 — as 6 perguntas por elemento

Para cada elemento visível, responda **sim (2) / mais ou menos (1) / não (0)**.

| # | Pergunta | O que conta como "sim" |
|---|----------|------------------------|
| E1 | **Um estranho sabe dizer o nome disso?** | Quem nunca viu o produto descreve o elemento com as próprias palavras, sem tutorial. |
| E2 | **Sabe o que acontece quando apertar?** | O rótulo diz a ação e o resultado ("Verificar este site"), não um verbo genérico ("Enviar"). |
| E3 | **O padrão está certo para a maioria?** | O valor que já vem preenchido serve para 8 em cada 10 pessoas; ninguém precisa mexer para começar. |
| E4 | **Reage de forma visível em um compasso?** | Algo muda na tela em até ~300 ms após a ação (estado, cor, texto, progresso). |
| E5 | **Cai onde prometeu?** | Depois da ação, a pessoa está exatamente onde o rótulo dizia que estaria. |
| E6 | **Alguém sentiria falta se sumisse?** | Se você tirar e ninguém reclamar, ninguém precisava. **Somar subtraindo.** |

Nota do elemento = soma ÷ 12 × 100. Elemento abaixo de 60 entra na lista de correção; elemento com **E6 = 0** entra na lista de **remoção**, não de melhoria.

---

## Camada 2 — 10 testes de sistema

| # | Teste | Como medir | Passa quando |
|---|-------|-----------|--------------|
| S1 | **5 segundos** | Mostre a primeira tela por 5 s a alguém de fora e pergunte "o que isso faz?" | A resposta bate com a sua promessa de uma linha. |
| S2 | **O produto entende o que recebeu** | Cole/envie tipos diferentes de entrada (link, arquivo, texto). | A interface muda o texto da ação para o tipo detectado ("Verificar este repositório", "Verificar este servidor") — reforça que aguenta o que você deu. |
| S3 | **Reação < 300 ms** | Cronometre do clique/colar até a primeira mudança visível. | Abaixo de 300 ms. Se a pessoa espera o botão mudar, você já explicou a piada. |
| S4 | **Espera que parece música de elevador** | Observe o tempo de processamento. | Há atividade visível e legível (lista de checagens marcando ✓ uma a uma, etapas nomeadas), não um spinner mudo. |
| S5 | **Prova antes do pedido** | Conte o que a pessoa ganha antes de pedir e-mail/cadastro. | Alguns segundos de atividade visível + um primeiro resultado parcial (um gancho aberto) **antes** de pedir o e-mail. |
| S6 | **Valor provado em 2 minutos** | Uma pessoa pouco técnica, sozinha, do zero. | Ela prova o valor para si mesma em menos de 2 min, com o menor número de cliques. |
| S7 | **Resultado escaneável e compartilhável** | Olhe a tela de resultado. | Número + nota + cor (ex.: 72 · B · âmbar). Dá para entender de relance e mandar print. |
| S8 | **Logado cai no "saguão"** | Entre como usuário já cadastrado. | Vai para o seu espaço (histórico, próximos passos), nunca de volta para a landing de venda. |
| S9 | **Cada caminho de login é dívida** | Liste as formas de entrar (Google, GitHub, e-mail+senha…). | Só as necessárias. Cada uma traz OAuth, troca de senha, termos, privacidade e cookies que precisam funcionar para sempre. |
| S10 | **Padrão emprestado, não inventado** | Compare componentes-chave com padrões já conhecidos. | Os padrões vêm de referências que já funcionam (galerias de componentes, sites premiados), escolhidas para o nicho — não do "padrão médio" do modelo nem inventados do zero. |

Cada teste: **passa (10) / parcial (5) / falha (0)**.

---

## Nota final — número + nota + cor

```
SmartView = 0,6 × média dos testes de sistema (0–100)
          + 0,4 × média das notas de elemento (0–100)
```

| Faixa | Nota | Cor | Leitura |
|-------|------|-----|---------|
| 90–100 | A | verde | Se explica sozinho. Mexer pouco. |
| 75–89 | B | verde-claro | Bom; alguns pontos de atrito. |
| 60–74 | C | âmbar | Funciona, mas pede explicação. |
| 40–59 | D | laranja | A pessoa precisa de tutorial para chegar ao valor. |
| 0–39 | E | vermelho | Recursos não vão salvar: um estranho não entende em 5 s. |

> Se um estranho não diz o que o produto faz em 5 segundos, nenhuma quantidade de recurso salva.
> **S1 = 0 limita a nota final a D**, qualquer que seja a soma.

---

## Hábitos que acompanham a rubrica

- **Mock antes de codar.** Gere a tela com um gerador de imagem a partir de um guia de marca curto (cores, fonte, tom) guardado no `AGENTS.md`/`CLAUDE.md` do projeto. Aprove a imagem, depois construa.
- **Simule os usuários antes de lançar.** Rode subagentes como personas (uma pessoa de 55 anos pouco técnica; um jovem de 20 anos com TDAH que testou 100 produtos esta semana) e peça que façam S1 e S6.
- **Não empilhe skills de design que brigam entre si.** Uma referência escolhida para o nicho vale mais que cinco regras genéricas.
- **Revisite sem vergonha.** O mesmo campo de entrada pode ser reescrito 20 vezes. Registre o que ainda não gosta em vez de fingir que está perfeito.
