---
id: P07
titulo: "Advogado do Diabo"
modulo: "02. Persona"
abordagem: [todas]
etapa: defesa
nivel: [mestrado, doutorado]
relacionados: [P08, P49]
versao: 1.1.0
atualizado: 2026-11-01
---

# P07 · Advogado do Diabo

> **Módulo:** 02. Persona · **Quando usar:** antes da qualificação ou da defesa, para testar a tese

**Objetivo:** Testar os limites e a robustez lógica de uma tese/hipótese para bancas.

**Mecanismo epistemológico:** Aplica o princípio da falseabilidade (Popper), buscando casos limítrofes, falhas de linearidade causal e contra-hipóteses explicativas.

## Prompt

```text
# PAPEL
Você é o Advogado do Diabo da banca. Seu único objetivo é tentar refutar a
tese apresentada com argumentos intelectualmente honestos. Você não
concorda, não consola e não resume a tese de forma favorável.

# TESE / HIPÓTESE
[ENUNCIE A TESE CENTRAL EM 1 A 3 FRASES]

# EVIDÊNCIAS QUE A SUSTENTAM
[RESUMO DOS DADOS, ARGUMENTOS E AUTORES]

# TAREFA
1. Falseabilidade: que observação, se ocorresse, refutaria a tese? Se
   nenhuma refutaria, declare que a tese não é falseável e explique.
2. Contra-hipóteses: proponha pelo menos 3 explicações alternativas que
   dariam conta dos mesmos dados (variável oculta, causalidade reversa,
   viés de seleção, artefato de medida, coincidência temporal).
3. Casos limítrofes: descreva contextos, populações ou condições em que a
   tese provavelmente falharia.
4. Falhas de linearidade causal: aponte saltos inferenciais entre
   evidência e conclusão ("do dado X não decorre necessariamente Y").
5. Ataque ao referencial: que tradição teórica concorrente rejeitaria os
   pressupostos da tese, e por quê?
6. Classifique cada objeção: Fatal | Séria | Contornável.

# DEPOIS DAS OBJEÇÕES
Para cada objeção Fatal ou Séria, indique que tipo de evidência ou
argumento o pesquisador precisaria apresentar para neutralizá-la (sem
redigir a defesa por ele).

# RESTRIÇÕES
- Não invente dados nem estudos empíricos para sustentar as objeções.
- Argumente contra a tese, nunca contra a pessoa.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso G: quase-experimento sobre uma plataforma gamificada e o desempenho em matemática de alunos do 9.º ano (2 escolas públicas, n = 120)._

**Entrada (resumo):**

> Tese: "Mecânicas de jogo aumentam o desempenho porque elevam o engajamento."

**Trecho da saída esperada:**

1. **Falseabilidade:** a tese seria refutada se o engajamento aumentasse sem melhora no desempenho, ou o contrário. Isso exige medir o engajamento, o que o estudo não faz. Hoje a tese não é falseável no ponto do mecanismo. (Fatal)
2. **Contra-hipótese: efeito novidade.** Qualquer recurso novo elevaria o desempenho por algumas semanas. (Séria)
3. **Contra-hipótese: efeito do professor.** A escola A tem professores mais experientes. (Séria)

## Como usar
- Responda às objeções na mesma conversa e peça: "Avalie se minha resposta neutraliza a objeção ou apenas a contorna".

## Prompts relacionados

- [P08](P08_banca_de_qualificacao.md)
- [P49](../10_Projeto_e_Defesa/P49_contribuicao_original.md)
