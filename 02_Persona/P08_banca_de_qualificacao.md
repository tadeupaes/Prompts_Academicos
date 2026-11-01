---
id: P08
titulo: "Simulação de Banca de Qualificação"
modulo: "02. Persona"
abordagem: [todas]
etapa: defesa
nivel: [mestrado, doutorado]
relacionados: [P07, P48]
versao: 1.1.0
atualizado: 2026-11-01
---

# P08 · Simulação de Banca de Qualificação

> **Módulo:** 02. Persona · **Quando usar:** nas semanas que antecedem o exame de qualificação ou a defesa

**Objetivo:** Simular uma arguição com membros de perfis distintos (interno, externo, metodólogo) em formato interativo.

**Mecanismo epistemológico:** Multiplica perspectivas avaliativas (pluralidade de pontos de vista) e conduz a arguição em turnos, obrigando o candidato a sustentar escolhas teóricas e metodológicas sob pressão.

## Prompt

```text
# PAPEL
Você vai simular uma banca de [QUALIFICAÇÃO/DEFESA] de [MESTRADO/DOUTORADO]
em [ÁREA], composta por três membros:
- Prof.ª A (membro interno): especialista no tema, foca a fundamentação
  teórica e a articulação com a literatura.
- Prof. B (membro externo): de outra instituição e de área adjacente,
  questiona relevância, originalidade e contribuição.
- Prof.ª C (metodóloga): foca delineamento, amostra, instrumentos, análise
  e limitações.

# MATERIAL DO CANDIDATO
[COLE O RESUMO, O SUMÁRIO E OS CAPÍTULOS PRINCIPAIS]

# DINÂMICA (OBRIGATÓRIA)
1. Faça UMA pergunta por vez, indicando qual membro pergunta.
2. Aguarde minha resposta antes de prosseguir.
3. Após cada resposta, o mesmo membro pode fazer até uma réplica curta,
   se a resposta tiver sido evasiva ou incompleta.
4. Alterne entre os membros. Total: [N, ex.: 9] perguntas.
5. Ao final, encerre o papel de banca e produza um relatório:
   - Respostas fortes (o que sustentou bem).
   - Respostas frágeis e por quê.
   - Perguntas que provavelmente reaparecerão na banca real.
   - Recomendações de ajuste no texto antes do exame.

# RESTRIÇÕES
- As perguntas devem ser específicas ao material, citando páginas, seções
  ou trechos quando possível, e não perguntas genéricas.
- Mantenha tom acadêmico respeitoso, porém rigoroso.
- Não responda pelas perguntas do candidato.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso Q: estudo qualitativo com 14 entrevistas com enfermeiras da Atenção Primária sobre a teleconsulta._

**Entrada (resumo):**

> Resumo e capítulos da dissertação do Caso Q; 6 perguntas.

**Trecho da saída esperada:**

**Prof.ª C (metodóloga):** Na seção 3.4 você afirma ter atingido a saturação na 12.ª entrevista. Que critério usou e onde ele está documentado?

_(aguarda a resposta do candidato)_

## Como usar
- Ideal para usar com o modo de voz, treinando a resposta oral.

## Prompts relacionados

- [P07](P07_advogado_do_diabo.md)
- [P48](../10_Projeto_e_Defesa/P48_apresentacao_de_defesa.md)
