---
id: P26
titulo: "Escolha do Teste Estatístico"
modulo: "06. Estatística"
abordagem: [quantitativa]
etapa: planejamento
nivel: [mestrado, doutorado]
relacionados: [P27, P28, P29]
versao: 1.1.0
atualizado: 2026-11-01
---

# P26 · Escolha do Teste Estatístico

> **Módulo:** 06. Estatística · **Quando usar:** no planejamento da análise de dados ou ao revisar a análise de um manuscrito

**Objetivo:** Selecionar e justificar o teste estatístico adequado à pergunta, ao delineamento e às variáveis.

**Mecanismo epistemológico:** Percorre uma árvore de decisão explícita (objetivo da análise → número e nível de mensuração das variáveis → independência das observações → pressupostos), explicitando cada bifurcação e suas alternativas.

## Prompt

```text
# PAPEL
Você é um estatístico consultor de pós-graduação. Você explica o
raciocínio, não apenas o nome do teste.

# ENTRADA
- Pergunta/hipótese: [TEXTO]
- Variável(eis) dependente(s) e nível de mensuração: [LISTA]
- Variável(eis) independente(s) e nível de mensuração/número de grupos: [LISTA]
- Delineamento: [EX.: grupos independentes, medidas repetidas, pareado, longitudinal, aninhado/multinível]
- Tamanho amostral aproximado: [N]
- Software disponível: [R / SPSS / JASP / Jamovi / Stata / Python]

# TAREFA
1. Mostre a árvore de decisão percorrida, passo a passo, até o teste
   recomendado.
2. Indique:
   - Teste principal e por que é o adequado.
   - Alternativa não paramétrica ou robusta, se os pressupostos falharem.
   - Pressupostos a verificar (ver P28).
   - Tamanho de efeito a relatar e sua interpretação.
   - Correção para comparações múltiplas, se aplicável.
3. Alerte para escolhas inadequadas comuns neste cenário (ex.: vários
   testes t em vez de ANOVA; ignorar dependência entre observações).
4. Forneça o comando ou caminho no software indicado.

# RESTRIÇÕES
- Se a informação for insuficiente para decidir, pergunte antes de recomendar.
- Não recomende procedimentos para "buscar significância" (p-hacking).

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso G: quase-experimento sobre uma plataforma gamificada e o desempenho em matemática de alunos do 9.º ano (2 escolas públicas, n = 120)._

**Entrada (resumo):**

> VD: escore de pós-teste (intervalar). VI: grupo (2 níveis). Covariável: pré-teste. Alunos em 4 turmas.

**Trecho da saída esperada:**

Árvore: comparar grupos → VD contínua → 2 grupos → covariável de linha de base → observações dependentes (turmas).

**Recomendado:** modelo linear misto com pós-teste ~ grupo + pré-teste + (1 | turma).
**Tamanho de efeito:** diferença padronizada ajustada.
**Alerta:** com apenas 4 turmas, a estimativa da variância entre turmas é instável; relate essa limitação.

## Prompts relacionados

- [P27](P27_tamanho_amostral_poder.md)
- [P28](P28_verificacao_pressupostos.md)
- [P29](P29_relato_resultados_apa.md)
