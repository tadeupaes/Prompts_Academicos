---
id: P46
titulo: "Projeto de Pesquisa para Seleção ou Fomento"
modulo: "10. Projeto e Defesa"
abordagem: [todas]
etapa: planejamento
nivel: [mestrado, doutorado]
relacionados: [P04, P47]
versao: 1.1.0
atualizado: 2026-11-01
---

# P46 · Projeto de Pesquisa para Seleção ou Fomento

> **Módulo:** 10. Projeto e Defesa · **Quando usar:** em processos seletivos de pós-graduação ou editais (CNPq, CAPES, FAPs)

**Objetivo:** Revisar e fortalecer um projeto segundo os critérios de avaliação do edital.

**Mecanismo epistemológico:** Converte o edital em uma rubrica de avaliação explícita e pontua o projeto critério por critério, como faria um parecerista ad hoc da agência.

## Prompt

```text
# PAPEL
Você é parecerista ad hoc de [AGÊNCIA/PROGRAMA] em [ÁREA].

# ENTRADA
- Critérios de avaliação do edital (cole o trecho do edital): [COLE]
- Projeto completo: [COLE]
- Limites de páginas/caracteres: [TEXTO]

# TAREFA
1. Transforme os critérios do edital em uma rubrica:
   | Critério | Peso | O que um projeto nota máxima apresenta |
2. Avalie o projeto em cada critério (nota + justificativa + trecho).
3. Aponte os pontos que costumam derrubar projetos: objetivo vago,
   viabilidade não demonstrada, cronograma irreal, orçamento incoerente,
   ausência de resultados esperados mensuráveis, falta de aderência à linha.
4. Sugira revisões específicas, em ordem de impacto na nota.
5. Verifique o cumprimento dos limites formais.

# RESTRIÇÕES
- Use somente os critérios do edital fornecido.
- Não invente produção prévia ou parcerias do proponente.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso G: quase-experimento sobre uma plataforma gamificada e o desempenho em matemática de alunos do 9.º ano (2 escolas públicas, n = 120)._

**Entrada (resumo):**

> Edital de iniciação à pesquisa de uma FAP; critérios: mérito, viabilidade, impacto e qualificação da equipe.

**Trecho da saída esperada:**

| Critério | Nota | Justificativa |
| --- | --- | --- |
| Viabilidade | 2/5 | O cronograma prevê a coleta antes da aprovação no CEP, e não há carta de anuência das escolas |
| Impacto | 3/5 | Os resultados esperados são genéricos ("melhorar o ensino"); defina produtos mensuráveis |

## Prompts relacionados

- [P04](../01_Metodologia/P04_matriz_de_amarracao.md)
- [P47](P47_cronograma_plano_de_riscos.md)
