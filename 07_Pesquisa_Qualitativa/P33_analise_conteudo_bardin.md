---
id: P33
titulo: "Análise de Conteúdo (Bardin)"
modulo: "07. Pesquisa Qualitativa"
abordagem: [qualitativa]
etapa: análise
nivel: [mestrado, doutorado]
relacionados: [P32, P34]
versao: 1.1.0
atualizado: 2026-11-01
---

# P33 · Análise de Conteúdo (Bardin)

> **Módulo:** 07. Pesquisa Qualitativa · **Quando usar:** em pesquisas que adotam a análise de conteúdo categorial

**Objetivo:** Estruturar as três fases da análise de conteúdo e construir um sistema de categorias válido.

**Mecanismo epistemológico:** Aplica as fases de Bardin (pré-análise, exploração do material, tratamento e inferência) e as regras de categorização: exclusão mútua, homogeneidade, pertinência, objetividade/fidelidade e produtividade.

## Prompt

```text
# PAPEL
Você é um especialista em análise de conteúdo segundo Laurence Bardin
(*L'analyse de contenu*, 1977).

# ENTRADA
- Objetivo da análise: [TEXTO]
- Corpus (tipo e volume): [EX.: 20 entrevistas, 50 documentos]
- Definição de categorias: [A PRIORI (lista) / A POSTERIORI / MISTA]
- Amostra do material: [COLE TRECHOS]

# TAREFA
1. Pré-análise: proponha critérios de constituição do corpus (exaustividade,
   representatividade, homogeneidade, pertinência) e verifique se o meu
   corpus os atende.
2. Defina a unidade de registro (palavra, tema, frase) e a unidade de
   contexto, justificando.
3. Proponha um sistema de categorias:
   | Categoria | Definição operacional | Regra de inclusão | Regra de exclusão | Exemplo do corpus |
4. Teste as categorias com as regras de Bardin e aponte sobreposições.
5. Codifique os trechos fornecidos nas categorias e indique os casos ambíguos.
6. Sugira como calcular a concordância entre codificadores (ex.: kappa de Cohen).

# RESTRIÇÕES
- Use apenas o material fornecido.
- Diferencie claramente inferência (fase 3) de mera descrição.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso Q: estudo qualitativo com 14 entrevistas com enfermeiras da Atenção Primária sobre a teleconsulta._

**Entrada (resumo):**

> Categorias a posteriori; unidade de registro: tema.

**Trecho da saída esperada:**

| Categoria | Definição | Inclusão | Exclusão | Exemplo |
| --- | --- | --- | --- | --- |
| Sobrecarga de registro | Relatos de tarefas documentais adicionais geradas pela teleconsulta | Menção a prontuário, planilhas, sistemas | Queixas gerais de carga de trabalho sem relação com a teleconsulta | "Cada ligação vira três registros" (E04) |

## Prompts relacionados

- [P32](P32_analise_tematica.md)
- [P34](P34_criterios_rigor_qualitativo.md)
