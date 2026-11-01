---
id: P18
titulo: "Matriz de Síntese da Literatura"
modulo: "04. Revisão de Literatura"
abordagem: [revisão]
etapa: revisão de literatura
nivel: [mestrado, doutorado]
relacionados: [P16, P17]
versao: 1.1.0
atualizado: 2026-11-01
---

# P18 · Matriz de Síntese da Literatura

> **Módulo:** 04. Revisão de Literatura · **Quando usar:** ao transformar fichamentos em um capítulo de revisão

**Objetivo:** Passar de uma revisão "autor por autor" para uma revisão "tema por tema", com síntese real.

**Mecanismo epistemológico:** Usa a matriz de síntese (Garrard, *Matrix Method*) para cruzar estudos e dimensões analíticas, produzindo parágrafos organizados por argumento e não por fonte.

## Prompt

```text
# PAPEL
Você é um especialista em escrita de revisões de literatura acadêmicas.

# ENTRADA
- Fichamentos ou resumos dos estudos: [COLE]
- Dimensões que me interessam (ex.: definição do conceito, contexto, método, achado, limitação): [LISTA]

# TAREFA
1. Construa a matriz:
   linhas = estudos; colunas = dimensões; células com o conteúdo resumido.
2. Leia a matriz por coluna e extraia de 4 a 6 temas/argumentos transversais.
3. Para cada tema, escreva um parágrafo de síntese com a estrutura:
   frase-tópico com o argumento → estudos que convergem → estudos que
   divergem → avaliação crítica → ligação com minha pesquisa.
4. Sugira a ordem lógica dos temas para compor o capítulo (do geral para o
   específico, até a lacuna).

# RESTRIÇÕES
- Cada frase com conteúdo de estudo deve indicar a fonte (Autor, ano).
- Use apenas estudos da entrada.
- Proibido o formato "Fulano (2020) disse... Beltrano (2021) disse...".

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso R: revisão sobre intervenções baseadas em mindfulness para burnout em professores da educação básica._

**Entrada (resumo):**

> Fichamentos de 22 estudos; dimensões: tipo de intervenção, duração, instrumento, efeito.

**Trecho da saída esperada:**

**Tema 2: a duração da intervenção parece mais relevante do que o formato.** Programas com 8 semanas ou mais relataram reduções na exaustão emocional (Autor A, 2018; Autor B, 2020), enquanto intervenções breves não mostraram diferença (Autor C, 2021). Essa divergência, porém, se confunde com o tipo de controle...

## Prompts relacionados

- [P16](P16_mapeamento_estado_da_arte.md)
- [P17](P17_fichamento_critico.md)
