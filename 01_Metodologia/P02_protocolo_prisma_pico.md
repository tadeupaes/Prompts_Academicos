---
id: P02
titulo: "Protocolo PRISMA & PICO"
modulo: "01. Metodologia"
abordagem: [revisão]
etapa: planejamento
nivel: [mestrado, doutorado]
relacionados: [P19, P20, P44]
versao: 1.1.0
atualizado: 2026-11-01
---

# P02 · Protocolo PRISMA & PICO

> **Módulo:** 01. Metodologia · **Quando usar:** no planejamento de uma Revisão Sistemática da Literatura (RSL)

**Objetivo:** Estruturar critérios de elegibilidade e equações de busca para RSL.

**Mecanismo epistemológico:** Decompõe a questão de pesquisa no framework PICO/SPIDER e constrói a *search string* booleana com operadores e truncamentos para bases indexadas.

## Prompt

```text
# PAPEL
Você é um bibliotecário especialista em revisões sistemáticas, com domínio
da diretriz PRISMA 2020 e das sintaxes de busca das principais bases.

# ENTRADA
- Questão de pesquisa em linguagem natural: [QUESTÃO]
- Área: [ÁREA]
- Bases pretendidas: [EX.: PubMed, Scopus, Web of Science, SciELO, LILACS, ERIC]
- Idiomas e recorte temporal: [IDIOMAS / ANOS]

# TAREFA
1. Classifique a questão: quantitativa/intervenção (use PICO), qualitativa
   (use SPIDER) ou exploratória (sugira PCC e indique a P20). Justifique.
2. Decomponha a questão no framework escolhido, em uma tabela:
   | Elemento | Definição no estudo | Termos controlados (MeSH/DeCS/Emtree) | Sinônimos e termos livres |
3. Construa a search string:
   - OR dentro de cada elemento; AND entre elementos.
   - Truncamento (*) e aspas para expressões exatas.
   - Uma versão adaptada à sintaxe de CADA base indicada (campos como
     [tiab], TITLE-ABS-KEY, TS=).
4. Defina critérios de elegibilidade:
   - Inclusão e exclusão, cada um com justificativa metodológica.
   - Tipos de estudo aceitos.
5. Proponha o fluxo de seleção conforme PRISMA 2020 (identificação →
   triagem → elegibilidade → inclusão), indicando quantos revisores
   independentes e como resolver divergências.

# FORMATO DE SAÍDA
Seções numeradas de 1 a 5, com as strings em blocos de código separados por base.

# RESTRIÇÕES
- Sinalize com [VERIFICAR] qualquer descritor MeSH/DeCS sobre o qual você
  não tenha certeza; o pesquisador deve conferir no tesauro oficial.
- Não estime número de resultados das buscas.
- Alerte se a questão estiver ampla demais para uma RSL viável.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso R: revisão sobre intervenções baseadas em mindfulness para burnout em professores da educação básica._

**Entrada (resumo):**

> Questão: intervenções de mindfulness reduzem o burnout de professores da educação básica? Bases: PubMed, ERIC, Scopus, SciELO.

**Trecho da saída esperada:**

| Elemento | Definição | Termos controlados | Termos livres |
| --- | --- | --- | --- |
| P | Professores da educação básica | "School Teachers" [VERIFICAR] | teacher*, educator*, "school staff" |
| I | Intervenções baseadas em mindfulness | "Mindfulness" [MeSH] | mindful*, MBSR, MBCT, "CARE program" |
| C | Lista de espera, controle ativo ou nenhum | — | "wait-list", control* |
| O | Burnout (MBI ou equivalente) | "Burnout, Professional" [MeSH] | burnout, "emotional exhaustion" |

PubMed: (teacher*[tiab] OR educator*[tiab]) AND (mindful*[tiab] OR MBSR[tiab] OR "Mindfulness"[Mesh]) AND (burnout[tiab] OR "emotional exhaustion"[tiab] OR "Burnout, Professional"[Mesh])

## Como usar
- Teste cada string na base real e ajuste a sensibilidade (muitos resultados irrelevantes → restringir; poucos → ampliar sinônimos).
- Registre o protocolo no PROSPERO (saúde) ou no OSF antes de iniciar a triagem.

## Prompts relacionados

- [P19](../04_Revisao_Literatura/P19_avaliacao_qualidade_estudos.md)
- [P20](../04_Revisao_Literatura/P20_revisao_de_escopo.md)
- [P44](../09_Publicacao/P44_checklist_diretrizes_equator.md)
