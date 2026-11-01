---
id: P23
titulo: "Revisão de Clareza, Coesão e Hedging"
modulo: "05. Escrita Acadêmica"
abordagem: [todas]
etapa: escrita
nivel: [mestrado, doutorado]
relacionados: [P25]
versao: 1.1.0
atualizado: 2026-11-01
---

# P23 · Revisão de Clareza, Coesão e Hedging

> **Módulo:** 05. Escrita Acadêmica · **Quando usar:** na revisão final de qualquer capítulo ou artigo

**Objetivo:** Melhorar a legibilidade do texto acadêmico sem alterar o conteúdo nem a voz autoral.

**Mecanismo epistemológico:** Avalia a progressão temática (informação dada → nova), a unidade do parágrafo (tópico frasal), os conectivos lógicos e a modalização (*hedging*) proporcional à evidência.

## Prompt

```text
# PAPEL
Você é revisor(a) de textos acadêmicos em português brasileiro, com foco
em argumentação, não apenas em gramática.

# TEXTO
[COLE ATÉ ~1500 PALAVRAS POR VEZ]

# TAREFA
1. Diagnóstico por parágrafo:
   | § | Tópico frasal (existe? qual?) | Problema de coesão/coerência | Sugestão |
2. Aponte:
   - Frases com mais de 40 palavras ou com várias ideias.
   - Conectivos mal empregados (ex.: "entretanto" sem contraste).
   - Repetições, nominalizações excessivas e voz passiva desnecessária.
   - Afirmações categóricas sem suporte (falta de hedging) e excesso de
     hedging que esvazia a afirmação.
   - Termos técnicos usados com sentidos diferentes ao longo do texto.
3. Entregue o texto revisado com as alterações marcadas:
   [-texto removido-] {+texto inserido+}
4. Liste as 5 alterações mais importantes e por quê.

# RESTRIÇÕES
- Preserve o conteúdo, os dados, as citações e a terminologia da área.
- Preserve o estilo do autor; não transforme o texto em "texto de IA".
- Siga a norma culta do português brasileiro e o Acordo Ortográfico vigente.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso Q: estudo qualitativo com 14 entrevistas com enfermeiras da Atenção Primária sobre a teleconsulta._

**Entrada (resumo):**

> Parágrafo com uma frase de 62 palavras e "entretanto" sem contraste.

**Trecho da saída esperada:**

A teleconsulta ampliou o acesso [-, entretanto,-] {+e+} também gerou novas demandas de registro. {+Entretanto,+} as participantes relataram...

## Prompts relacionados

- [P25](P25_traducao_academica_pt_en.md)
