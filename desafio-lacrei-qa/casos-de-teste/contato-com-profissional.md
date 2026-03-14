# Casos de Teste — Contato com Profissional

## Funcionalidade: Contato com profissional de saúde na plataforma Lacrei Saúde

Como uma pessoa usuária da plataforma  
Quero entrar em contato com um profissional de saúde  
Para iniciar o fluxo de atendimento ou agendamento  

---

## Cenário 1: Acessar a funcionalidade de contato com profissional

Dado que a pessoa usuária está autenticada na plataforma  
Quando acessa o fluxo de contato com um profissional  
Então o sistema deve exibir a tela de contato com o profissional  
E apresentar as informações iniciais necessárias para o atendimento  

---

## Cenário 2: Exibir formulário de confirmação de número de celular

Dado que a pessoa usuária acessou a tela de contato com o profissional  
Quando o sistema solicita a confirmação do número de celular  
Então o sistema deve exibir um campo para preenchimento do telefone  
E disponibilizar a opção **“Enviar código”**  

---

## Cenário 3: Solicitar envio do código de verificação por SMS

Dado que a pessoa usuária está na tela de confirmação de celular  
Quando informa um número de telefone válido  
E aciona a opção **“Enviar código”**  
Então o sistema deve registrar a solicitação de envio  
E apresentar a mensagem informando que o código foi enviado por SMS  

## Cenário 4: Exibir campo para preenchimento do código de verificação

Dado que a pessoa usuária solicitou o envio do código por SMS  
Quando o sistema conclui a solicitação  
Então o sistema deve exibir os campos para preenchimento do código de verificação  
E apresentar a opção de corrigir o número de celular informado  


## Cenário 5: Validar código de verificação informado pela pessoa usuária

Dado que a pessoa usuária recebeu o código de verificação  
Quando preenche o código nos campos disponíveis  
E aciona a opção **“Confirmar”**  
Então o sistema deve validar o código informado  
E permitir o prosseguimento do fluxo de contato com o profissional  


## Cenário 6: Exibir mensagem de erro em caso de falha de comunicação com o servidor

Dado que a pessoa usuária informou o código de verificação  
Quando ocorre uma falha de comunicação com o servidor durante a validação  
Então o sistema deve apresentar uma mensagem de erro  
E informar que a pessoa usuária deve tentar novamente mais tarde  


## Cenário 7: Impedir prosseguimento do fluxo quando a validação do código falhar

Dado que ocorreu erro na validação do código de verificação  
Quando a pessoa usuária permanece na tela de confirmação  
Então o sistema não deve permitir o avanço para a próxima etapa do contato  
E deve manter o fluxo bloqueado até que a validação seja concluída com sucesso  
