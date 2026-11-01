---
id: P39
titulo: "Verificação de Citações e Paráfrase"
modulo: "08. Ética e Integridade"
abordagem: [todas]
etapa: revisão final
nivel: [mestrado, doutorado]
relacionados: [P11, P38]
versao: 1.1.0
atualizado: 2026-11-01
---

# P39 · Verificação de Citações e Paráfrase

> **Módulo:** 08. Ética e Integridade · **Quando usar:** na revisão final, especialmente se houve apoio de IA na escrita

**Objetivo:** Conferir se cada citação sustenta de fato a afirmação a que está associada e se as paráfrases não configuram plágio.

**Mecanismo epistemológico:** Aplica a verificação afirmação → fonte (*citation accuracy*), classificando cada citação como apoio total, parcial, inexistente ou distorcido, e avalia a paráfrase pela transformação da estrutura e não apenas pela troca de sinônimos.

## Prompt

```text
# PAPEL
Você é auditor de integridade acadêmica.

# ENTRADA
- Trecho do meu texto com citações: [COLE]
- Trechos das fontes originais correspondentes (copiados dos PDFs): [COLE, IDENTIFICANDO A FONTE]

# TAREFA
1. Para cada citação, compare minha afirmação com o trecho original:
   | Minha afirmação | Fonte citada | Trecho original | Classificação (Apoio total / Parcial / Não apoia / Distorce) | Ajuste necessário |
2. Avalie as paráfrases:
   - Paráfrase adequada (ideia reformulada com estrutura própria e citação).
   - Paráfrase superficial (troca de sinônimos com estrutura original;
     risco de plágio).
   - Cópia sem aspas.
   Para as superficiais, sugira reformulação ou citação direta.
3. Aponte citações de segunda mão (apud) que deveriam ser conferidas no original.
4. Liste as citações do meu texto para as quais NÃO forneci o trecho
   original, como pendências de verificação.

# RESTRIÇÕES
- Não verifique fontes que eu não forneci; nunca presuma que uma
  referência existe ou diz algo.
- Lembre-me de usar também um software de detecção de similaridade da instituição.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso R: revisão sobre intervenções baseadas em mindfulness para burnout em professores da educação básica._

**Entrada (resumo):**

> Afirmação: "Programas de mindfulness reduzem o burnout em 50% (Autor B, 2020)." O trecho original informa redução de 50% apenas na subescala de exaustão emocional.

**Trecho da saída esperada:**

| Minha afirmação | Fonte | Trecho original | Classificação | Ajuste |
| --- | --- | --- | --- | --- |
| "reduzem o burnout em 50%" | Autor B (2020) | "reduction of 50% in the emotional exhaustion subscale" | Distorce | "reduziram em 50% os escores de exaustão emocional, uma das dimensões do burnout (Autor B, 2020)" |

## Prompts relacionados

- [P11](../03_Dados/P11_confronto_com_literatura.md)
- [P38](P38_declaracao_uso_ia.md)
