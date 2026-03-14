# Casos de Teste — Recuperação de Senha

## Funcionalidade: Recuperação de acesso à conta na plataforma Lacrei Saúde

Como uma pessoa usuária cadastrada  
Quero recuperar o acesso à minha conta  
Para redefinir minha senha caso eu a tenha esquecido  

## Cenário 1: Solicitar recuperação de senha com e-mail válido

Dado que a pessoa usuária está na tela de recuperação de senha  
Quando informa um e-mail cadastrado na plataforma  
E aciona a opção para enviar instruções de recuperação  
Então o sistema deve registrar a solicitação  
E informar que as instruções foram enviadas para o e-mail informado  


## Cenário 2: Tentar recuperar senha sem informar e-mail

Dado que a pessoa usuária está na tela de recuperação de senha  
Quando tenta enviar a solicitação sem preencher o campo de e-mail  
Então o sistema deve apresentar mensagem de validação  
E impedir o envio da solicitação  


## Cenário 3: Informar e-mail em formato inválido na recuperação de senha

Dado que a pessoa usuária está na tela de recuperação de senha  
Quando informa um e-mail em formato inválido  
E tenta enviar a solicitação  
Então o sistema deve apresentar mensagem de validação  
E impedir o envio  

## Cenário 4: Solicitar recuperação de senha com e-mail não cadastrado

Dado que a pessoa usuária está na tela de recuperação de senha  
Quando informa um e-mail que não possui cadastro na plataforma  
E aciona a opção de envio  
Então o sistema deve apresentar mensagem informando que não foi possível localizar a conta  
