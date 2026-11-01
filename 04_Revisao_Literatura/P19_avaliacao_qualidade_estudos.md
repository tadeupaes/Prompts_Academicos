---
id: P19
titulo: "Avaliação de Qualidade e Risco de Viés"
modulo: "04. Revisão de Literatura"
abordagem: [revisão]
etapa: revisão de literatura
nivel: [mestrado, doutorado]
relacionados: [P02, P44]
versao: 1.1.0
atualizado: 2026-11-01
---

# P19 · Avaliação de Qualidade e Risco de Viés

> **Módulo:** 04. Revisão de Literatura · **Quando usar:** na etapa de avaliação crítica de uma revisão sistemática

**Objetivo:** Avaliar sistematicamente a qualidade metodológica e o risco de viés de estudos incluídos em uma revisão.

**Mecanismo epistemológico:** Seleciona a ferramenta adequada ao delineamento (RoB 2, ROBINS-I, Newcastle-Ottawa, CASP, JBI, MMAT) e aplica seus domínios item a item, com justificativa textual para cada julgamento.

## Prompt

```text
# PAPEL
Você é um avaliador metodológico treinado em ferramentas de risco de viés.
Você atua como SEGUNDO avaliador: sua avaliação será comparada à minha.

# ESTUDO
[COLE O TEXTO DO ESTUDO, ESPECIALMENTE MÉTODO E RESULTADOS]

# TAREFA
1. Identifique o delineamento do estudo e indique a ferramenta mais
   adequada (ex.: RoB 2 para ensaios randomizados; ROBINS-I para estudos
   não randomizados de intervenção; Newcastle-Ottawa para coorte/caso-
   controle; CASP ou JBI para qualitativos; MMAT para métodos mistos).
   Justifique.
2. Aplique a ferramenta domínio por domínio:
   | Domínio | Pergunta-guia | Evidência no texto (trecho) | Julgamento | Justificativa |
3. Atribua o julgamento global conforme as regras da própria ferramenta.
4. Liste as informações ausentes que impediram um julgamento seguro.

# RESTRIÇÕES
- Use apenas o que está no texto. Informação ausente = "Sem informação",
  nunca suposição favorável.
- Lembre-me de que a avaliação final deve ser feita por dois revisores
  humanos independentes, com resolução de divergências.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso R: revisão sobre intervenções baseadas em mindfulness para burnout em professores da educação básica._

**Entrada (resumo):**

> Estudo: ensaio randomizado por escola (cluster).

**Trecho da saída esperada:**

Ferramenta: RoB 2, com a extensão para ensaios randomizados por cluster.

| Domínio | Evidência no texto | Julgamento | Justificativa |
| --- | --- | --- | --- |
| D1: processo de randomização | "As escolas foram sorteadas" | Algumas preocupações | Não descreve o sigilo da alocação |
| D4: mensuração do desfecho | Burnout autorrelatado; participantes não cegos | Alto risco | Desfecho subjetivo com conhecimento da intervenção |

## Prompts relacionados

- [P02](../01_Metodologia/P02_protocolo_prisma_pico.md)
- [P44](../09_Publicacao/P44_checklist_diretrizes_equator.md)
