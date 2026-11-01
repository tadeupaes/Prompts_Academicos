---
id: P20
titulo: "Protocolo de Revisão de Escopo (PCC / PRISMA-ScR)"
modulo: "04. Revisão de Literatura"
abordagem: [revisão]
etapa: planejamento
nivel: [mestrado, doutorado]
relacionados: [P02, P18]
versao: 1.1.0
atualizado: 2026-11-01
---

# P20 · Protocolo de Revisão de Escopo (PCC / PRISMA-ScR)

> **Módulo:** 04. Revisão de Literatura · **Quando usar:** quando o objetivo é mapear um campo amplo ou emergente, e não responder a uma pergunta de efeito

**Objetivo:** Planejar uma *scoping review* com pergunta, critérios e plano de extração adequados.

**Mecanismo epistemológico:** Aplica o framework PCC (População, Conceito, Contexto) do JBI e a extensão PRISMA-ScR, diferenciando claramente a revisão de escopo da revisão sistemática (mapeamento × síntese de efeito).

## Prompt

```text
# PAPEL
Você é um metodólogo especializado em revisões de escopo segundo o manual
do JBI (Peters et al.) e o PRISMA-ScR (Tricco et al., 2018).

# ENTRADA
- Tema que desejo mapear: [TEMA]
- Motivo do mapeamento: [EX.: campo emergente, conceito difuso, preparar uma RSL]

# TAREFA
1. Confirme se a revisão de escopo é o tipo adequado ou se outro tipo
   (sistemática, integrativa, rápida, umbrella) seria mais adequado. Justifique.
2. Defina o PCC:
   | Elemento | Definição | Incluir | Excluir |
3. Redija a pergunta principal e de 2 a 4 subperguntas de mapeamento.
4. Proponha fontes: bases indexadas, literatura cinzenta, repositórios de
   teses (ex.: Catálogo de Teses e Dissertações da CAPES, BDTD).
5. Monte o formulário de extração de dados (campos e definição de cada um).
6. Proponha como apresentar os resultados (mapa de evidências, tabelas,
   gráficos de frequência, síntese narrativa).

# RESTRIÇÕES
- Lembre que revisões de escopo normalmente não avaliam risco de viés;
  se eu quiser fazê-lo, explique as implicações.
- Marque com [VERIFICAR] qualquer detalhe de diretriz sobre o qual tenha dúvida.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso R: revisão sobre intervenções baseadas em mindfulness para burnout em professores da educação básica._

**Entrada (resumo):**

> Objetivo: mapear como "bem-estar docente" vem sendo definido e medido nos estudos de intervenção.

**Trecho da saída esperada:**

A revisão de escopo é adequada, porque o objetivo é mapear conceitos e instrumentos, e não estimar efeito.

| Elemento | Definição | Incluir | Excluir |
| --- | --- | --- | --- |
| P | Professores da educação básica | Ensino infantil, fundamental e médio | Ensino superior |
| C | Conceituação e mensuração de bem-estar docente | Estudos que definem ou medem o construto | Estudos que só citam o termo |
| C | Intervenções em contexto escolar | Qualquer país | — |

## Prompts relacionados

- [P02](../01_Metodologia/P02_protocolo_prisma_pico.md)
- [P18](P18_matriz_de_sintese.md)
