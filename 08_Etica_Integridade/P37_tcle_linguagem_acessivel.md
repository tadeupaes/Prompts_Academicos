---
id: P37
titulo: "TCLE em Linguagem Acessível"
modulo: "08. Ética e Integridade"
abordagem: [todas]
etapa: planejamento
nivel: [mestrado, doutorado]
relacionados: [P36]
versao: 1.1.0
atualizado: 2026-11-01
---

# P37 · TCLE em Linguagem Acessível

> **Módulo:** 08. Ética e Integridade · **Quando usar:** ao redigir ou revisar o Termo de Consentimento Livre e Esclarecido (ou o TALE)

**Objetivo:** Produzir um termo de consentimento completo e compreensível para o participante real.

**Mecanismo epistemológico:** Aplica princípios de linguagem simples (frases curtas, voz ativa, segunda pessoa, vocabulário cotidiano) sem perder nenhum elemento obrigatório do consentimento informado.

## Prompt

```text
# PAPEL
Você é especialista em ética em pesquisa e em linguagem simples.

# ENTRADA
- Resumo do projeto: [TEXTO]
- Perfil dos participantes (escolaridade, idade, contexto): [TEXTO]
- Tipo de termo: [TCLE (adultos) / TALE (crianças e adolescentes, com TCLE para responsáveis)]
- Rascunho atual (se houver): [COLE]

# TAREFA
1. Verifique a presença dos elementos essenciais: convite e justificativa;
   objetivos; procedimentos e duração; riscos e desconfortos com medidas de
   minimização; benefícios; liberdade de recusa e retirada sem prejuízo;
   sigilo e uso dos dados; ressarcimento e indenização; contatos do
   pesquisador e do CEP; via do participante.
2. Redija (ou reescreva) o termo:
   - Frases de até 20 palavras.
   - "Você" em vez de "o(a) participante".
   - Sem jargão (ou com explicação entre parênteses).
3. Avalie a legibilidade e aponte trechos ainda difíceis.
4. Se for TALE, adapte para a faixa etária indicada.

# RESTRIÇÕES
- Não omita nem suavize riscos.
- Não prometa benefícios diretos que o estudo não oferece.
- Inclua campos [PREENCHER] para dados de contato e número do CAAE.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso G: quase-experimento sobre uma plataforma gamificada e o desempenho em matemática de alunos do 9.º ano (2 escolas públicas, n = 120)._

**Entrada (resumo):**

> TALE para alunos de 14 a 15 anos, com TCLE para os responsáveis.

**Trecho da saída esperada:**

**Você está sendo convidado(a) para participar de uma pesquisa.** Queremos saber se um jogo no computador ajuda a aprender matemática. Se você aceitar, vai usar o jogo nas aulas por 8 semanas e fazer duas provinhas. Essas provas **não valem nota**. Você pode desistir quando quiser, e nada vai acontecer com você por isso.

## Prompts relacionados

- [P36](P36_submissao_cep_plataforma_brasil.md)
