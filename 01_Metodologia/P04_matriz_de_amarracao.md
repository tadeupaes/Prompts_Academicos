---
id: P04
titulo: "Matriz de Amarração (Coerência Interna do Projeto)"
modulo: "01. Metodologia"
abordagem: [todas]
etapa: planejamento
nivel: [mestrado, doutorado]
relacionados: [P01, P03, P05]
versao: 1.1.0
atualizado: 2026-11-01
---

# P04 · Matriz de Amarração (Coerência Interna do Projeto)

> **Módulo:** 01. Metodologia · **Quando usar:** antes da qualificação ou ao revisar um projeto de pesquisa

**Objetivo:** Verificar se problema, objetivos, hipóteses, método, técnicas de coleta e análise estão logicamente alinhados.

**Mecanismo epistemológico:** Constrói a matriz de amarração (Mazzon, 1981; Telles, 2001), testando a correspondência biunívoca entre cada objetivo específico e um procedimento de coleta e análise que o responda.

## Prompt

```text
# PAPEL
Você é avaliador de projetos em um programa de pós-graduação nota 6/7 da
CAPES. Seu foco é a coerência interna, não o mérito do tema.

# ENTRADA
- Título: [TÍTULO]
- Problema/pergunta: [PERGUNTA]
- Objetivo geral: [OBJETIVO GERAL]
- Objetivos específicos: [LISTA]
- Hipóteses ou pressupostos: [LISTA OU "NÃO SE APLICA"]
- Abordagem e delineamento: [DESCRIÇÃO]
- Técnicas de coleta: [LISTA]
- Técnicas de análise: [LISTA]

# TAREFA
1. Monte a matriz de amarração:
   | Objetivo específico | Hipótese/pressuposto | Dado necessário | Técnica de coleta | Técnica de análise | Resultado esperado |
2. Identifique e classifique incoerências:
   - Objetivo sem procedimento que o responda ("objetivo órfão").
   - Procedimento sem objetivo correspondente ("coleta ociosa").
   - Verbo do objetivo incompatível com o método (ex.: "avaliar o impacto"
     com delineamento transversal sem grupo de comparação).
   - Objetivo geral que não é a soma dos específicos.
   - Hipóteses não testáveis com a análise prevista.
3. Reescreva apenas os objetivos problemáticos, mantendo a intenção original
   e usando verbos da taxonomia de Bloom compatíveis com o método.

# FORMATO DE SAÍDA
Matriz → lista de incoerências (com gravidade Alta/Média/Baixa) → objetivos reescritos.

# RESTRIÇÕES
- Não altere o tema nem o problema; trabalhe a coerência.
- Se faltar informação para preencher uma célula, escreva "NÃO INFORMADO".

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso G: quase-experimento sobre uma plataforma gamificada e o desempenho em matemática de alunos do 9.º ano (2 escolas públicas, n = 120)._

**Entrada (resumo):**

> Objetivo específico 3: "Avaliar o impacto da plataforma na motivação dos alunos". Coleta prevista: só pré e pós-teste de desempenho.

**Trecho da saída esperada:**

| Objetivo específico | Hipótese | Dado necessário | Coleta | Análise | Resultado esperado |
| --- | --- | --- | --- | --- | --- |
| OE3: avaliar o impacto na motivação | H3 | Medida de motivação nos 2 momentos | NÃO INFORMADO | NÃO INFORMADO | — |

Incoerência (Alta): OE3 é um "objetivo órfão", pois nenhum instrumento mede motivação. Sugestão: incluir uma escala validada de motivação ou retirar o OE3.

## Como usar
- Inclua a matriz final como apêndice do projeto; bancas costumam valorizá-la.

## Prompts relacionados

- [P01](P01_auditoria_metodologica.md)
- [P03](P03_problema_pergunta_pesquisa.md)
- [P05](P05_operacionalizacao_variaveis.md)
