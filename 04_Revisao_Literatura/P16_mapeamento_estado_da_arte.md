---
id: P16
titulo: "Mapeamento do Estado da Arte e das Lacunas"
modulo: "04. Revisão de Literatura"
abordagem: [revisão]
etapa: revisão de literatura
nivel: [mestrado, doutorado]
relacionados: [P17, P18]
versao: 1.1.0
atualizado: 2026-11-01
---

# P16 · Mapeamento do Estado da Arte e das Lacunas

> **Módulo:** 04. Revisão de Literatura · **Quando usar:** ao construir a justificativa e a lacuna de pesquisa

**Objetivo:** Organizar a literatura lida em correntes, consensos, controvérsias e lacunas verificáveis.

**Mecanismo epistemológico:** Diferencia os sete tipos de lacuna de Miles (2017): de evidência, de conhecimento, de conflito prática-conhecimento, metodológica, empírica, teórica e populacional, e exige que cada lacuna seja demonstrada por um conjunto de estudos, não apenas afirmada.

## Prompt

```text
# PAPEL
Você é um pesquisador experiente em revisões narrativas críticas. Você
trabalha SOMENTE com o corpus que eu fornecer.

# CORPUS
Lista de estudos lidos (autor, ano, objetivo, método, achado principal):
[COLE A LISTA OU OS FICHAMENTOS]

# TAREFA
1. Agrupe os estudos em correntes/abordagens, nomeando cada grupo e o
   pressuposto que o une.
2. Identifique:
   - Consensos (o que a maioria encontra, e com que tipo de evidência).
   - Controvérsias (resultados contraditórios e possíveis razões).
   - Evolução temporal (como o debate mudou ao longo dos anos).
3. Mapeie lacunas em tabela:
   | Tipo de lacuna | Descrição | Estudos que a evidenciam | Força da evidência da lacuna (forte/moderada/fraca) |
4. Indique qual lacuna minha pesquisa ([DESCREVA EM 1 FRASE]) preenche e
   se a afirmação de lacuna é defensável com este corpus.

# RESTRIÇÕES
- Não acrescente estudos ao corpus. Se a ausência de uma área for
  relevante, escreva [VERIFICAR NA LITERATURA: tema].
- Não afirme que "não existem estudos sobre X"; diga "no corpus analisado,
  não foram identificados estudos sobre X".

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso R: revisão sobre intervenções baseadas em mindfulness para burnout em professores da educação básica._

**Entrada (resumo):**

> Corpus: 22 estudos fichados, sendo 15 dos EUA e Reino Unido e nenhum da América Latina.

**Trecho da saída esperada:**

| Tipo de lacuna | Descrição | Estudos que a evidenciam | Força |
| --- | --- | --- | --- |
| Populacional | Ausência de estudos com professores latino-americanos | 15 de 22 estudos são de EUA e Reino Unido; os demais, da Ásia | Forte (no corpus analisado) |
| Metodológica | Desfechos medidos só imediatamente após a intervenção | 19 de 22 sem seguimento | Moderada |

## Prompts relacionados

- [P17](P17_fichamento_critico.md)
- [P18](P18_matriz_de_sintese.md)
