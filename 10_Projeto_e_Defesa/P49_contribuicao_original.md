---
id: P49
titulo: "Enunciado da Contribuição Original da Tese"
modulo: "10. Projeto e Defesa"
abordagem: [todas]
etapa: escrita
nivel: [mestrado, doutorado]
relacionados: [P07, P15, P09]
versao: 1.1.0
atualizado: 2026-11-01
---

# P49 · Enunciado da Contribuição Original da Tese

> **Módulo:** 10. Projeto e Defesa · **Quando usar:** ao escrever a introdução e a conclusão da tese, ou ao preparar a defesa de doutorado

**Objetivo:** Formular, de modo preciso e defensável, qual é a contribuição original da tese.

**Mecanismo epistemológico:** Classifica a originalidade com base nas definições reunidas por Phillips & Pugh em *How to Get a PhD* (ex.: novo dado, nova síntese, nova aplicação, novo método, novo contexto, nova interpretação) e testa o enunciado contra a pergunta "em relação a quê isso é novo?".

## Prompt

```text
# PAPEL
Você é um examinador externo de teses de doutorado. Seu critério central
é a contribuição original ao conhecimento.

# ENTRADA
- Pergunta e tese central: [TEXTO]
- Principais achados: [LISTA]
- Estudos mais próximos ao meu (o que fizeram): [LISTA]
- O que eu acredito ser original: [TEXTO]

# TAREFA
1. Classifique a originalidade declarada em uma ou mais tipologias (novo
   dado empírico, nova síntese, novo método/instrumento, aplicação em novo
   contexto, nova interpretação/teoria, refutação).
2. Teste cada alegação de originalidade:
   | Alegação | Em relação a quais estudos é nova? | Evidência de que é nova | Força (forte/moderada/frágil) | Risco de ser contestada pela banca |
3. Proponha 3 versões do enunciado de contribuição (1 a 3 frases cada),
   do mais conservador ao mais ambicioso, e diga qual é defensável.
4. Indique onde o enunciado deve aparecer na tese (resumo, introdução,
   conclusão) e como mantê-lo consistente.

# RESTRIÇÕES
- Não afirme ineditismo absoluto; enquadre a novidade em relação à
  literatura analisada.
- Não infle a contribuição.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso M: métodos mistos sobre tutoria entre pares e evasão em cursos de engenharia (questionário n = 300 + 4 grupos focais)._

**Entrada (resumo):**

> Originalidade declarada: "primeiro estudo sobre tutoria e evasão no Brasil".

**Trecho da saída esperada:**

| Alegação | Em relação a quê | Força | Risco |
| --- | --- | --- | --- |
| "Primeiro estudo sobre tutoria e evasão no Brasil" | Não demonstrado | Frágil | Alto: basta a banca citar um estudo |
| "Identifica o pertencimento como mecanismo, por integração de métodos" | Estudos de efeito sem explicação do mecanismo | Forte | Baixo |

Versão defensável: "Esta tese contribui ao explicar, por integração de métodos, o mecanismo pelo qual a tutoria entre pares se associa à menor intenção de evasão em engenharia."

## Prompts relacionados

- [P07](../02_Persona/P07_advogado_do_diabo.md)
- [P15](../03_Dados/P15_implicacoes_teoricas_praticas.md)
- [P09](../02_Persona/P09_orientador_socratico.md)
