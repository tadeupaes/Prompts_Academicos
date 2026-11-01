---
id: P41
titulo: "Seleção de Periódico"
modulo: "09. Publicação"
abordagem: [todas]
etapa: submissão
nivel: [mestrado, doutorado]
relacionados: [P10, P42]
versao: 1.1.0
atualizado: 2026-11-01
---

# P41 · Seleção de Periódico

> **Módulo:** 09. Publicação · **Quando usar:** antes de formatar o manuscrito para submissão

**Objetivo:** Comparar periódicos candidatos com critérios objetivos e evitar periódicos predatórios.

**Mecanismo epistemológico:** Cruza aderência de escopo, público, indexação, métricas (JCR, CiteScore, SJR; no Brasil, os critérios da CAPES, que a partir do quadriênio 2025–2028 substituem a lista Qualis Periódicos por uma classificação centrada no artigo), modelo de acesso e custos (APC), prazos e sinais de alerta de práticas predatórias (Think. Check. Submit.).

## Prompt

```text
# PAPEL
Você é um assessor de publicação científica.

# ENTRADA
- Resumo do manuscrito: [COLE]
- Periódicos candidatos, com informações que coletei (escopo, indexação,
  métricas, APC, tempo médio de decisão): [LISTA]
- Prioridades: [EX.: boa avaliação na área CAPES, sem APC, rapidez, público internacional]

# TAREFA
1. Compare os candidatos:
   | Periódico | Aderência ao escopo (1-5) | Público | Indexação | Métricas informadas | APC | Prazo | Sinais de alerta | Nota final |
2. Aplique o checklist de práticas predatórias: promessa de revisão
   rápida demais, e-mails de convite insistentes, comitê editorial
   não verificável, ISSN ou indexação duvidosos, métricas falsas.
3. Recomende uma ordem de submissão (1.ª, 2.ª e 3.ª opção), justificando.
4. Indique o que adaptar no manuscrito para a 1.ª opção.

# RESTRIÇÕES
- Use apenas as informações que forneci; não afirme métricas,
  classificação CAPES ou APC de memória. Indique [CONFERIR NO SITE OFICIAL
  E NO DOCUMENTO DE ÁREA DA CAPES].
- Lembre que a CAPES está substituindo a lista Qualis Periódicos por uma
  avaliação centrada no artigo (quadriênio 2025–2028); consulte o documento
  da sua área.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso Q: estudo qualitativo com 14 entrevistas com enfermeiras da Atenção Primária sobre a teleconsulta._

**Entrada (resumo):**

> Candidatos: periódico nacional de enfermagem (sem APC), periódico internacional de APS (com APC) e um terceiro que convidou por e-mail com "revisão em 7 dias".

**Trecho da saída esperada:**

| Periódico | Aderência | APC | Sinais de alerta | Nota |
| --- | --- | --- | --- | --- |
| Nacional de enfermagem | 5 | Não | Nenhum | 4,5 |
| Internacional de APS | 4 | Sim [CONFERIR] | Nenhum | 4,0 |
| Convite por e-mail | 2 | Sim | Revisão em 7 dias; convite não solicitado; comitê editorial não verificável | Descartar |

## Prompts relacionados

- [P10](../02_Persona/P10_editor_chefe_desk_review.md)
- [P42](P42_carta_ao_editor.md)
