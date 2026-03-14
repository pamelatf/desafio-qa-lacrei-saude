# Bugs Identificados

# Funcionalidade: Onboarding / Continuação de cadastro

## Bug: Informações selecionadas não permanecem ao editar cadastro

**Descrição**

Ao retornar para editar informações previamente selecionadas no fluxo de cadastro, as opções escolhidas anteriormente não permanecem marcadas.

**Passos para reprodução**

1. Acessar o fluxo de cadastro da plataforma.
2. Selecionar opções durante o onboarding.
3. Avançar no fluxo.
4. Retornar para editar as informações preenchidas.

**Impacto**

Gera retrabalho e pode levar a inconsistência nos dados informados.

**Prioridade sugerida**

Média

# Funcionalidade: Login

## Bug: Feedback inconsistente ao tentar login com conta não ativada

**Descrição**

Ao tentar realizar login com uma conta não ativada, o sistema apresenta apenas um carregamento na primeira tentativa e somente exibe mensagem de erro na segunda tentativa.

**Passos para reprodução**

1. Acessar a tela de login.
2. Informar credenciais de conta não ativada.
3. Clicar em **Entrar**.

**Impacto**

Pode gerar confusão para a pessoa usuária, pois o sistema não fornece feedback imediato.

**Prioridade sugerida**

Média

# Funcionalidade: Recuperação de senha

## Bug: Recuperação de senha não confirma envio de e-mail

**Descrição**

Ao solicitar recuperação de senha com e-mail válido, o sistema retorna para a tela de login sem exibir confirmação clara de envio do e-mail.

**Passos para reprodução**

1. Acessar **Esqueci minha senha**.
2. Informar e-mail cadastrado.
3. Solicitar envio da recuperação.

**Impacto**

Usuário não tem certeza se o processo foi iniciado.

**Prioridade sugerida**

Alta

## Bug: Mensagem de validação pouco clara na recuperação de senha

**Descrição**

Durante testes de recuperação de senha com e-mail inválido ou não informado, a mensagem de validação exibida não é suficientemente clara para orientar a pessoa usuária.

**Passos para reprodução**

1. Acessar recuperação de senha.
2. Informar e-mail inválido ou deixar o campo vazio.
3. Tentar enviar solicitação.

**Impacto**

Pode gerar dificuldade de entendimento sobre o erro.

**Prioridade sugerida**

Baixa

# Funcionalidade: Busca de profissionais

## Bug: Aplicação falha ao acessar perfil de profissional

**Descrição**

Ao clicar em um profissional exibido nos resultados da busca, a aplicação apresenta falha e retorna para a tela inicial de busca.

**Passos para reprodução**

1. Realizar busca por localidade (ex: São Paulo).
2. Clicar em um profissional listado.

**Impacto**

Bloqueia o acesso ao perfil do profissional.

**Prioridade sugerida**

Alta

## Bug: Busca retorna resultados apenas em alguns tipos de termos

**Descrição**

A busca retornou resultados apenas quando o termo informado foi uma localidade.

**Passos para reprodução**

1. Informar diferentes termos de busca (nome, especialidade).
2. Executar busca.

**Impacto**

Limita a funcionalidade de busca.

**Prioridade sugerida**

Alta

## Bug: Interface não deixa claro que é necessário clicar na lupa para buscar

**Descrição**

O campo de busca não executa a pesquisa automaticamente ao pressionar Enter ou digitar o termo, exigindo o clique no ícone de lupa.

**Passos para reprodução**

1. Informar termo no campo de busca.
2. Pressionar Enter.

**Impacto**

Pode causar confusão para usuários.

**Prioridade sugerida**

Baixa

## Bug: Falta de estado claro quando não há resultados

**Descrição**

Quando a busca não retorna resultados, o sistema não apresenta uma mensagem clara informando que nenhum profissional foi encontrado.

**Passos para reprodução**

1. Informar termo sem correspondência.
2. Executar busca.

**Impacto**

Usuário pode interpretar que a busca falhou.

**Prioridade sugerida**

Média

# Funcionalidade: Contato com profissional

## Bug: Falha na validação do código SMS

**Descrição**

Após informar o código de verificação enviado por SMS, o sistema apresenta erro de comunicação com o servidor.

**Passos para reprodução**

1. Iniciar contato com profissional.
2. Informar telefone.
3. Solicitar código SMS.
4. Informar código recebido.
5. Confirmar.

**Impacto**

Impede o fluxo de contato com profissional.

**Prioridade sugerida**

Alta

## Bug: Fluxo fica bloqueado após erro de comunicação

**Descrição**

Após o erro de comunicação com o servidor, o sistema não permite continuar o fluxo ou tentar novamente de forma clara.

**Passos para reprodução**

1. Informar código SMS.
2. Receber erro de comunicação.

**Impacto**

Bloqueia completamente a jornada.

**Prioridade sugerida**

Alta
