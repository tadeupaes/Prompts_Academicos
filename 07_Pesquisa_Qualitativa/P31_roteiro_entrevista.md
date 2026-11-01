---
id: P31
titulo: "Roteiro de Entrevista Semiestruturada"
modulo: "07. Pesquisa Qualitativa"
abordagem: [qualitativa]
etapa: planejamento
nivel: [mestrado, doutorado]
relacionados: [P35, P36]
versao: 1.1.0
atualizado: 2026-11-01
---

# P31 · Roteiro de Entrevista Semiestruturada

> **Módulo:** 07. Pesquisa Qualitativa · **Quando usar:** ao elaborar o instrumento de coleta qualitativa

**Objetivo:** Construir um roteiro de entrevista alinhado aos objetivos, com perguntas abertas, neutras e bem sequenciadas.

**Mecanismo epistemológico:** Deriva cada pergunta de um objetivo específico (matriz objetivo → tema → pergunta → sondagem), elimina perguntas indutoras, duplas ou dicotômicas e organiza o funil (abertura → núcleo → fechamento).

## Prompt

```text
# PAPEL
Você é um pesquisador qualitativo experiente em entrevistas em
profundidade (Kvale; Brinkmann).

# ENTRADA
- Objetivos específicos: [LISTA]
- Participantes (perfil): [DESCRIÇÃO]
- Abordagem teórico-metodológica: [EX.: fenomenologia, teoria fundamentada, estudo de caso]
- Duração prevista: [MINUTOS]

# TAREFA
1. Monte a matriz:
   | Objetivo específico | Tema | Pergunta principal | Sondagens (probes) |
2. Organize o roteiro em blocos: rapport e perguntas de abertura → núcleo
   temático → perguntas de fechamento ("Há algo mais que gostaria de dizer?").
3. Revise cada pergunta e aponte:
   - Indução de resposta ("Você não acha que...?").
   - Pergunta dupla (duas questões em uma).
   - Fechada (sim/não) sem necessidade.
   - Jargão inacessível ao participante.
4. Sugira um protocolo de piloto (com quantas pessoas e o que observar).

# RESTRIÇÕES
- Linguagem adequada ao perfil dos participantes.
- Se o tema for sensível, sinalize cuidados éticos e de acolhimento (ver P36).

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso Q: estudo qualitativo com 14 entrevistas com enfermeiras da Atenção Primária sobre a teleconsulta._

**Entrada (resumo):**

> OE2: compreender como a teleconsulta alterou a relação enfermeira-paciente.

**Trecho da saída esperada:**

| Objetivo | Tema | Pergunta principal | Sondagens |
| --- | --- | --- | --- |
| OE2 | Relação de cuidado | "Conte-me sobre uma teleconsulta que ficou marcada para você." | "O que foi diferente de um atendimento presencial?" / "Como você percebeu a reação do paciente?" |

Pergunta a evitar: "Você não acha que a teleconsulta deixa o atendimento mais frio?" (indutora).

## Prompts relacionados

- [P35](P35_saturacao_amostragem.md)
- [P36](../08_Etica_Integridade/P36_submissao_cep_plataforma_brasil.md)
