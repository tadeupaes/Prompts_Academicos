---
id: P35
titulo: "Saturação e Amostragem em Pesquisa Qualitativa"
modulo: "07. Pesquisa Qualitativa"
abordagem: [qualitativa]
etapa: planejamento
nivel: [mestrado, doutorado]
relacionados: [P31, P34]
versao: 1.1.0
atualizado: 2026-11-01
---

# P35 · Saturação e Amostragem em Pesquisa Qualitativa

> **Módulo:** 07. Pesquisa Qualitativa · **Quando usar:** ao justificar o número de participantes ou decidir quando parar a coleta

**Objetivo:** Justificar a amostra qualitativa com critérios transparentes, e não com um número arbitrário.

**Mecanismo epistemológico:** Diferencia os modelos de saturação (teórica, temática indutiva, temática a priori e de dados; Saunders et al., 2018), a saturação de código e de significado (Hennink; Kaiser; Marconi, 2017) e o conceito de poder de informação (Malterud et al., 2016), exigindo evidência documentada do critério de encerramento.

## Prompt

```text
# PAPEL
Você é metodólogo qualitativo e revisor de projetos.

# ENTRADA
- Abordagem: [EX.: teoria fundamentada, fenomenologia, análise temática]
- Objetivo e amplitude do estudo: [TEXTO]
- Perfil e acessibilidade da população: [TEXTO]
- Estratégia de amostragem: [INTENCIONAL / BOLA DE NEVE / TEÓRICA / OUTRA]
- N previsto ou já coletado: [N]

# TAREFA
1. Avalie se a estratégia de amostragem é coerente com a abordagem.
2. Explique qual conceito de saturação ou de poder de informação se aplica
   ao estudo e por quê.
3. Proponha um procedimento verificável para documentar a saturação
   (ex.: tabela de novos códigos por entrevista, critério de parada
   definido a priori).
4. Analise o poder de informação considerando: objetivo amplo/estreito,
   especificidade da amostra, uso de teoria, qualidade do diálogo e
   estratégia de análise.
5. Redija o parágrafo de justificativa da amostra.

# RESTRIÇÕES
- Não afirme números "padrão" de entrevistas como regra.
- Não use "atingimos a saturação" sem descrever como foi verificada.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso Q: estudo qualitativo com 14 entrevistas com enfermeiras da Atenção Primária sobre a teleconsulta._

**Entrada (resumo):**

> Análise temática reflexiva; amostragem intencional; 14 entrevistas.

**Trecho da saída esperada:**

Na análise temática reflexiva, Braun & Clarke criticam o uso de "saturação de dados". O poder de informação (Malterud et al., 2016) é mais coerente com a abordagem.

Poder de informação: objetivo estreito (+), amostra específica (+), diálogo denso (+), análise em profundidade (+). Isso sustenta uma amostra moderada. Justifique a amostra por esses critérios, e não por "atingimos a saturação".

## Prompts relacionados

- [P31](P31_roteiro_entrevista.md)
- [P34](P34_criterios_rigor_qualitativo.md)
