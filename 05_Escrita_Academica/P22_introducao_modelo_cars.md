---
id: P22
titulo: "Introdução em Funil (Modelo CARS)"
modulo: "05. Escrita Acadêmica"
abordagem: [todas]
etapa: escrita
nivel: [mestrado, doutorado]
relacionados: [P16, P21]
versao: 1.1.0
atualizado: 2026-11-01
---

# P22 · Introdução em Funil (Modelo CARS)

> **Módulo:** 05. Escrita Acadêmica · **Quando usar:** ao escrever ou revisar a introdução de um artigo ou capítulo

**Objetivo:** Estruturar uma introdução que conduza o leitor do território geral até a lacuna e a proposta do estudo.

**Mecanismo epistemológico:** Aplica o modelo CARS (*Create a Research Space*) de Swales (1990): Movimento 1 (estabelecer o território), Movimento 2 (estabelecer o nicho) e Movimento 3 (ocupar o nicho).

## Prompt

```text
# PAPEL
Você é um professor de escrita científica que domina análise de gêneros
acadêmicos (Swales, 1990; 2004).

# ENTRADA
- Minha introdução atual (ou anotações): [COLE]
- Pergunta, objetivo e principal contribuição: [TEXTO]

# TAREFA
1. Diagnóstico: classifique cada parágrafo/frase da minha introdução nos
   movimentos CARS:
   | Trecho | Movimento | Passo (ex.: generalização do tópico, revisão de pesquisas anteriores, indicação de lacuna, anúncio do objetivo, anúncio da estrutura) |
2. Aponte problemas: movimentos ausentes, ordem invertida, lacuna afirmada
   sem apoio na literatura, objetivo enunciado tarde demais, excesso de
   contexto genérico.
3. Proponha um esqueleto reorganizado (tópicos frasais de cada parágrafo).
4. Reescreva a introdução seguindo o esqueleto, mantendo minhas citações e
   minhas ideias.

# RESTRIÇÕES
- Não acrescente citações nem dados. Onde faltar suporte, insira
  [CITAÇÃO NECESSÁRIA].
- Evite aberturas genéricas ("Nos dias atuais...", "Desde os primórdios...").

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso M: métodos mistos sobre tutoria entre pares e evasão em cursos de engenharia (questionário n = 300 + 4 grupos focais)._

**Entrada (resumo):**

> Introdução atual com 6 parágrafos; o objetivo só aparece no último.

**Trecho da saída esperada:**

| Trecho | Movimento | Passo |
| --- | --- | --- |
| §1–§4 | M1 | Generalização do tópico (evasão no ensino superior) |
| §5 | M1 | Revisão de pesquisas anteriores |
| §6 | M3 | Anúncio do objetivo |

Problema: falta o Movimento 2. A lacuna (falta de estudos que expliquem *por que* a tutoria funciona) nunca é declarada.

## Prompts relacionados

- [P16](../04_Revisao_Literatura/P16_mapeamento_estado_da_arte.md)
- [P21](P21_resumo_estruturado.md)
