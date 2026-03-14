# Desafio Técnico QA — Lacrei Saúde

## Objetivo
Este repositório reúne os artefatos produzidos durante a execução do desafio técnico de Quality Assurance da Lacrei Saúde, incluindo casos de teste, evidências, bugs identificados, sugestões de melhoria e análises complementares.

## Escopo avaliado
As seguintes funcionalidades foram analisadas:

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
2. Utilizar navegador com modo responsivo habilitado.
3. Configurar viewport mobile conforme escopo do desafio.
4. Utilizar contas de teste válidas para navegação autenticada, quando necessário.

## Como executar os testes

### Testes manuais
1. Consultar os arquivos da pasta `casos-de-teste/`.
2. Executar os fluxos descritos em linguagem Gherkin.
3. Registrar os resultados observados.
4. Relacionar as evidências e bugs encontrados.

### Testes automatizados
Os testes automatizados, quando aplicáveis, devem ser executados a partir da pasta `automacao/`.

## Organização da documentação
- `casos-de-teste/`: cenários de teste por funcionalidade
- `bugs/`: registro dos bugs identificados
- `melhorias/`: sugestões de melhoria
- `evidencias/`: gifs, prints e vídeos
- `acessibilidade/`: análise de acessibilidade
- `desempenho/`: análise de desempenho
- `responsividade/`: análise de responsividade
- `automacao/`: estrutura destinada aos testes automatizados

## Checklist de segurança aplicado
Durante a análise foram observados os seguintes pontos:
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

## Observação
As evidências completas e a documentação consolidada também foram organizadas no Notion, conforme solicitado no desafio.
