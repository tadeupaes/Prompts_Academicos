---
id: P40
titulo: "Plano de Gestão de Dados (FAIR + LGPD)"
modulo: "08. Ética e Integridade"
abordagem: [todas]
etapa: planejamento
nivel: [mestrado, doutorado]
relacionados: [P36, P38]
versao: 1.1.0
atualizado: 2026-11-01
---

# P40 · Plano de Gestão de Dados (FAIR + LGPD)

> **Módulo:** 08. Ética e Integridade · **Quando usar:** em projetos para agências de fomento ou antes de iniciar a coleta

**Objetivo:** Elaborar um Plano de Gestão de Dados (PGD) que garanta proteção dos participantes e reutilização dos dados.

**Mecanismo epistemológico:** Equilibra os princípios FAIR (Encontráveis, Acessíveis, Interoperáveis, Reutilizáveis) com as exigências da LGPD (Lei n.º 13.709/2018), aplicando anonimização/pseudonimização e níveis de acesso proporcionais à sensibilidade dos dados.

## Prompt

```text
# PAPEL
Você é especialista em gestão de dados de pesquisa e proteção de dados pessoais.

# ENTRADA
- Tipo de dado coletado (quanti/quali, áudio, vídeo, imagens, dados de saúde): [LISTA]
- Volume estimado e formatos: [TEXTO]
- Agência de fomento/instituição e exigências: [EX.: FAPESP, CNPq]
- Repositório pretendido: [EX.: repositório institucional, Zenodo, OSF, Dataverse]

# TAREFA
Elabore o PGD com as seções:
1. Descrição dos dados (tipo, formato, volume, origem).
2. Documentação e metadados (dicionário de variáveis, README, padrão de metadados).
3. Armazenamento e backup durante a pesquisa (regra 3-2-1, controle de acesso).
4. Dados pessoais e sensíveis: base legal na LGPD, anonimização ou
   pseudonimização, quem tem acesso, descarte.
5. Compartilhamento e preservação: o que será aberto, o que terá acesso
   restrito e por quê; repositório, licença (ex.: CC BY 4.0) e prazo.
6. Responsabilidades e recursos.
7. Checklist de anonimização para transcrições qualitativas.

# RESTRIÇÕES
- Marque [VERIFICAR] em exigências específicas de agências ou artigos da LGPD.
- Dados sensíveis (saúde, origem racial, religião etc.) exigem atenção
  especial; explicite os cuidados.

# ENCERRAMENTO
Ao final, inclua um bloco "RESUMO PARA O PRÓXIMO PROMPT" (até 8 linhas)
com as decisões e os resultados principais desta etapa, para que eu possa
colá-lo no próximo prompt do fluxo.
```

## Exemplo (caso fictício)

_Caso Q: estudo qualitativo com 14 entrevistas com enfermeiras da Atenção Primária sobre a teleconsulta._

**Entrada (resumo):**

> Dados: áudios de entrevistas, transcrições e dados sociodemográficos; repositório pretendido: institucional.

**Trecho da saída esperada:**

**4. Dados pessoais e sensíveis.** Os áudios são dados pessoais identificáveis (voz) e serão excluídos após a transcrição e a conferência. As transcrições serão pseudonimizadas (E01–E14), com remoção de nomes de unidades e bairros.

**5. Compartilhamento.** Apenas as transcrições anonimizadas, com acesso restrito mediante termo de uso, porque o risco de reidentificação em municípios pequenos é alto.

## Prompts relacionados

- [P36](P36_submissao_cep_plataforma_brasil.md)
- [P38](P38_declaracao_uso_ia.md)
