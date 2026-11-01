---
id: P28
titulo: "Verificação de Pressupostos Estatísticos"
modulo: "06. Estatística"
abordagem: [quantitativa]
etapa: análise
nivel: [mestrado, doutorado]
relacionados: [P26, P29]
versao: 1.1.0
atualizado: 2026-11-01
---

# P28 · Verificação de Pressupostos Estatísticos

> **Módulo:** 06. Estatística · **Quando usar:** antes de rodar a análise principal

**Objetivo:** Planejar e interpretar a verificação dos pressupostos do modelo escolhido e decidir o que fazer quando eles são violados.

**Mecanismo epistemológico:** Prioriza o diagnóstico gráfico e a robustez do modelo sobre testes formais isolados (ex.: Shapiro-Wilk com N grande), conectando cada violação à consequência sobre o erro tipo I/II e a uma solução proporcional.

## Prompt

```text
# PAPEL
Você é um estatístico aplicado que ensina análise de dados a pós-graduandos.

# ENTRADA
- Modelo/teste que pretendo usar: [EX.: ANOVA de 2 fatores, regressão linear múltipla, regressão logística]
- Características dos dados: [N, distribuição, outliers, dados faltantes]
- Resultados dos diagnósticos (se já rodou): [COLE SAÍDAS, DESCREVA GRÁFICOS]

# TAREFA
1. Liste os pressupostos do modelo em tabela:
   | Pressuposto | Como verificar (gráfico + teste) | Consequência se violado | Solução proporcional |
2. Interprete os diagnósticos que forneci e diga quais pressupostos parecem
   atendidos, violados ou inconclusivos.
3. Recomende a decisão: manter o modelo, aplicar correção (ex.: Welch,
   erros-padrão robustos), transformar, usar alternativa não paramétrica,
   bootstrap ou outro modelo (ex.: modelo linear generalizado).
4. Indique como tratar outliers e dados faltantes de forma transparente
   (sem excluir casos "para melhorar o resultado").
5. Redija o parágrafo de relato da verificação para a seção de método.

# RESTRIÇÕES
- Não interprete gráficos que não foram descritos ou enviados.
- Explique a limitação de testes de normalidade com amostras grandes ou pequenas.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso G: quase-experimento sobre uma plataforma gamificada e o desempenho em matemática de alunos do 9.º ano (2 escolas públicas, n = 120)._

**Entrada (resumo):**

> Resíduos com assimetria leve; 2 outliers no pós-teste; 8% de dados faltantes no pós.

**Trecho da saída esperada:**

| Pressuposto | Situação | Decisão |
| --- | --- | --- |
| Normalidade dos resíduos | Assimetria leve; com n = 120 o modelo é robusto | Manter; relatar o gráfico Q-Q |
| Outliers | 2 casos com |resíduo| > 3 | Análise de sensibilidade com e sem os casos; não excluir sem justificativa |
| Dados faltantes | 8% no pós-teste | Comparar quem respondeu com quem não respondeu; considerar imputação múltipla |

## Prompts relacionados

- [P26](P26_escolha_teste_estatistico.md)
- [P29](P29_relato_resultados_apa.md)
