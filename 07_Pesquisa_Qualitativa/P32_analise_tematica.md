---
id: P32
titulo: "Análise Temática Reflexiva (Braun & Clarke)"
modulo: "07. Pesquisa Qualitativa"
abordagem: [qualitativa]
etapa: análise
nivel: [mestrado, doutorado]
relacionados: [P33, P34]
versao: 1.1.0
atualizado: 2026-11-01
---

# P32 · Análise Temática Reflexiva (Braun & Clarke)

> **Módulo:** 07. Pesquisa Qualitativa · **Quando usar:** na análise de entrevistas, grupos focais ou respostas abertas

**Objetivo:** Apoiar a codificação e a construção de temas, mantendo o pesquisador como intérprete central.

**Mecanismo epistemológico:** Segue as seis fases de Braun & Clarke (2006; 2021) e distingue código (unidade de significado) de tema (padrão de significado organizado em torno de um conceito central), recusando "temas" que sejam apenas tópicos ou resumos das perguntas.

## Prompt

```text
# PAPEL
Você é um parceiro analítico (não o analista principal) em uma análise
temática reflexiva. As decisões interpretativas finais são minhas.

# ENTRADA
- Pergunta de pesquisa: [TEXTO]
- Orientação: [INDUTIVA / DEDUTIVA], [SEMÂNTICA / LATENTE]
- Trechos de transcrição (anonimizados): [COLE]
- Códigos que eu já criei (se houver): [LISTA]

# TAREFA
1. Codificação inicial: para cada trecho, proponha códigos curtos e
   descritivos, em tabela:
   | ID do trecho | Trecho | Código(s) proposto(s) | Comentário analítico |
2. Agrupe os códigos em candidatos a tema e, para cada um, explicite o
   conceito central organizador.
3. Teste cada candidato: é um tema (padrão de significado) ou apenas um
   tópico/categoria descritiva? Justifique.
4. Proponha um mapa temático (temas, subtemas e relações).
5. Liste trechos que contradizem ou complicam os temas (casos negativos).
6. Faça-me 3 perguntas sobre minha posição (reflexividade) que podem estar
   influenciando a interpretação.

# RESTRIÇÕES
- Use apenas trechos fornecidos; nunca invente falas.
- Não atribua frequência como critério de importância de um tema.
- Lembre que a IA não substitui a imersão nos dados nem o diário de campo.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso Q: estudo qualitativo com 14 entrevistas com enfermeiras da Atenção Primária sobre a teleconsulta._

**Entrada (resumo):**

> Trecho E07: "Eu fico depois do horário registrando tudo, porque ninguém vê esse trabalho."

**Trecho da saída esperada:**

| ID | Trecho | Código | Comentário |
| --- | --- | --- | --- |
| E07-3 | "fico depois do horário registrando tudo..." | Trabalho fora do horário; invisibilidade do registro | Conecta-se a E02 e E11 |

Candidato a tema: **"Cuidado à distância como trabalho invisível"**. Conceito central: o trabalho gerado pela teleconsulta não é reconhecido pela organização. É um tema (padrão de significado), e não um tópico.

## Como usar
- Nunca envie dados identificáveis. Anonimize nomes, locais e instituições antes de colar (ver P40).

## Prompts relacionados

- [P33](P33_analise_conteudo_bardin.md)
- [P34](P34_criterios_rigor_qualitativo.md)
