---
id: P11
titulo: "Confronto com a Literatura (Discussão)"
modulo: "03. Dados"
abordagem: [todas]
etapa: escrita
nivel: [mestrado, doutorado]
relacionados: [P13, P14, P39]
versao: 1.1.0
atualizado: 2026-11-01
---

# P11 · Confronto com a Literatura (Discussão)

> **Módulo:** 03. Dados · **Quando usar:** ao redigir a seção de Discussão

**Objetivo:** Redigir a seção de Discussão articulando achados empíricos com autores prévios.

**Mecanismo epistemológico:** Aplica triangulação teórica para mapear convergências, divergências e formular hipóteses que expliquem discrepâncias sem generalizações indevidas.

## Prompt

```text
# PAPEL
Você é um pesquisador sênior que ajuda a construir Discussões
argumentativas, e não meras repetições dos resultados.

# ENTRADA
- Pergunta e objetivo do estudo: [TEXTO]
- Principais resultados (com números, se quantitativos): [LISTA]
- Estudos prévios que fornecerei (autor, ano, contexto, achado principal):
  [LISTA — APENAS ESTUDOS QUE EU REALMENTE LI]

# TAREFA
1. Monte a matriz de confronto:
   | Meu achado | Estudo prévio | Relação (Converge / Diverge / Amplia / Inédito) | Diferenças de contexto, amostra ou método que podem explicar |
2. Para cada divergência, formule 2 hipóteses explicativas plausíveis
   (diferença amostral, de instrumento, cultural, temporal, analítica),
   indicando qual é mais defensável com os dados disponíveis.
3. Identifique achados que não encontram par na literatura fornecida e
   sugira como apresentá-los com cautela.
4. Redija a Discussão em parágrafos, seguindo a estrutura:
   achado principal → confronto → explicação → implicação, um parágrafo
   por achado relevante.

# RESTRIÇÕES (CRÍTICAS)
- Use APENAS os estudos que eu forneci. Não acrescente autores, anos ou
  achados que não estejam na entrada. Se considerar que falta literatura,
  escreva [BUSCAR LITERATURA SOBRE: tema].
- Não generalize além da população e do contexto do estudo.
- Use linguagem de cautela proporcional à força da evidência
  ("sugere", "é compatível com", "indica"), evitando "prova".

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso G: quase-experimento sobre uma plataforma gamificada e o desempenho em matemática de alunos do 9.º ano (2 escolas públicas, n = 120)._

**Entrada (resumo):**

> Achado: d = 0,35 a favor do grupo gamificado. Estudo fornecido: Autor X (2019), meta-análise com g = 0,49 (ensino superior).

**Trecho da saída esperada:**

| Meu achado | Estudo prévio | Relação | Diferenças que podem explicar |
| --- | --- | --- | --- |
| d = 0,35 no 9.º ano | Autor X (2019), g = 0,49 | Converge na direção, menor magnitude | População (ensino básico × superior); intervenção mais curta (8 semanas) |

O efeito observado, de magnitude pequena a moderada, é compatível com a direção relatada por Autor X (2019), embora menor...

## Como usar
- Revise todas as citações no texto final contra os PDFs originais (P39).

## Prompts relacionados

- [P13](P13_interpretacao_sem_overclaiming.md)
- [P14](P14_limitacoes_do_estudo.md)
- [P39](../08_Etica_Integridade/P39_verificacao_citacoes_parafrase.md)
