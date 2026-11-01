---
id: P45
titulo: "Transformação de Tese/Dissertação em Artigos"
modulo: "09. Publicação"
abordagem: [todas]
etapa: pós-defesa
nivel: [mestrado, doutorado]
relacionados: [P41, P49]
versao: 1.1.0
atualizado: 2026-11-01
---

# P45 · Transformação de Tese/Dissertação em Artigos

> **Módulo:** 09. Publicação · **Quando usar:** após a defesa, ou durante o doutorado no formato de tese por artigos

**Objetivo:** Planejar quantos e quais artigos derivam da tese, sem fatiamento indevido (*salami slicing*) nem autoplágio.

**Mecanismo epistemológico:** Identifica unidades de contribuição independentes (cada artigo deve responder a uma pergunta completa) e verifica sobreposições de dados, texto e resultados entre os artigos planejados.

## Prompt

```text
# PAPEL
Você é um orientador com longa experiência em publicar resultados de teses.

# ENTRADA
- Sumário da tese e resumo de cada capítulo: [COLE]
- Objetivos específicos e principais achados: [LISTA]
- Formato da tese: [TRADICIONAL / POR ARTIGOS]

# TAREFA
1. Proponha um plano de artigos:
   | Artigo | Pergunta própria | Dados/capítulos usados | Tipo (empírico, revisão, metodológico, teórico) | Periódico-alvo (perfil) | Autoria sugerida |
2. Verifique riscos:
   - Salami slicing (artigos que não se sustentam sozinhos).
   - Sobreposição de resultados que exija citação cruzada ou declaração.
   - Reutilização de texto (autoplágio) e como reescrever.
3. Para o artigo prioritário, proponha a estrutura IMRaD e o que cortar da tese.
4. Sugira a ordem de submissão e um cronograma realista.

# RESTRIÇÕES
- Respeite as regras do programa sobre tese por artigos e os critérios de
  autoria (ICMJE/CRediT).

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso M: métodos mistos sobre tutoria entre pares e evasão em cursos de engenharia (questionário n = 300 + 4 grupos focais)._

**Entrada (resumo):**

> Tese com 3 objetivos específicos: fatores de evasão (quanti), experiências dos tutorados (quali) e integração.

**Trecho da saída esperada:**

| Artigo | Pergunta própria | Dados | Tipo |
| --- | --- | --- | --- |
| 1 | Quais fatores se associam à intenção de evasão? | Questionário (n = 300) | Empírico quantitativo |
| 2 | Como os estudantes vivenciam a tutoria? | Grupos focais | Empírico qualitativo |
| 3 | Por que a tutoria reduz a evasão? | Integração | Métodos mistos (principal) |

Risco: os artigos 1 e 3 compartilham resultados; o 3 deve citar o 1 e apresentar apenas o necessário.

## Prompts relacionados

- [P41](P41_selecao_de_periodico.md)
- [P49](../10_Projeto_e_Defesa/P49_contribuicao_original.md)
