# Como contribuir

Contribuições são bem-vindas: novos prompts, correções de referências, exemplos e resultados de testes.

## Propor um novo prompt

1. Copie o [`TEMPLATE_PROMPT.md`](TEMPLATE_PROMPT.md) para a pasta do módulo adequado.
2. Use o próximo código livre (`P51`, `P52`...) e nomeie o arquivo como `PNN_nome_em_minusculas.md`.
3. Preencha **todos** os campos do front-matter YAML.
4. Atualize o `README.md` do módulo e o índice do `README.md` principal.
5. Registre a mudança no [`CHANGELOG.md`](CHANGELOG.md).

## Critérios de qualidade

Todo prompt precisa ter:

- [ ] **Mecanismo epistemológico explícito** e com referência verificável (autor, ano, diretriz oficial).
- [ ] **Papel** com instrução de comportamento (auditar, questionar, não bajular).
- [ ] **Campos de entrada** em `[MAIÚSCULAS ENTRE COLCHETES]`.
- [ ] **Saída estruturada** (tabelas com colunas definidas, classificações com critérios).
- [ ] **Restrições anti-alucinação**: proibir referências, dados e falas inventadas; marcar incertezas com `[VERIFICAR]`.
- [ ] **Bloco de encerramento** "RESUMO PARA O PRÓXIMO PROMPT".
- [ ] **Exemplo fictício** com um trecho da saída esperada.
- [ ] Pelo menos **um teste registrado** em `testes/resultados.csv`, seguindo o [protocolo](testes/README.md).

## Corrigir uma referência

Abra uma *issue* informando o prompt, o trecho, a referência correta e a fonte (link para o DOI, a editora ou o documento oficial).

## Versionamento

O campo `versao` segue o versionamento semântico:

- **Patch** (1.1.**1**): correção de texto ou de referência.
- **Minor** (1.**2**.0): nova seção, passo ou restrição que não muda o uso do prompt.
- **Major** (**2**.0.0): mudança na estrutura de entrada ou de saída.
