# Casos de Teste — Cadastro de Pessoa Usuária

## Funcionalidade: Cadastro de pessoa usuária na plataforma Lacrei Saúde

Como uma pessoa usuária  
Quero criar uma conta na plataforma  
Para acessar os serviços disponíveis e buscar profissionais de saúde

---

## Cenário 1: Realizar cadastro com dados válidos

Dado que a pessoa usuária está na tela de criação de conta  
Quando preenche todos os campos obrigatórios com dados válidos  
E aceita os termos de uso e a política de privacidade  
E confirma ter 18 anos ou mais  
E aciona a opção **"Cadastrar"**  
Então o sistema deve concluir o cadastro com sucesso  
E informar que é necessário ativar a conta por meio do e-mail cadastrado  
E redirecionar a pessoa usuária para a tela de login  

---

## Cenário 2: Tentar realizar cadastro sem preencher campos obrigatórios

Dado que a pessoa usuária está na tela de criação de conta  
Quando tenta acionar a opção **"Cadastrar"** sem preencher os campos obrigatórios  
Então o sistema deve manter o botão **Cadastrar** desabilitado  
E apenas habilitá-lo quando todos os campos obrigatórios forem informados  

---

## Cenário 3: Informar e-mails diferentes nos campos de e-mail e confirmação

Dado que a pessoa usuária está na tela de criação de conta  
Quando informa um e-mail no campo **"E-mail"**  
E informa um e-mail diferente no campo **"Confirme seu e-mail"**  
Então o sistema deve apresentar uma mensagem de inconsistência entre os e-mails  
E impedir a continuidade do cadastro  

---

## Cenário 4: Informar senha que não atende aos critérios mínimos

Dado que a pessoa usuária está na tela de criação de conta  
Quando informa uma senha que não atende aos critérios mínimos de segurança  
Então o sistema deve indicar quais critérios não foram atendidos  
E impedir a criação da conta  

---

## Cenário 5: Informar confirmação de senha diferente da senha principal

Dado que a pessoa usuária está na tela de criação de conta  
Quando informa uma senha válida  
E informa uma confirmação de senha diferente  
Então o sistema deve apresentar uma mensagem de inconsistência entre as senhas  
E impedir a conclusão do cadastro  

---

## Cenário 6: Tentar realizar cadastro sem aceitar os termos de uso

Dado que a pessoa usuária está na tela de criação de conta  
Quando preenche todos os campos obrigatórios  
E não aceita os termos de uso e a política de privacidade  
Então o botão **Cadastrar** deve permanecer desabilitado  
E o sistema deve exigir o aceite dos termos para prosseguir  

---

## Cenário 7: Tentar realizar cadastro sem confirmar idade mínima

Dado que a pessoa usuária está na tela de criação de conta  
Quando preenche todos os campos obrigatórios  
E não seleciona a opção de confirmação de idade mínima  
Então o botão **Cadastrar** deve permanecer desabilitado  
E o sistema deve exigir a confirmação de maioridade para prosseguir  

---

## Cenário 8: Exibir tela de continuação do cadastro no primeiro acesso

Dado que a pessoa usuária concluiu o cadastro inicial  
Quando acessa a plataforma pela primeira vez  
E o sistema autentica o acesso  
Então o sistema deve apresentar a tela de boas-vindas do onboarding  
E exibir o botão **“Continuar cadastro”**  

---

## Cenário 9: Iniciar o fluxo de continuação do cadastro

Dado que a pessoa usuária iniciou a continuação do cadastro  
Quando responde todas as perguntas obrigatórias do fluxo  
E finaliza o onboarding  
Então o sistema deve apresentar a mensagem **“Seu cadastro foi concluído!”**  
E exibir o resumo das informações preenchidas  
E permitir o acesso à área principal da plataforma  

---

## Cenário 10: Impedir avanço no onboarding com informações obrigatórias não preenchidas

Dado que a pessoa usuária está em uma etapa da continuação do cadastro  
Quando tenta avançar sem preencher informações obrigatórias  
Então o sistema deve apresentar validações de preenchimento  
E impedir a continuidade do fluxo  

---

## Cenário 11: Editar informações do cadastro após conclusão do onboarding

Dado que a pessoa usuária concluiu o onboarding  
E está na tela de resumo do cadastro  
Quando acessa a opção **“Editar dados”**  
Então o sistema deve permitir a alteração das informações do perfil  
E salvar as modificações realizadas  

---

## Cenário 12: Não exibir novamente a continuação do cadastro após conclusão do fluxo

Dado que a pessoa usuária já concluiu a continuação do cadastro  
Quando acessa novamente a plataforma  
Então o sistema não deve reapresentar a tela de boas-vindas do primeiro acesso  
E deve direcionar a pessoa usuária para a área principal da plataforma  
