---
id: P14
titulo: "Seção de Limitações"
modulo: "03. Dados"
abordagem: [todas]
etapa: escrita
nivel: [mestrado, doutorado]
relacionados: [P13, P15]
versao: 1.1.0
atualizado: 2026-11-01
---

# P14 · Seção de Limitações

> **Módulo:** 03. Dados · **Quando usar:** ao redigir as limitações da dissertação, tese ou artigo

**Objetivo:** Redigir limitações honestas, específicas e acompanhadas de seu impacto e das estratégias de mitigação.

**Mecanismo epistemológico:** Trata a limitação como parte do argumento científico: identifica a ameaça à validade, estima a direção provável do viés e diferencia limitações que restringem a generalização das que ameaçam a conclusão.

## Prompt

```text
# PAPEL
Você é um metodólogo que considera uma boa seção de limitações sinal de
maturidade científica, e não de fraqueza.

# ENTRADA
- Resumo do método (desenho, amostra, instrumentos, análise): [TEXTO]
- Principais conclusões: [TEXTO]
- Limitações que eu já identifiquei: [LISTA]

# TAREFA
1. Complete a lista de limitações, considerando: amostragem, aferição,
   delineamento, análise, contexto temporal/geográfico, papel do
   pesquisador (no caso qualitativo) e dados faltantes.
2. Para cada limitação, preencha:
   | Limitação | Ameaça à validade | Direção provável do viés (super/subestima/incerta) | Impacto na conclusão (Alto/Médio/Baixo) | O que foi feito para mitigar | Sugestão para estudos futuros |
3. Redija a seção em texto corrido (3 a 5 parágrafos), começando pelas
   limitações de maior impacto.

# RESTRIÇÕES
- Evite limitações genéricas ("tamanho da amostra pequeno") sem
  especificar a consequência.
- Não liste como limitação algo que seja, na verdade, uma escolha de
  escopo deliberada; nesse caso, chame de delimitação.
- Não minimize limitações de alto impacto.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso Q: estudo qualitativo com 14 entrevistas com enfermeiras da Atenção Primária sobre a teleconsulta._

**Entrada (resumo):**

> Limitação já identificada: "amostra pequena".

**Trecho da saída esperada:**

| Limitação | Ameaça | Direção provável do viés | Impacto | Mitigação | Estudos futuros |
| --- | --- | --- | --- | --- | --- |
| Participantes indicadas pelas gestoras das unidades | Credibilidade e transferibilidade | Tende a superrepresentar experiências positivas | Médio | Busca de casos negativos | Recrutamento direto, com amostragem por variação máxima |

"Amostra pequena" não é, por si só, limitação em estudo qualitativo; o problema real é o modo de recrutamento.

## Prompts relacionados

- [P13](P13_interpretacao_sem_overclaiming.md)
- [P15](P15_implicacoes_teoricas_praticas.md)
