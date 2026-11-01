---
id: P47
titulo: "Cronograma e Plano de Riscos da Pesquisa"
modulo: "10. Projeto e Defesa"
abordagem: [todas]
etapa: planejamento
nivel: [mestrado, doutorado]
relacionados: [P46, P36]
versao: 1.1.0
atualizado: 2026-11-01
---

# P47 · Cronograma e Plano de Riscos da Pesquisa

> **Módulo:** 10. Projeto e Defesa · **Quando usar:** no projeto, no início do ano letivo ou quando o cronograma atrasou

**Objetivo:** Construir um cronograma realista até a defesa, com dependências, marcos e plano de contingência.

**Mecanismo epistemológico:** Aplica decomposição de trabalho (WBS), identifica o caminho crítico (etapas que atrasam tudo) e a matriz de riscos probabilidade × impacto, com ação preventiva e plano B para cada risco alto.

## Prompt

```text
# PAPEL
Você é um orientador pragmático com experiência em gestão de projetos de pesquisa.

# ENTRADA
- Data de início e prazo final (defesa/depósito): [DATAS]
- Etapas previstas e status atual: [LISTA]
- Obrigações paralelas (disciplinas, estágio docência, trabalho, qualificação): [LISTA]
- Dependências externas (CEP, acesso a campo, coorientador, equipamentos): [LISTA]

# TAREFA
1. Decomponha a pesquisa em etapas e tarefas com duração estimada
   (otimista / provável / pessimista).
2. Monte o cronograma mensal (tabela tipo Gantt em texto ou Markdown).
3. Identifique o caminho crítico e os marcos (qualificação, aprovação no
   CEP, fim da coleta, versão para a banca).
4. Matriz de riscos:
   | Risco | Probabilidade | Impacto | Ação preventiva | Plano B | Gatilho para acionar o plano B |
5. Se o prazo for inviável, diga com franqueza e proponha cortes de escopo.

# RESTRIÇÕES
- Inclua folga (buffer) realista; tempo de revisão do orientador e de
  aprovação ética costuma ser subestimado.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso Q: estudo qualitativo com 14 entrevistas com enfermeiras da Atenção Primária sobre a teleconsulta._

**Entrada (resumo):**

> Início em março/2026; defesa em fevereiro/2028; CEP ainda não submetido.

**Trecho da saída esperada:**

Caminho crítico: submissão ao CEP → aprovação (prever de 2 a 4 meses) → entrevistas → análise → escrita.

| Risco | Probabilidade | Impacto | Prevenção | Plano B | Gatilho |
| --- | --- | --- | --- | --- | --- |
| Atraso na aprovação do CEP | Alta | Alto | Submeter até maio/2026 | Adiantar a revisão de literatura e o roteiro piloto | Sem parecer até agosto/2026 |

## Prompts relacionados

- [P46](P46_projeto_para_fomento.md)
- [P36](../08_Etica_Integridade/P36_submissao_cep_plataforma_brasil.md)
