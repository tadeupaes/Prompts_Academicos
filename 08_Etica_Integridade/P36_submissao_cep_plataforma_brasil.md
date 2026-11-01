---
id: P36
titulo: "Preparação para o CEP / Plataforma Brasil"
modulo: "08. Ética e Integridade"
abordagem: [todas]
etapa: planejamento
nivel: [mestrado, doutorado]
relacionados: [P37, P40]
versao: 1.1.0
atualizado: 2026-11-01
---

# P36 · Preparação para o CEP / Plataforma Brasil

> **Módulo:** 08. Ética e Integridade · **Quando usar:** antes de submeter o projeto ao Comitê de Ética em Pesquisa

**Objetivo:** Revisar o projeto quanto aos requisitos éticos e antecipar pendências do parecer do CEP.

**Mecanismo epistemológico:** Confronta o projeto com as Resoluções CNS n.º 466/2012 e n.º 510/2016 (ciências humanas e sociais), verificando riscos e benefícios, proteção de vulneráveis, confidencialidade e coerência entre documentos.

## Prompt

```text
# PAPEL
Você é membro experiente de um Comitê de Ética em Pesquisa (CEP) do
sistema CEP/Conep.

# ENTRADA
- Área: [SAÚDE / CIÊNCIAS HUMANAS E SOCIAIS / OUTRA]
- Projeto (objetivo, método, participantes, coleta, riscos, benefícios): [COLE]
- TCLE/TALE (se já existir): [COLE]
- Cronograma e orçamento: [COLE]

# TAREFA
1. Indique a resolução aplicável (466/2012, 510/2016 ou ambas) e justifique.
2. Faça uma revisão como parecerista, listando pendências prováveis:
   | Item | Problema | Fundamento (resolução/artigo, se tiver certeza) | Como corrigir |
   Verifique: riscos descritos de forma genérica ("risco mínimo") sem
   medidas de minimização; benefícios exagerados; participantes vulneráveis
   (menores, pessoas institucionalizadas, subordinados); confidencialidade
   e armazenamento dos dados; ressarcimento e indenização; coleta iniciada
   antes da aprovação no cronograma; incoerência entre projeto, TCLE e
   formulário da Plataforma Brasil.
3. Gere um checklist dos documentos a anexar.

# RESTRIÇÕES
- Marque [VERIFICAR NA RESOLUÇÃO] se não tiver certeza do artigo/inciso.
- Este prompt não substitui o parecer oficial nem a consulta ao CEP local.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso Q: estudo qualitativo com 14 entrevistas com enfermeiras da Atenção Primária sobre a teleconsulta._

**Entrada (resumo):**

> Área: ciências da saúde, com metodologia qualitativa; participantes são enfermeiras subordinadas às gestoras que farão a indicação.

**Trecho da saída esperada:**

| Item | Problema | Fundamento | Como corrigir |
| --- | --- | --- | --- |
| Recrutamento | Indicação pela chefia compromete a voluntariedade | Res. 510/2016 (pesquisa em ciências humanas e sociais) [VERIFICAR NA RESOLUÇÃO] | Convite direto pela pesquisadora, sem que a chefia saiba quem aceitou |
| Riscos | "Risco mínimo" sem medidas de minimização | Res. 466/2012 [VERIFICAR NA RESOLUÇÃO] | Descrever o risco de constrangimento e o direito de interromper a entrevista |

## Prompts relacionados

- [P37](P37_tcle_linguagem_acessivel.md)
- [P40](P40_plano_gestao_dados_lgpd.md)
