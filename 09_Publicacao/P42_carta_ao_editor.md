---
id: P42
titulo: "Carta ao Editor (Cover Letter)"
modulo: "09. Publicação"
abordagem: [todas]
etapa: submissão
nivel: [mestrado, doutorado]
relacionados: [P41, P10]
versao: 1.1.0
atualizado: 2026-11-01
---

# P42 · Carta ao Editor (Cover Letter)

> **Módulo:** 09. Publicação · **Quando usar:** no momento da submissão

**Objetivo:** Redigir uma carta de apresentação concisa que mostre ao editor por que o manuscrito interessa ao periódico.

**Mecanismo epistemológico:** Organiza a carta em argumento editorial (contribuição → aderência ao público do periódico → originalidade) e inclui as declarações formais exigidas (ineditismo, conflitos de interesse, aprovação ética).

## Prompt

```text
# PAPEL
Você é um pesquisador experiente que já publicou e avaliou em periódicos
internacionais.

# ENTRADA
- Periódico e nome do editor (se conhecido): [TEXTO]
- Título e resumo: [COLE]
- Principal contribuição em 1 a 2 frases: [TEXTO]
- Por que este periódico (artigos recentes dele com os quais dialogamos): [TEXTO]
- Declarações: ineditismo, conflitos, financiamento, ética (CAAE), dados disponíveis: [TEXTO]
- Sugestão de revisores (se solicitado): [LISTA]

# TAREFA
1. Redija a carta (máx. 1 página) com:
   - Apresentação do manuscrito e do tipo de artigo.
   - O problema e a contribuição, em linguagem direta.
   - A conexão com o escopo e com publicações recentes do periódico.
   - As declarações formais.
2. Produza a versão em inglês.
3. Liste o que NÃO deve constar (repetir o resumo, exagerar, elogiar o periódico de forma genérica).

# RESTRIÇÕES
- Não invente artigos do periódico; use apenas os que eu informei.
- Tom profissional, sem bajulação.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso M: métodos mistos sobre tutoria entre pares e evasão em cursos de engenharia (questionário n = 300 + 4 grupos focais)._

**Entrada (resumo):**

> Contribuição: identificar o pertencimento como mecanismo da tutoria na engenharia.

**Trecho da saída esperada:**

Prezada Editora,

Submetemos o artigo "Tutoria entre pares e evasão na engenharia: um estudo de métodos mistos" para a seção de Artigos Originais. Embora a tutoria seja amplamente adotada, pouco se sabe sobre *por que* ela reduz a evasão. Ao integrar dados de 300 estudantes com grupos focais, mostramos que...

## Prompts relacionados

- [P41](P41_selecao_de_periodico.md)
- [P10](../02_Persona/P10_editor_chefe_desk_review.md)
