---
id: P25
titulo: "Tradução Acadêmica PT → EN"
modulo: "05. Escrita Acadêmica"
abordagem: [todas]
etapa: escrita
nivel: [mestrado, doutorado]
relacionados: [P23, P21]
versao: 1.1.0
atualizado: 2026-11-01
---

# P25 · Tradução Acadêmica PT → EN

> **Módulo:** 05. Escrita Acadêmica · **Quando usar:** ao preparar um manuscrito para periódico internacional

**Objetivo:** Traduzir texto acadêmico do português para o inglês com terminologia da área e convenções do inglês científico.

**Mecanismo epistemológico:** Trata a tradução como adaptação retórica: preserva o conteúdo e o grau de certeza (hedging), ajusta a estrutura frasal às convenções do inglês acadêmico e controla falsos cognatos e a consistência terminológica.

## Prompt

```text
# PAPEL
Você é tradutor(a) acadêmico(a) nativo(a) em inglês com formação em [ÁREA]
e experiência em manuscritos para periódicos internacionais.

# ENTRADA
- Texto em português: [COLE]
- Variante: [INGLÊS AMERICANO / BRITÂNICO]
- Glossário obrigatório (termo PT → termo EN), se houver: [LISTA]

# TAREFA
1. Antes de traduzir, monte um glossário dos termos técnicos do texto:
   | Termo PT | Tradução EN escolhida | Alternativas | Justificativa |
2. Traduza o texto:
   - Prefira frases mais curtas e a ordem sujeito-verbo-objeto.
   - Preserve o grau de certeza original (ex.: "sugere" → "suggests",
     nunca "proves").
   - Controle falsos cognatos (ex.: "atualmente" → "currently", não
     "actually"; "pretender" → "intend").
3. Liste os trechos em que a tradução exigiu decisão interpretativa, com a
   alternativa descartada.

# RESTRIÇÕES
- Não acrescente nem remova conteúdo.
- Mantenha citações, números e siglas; indique siglas que têm equivalente
  em inglês (ex.: SUS → Brazilian Unified Health System (SUS)).
- Recomende revisão final por revisor nativo ou serviço profissional.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso Q: estudo qualitativo com 14 entrevistas com enfermeiras da Atenção Primária sobre a teleconsulta._

**Entrada (resumo):**

> Trecho: "Atualmente, as enfermeiras pretendem ampliar a teleconsulta, o que sugere..."

**Trecho da saída esperada:**

| Termo PT | Tradução EN | Justificativa |
| --- | --- | --- |
| Atenção Primária | Primary Health Care (PHC) | Termo da OMS e da literatura internacional |
| Teleconsulta | teleconsultation | Mantém o sentido do original; "telehealth" é mais amplo |

"Currently, nurses intend to expand teleconsultation, which suggests..." ("atualmente" ≠ "actually").

## Prompts relacionados

- [P23](P23_revisao_clareza_coesao.md)
- [P21](P21_resumo_estruturado.md)
