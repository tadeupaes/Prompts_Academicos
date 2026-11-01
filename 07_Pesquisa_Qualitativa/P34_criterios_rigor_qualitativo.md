---
id: P34
titulo: "Critérios de Rigor Qualitativo (Lincoln & Guba / COREQ)"
modulo: "07. Pesquisa Qualitativa"
abordagem: [qualitativa]
etapa: revisão do método
nivel: [mestrado, doutorado]
relacionados: [P32, P35, P44]
versao: 1.1.0
atualizado: 2026-11-01
---

# P34 · Critérios de Rigor Qualitativo (Lincoln & Guba / COREQ)

> **Módulo:** 07. Pesquisa Qualitativa · **Quando usar:** ao revisar o método de um estudo qualitativo antes da defesa ou submissão

**Objetivo:** Auditar a confiabilidade de um estudo qualitativo e a completude do seu relato.

**Mecanismo epistemológico:** Aplica os critérios de *trustworthiness* (credibilidade, transferibilidade, dependabilidade, confirmabilidade) de Lincoln & Guba (1985) e o checklist COREQ (32 itens) de Tong, Sainsbury & Craig (2007).

## Prompt

```text
# PAPEL
Você é revisor especializado em pesquisa qualitativa.

# ENTRADA
- Seção de método completa: [COLE]
- Tipo de dado: [ENTREVISTAS / GRUPOS FOCAIS / OBSERVAÇÃO / DOCUMENTOS]

# TAREFA
1. Avalie os critérios de trustworthiness:
   | Critério | Estratégias esperadas (ex.: triangulação, member checking, descrição densa, trilha de auditoria, reflexividade) | Presente no texto? | Trecho | Recomendação |
2. Verifique os 3 domínios do COREQ (equipe e reflexividade; desenho do
   estudo; análise e achados), apontando os itens ausentes.
3. Avalie a coerência entre paradigma declarado, abordagem e procedimentos
   (ex.: falar em "viés" e "neutralidade" em estudo construtivista).
4. Liste as 5 inserções mais importantes no texto, com sugestão de redação.

# RESTRIÇÕES
- Não aplique critérios positivistas (validade, generalização estatística)
  a estudos interpretativos sem explicar a incompatibilidade.
- Marque [VERIFICAR] se não tiver certeza da redação exata de um item do COREQ.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso Q: estudo qualitativo com 14 entrevistas com enfermeiras da Atenção Primária sobre a teleconsulta._

**Entrada (resumo):**

> Seção de método do Caso Q.

**Trecho da saída esperada:**

| Critério | Estratégia esperada | Presente? | Recomendação |
| --- | --- | --- | --- |
| Confirmabilidade | Trilha de auditoria, diário reflexivo | Não | Descrever como as decisões analíticas foram registradas |
| Credibilidade | Member checking ou validação com pares | Parcial | Explicitar quem revisou os temas e como as divergências foram tratadas |

COREQ, domínio 1: falta informar a relação prévia da pesquisadora com as participantes.

## Prompts relacionados

- [P32](P32_analise_tematica.md)
- [P35](P35_saturacao_amostragem.md)
- [P44](../09_Publicacao/P44_checklist_diretrizes_equator.md)
