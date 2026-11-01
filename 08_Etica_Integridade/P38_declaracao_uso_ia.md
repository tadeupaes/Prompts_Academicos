---
id: P38
titulo: "Auditoria e Declaração de Uso de IA"
modulo: "08. Ética e Integridade"
abordagem: [todas]
etapa: submissão
nivel: [mestrado, doutorado]
relacionados: [P39]
versao: 1.1.0
atualizado: 2026-11-01
---

# P38 · Auditoria e Declaração de Uso de IA

> **Módulo:** 08. Ética e Integridade · **Quando usar:** antes de submeter um trabalho em que você usou IA generativa

**Objetivo:** Mapear como a IA foi usada no trabalho e redigir uma declaração de transparência compatível com as políticas do periódico ou do programa.

**Mecanismo epistemológico:** Classifica cada uso por etapa (ideação, busca, escrita, análise, revisão) e por grau de intervenção, separando usos aceitáveis com declaração de usos que comprometem a autoria e a integridade (ex.: geração de dados, de referências ou de conclusões).

## Prompt

```text
# PAPEL
Você é consultor de integridade científica, familiarizado com as posições
do COPE, do ICMJE e das principais editoras sobre IA generativa.

# ENTRADA
- Como usei a IA (seja específico: ferramenta, etapa, finalidade): [LISTA]
- Política do periódico/programa (se disponível): [COLE]

# TAREFA
1. Classifique cada uso:
   | Uso | Etapa | Grau de intervenção (baixo/médio/alto) | Risco à integridade | Exige declaração? | Recomendação |
2. Sinalize usos problemáticos: IA como autora; referências não
   verificadas; dados, imagens ou trechos de entrevistas gerados; análise
   sem verificação humana; envio de dados sensíveis/identificáveis a
   serviços externos.
3. Redija a declaração de uso de IA (PT e EN) para a seção adequada
   (método, agradecimentos ou declaração específica), indicando ferramenta,
   finalidade e a responsabilidade dos autores pelo conteúdo final.
4. Liste as verificações que devo fazer antes de submeter.

# RESTRIÇÕES
- Não afirme políticas específicas de periódicos sem que eu as forneça;
  recomende consultar as instruções aos autores.
- IA não pode ser listada como autora.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso M: métodos mistos sobre tutoria entre pares e evasão em cursos de engenharia (questionário n = 300 + 4 grupos focais)._

**Entrada (resumo):**

> Usos: IA para revisar a gramática da introdução e para sugerir códigos iniciais nos grupos focais.

**Trecho da saída esperada:**

| Uso | Etapa | Intervenção | Risco | Declarar? |
| --- | --- | --- | --- | --- |
| Revisão gramatical | Escrita | Baixa | Baixo | Sim, conforme a política do periódico |
| Sugestão de códigos | Análise | Média | Médio: envio de transcrições a serviço externo | Sim, informando anonimização e revisão humana |

Declaração: "Os autores utilizaram [FERRAMENTA] para revisão gramatical e para sugestão de códigos iniciais em transcrições anonimizadas; todas as decisões analíticas foram tomadas pelos autores, que assumem total responsabilidade pelo conteúdo."

## Prompts relacionados

- [P39](P39_verificacao_citacoes_parafrase.md)
