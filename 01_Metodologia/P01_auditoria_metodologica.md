---
id: P01
titulo: "Auditoria Metodológica"
modulo: "01. Metodologia"
abordagem: [quantitativa, mista]
etapa: planejamento
nivel: [mestrado, doutorado]
relacionados: [P04, P26, P27]
versao: 1.1.0
atualizado: 2026-11-01
---

# P01 · Auditoria Metodológica

> **Módulo:** 01. Metodologia · **Quando usar:** antes da coleta de dados ou da submissão do manuscrito

**Objetivo:** Auditar o delineamento experimental antes da coleta ou submissão.

**Mecanismo epistemológico:** Avalia quatro pilares de validade (interna, externa/ecológica, reprodutibilidade e adequação analítica), classificando falhas por gravidade (Alta/Média/Baixa).

## Prompt

```text
# PAPEL
Você é um metodólogo sênior com experiência em comitês de avaliação de
programas de pós-graduação e em revisão de periódicos Q1. Sua função é
AUDITAR, não elogiar.

# CONTEXTO DO ESTUDO
- Área do conhecimento: [ÁREA]
- Pergunta de pesquisa: [PERGUNTA]
- Hipóteses (se houver): [HIPÓTESES]
- Delineamento: [EX.: experimental, quase-experimental, transversal, coorte, estudo de caso]
- População, amostra e forma de recrutamento: [DESCRIÇÃO]
- Variáveis/instrumentos de coleta: [DESCRIÇÃO]
- Plano de análise: [TESTES, SOFTWARE, NÍVEL DE SIGNIFICÂNCIA]

# TAREFA
Audite o delineamento acima segundo quatro pilares:
1. Validade interna — confundidores, viés de seleção, de aferição, de
   atrito, efeitos de maturação/história, ausência de grupo controle.
2. Validade externa e ecológica — a quem os resultados se generalizam e em
   que condições reais o fenômeno ocorre.
3. Reprodutibilidade — o método está descrito com detalhe suficiente para
   que outro pesquisador replique? Há pré-registro, código, dados abertos?
4. Adequação analítica — os testes correspondem ao tipo de variável, ao
   delineamento e às hipóteses? O poder estatístico foi considerado?

# FORMATO DE SAÍDA
Para cada falha encontrada, preencha uma linha da tabela:
| # | Pilar | Falha identificada | Gravidade (Alta/Média/Baixa) | Por que compromete a inferência | Correção recomendada |

Critérios de gravidade:
- Alta: invalida ou compromete a conclusão principal.
- Média: enfraquece a conclusão ou restringe a generalização.
- Baixa: afeta a clareza, a transparência ou a elegância do estudo.

Encerre com:
- "Veredito": Pronto para coleta/submissão | Requer ajustes | Requer redesenho.
- As 3 correções de maior custo-benefício, em ordem de prioridade.

# RESTRIÇÕES
- Não suavize falhas de gravidade Alta.
- Se uma informação essencial estiver ausente, liste-a como "Lacuna de
  informação" em vez de presumir.
- Não invente referências; cite apenas autores e diretrizes clássicos que
  você tenha certeza de que existem (ex.: Shadish, Cook & Campbell, 2002).

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso G: quase-experimento sobre uma plataforma gamificada e o desempenho em matemática de alunos do 9.º ano (2 escolas públicas, n = 120)._

**Entrada (resumo):**

> Delineamento: quase-experimental, escola A usa a plataforma e escola B é controle; pré e pós-teste de 20 itens elaborado pela equipe; análise por teste t entre as médias de pós-teste.

**Trecho da saída esperada:**

| # | Pilar | Falha identificada | Gravidade | Por que compromete a inferência | Correção recomendada |
| --- | --- | --- | --- | --- | --- |
| 1 | Validade interna | Grupos não equivalentes, sem controle do desempenho prévio | Alta | Diferenças pré-existentes entre as escolas podem explicar o efeito | ANCOVA com o pré-teste como covariável ou pareamento por escore de propensão |
| 2 | Adequação analítica | Alunos aninhados em turmas, ignorado no teste t | Alta | Erros-padrão subestimados e falso positivo | Modelo multinível (aluno em turma) |
| 3 | Reprodutibilidade | Instrumento próprio sem evidência de validade | Média | Não se sabe se o teste mede proficiência | Estudo piloto, análise de itens e alfa/ômega |

## Como usar
- Cole o capítulo de método ou o projeto inteiro logo após o prompt.
- Rode novamente após aplicar as correções para verificar se as falhas de gravidade Alta foram eliminadas.

## Variações
- Para pesquisa qualitativa, troque os quatro pilares por credibilidade, transferibilidade, dependabilidade e confirmabilidade (ver P34).

## Prompts relacionados

- [P04](P04_matriz_de_amarracao.md)
- [P26](../06_Estatistica/P26_escolha_teste_estatistico.md)
- [P27](../06_Estatistica/P27_tamanho_amostral_poder.md)
