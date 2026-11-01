---
id: P12
titulo: "Triangulação Quali-Quanti (Métodos Mistos)"
modulo: "03. Dados"
abordagem: [mista]
etapa: análise
nivel: [mestrado, doutorado]
relacionados: [P11, P32]
versao: 1.1.0
atualizado: 2026-11-01
---

# P12 · Triangulação Quali-Quanti (Métodos Mistos)

> **Módulo:** 03. Dados · **Quando usar:** na etapa de integração de uma pesquisa de métodos mistos

**Objetivo:** Integrar dados quantitativos e qualitativos em pesquisas de métodos mistos.

**Mecanismo epistemológico:** Constrói uma matriz de integração (*Joint Display Matrix*) com paridade epistemológica, definindo se o qualitativo confirma, expande ou tensiona os números.

## Prompt

```text
# PAPEL
Você é especialista em métodos mistos, com base em Creswell & Plano Clark
e Fetters, Curry & Creswell (2013).

# ENTRADA
- Delineamento misto: [CONVERGENTE / EXPLANATÓRIO SEQUENCIAL / EXPLORATÓRIO SEQUENCIAL / COMPLEXO (ex.: incorporado em experimento, avaliação de programa)]
- Pergunta de integração (mixed methods question): [PERGUNTA]
- Resultados quantitativos: [TABELAS, ESTATÍSTICAS, TAMANHOS DE EFEITO]
- Resultados qualitativos: [CATEGORIAS/TEMAS COM TRECHOS ILUSTRATIVOS]

# TAREFA
1. Verifique se o delineamento declarado é coerente com a ordem e o
   propósito das fases. Aponte inconsistências.
2. Construa a Joint Display Matrix:
   | Dimensão/constructo | Resultado quantitativo | Resultado qualitativo (tema + trecho) | Tipo de integração (Confirma / Expande / Diverge) | Meta-inferência |
3. Para cada divergência ("discordância"), proponha uma explicação e diga
   se ela exige nova análise, nova coleta ou apenas discussão.
4. Garanta a paridade epistemológica: o qualitativo não pode servir apenas
   para "ilustrar" números. Aponte onde isso ocorre.
5. Redija 3 a 5 meta-inferências, isto é, conclusões que só são possíveis
   pela integração dos dois tipos de dados.

# RESTRIÇÕES
- Não converta dados qualitativos em frequências sem que eu peça
  (quantitização) e, se o fizer, explicite a perda interpretativa.
- Não invente trechos de entrevistas; use apenas os que eu fornecer.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso M: métodos mistos sobre tutoria entre pares e evasão em cursos de engenharia (questionário n = 300 + 4 grupos focais)._

**Entrada (resumo):**

> Quanti: alunos tutorados têm 18% menos intenção de evasão. Quali: o tema "pertencimento" aparece nos 4 grupos focais.

**Trecho da saída esperada:**

| Dimensão | Quantitativo | Qualitativo | Integração | Meta-inferência |
| --- | --- | --- | --- | --- |
| Intenção de evasão | −18% entre tutorados (IC 95% −26% a −10%) | Tema "pertencimento": "Foi a primeira vez que alguém do curso perguntou como eu estava" (GF2) | Expande | A tutoria parece reduzir a evasão principalmente pela via do pertencimento, e não do reforço acadêmico |

## Como usar
- A matriz pode entrar diretamente no artigo como figura/tabela de integração.

## Prompts relacionados

- [P11](P11_confronto_com_literatura.md)
- [P32](../07_Pesquisa_Qualitativa/P32_analise_tematica.md)
