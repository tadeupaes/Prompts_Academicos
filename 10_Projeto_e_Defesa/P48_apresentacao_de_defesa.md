---
id: P48
titulo: "Roteiro da Apresentação de Defesa"
modulo: "10. Projeto e Defesa"
abordagem: [todas]
etapa: defesa
nivel: [mestrado, doutorado]
relacionados: [P08, P49]
versao: 1.1.0
atualizado: 2026-11-01
---

# P48 · Roteiro da Apresentação de Defesa

> **Módulo:** 10. Projeto e Defesa · **Quando usar:** ao preparar os slides da qualificação ou da defesa

**Objetivo:** Organizar uma apresentação oral clara, no tempo regulamentar, centrada no argumento da tese.

**Mecanismo epistemológico:** Estrutura a apresentação como argumento (problema → lacuna → tese → evidências → contribuição), com uma mensagem por slide em forma de frase afirmativa (*assertion-evidence*, Alley) e distribuição de tempo por seção.

## Prompt

```text
# PAPEL
Você é um especialista em comunicação científica que já assistiu a
centenas de defesas.

# ENTRADA
- Resumo da tese/dissertação: [COLE]
- Tempo disponível: [EX.: 30 MINUTOS]
- Tipo: [QUALIFICAÇÃO / DEFESA]
- Público: [BANCA ESPECIALISTA / BANCA MISTA]

# TAREFA
1. Defina a mensagem central em uma frase (o que a banca deve lembrar).
2. Proponha o roteiro slide a slide:
   | Nº | Título-afirmação (frase completa) | Evidência visual sugerida (gráfico, esquema, tabela, citação) | Fala-chave | Tempo (min) |
3. Distribua o tempo (ex.: introdução e problema 15%, método 25%,
   resultados 35%, discussão e contribuição 20%, encerramento 5%) e ajuste
   ao tipo de exame.
4. Indique 3 slides de reserva (backup) para perguntas previsíveis.
5. Liste erros a evitar (slides com texto corrido, revisão de literatura
   longa demais, ultrapassar o tempo).

# RESTRIÇÕES
- O roteiro deve caber no tempo; aproximadamente 1 slide por minuto como teto.
- Não inclua resultados que não estejam no texto.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso M: métodos mistos sobre tutoria entre pares e evasão em cursos de engenharia (questionário n = 300 + 4 grupos focais)._

**Entrada (resumo):**

> Defesa de doutorado; 40 minutos; banca mista.

**Trecho da saída esperada:**

Mensagem central: "A tutoria entre pares reduz a evasão porque cria pertencimento."

| Nº | Título-afirmação | Evidência visual | Tempo |
| --- | --- | --- | --- |
| 3 | Um em cada três ingressantes de engenharia abandona o curso | Gráfico de barras da evasão por ano | 2 min |
| 12 | O pertencimento explica a maior parte do efeito da tutoria | Joint display (resumo) | 4 min |

## Como usar
- Depois de montar os slides, treine com a P08 (Simulação de Banca).

## Prompts relacionados

- [P08](../02_Persona/P08_banca_de_qualificacao.md)
- [P49](P49_contribuicao_original.md)
