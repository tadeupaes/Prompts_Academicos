---
id: P21
titulo: "Resumo Estruturado e Palavras-Chave"
modulo: "05. Escrita Acadêmica"
abordagem: [todas]
etapa: escrita
nivel: [mestrado, doutorado]
relacionados: [P24, P25]
versao: 1.1.0
atualizado: 2026-11-01
---

# P21 · Resumo Estruturado e Palavras-Chave

> **Módulo:** 05. Escrita Acadêmica · **Quando usar:** ao finalizar o artigo, a dissertação ou a tese

**Objetivo:** Produzir um resumo fiel ao texto, dentro do limite de palavras, com palavras-chave indexáveis.

**Mecanismo epistemológico:** Aplica a estrutura IMRaD condensada (contexto, objetivo, método, resultados, conclusão) e verifica a correspondência de cada frase do resumo com o corpo do texto, evitando afirmações ausentes no manuscrito.

## Prompt

```text
# PAPEL
Você é um editor científico especializado em resumos para indexação.

# ENTRADA
- Texto completo ou seções principais: [COLE]
- Limite de palavras: [EX.: 250]
- Formato: [ESTRUTURADO COM SUBTÍTULOS / CORRIDO]
- Norma: [ABNT NBR 6028 / NORMAS DO PERIÓDICO]
- Idiomas: [PT / EN / ES]

# TAREFA
1. Extraia do texto, para cada elemento, a frase-fonte:
   | Elemento | Frase-fonte no manuscrito |
   (Contexto, Objetivo, Método, Resultados principais com números, Conclusão)
2. Redija o resumo respeitando o limite de palavras e informe a contagem.
3. Proponha de 3 a 6 palavras-chave e indique, para cada uma, se parece
   corresponder a um descritor controlado (DeCS/MeSH, Thesaurus ERIC,
   tesauro da área), marcando [VERIFICAR NO TESAURO].
4. Produza a versão em inglês (abstract e keywords), sem tradução literal.

# RESTRIÇÕES
- Nenhuma informação no resumo pode estar ausente do texto.
- Resultados devem conter dados concretos, não "os resultados foram discutidos".
- Sem citações bibliográficas no resumo.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso Q: estudo qualitativo com 14 entrevistas com enfermeiras da Atenção Primária sobre a teleconsulta._

**Entrada (resumo):**

> Dissertação do Caso Q; limite de 250 palavras; formato estruturado.

**Trecho da saída esperada:**

**Objetivo:** compreender as experiências de enfermeiras da Atenção Primária com a teleconsulta. **Método:** estudo qualitativo com 14 entrevistas semiestruturadas, analisadas por análise temática reflexiva. **Resultados:** foram construídos três temas: (1) cuidado à distância como trabalho invisível; ... **Conclusão:** ...

(Contagem: 243 palavras.) Palavras-chave: Teleconsulta [VERIFICAR NO DeCS]; Enfermagem de Atenção Primária; Pesquisa Qualitativa.

## Prompts relacionados

- [P24](P24_titulo_cientifico.md)
- [P25](P25_traducao_academica_pt_en.md)
