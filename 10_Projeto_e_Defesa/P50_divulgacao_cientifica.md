---
id: P50
titulo: "Divulgação Científica para Público Leigo"
modulo: "10. Projeto e Defesa"
abordagem: [todas]
etapa: divulgação
nivel: [mestrado, doutorado]
relacionados: [P13, P21]
versao: 1.1.0
atualizado: 2026-11-01
---

# P50 · Divulgação Científica para Público Leigo

> **Módulo:** 10. Projeto e Defesa · **Quando usar:** ao comunicar a pesquisa para a sociedade (redes, imprensa, relatório de impacto, pitch de 3 minutos)

**Objetivo:** Traduzir a pesquisa para o público não especialista sem distorcer os achados.

**Mecanismo epistemológico:** Aplica a pirâmide invertida (achado e relevância primeiro) e o controle de fidelidade: cada afirmação simplificada é confrontada com o achado original para evitar exagero, causalidade indevida e generalização.

## Prompt

```text
# PAPEL
Você é jornalista científico(a) com formação em [ÁREA], conhecido(a) por
textos acessíveis e rigorosos.

# ENTRADA
- Resumo do estudo: [COLE]
- Formato desejado: [POST DE REDE SOCIAL / TEXTO DE 400 PALAVRAS / ROTEIRO DE PITCH DE 3 MINUTOS / RELEASE]
- Público: [EX.: público geral, gestores públicos, professores da educação básica]

# TAREFA
1. Responda em uma frase cada: o que foi descoberto? por que importa para
   esse público? como sabemos? qual é o limite do que sabemos?
2. Produza o texto no formato pedido, com:
   - Abertura pelo achado ou por uma situação concreta.
   - Uma analogia ou exemplo do cotidiano.
   - Explicação breve de como o estudo foi feito.
   - Uma frase honesta sobre as limitações.
3. Faça o controle de fidelidade:
   | Frase simplificada | Achado original | Distorce? (Não / Risco / Sim) | Ajuste |
4. Sugira um título que não seja sensacionalista.

# RESTRIÇÕES
- Não transforme associação em causa nem "pode contribuir" em "resolve".
- Sem jargão; quando inevitável, explique o termo.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso G: quase-experimento sobre uma plataforma gamificada e o desempenho em matemática de alunos do 9.º ano (2 escolas públicas, n = 120)._

**Entrada (resumo):**

> Formato: post de rede social; público: professores da educação básica.

**Trecho da saída esperada:**

"Jogos digitais nas aulas de matemática: ajudam? Num estudo com 120 alunos do 9.º ano, quem usou uma plataforma com desafios e pontos teve notas um pouco maiores. Mas atenção: comparamos só duas escolas, então ainda não dá para dizer que foi o jogo que causou a melhora."

| Frase simplificada | Distorce? |
| --- | --- |
| "teve notas um pouco maiores" | Não (d = 0,35) |

## Prompts relacionados

- [P13](../03_Dados/P13_interpretacao_sem_overclaiming.md)
- [P21](../05_Escrita_Academica/P21_resumo_estruturado.md)
