# Casos de Teste — Autenticação (Login)

## Funcionalidade: Autenticação de pessoa usuária na plataforma Lacrei Saúde

Como uma pessoa usuária já cadastrada  
Quero acessar minha conta na plataforma  
Para acessar os serviços disponíveis e buscar profissionais de saúde  

---

## Cenário 1: Realizar login com credenciais válidas

Dado que a pessoa usuária está na tela de login da plataforma  
Quando informa um e-mail cadastrado  
E informa uma senha válida  
E aciona a opção **"Entrar"**  
Então o sistema deve autenticar a pessoa usuária  
E exibir mensagem de boas-vindas exibindo a área principal  

---

## Cenário 2: Tentar realizar login sem preencher os campos obrigatórios

Dado que a pessoa usuária está na tela de login  
Quando tenta acionar a opção **"Entrar"** sem preencher os campos  
Então o sistema deve apresentar mensagens de validação de campos obrigatórios  
E abortar a tentativa de autenticação  

---

## Cenário 3: Tentar realizar login com credenciais inválidas

Dado que a pessoa usuária está na tela de login  
Quando informa um e-mail não cadastrado ou uma senha incorreta  
E aciona a opção **"Entrar"**  
Então o sistema deve informar que as credenciais são inválidas  
E impedir o acesso à plataforma  

---

## Cenário 4: Alternar visibilidade da senha no campo de autenticação

Dado que a pessoa usuária está na tela de login  
Quando informa um valor no campo de senha  
E aciona o ícone de visualização da senha  
Então o sistema deve exibir a senha informada  
E permitir ocultá-la novamente ao acionar o ícone  

---

## Cenário 5: Tentar realizar login sem ativação da conta

Dado que a pessoa usuária está na tela de login  
Quando informa os dados de um cadastro recém realizado  
E sem validar o e-mail  
Então o sistema deve informar que é necessária a ativação do cadastro  
E impedir o acesso à plataforma  

---

## Cenário 6: Manter a pessoa usuária autenticada após recarregar a página

Dado que a pessoa usuária realizou login com sucesso  
Quando recarrega a página ou acessa novamente a plataforma na mesma sessão  
Então o sistema deve manter o estado autenticado corretamente  
E exibir os elementos compatíveis com uma pessoa usuária logada  

---

## Cenário 7: Exibir opção de logout para pessoa usuária autenticada

Dado que a pessoa usuária está autenticada na plataforma  
Quando acessa os elementos de perfil ou navegação da conta  
Então o sistema deve disponibilizar uma opção visível para encerramento da sessão  
