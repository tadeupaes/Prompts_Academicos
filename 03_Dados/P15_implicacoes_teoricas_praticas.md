---
id: P15
titulo: "Implicações Teóricas e Práticas"
modulo: "03. Dados"
abordagem: [todas]
etapa: escrita
nivel: [mestrado, doutorado]
relacionados: [P11, P49]
versao: 1.1.0
atualizado: 2026-11-01
---

# P15 · Implicações Teóricas e Práticas

> **Módulo:** 03. Dados · **Quando usar:** ao escrever a conclusão ou a seção de contribuições

**Objetivo:** Explicitar o que o estudo muda na teoria e na prática, sem exagero e com destinatários definidos.

**Mecanismo epistemológico:** Distingue contribuição incremental, de extensão de fronteira (novo contexto/população) e de revisão teórica (contradiz ou reformula), conectando cada implicação a um achado específico.

## Prompt

```text
# PAPEL
Você é um editor associado que exige que os autores digam com precisão
"so what?": o que muda por causa deste estudo.

# ENTRADA
- Referencial teórico central: [TEORIAS/AUTORES]
- Principais achados: [LISTA]
- Público prático potencial (gestores, professores, clínicos, formuladores de políticas): [LISTA]

# TAREFA
1. Implicações teóricas, em tabela:
   | Achado | Teoria/modelo afetado | Tipo de contribuição (confirma / estende / tensiona / reformula) | Formulação da contribuição em 1 frase |
2. Implicações práticas:
   | Achado | Destinatário | Ação concreta possível | Condições/cautelas para aplicar |
3. Agenda de pesquisa futura: 3 a 5 perguntas derivadas diretamente das
   lacunas ou tensões deste estudo, não perguntas genéricas.
4. Redija a seção em texto corrido.

# RESTRIÇÕES
- Cada implicação deve estar ancorada em um achado específico.
- Não recomende políticas públicas a partir de evidência exploratória sem
  explicitar a cautela.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso M: métodos mistos sobre tutoria entre pares e evasão em cursos de engenharia (questionário n = 300 + 4 grupos focais)._

**Entrada (resumo):**

> Referencial: modelo de integração de Tinto. Achado: o pertencimento é o mecanismo central da tutoria.

**Trecho da saída esperada:**

| Achado | Teoria afetada | Tipo de contribuição | Formulação |
| --- | --- | --- | --- |
| Tutoria reduz a evasão via pertencimento | Modelo de Tinto | Estende | O estudo mostra que a integração social pode ser construída de forma deliberada por programas de pares nos cursos de engenharia |

## Prompts relacionados

- [P11](P11_confronto_com_literatura.md)
- [P49](../10_Projeto_e_Defesa/P49_contribuicao_original.md)
