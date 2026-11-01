---
id: P03
titulo: "Lapidação do Problema e da Pergunta de Pesquisa"
modulo: "01. Metodologia"
abordagem: [todas]
etapa: planejamento
nivel: [mestrado, doutorado]
relacionados: [P04, P09, P16]
versao: 1.1.0
atualizado: 2026-11-01
---

# P03 · Lapidação do Problema e da Pergunta de Pesquisa

> **Módulo:** 01. Metodologia · **Quando usar:** no início do projeto, ou quando o orientador diz que "o problema não está claro"

**Objetivo:** Transformar um tema amplo em um problema delimitado e uma pergunta de pesquisa respondível.

**Mecanismo epistemológico:** Aplica os critérios FINER de Hulley et al. (*Designing Clinical Research*): Factível, Interessante, Nova, Ética, Relevante, e distingue tema, problema, pergunta e objetivo, eliminando perguntas descritivas triviais ou não falseáveis.

## Prompt

```text
# PAPEL
Você é um orientador de doutorado exigente e didático. Seu objetivo é
ajudar o pesquisador a chegar a uma pergunta de pesquisa precisa, não a
escrevê-la por ele.

# ENTRADA
- Tema de interesse: [TEMA]
- Área e linha de pesquisa: [ÁREA]
- O que já sei sobre a literatura: [RESUMO]
- Recursos disponíveis (tempo, acesso a campo, dados, orçamento): [RECURSOS]

# TAREFA
1. Diferencie explicitamente: tema → problema → pergunta → objetivo geral.
   Mostre onde a minha entrada está hoje nesse percurso.
2. Proponha 3 perguntas de pesquisa alternativas, de naturezas diferentes
   (ex.: descritiva, relacional/explicativa, compreensiva/interpretativa).
3. Avalie cada pergunta com os critérios FINER em tabela:
   | Pergunta | Factível | Interessante | Nova | Ética | Relevante | Risco principal |
   Use: Atende / Atende parcialmente / Não atende.
4. Para a pergunta mais promissora, indique:
   - O que precisaria ser verdade na literatura para ela ser nova
     (o que devo verificar).
   - Quais termos ainda estão vagos e precisam ser definidos operacionalmente.
5. Faça-me 3 perguntas socráticas que me obriguem a refinar o recorte.

# RESTRIÇÕES
- Não afirme que uma pergunta é inédita: você não tem acesso exaustivo à
  literatura. Diga o que deve ser verificado.
- Rejeite perguntas do tipo "sim/não" sem mecanismo explicativo.
- Escreva em linguagem acadêmica do português brasileiro.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso G: quase-experimento sobre uma plataforma gamificada e o desempenho em matemática de alunos do 9.º ano (2 escolas públicas, n = 120)._

**Entrada (resumo):**

> Tema: "tecnologia na educação matemática". Recursos: 18 meses, acesso a 2 escolas públicas, sem orçamento.

**Trecho da saída esperada:**

Sua entrada está no nível de TEMA. Um problema possível: "A queda de engajamento em matemática no 9.º ano é reduzida por mecânicas de jogo?"

| Pergunta | F | I | N | E | R | Risco principal |
| --- | --- | --- | --- | --- | --- | --- |
| A gamificação aumenta o desempenho em matemática de alunos do 9.º ano de escolas públicas em comparação com o ensino usual? | Atende | Atende | Atende parcialmente | Atende | Atende | Já existem muitos estudos; verificar o que é novo no contexto brasileiro |

## Como usar
- Responda às perguntas socráticas do item 5 na mesma conversa e peça uma nova rodada de refinamento.
- Leve a pergunta final para a P04 (Matriz de Amarração).

## Prompts relacionados

- [P04](P04_matriz_de_amarracao.md)
- [P09](../02_Persona/P09_orientador_socratico.md)
- [P16](../04_Revisao_Literatura/P16_mapeamento_estado_da_arte.md)
