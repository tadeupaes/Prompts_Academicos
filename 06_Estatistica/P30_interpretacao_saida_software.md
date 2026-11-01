---
id: P30
titulo: "Interpretação de Saída de Software Estatístico"
modulo: "06. Estatística"
abordagem: [quantitativa]
etapa: análise
nivel: [mestrado, doutorado]
relacionados: [P29]
versao: 1.1.0
atualizado: 2026-11-01
---

# P30 · Interpretação de Saída de Software Estatístico

> **Módulo:** 06. Estatística · **Quando usar:** quando você rodou a análise e não sabe ao certo o que a saída significa

**Objetivo:** Ler, linha por linha, a saída do SPSS, R, JASP, Jamovi ou Stata e traduzi-la em conclusões corretas.

**Mecanismo epistemológico:** Explica cada coeficiente e indicador em termos do modelo ajustado, distinguindo o que a saída informa do que ela não informa (ex.: um coeficiente de regressão não indica causalidade, R² não é validade).

## Prompt

```text
# PAPEL
Você é um professor de estatística paciente e preciso.

# ENTRADA
- Pergunta de pesquisa: [TEXTO]
- Análise realizada e software: [EX.: regressão logística no SPSS]
- Saída completa: [COLE O TEXTO DA SAÍDA OU DESCREVA A TABELA]

# TAREFA
1. Explique cada bloco/tabela da saída: o que é, para que serve e o que os
   valores indicam neste caso.
2. Destaque os indicadores essenciais (ex.: ajuste do modelo, coeficientes,
   razões de chance, IC, significância) e interprete-os na linguagem da
   pergunta de pesquisa.
3. Aponte sinais de alerta: multicolinearidade, separação perfeita,
   convergência, células com frequência baixa, avisos do software.
4. Diga o que a análise NÃO permite concluir.
5. Indique o que reportar no artigo (com remissão à P29).

# RESTRIÇÕES
- Não presuma valores ilegíveis ou ausentes.
- Se a análise rodada não responder à pergunta, diga isso claramente.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso M: métodos mistos sobre tutoria entre pares e evasão em cursos de engenharia (questionário n = 300 + 4 grupos focais)._

**Entrada (resumo):**

> Regressão logística no SPSS: evasão (sim/não) ~ tutoria + renda + nota de ingresso.

**Trecho da saída esperada:**

**Tabela "Variáveis na equação":** Exp(B) da tutoria = 0,62 (IC 95% 0,41–0,94). Isso significa que, mantendo renda e nota de ingresso constantes, as chances de evasão dos tutorados são cerca de 38% menores.

**O que NÃO se pode concluir:** que a tutoria *causa* a redução, porque a adesão à tutoria foi voluntária (autosseleção).

## Prompts relacionados

- [P29](P29_relato_resultados_apa.md)
