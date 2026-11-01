---
id: P24
titulo: "Título Científico"
modulo: "05. Escrita Acadêmica"
abordagem: [todas]
etapa: escrita
nivel: [mestrado, doutorado]
relacionados: [P21]
versao: 1.1.0
atualizado: 2026-11-01
---

# P24 · Título Científico

> **Módulo:** 05. Escrita Acadêmica · **Quando usar:** ao definir ou revisar o título de artigo, dissertação ou tese

**Objetivo:** Gerar e avaliar títulos informativos, precisos e encontráveis em buscas.

**Mecanismo epistemológico:** Avalia títulos por precisão (reflete o estudo?), informatividade (indica variável, população, desenho ou achado?), encontrabilidade (contém termos indexáveis?) e concisão.

## Prompt

```text
# PAPEL
Você é um editor de periódico que sabe que o título determina se o artigo
será encontrado e lido.

# ENTRADA
- Resumo do estudo: [COLE]
- Título atual: [TÍTULO]
- Limite de caracteres/palavras do periódico: [LIMITE]

# TAREFA
1. Avalie o título atual pelos critérios: precisão, informatividade,
   encontrabilidade, concisão e ausência de jargão desnecessário.
2. Proponha 8 títulos em 4 estilos (2 de cada):
   - Descritivo (o que foi estudado).
   - Declarativo (o principal achado).
   - Interrogativo (a pergunta).
   - Com subtítulo (título: delimitação de contexto/método).
3. Pontue cada título de 1 a 5 em cada critério e indique os 2 melhores.
4. Gere a versão em inglês dos 2 melhores.

# RESTRIÇÕES
- O título declarativo não pode afirmar mais do que os resultados sustentam.
- Evite siglas não consagradas e trocadilhos que prejudiquem a busca.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso M: métodos mistos sobre tutoria entre pares e evasão em cursos de engenharia (questionário n = 300 + 4 grupos focais)._

**Entrada (resumo):**

> Título atual: "Tutoria e evasão: um estudo de caso".

**Trecho da saída esperada:**

| Título | Precisão | Informatividade | Encontrabilidade | Concisão |
| --- | --- | --- | --- | --- |
| Declarativo: "Tutoria entre pares reduz a intenção de evasão em cursos de engenharia por meio do pertencimento" | 4 | 5 | 5 | 3 |
| Com subtítulo: "Tutoria entre pares e evasão na engenharia: um estudo de métodos mistos" | 5 | 4 | 5 | 4 |

## Prompts relacionados

- [P21](P21_resumo_estruturado.md)
