---
id: P27
titulo: "Cálculo e Justificativa do Tamanho Amostral"
modulo: "06. Estatística"
abordagem: [quantitativa]
etapa: planejamento
nivel: [mestrado, doutorado]
relacionados: [P26]
versao: 1.1.0
atualizado: 2026-11-01
---

# P27 · Cálculo e Justificativa do Tamanho Amostral

> **Módulo:** 06. Estatística · **Quando usar:** no projeto de pesquisa, na submissão ao CEP ou quando o revisor questiona o N

**Objetivo:** Estimar e justificar o tamanho amostral com base em análise de poder ou em precisão de estimativa.

**Mecanismo epistemológico:** Explicita os quatro parâmetros da análise de poder (α, poder 1−β, tamanho de efeito esperado e teste) e exige que o tamanho de efeito seja justificado por literatura, estudo piloto ou menor efeito de interesse (SESOI), e não escolhido por conveniência.

## Prompt

```text
# PAPEL
Você é um bioestatístico que revisa justificativas de tamanho amostral.

# ENTRADA
- Hipótese principal e teste estatístico previsto: [TEXTO]
- Tamanho de efeito esperado e de onde ele vem: [EX.: d = 0,5 de meta-análise X / estudo piloto / não sei]
- α e poder desejados: [EX.: 0,05 e 0,80]
- Restrições práticas (população acessível, tempo, custo): [TEXTO]
- Perdas esperadas (%): [VALOR]

# TAREFA
1. Avalie a justificativa do tamanho de efeito. Se não houver, apresente as
   opções (literatura, piloto, SESOI, convenções de Cohen como último recurso)
   e seus riscos.
2. Calcule o N necessário, mostrando a fórmula ou os parâmetros a inserir
   no G*Power ou no R (pacote pwr), e acrescente a margem de perdas.
3. Faça uma análise de sensibilidade: N para efeitos 20% menores e 20% maiores.
4. Se o N viável for menor do que o necessário, proponha alternativas:
   delineamento intrassujeitos, covariáveis, desfecho mais sensível, estudo
   piloto declarado ou estimação com precisão em vez de teste de hipótese.
5. Redija o parágrafo de justificativa para o projeto/artigo.

# RESTRIÇÕES
- Mostre o cálculo de modo que eu possa reproduzi-lo; recomende conferir
  no software.
- Para pesquisa qualitativa, não aplique cálculo de poder; indique a P35.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso G: quase-experimento sobre uma plataforma gamificada e o desempenho em matemática de alunos do 9.º ano (2 escolas públicas, n = 120)._

**Entrada (resumo):**

> Efeito esperado: d = 0,40 (meta-análise do ensino básico). α = 0,05; poder = 0,80; perdas de 15%.

**Trecho da saída esperada:**

Teste t bilateral, d = 0,40 → n = 100 por grupo (200 no total). Com 15% de perdas, são 236 alunos.

| d | N total (sem perdas) |
| --- | --- |
| 0,32 | ≈ 310 |
| 0,48 | ≈ 140 |

O N disponível (120) só tem poder de cerca de 80% para d ≈ 0,52. Alternativas: incluir o pré-teste como covariável ou declarar o estudo como piloto. [CONFERIR NO G*POWER]

## Prompts relacionados

- [P26](P26_escolha_teste_estatistico.md)
