---
id: P17
titulo: "Fichamento Crítico de Artigo"
modulo: "04. Revisão de Literatura"
abordagem: [todas]
etapa: revisão de literatura
nivel: [mestrado, doutorado]
relacionados: [P16, P18]
versao: 1.1.0
atualizado: 2026-11-01
---

# P17 · Fichamento Crítico de Artigo

> **Módulo:** 04. Revisão de Literatura · **Quando usar:** a cada artigo lido para a revisão

**Objetivo:** Produzir um fichamento padronizado que vá além do resumo, registrando avaliação crítica e utilidade para a própria pesquisa.

**Mecanismo epistemológico:** Separa o que o autor afirma (descrição) do que a evidência sustenta (avaliação) e do que o leitor fará com isso (apropriação), evitando a citação acrítica.

## Prompt

```text
# PAPEL
Você é um assistente de leitura crítica para pós-graduandos.

# ARTIGO
[COLE O TEXTO COMPLETO OU AS SEÇÕES PRINCIPAIS]

# MINHA PESQUISA (para avaliar a utilidade)
[1 A 3 FRASES SOBRE O SEU TEMA E A SUA PERGUNTA]

# TAREFA
Produza o fichamento com os campos:
1. Referência (no padrão [ABNT/APA], usando apenas dados presentes no texto;
   campos ausentes como [COMPLETAR]).
2. Problema e objetivo do estudo.
3. Referencial teórico e conceitos-chave (com definições usadas pelo autor).
4. Método: delineamento, amostra, instrumentos e análise.
5. Principais resultados (com números, se houver).
6. Conclusões declaradas pelos autores.
7. Avaliação crítica:
   - Pontos fortes metodológicos.
   - Limitações (declaradas e não declaradas).
   - As conclusões decorrem dos resultados?
8. Citações literais úteis (entre aspas, com página/seção, se disponíveis).
9. Utilidade para a minha pesquisa: como posso usar (base teórica,
   contraponto, comparação de resultados, modelo metodológico).
10. Palavras-chave para minha base de leitura.

# RESTRIÇÕES
- Citações literais devem ser cópia exata do texto fornecido.
- Não atribua ao artigo afirmações que não estão nele.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso R: revisão sobre intervenções baseadas em mindfulness para burnout em professores da educação básica._

**Entrada (resumo):**

> Artigo: ensaio clínico de um programa de mindfulness com 80 professores.

**Trecho da saída esperada:**

7. **Avaliação crítica**
- Ponto forte: randomização por escola, com sigilo de alocação descrito.
- Limitação não declarada: o desfecho é autorrelatado e os participantes sabiam o grupo, o que gera risco de viés de expectativa.
- As conclusões sobre "redução do burnout em longo prazo" não decorrem dos dados, porque o seguimento foi de apenas 8 semanas.

9. **Utilidade:** modelo de protocolo de intervenção; contraponto quanto à duração do efeito.

## Como usar
- Salve os fichamentos em uma pasta e use-os como corpus na P16 e na P18.

## Prompts relacionados

- [P16](P16_mapeamento_estado_da_arte.md)
- [P18](P18_matriz_de_sintese.md)
