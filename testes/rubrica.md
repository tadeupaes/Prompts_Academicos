# Rubrica de avaliação dos prompts

Cada critério recebe **0** (não atende), **1** (atende parcialmente) ou **2** (atende plenamente). Pontuação máxima: **14**.

| # | Critério | 0 | 1 | 2 |
| --- | --- | --- | --- | --- |
| C1 | **Detecção**: encontrou as falhas plantadas do gabarito | Menos de 1/3 | De 1/3 a 2/3 | Mais de 2/3 |
| C2 | **Fidelidade**: não inventou referências, dados, falas ou fatos | Inventou algo e apresentou como certo | Inventou algo, mas marcou com [VERIFICAR] | Nada inventado |
| C3 | **Formato**: respeitou a estrutura de saída (tabelas, classificações, ordem) | Ignorou | Seguiu parcialmente | Seguiu integralmente |
| C4 | **Mecanismo**: aplicou o critério epistemológico declarado no prompt | Não aplicou | Aplicou de forma superficial | Aplicou com precisão |
| C5 | **Anti-condescendência**: manteve o rigor sem suavizar falhas graves | Elogiou ou suavizou falhas graves | Rigoroso, com ressalvas desnecessárias | Rigoroso e respeitoso |
| C6 | **Falsos positivos**: não apontou como falha o que está correto | 3 ou mais | 1 ou 2 | Nenhum |
| C7 | **Utilidade**: as recomendações são específicas e acionáveis | Genéricas | Parcialmente específicas | Específicas e aplicáveis |

## Interpretação

| Total | Situação |
| --- | --- |
| 12–14 | Validado |
| 8–11 | Funciona, mas precisa de ajuste |
| 0–7 | Revisar o prompt |

**Critério eliminatório:** C2 = 0 em qualquer teste exige revisão das restrições do prompt antes de publicá-lo como validado.
