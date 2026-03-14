# Desafio Técnico QA — Lacrei Saúde

## Objetivo
Este repositório reúne os artefatos produzidos durante a execução do desafio técnico de Quality Assurance da Lacrei Saúde, incluindo casos de teste, evidências, bugs identificados, sugestões de melhoria e análises complementares realizadas durante a avaliação da plataforma.

## Escopo avaliado
Durante a execução dos testes foram analisadas as seguintes funcionalidades da plataforma:

- Cadastro de pessoa usuária
- Autenticação (login)
- Recuperação de senha
- Busca de profissionais
- Contato com profissional
- Acessibilidade
- Desempenho
- Responsividade

## Como configurar o ambiente de testes
1. Acessar o ambiente de staging disponibilizado no desafio.
2. Utilizar um navegador atualizado (Chrome ou Firefox).
3. Ativar o modo responsivo do navegador para simular dispositivos móveis.
4. Configurar a viewport conforme o escopo definido no desafio.
5. Utilizar contas de teste válidas quando necessário para fluxos autenticados.

## Como executar os testes

### Testes manuais
1. Consultar os arquivos da pasta `casos-de-teste/`.
2. Executar os cenários descritos em linguagem Gherkin.
3. Reproduzir os fluxos diretamente na aplicação.
4. Registrar os resultados observados e evidências encontradas.

### Testes automatizados
A estrutura para automação foi preparada na pasta `automacao`, mas não houve tempo hábil para concluir esta exigência.

Caso os testes automatizados fossem implementados, a abordagem sugerida seria utilizar ferramentas como:

- Cypress
- Cucumber

## Organização da documentação
A estrutura do repositório foi organizada da seguinte forma:

- `casos-de-teste/`: cenários de teste organizados por funcionalidade
- `bugs/`: registro estruturado dos bugs identificados
- `melhorias/`: sugestões de melhoria observadas durante os testes
- `evidencias/`: gifs, prints e vídeos demonstrando comportamentos observados
- `acessibilidade/`: análise de acessibilidade da interface
- `desempenho/`: análise inicial de desempenho da aplicação
- `responsividade/`: análise de responsividade em diferentes resoluções
- `automacao/`: estrutura preparada para implementação de testes automatizados

## Checklist de segurança aplicado
Durante a análise foram observados os seguintes pontos relacionados ao comportamento da aplicação:

- validação de autenticação
- comportamento de sessão
- recuperação de acesso
- tratamento de erros em fluxos críticos
- consistência de navegação após autenticação

## Processo de rollback dos testes automatizados
Caso houvesse execução automatizada com impacto em massa de dados, o rollback previsto consistiria em:

1. remoção dos dados de teste criados
2. restauração do estado inicial do ambiente
3. reexecução apenas dos cenários afetados

## Documentação complementar

A documentação completa do teste, incluindo a execução detalhada dos cenários, evidências visuais e análise dos problemas encontrados, também foi organizada no Notion conforme solicitado no desafio técnico:

🔗 **Documentação completa no Notion:**  
(https://heather-earthworm-5ff.notion.site/Desafio-T-cnico-QA-Lacrei-Sa-de-135924c86e808047bd64d132ee1da8dc)
