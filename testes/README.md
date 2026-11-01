# Testes dos prompts

Esta pasta serve para **avaliar empiricamente** se cada prompt faz o que promete, em diferentes modelos de IA. Um prompt só é considerado validado depois de ser testado com ao menos dois casos e dois modelos.

## Estrutura

| Arquivo | Conteúdo |
| --- | --- |
| [`rubrica.md`](rubrica.md) | Critérios de avaliação (0 a 2 pontos cada) |
| [`casos/`](casos/) | Quatro casos fictícios com **falhas plantadas** |
| [`gabaritos/`](gabaritos/) | Lista das falhas plantadas em cada caso, a que o modelo **não** deve ter acesso |
| [`resultados.csv`](resultados.csv) | Planilha de registro dos testes |

## Protocolo

1. **Escolha o prompt e o caso.** Use a coluna "Prompts indicados" da tabela abaixo.
2. **Abra uma conversa nova**, sem memória ou instruções personalizadas ativas, para não contaminar o teste.
3. **Cole o prompt** e preencha os campos com o texto do caso. Não envie o gabarito.
4. **Salve a resposta completa** em `testes/saidas/PNN_caso_modelo_data.md`.
5. **Pontue com a rubrica**, comparando a saída com o gabarito.
6. **Registre** uma linha em `resultados.csv`.
7. **Repita** com pelo menos mais um modelo (ex.: Claude, ChatGPT, Gemini) e, se possível, rode duas vezes no mesmo modelo para avaliar a consistência.

Quando um prompt tiver pontuação baixa em algum critério, ajuste o texto, aumente a versão (`versao` no YAML) e teste de novo.

## Casos disponíveis

| Caso | Arquivo | Tipo | Prompts indicados |
| --- | --- | --- | --- |
| G | [`caso_G_gamificacao.md`](casos/caso_G_gamificacao.md) | Quase-experimento quantitativo | P01, P04, P06, P07, P13, P26, P27 |
| Q | [`caso_Q_teleconsulta.md`](casos/caso_Q_teleconsulta.md) | Qualitativo com entrevistas | P08, P14, P34, P35, P36, P44 |
| R | [`caso_R_mindfulness.md`](casos/caso_R_mindfulness.md) | Revisão de literatura | P02, P11, P16, P39 |
| M | [`caso_M_tutoria.md`](casos/caso_M_tutoria.md) | Métodos mistos | P12, P13, P30, P49 |
