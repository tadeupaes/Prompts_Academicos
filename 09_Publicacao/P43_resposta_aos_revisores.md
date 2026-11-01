---
id: P43
titulo: "Resposta aos Revisores (Rebuttal)"
modulo: "09. Publicação"
abordagem: [todas]
etapa: submissão
nivel: [mestrado, doutorado]
relacionados: [P06, P13]
versao: 1.1.0
atualizado: 2026-11-01
---

# P43 · Resposta aos Revisores (Rebuttal)

> **Módulo:** 09. Publicação · **Quando usar:** após receber um parecer de Minor/Major Revision

**Objetivo:** Organizar e redigir uma resposta ponto a ponto, cortês e técnica, que aumente a chance de aceitação.

**Mecanismo epistemológico:** Decompõe o parecer em comentários atômicos, classifica cada um (aceitar, aceitar parcialmente, contestar com argumento) e exige que cada resposta indique a alteração concreta e sua localização no manuscrito.

## Prompt

```text
# PAPEL
Você é um coautor experiente em processos de revisão por pares.

# ENTRADA
- Pareceres dos revisores e do editor: [COLE]
- Manuscrito (ou seções relevantes): [COLE]
- Minhas reações iniciais a cada comentário: [OPCIONAL]

# TAREFA
1. Decomponha os pareceres em comentários numerados (R1.1, R1.2, R2.1...)
   e classifique:
   | ID | Comentário (resumo) | Tipo (método, análise, teoria, escrita, formatação) | Decisão sugerida (Aceitar / Aceitar parcialmente / Contestar) | Esforço (baixo/médio/alto) |
2. Para comentários a contestar, verifique se há base real (ex.: o revisor
   leu errado, a sugestão está fora do escopo) e construa o argumento técnico.
3. Redija a carta de resposta:
   - Agradecimento breve ao editor e revisores.
   - Para cada comentário: comentário original (em itálico) → resposta →
     alteração feita, com página/linha → trecho novo citado.
4. Monte um checklist de alterações a fazer no manuscrito.

# RESTRIÇÕES
- Nunca afirme ter feito uma alteração que ainda não foi feita; marque
  [ALTERAÇÃO A FAZER].
- Tom cordial e firme; sem defensividade nem subserviência.
- Não invente referências para atender a pedidos dos revisores.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso G: quase-experimento sobre uma plataforma gamificada e o desempenho em matemática de alunos do 9.º ano (2 escolas públicas, n = 120)._

**Entrada (resumo):**

> Revisor 1, comentário 1: "O delineamento não permite inferência causal."

**Trecho da saída esperada:**

**R1.1** _O delineamento não permite inferência causal._

**Resposta:** Agradecemos a observação e concordamos. Reformulamos o título, o resumo e a conclusão, substituindo "melhora" por "associa-se a", e incluímos a ANCOVA com o pré-teste como covariável (seção 3.5).

**Alteração:** p. 9, linhas 210–224. [ALTERAÇÃO A FAZER]

## Prompts relacionados

- [P06](../02_Persona/P06_revisor_ad_hoc_q1.md)
- [P13](../03_Dados/P13_interpretacao_sem_overclaiming.md)
