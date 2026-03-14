# Casos de Teste — Busca de Profissionais

## Funcionalidade: Busca de profissionais de saúde na plataforma Lacrei Saúde

Como uma pessoa usuária da plataforma  
Quero buscar profissionais de saúde  
Para encontrar opções compatíveis com minha necessidade  

## Cenário 1: Acessar a área de busca de profissionais

Dado que a pessoa usuária concluiu o cadastro e está autenticada na plataforma  
Quando acessa a área principal da aplicação  
Então o sistema deve exibir a interface de busca de profissionais  
E apresentar um campo de busca com botão de pesquisa  

## Cenário 2: Realizar busca informando o nome de um profissional

Dado que a pessoa usuária está na área de busca de profissionais  
Quando informa o nome de um profissional no campo de busca  
E aciona o botão de pesquisa (ícone de lupa)  
Então o sistema deve processar a busca  
E exibir uma lista de profissionais compatíveis com o termo informado  


## Cenário 3: Visualizar resultados após realizar uma busca

Dado que a pessoa usuária realizou uma busca por profissionais  
Quando existem resultados compatíveis com o termo informado  
Então o sistema deve apresentar uma lista de profissionais encontrados  
E exibir informações iniciais de identificação do profissional  


## Cenário 4: Acessar o perfil de um profissional a partir da lista de resultados

Dado que a pessoa usuária visualiza os resultados de uma busca  
Quando seleciona um profissional listado  
Então o sistema deve direcionar para a página de detalhes do profissional selecionado  
E apresentar as informações completas do perfil  


## Cenário 5: Disponibilizar mecanismo de retorno para a lista de resultados

Dado que a pessoa usuária acessou o perfil de um profissional a partir da busca  
Quando deseja retornar à lista de resultados  
Então o sistema deveria disponibilizar um mecanismo de navegação para retornar à busca  
