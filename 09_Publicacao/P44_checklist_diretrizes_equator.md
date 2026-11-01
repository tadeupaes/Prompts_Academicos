---
id: P44
titulo: "Checklist de Diretrizes de Relato (EQUATOR)"
modulo: "09. Publicação"
abordagem: [todas]
etapa: submissão
nivel: [mestrado, doutorado]
relacionados: [P02, P19, P34]
versao: 1.1.0
atualizado: 2026-11-01
---

# P44 · Checklist de Diretrizes de Relato (EQUATOR)

> **Módulo:** 09. Publicação · **Quando usar:** antes da submissão, quando o periódico exige diretriz de relato

**Objetivo:** Identificar a diretriz de relato adequada ao delineamento e verificar a conformidade do manuscrito item a item.

**Mecanismo epistemológico:** Usa a rede EQUATOR para associar delineamento e diretriz (CONSORT, STROBE, PRISMA, COREQ, SRQR, STARD, CARE, SPIRIT, ARRIVE, CHEERS, GRAMMS) e aplica o checklist com localização exata de cada item no texto.

## Prompt

```text
# PAPEL
Você é um editor de método que verifica conformidade com diretrizes de relato.

# ENTRADA
- Delineamento do estudo: [TEXTO]
- Manuscrito completo: [COLE]

# TAREFA
1. Indique a diretriz principal (e extensões, se houver) para este
   delineamento e justifique.
2. Aplique o checklist:
   | Item | Descrição (resumida) | Atendido? (Sim/Parcial/Não) | Seção/parágrafo onde aparece | O que falta |
3. Liste os itens não atendidos em ordem de importância e sugira a redação.
4. Indique se a diretriz exige fluxograma (ex.: CONSORT, PRISMA) e o que
   deve constar nele.

# RESTRIÇÕES
- Se não tiver certeza da redação exata ou da numeração de um item, marque
  [CONFERIR NO CHECKLIST OFICIAL — equator-network.org].
- Diretriz de relato não é ferramenta de avaliação de qualidade; não as confunda.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso Q: estudo qualitativo com 14 entrevistas com enfermeiras da Atenção Primária sobre a teleconsulta._

**Entrada (resumo):**

> Manuscrito qualitativo com entrevistas.

**Trecho da saída esperada:**

Diretriz: COREQ, que é específica para entrevistas e grupos focais. A SRQR é a alternativa para outros delineamentos qualitativos.

| Item | Atendido? | Onde | O que falta |
| --- | --- | --- | --- |
| Relação prévia com os participantes | Não | — | Declarar se a pesquisadora trabalhava nas unidades |
| Duração das entrevistas | Sim | Método, §3 | — |

## Prompts relacionados

- [P02](../01_Metodologia/P02_protocolo_prisma_pico.md)
- [P19](../04_Revisao_Literatura/P19_avaliacao_qualidade_estudos.md)
- [P34](../07_Pesquisa_Qualitativa/P34_criterios_rigor_qualitativo.md)
