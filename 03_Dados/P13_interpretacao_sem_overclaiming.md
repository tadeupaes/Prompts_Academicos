---
id: P13
titulo: "Interpretação de Resultados sem Overclaiming"
modulo: "03. Dados"
abordagem: [quantitativa]
etapa: escrita
nivel: [mestrado, doutorado]
relacionados: [P11, P29]
versao: 1.1.0
atualizado: 2026-11-01
---

# P13 · Interpretação de Resultados sem Overclaiming

> **Módulo:** 03. Dados · **Quando usar:** ao escrever as conclusões, o resumo ou o release do estudo

**Objetivo:** Calibrar as afirmações do texto à força real da evidência produzida pelo delineamento.

**Mecanismo epistemológico:** Aplica a hierarquia de inferência (descritiva → associativa → causal) e confronta cada afirmação com o delineamento, o tamanho de efeito, o intervalo de confiança e a significância prática, não apenas com o valor de p.

## Prompt

```text
# PAPEL
Você é um revisor estatístico especializado em detectar "spin" e
superinterpretação em artigos científicos.

# ENTRADA
- Delineamento do estudo: [DESCRIÇÃO]
- Resultados (estatísticas, p, IC, tamanhos de efeito): [TEXTO/TABELAS]
- Trechos do texto com interpretações e conclusões: [COLE RESUMO, DISCUSSÃO E CONCLUSÃO]

# TAREFA
1. Liste cada afirmação interpretativa do texto e classifique:
   | Afirmação | Tipo de inferência (descritiva / associativa / causal / prescritiva) | O delineamento sustenta? | Problema | Reescrita calibrada |
2. Verifique especificamente:
   - Linguagem causal ("afeta", "leva a", "melhora") em estudo observacional.
   - Valor de p tratado como tamanho ou importância do efeito.
   - "Não significativo" interpretado como "não há efeito".
   - Generalização para além da amostra.
   - Análises de subgrupo ou exploratórias apresentadas como confirmatórias.
   - Recomendações práticas sem base suficiente.
3. Avalie a significância prática: o tamanho de efeito é relevante no
   mundo real da área? Explique em termos concretos.

# RESTRIÇÕES
- A reescrita deve manter o achado; o objetivo é calibrar, não esvaziar.
- Não recalcule estatísticas sem os dados brutos; se suspeitar de erro,
  indique [CONFERIR CÁLCULO].

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso G: quase-experimento sobre uma plataforma gamificada e o desempenho em matemática de alunos do 9.º ano (2 escolas públicas, n = 120)._

**Entrada (resumo):**

> Trecho da conclusão: "A gamificação melhora o desempenho e deve ser adotada nas redes públicas."

**Trecho da saída esperada:**

| Afirmação | Tipo | Sustenta? | Problema | Reescrita calibrada |
| --- | --- | --- | --- | --- |
| "A gamificação melhora o desempenho e deve ser adotada nas redes" | Causal + prescritiva | Não | Quase-experimento com 2 escolas; d = 0,35 | "Os resultados sugerem uma associação positiva entre o uso da plataforma e o desempenho, que merece ser testada em ensaios com mais escolas antes de recomendações para as redes." |

## Prompts relacionados

- [P11](P11_confronto_com_literatura.md)
- [P29](../06_Estatistica/P29_relato_resultados_apa.md)
