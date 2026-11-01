---
id: P29
titulo: "Relato de Resultados no Padrão APA 7"
modulo: "06. Estatística"
abordagem: [quantitativa]
etapa: escrita
nivel: [mestrado, doutorado]
relacionados: [P13, P30]
versao: 1.1.0
atualizado: 2026-11-01
---

# P29 · Relato de Resultados no Padrão APA 7

> **Módulo:** 06. Estatística · **Quando usar:** ao redigir a seção de Resultados

**Objetivo:** Redigir os resultados estatísticos de forma completa, padronizada e reprodutível.

**Mecanismo epistemológico:** Segue as JARS (*Journal Article Reporting Standards*) da APA: estatística, graus de liberdade, valor exato de p, tamanho de efeito e intervalo de confiança, separando a descrição do resultado de sua interpretação.

## Prompt

```text
# PAPEL
Você é um editor de estatística que aplica o Manual de Publicação da APA,
7.ª edição.

# ENTRADA
- Hipóteses: [LISTA]
- Saídas do software (cole as tabelas): [COLE]
- Idioma: [PT / EN] (em PT, use vírgula decimal, salvo norma contrária do periódico)

# TAREFA
1. Para cada hipótese, extraia da saída: estatística do teste, gl, p exato,
   tamanho de efeito e IC 95%. Se faltar algum, marque [CALCULAR/OBTER].
2. Redija o parágrafo de resultado de cada hipótese, por exemplo:
   "O grupo X apresentou média maior (M = 4,2; DP = 0,8) que o grupo Y
   (M = 3,6; DP = 0,9), t(58) = 2,74, p = 0,008, d = 0,71, IC 95% [0,19; 1,23]."
3. Sugira tabelas no formato APA (título, notas, casas decimais) quando
   houver muitos resultados.
4. Verifique a consistência interna (ex.: gl compatível com N; p compatível
   com a estatística; DP plausível).

# RESTRIÇÕES
- Não interprete na seção de resultados; interpretação vai para a Discussão (P11).
- Não arredonde p para "p < 0,05"; use valor exato (exceto p < 0,001).
- Use apenas os números da saída fornecida.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso G: quase-experimento sobre uma plataforma gamificada e o desempenho em matemática de alunos do 9.º ano (2 escolas públicas, n = 120)._

**Entrada (resumo):**

> Saída: F(1, 117) = 8,12; p = 0,005; η²p = 0,065; médias ajustadas de 6,8 e 6,1.

**Trecho da saída esperada:**

Controlando o desempenho no pré-teste, o grupo que usou a plataforma obteve média ajustada maior no pós-teste (M = 6,8) do que o grupo controle (M = 6,1), F(1, 117) = 8,12, p = 0,005, η²p = 0,065. [OBTER IC 95% DA DIFERENÇA AJUSTADA]

## Prompts relacionados

- [P13](../03_Dados/P13_interpretacao_sem_overclaiming.md)
- [P30](P30_interpretacao_saida_software.md)
