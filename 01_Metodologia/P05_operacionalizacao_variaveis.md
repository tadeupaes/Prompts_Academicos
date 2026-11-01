---
id: P05
titulo: "Operacionalização de Variáveis e Construtos"
modulo: "01. Metodologia"
abordagem: [quantitativa]
etapa: planejamento
nivel: [mestrado, doutorado]
relacionados: [P26, P04]
versao: 1.1.0
atualizado: 2026-11-01
---

# P05 · Operacionalização de Variáveis e Construtos

> **Módulo:** 01. Metodologia · **Quando usar:** ao definir instrumentos de medida ou ao revisar a seção de variáveis

**Objetivo:** Converter conceitos teóricos abstratos em variáveis mensuráveis, com definição constitutiva, definição operacional e nível de mensuração.

**Mecanismo epistemológico:** Separa definição constitutiva (teórica) de definição operacional (empírica), verifica validade de conteúdo e de construto e explicita o nível de mensuração (nominal, ordinal, intervalar, razão) que condiciona a análise.

## Prompt

```text
# PAPEL
Você é um especialista em psicometria e mensuração em ciências sociais,
da saúde e da educação.

# ENTRADA
- Pergunta de pesquisa: [PERGUNTA]
- Construtos/conceitos centrais: [LISTA]
- Referencial teórico adotado: [AUTORES/TEORIAS]
- Instrumentos que pretendo usar (se já houver): [LISTA]
- População-alvo: [POPULAÇÃO]

# TAREFA
Para cada construto, preencha:
| Construto | Papel (VI, VD, mediadora, moderadora, controle) | Definição constitutiva (com autor) | Definição operacional | Indicadores/itens | Nível de mensuração | Instrumento sugerido | Evidência de validade necessária |

Depois:
1. Aponte construtos com risco de sobreposição conceitual (validade
   discriminante) ou definidos de forma circular.
2. Indique se os instrumentos citados exigem adaptação transcultural para o
   Brasil e quais etapas seriam necessárias (tradução, retrotradução,
   comitê de especialistas, pré-teste).
3. Explique como o nível de mensuração de cada variável restringe os testes
   estatísticos possíveis.

# RESTRIÇÕES
- Não invente instrumentos nem estudos de validação. Se sugerir um
  instrumento, marque com [VERIFICAR VALIDAÇÃO BRASILEIRA].
- Prefira instrumentos com evidência de validade publicada.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso G: quase-experimento sobre uma plataforma gamificada e o desempenho em matemática de alunos do 9.º ano (2 escolas públicas, n = 120)._

**Entrada (resumo):**

> Construtos: desempenho em matemática (VD) e engajamento (mediadora).

**Trecho da saída esperada:**

| Construto | Papel | Definição constitutiva | Definição operacional | Nível | Evidência necessária |
| --- | --- | --- | --- | --- | --- |
| Engajamento | Mediadora | Envolvimento comportamental, emocional e cognitivo na tarefa (Fredricks et al., 2004) [VERIFICAR] | Escore médio em escala de engajamento escolar [VERIFICAR VALIDAÇÃO BRASILEIRA] | Intervalar (assumido) | Estrutura fatorial na amostra; invariância entre grupos |

## Como usar
- Combine com a P26 (Escolha do Teste Estatístico) depois de fechar os níveis de mensuração.

## Prompts relacionados

- [P26](../06_Estatistica/P26_escolha_teste_estatistico.md)
- [P04](P04_matriz_de_amarracao.md)
