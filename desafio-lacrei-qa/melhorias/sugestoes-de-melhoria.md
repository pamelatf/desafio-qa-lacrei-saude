# Sugestões de Melhoria

---

# Funcionalidade: Onboarding / Cadastro

## Melhoria: Preservar informações previamente selecionadas ao editar cadastro

**Descrição da melhoria**

Ao retornar para editar informações previamente preenchidas no fluxo de cadastro, o sistema deveria manter as opções anteriormente selecionadas marcadas.

**Justificativa**

Isso evita retrabalho e melhora a experiência da pessoa usuária ao revisar ou atualizar suas informações.

**Sugestão de implementação**

Persistir o estado das seleções feitas durante o cadastro, mantendo os dados carregados quando a pessoa usuária retorna para edição.

---

# Funcionalidade: Login / Autenticação

## Melhoria: Exibir mensagens de feedback mais claras durante o login

**Descrição da melhoria**

O sistema deveria apresentar mensagens claras e imediatas em todas as tentativas de login, principalmente quando o acesso não é permitido por conta não ativada.

**Justificativa**

Feedback claro reduz tentativas repetidas de login e melhora a compreensão da pessoa usuária sobre o que ocorreu.

**Sugestão de implementação**

Exibir mensagem informando que a conta ainda não foi ativada e orientar a pessoa usuária a verificar o e-mail de ativação.

---

# Funcionalidade: Recuperação de senha

## Melhoria: Confirmar envio de instruções de recuperação de senha

**Descrição da melhoria**

Após solicitar a recuperação de senha, o sistema deveria apresentar uma confirmação clara informando que o e-mail de recuperação foi enviado.

**Justificativa**

Isso dá segurança para a pessoa usuária de que o processo foi iniciado corretamente.

**Sugestão de implementação**

Exibir uma tela ou mensagem de confirmação com texto semelhante a:

"Enviamos instruções para redefinição de senha para o e-mail informado."

---

# Funcionalidade: Busca de profissionais

## Melhoria: Tornar comportamento da busca mais intuitivo

**Descrição da melhoria**

Permitir que a busca seja executada também ao pressionar **Enter** no campo de pesquisa, sem exigir o clique no ícone de lupa.

**Justificativa**

Esse comportamento é esperado pela maioria das pessoas usuárias em campos de busca.

**Sugestão de implementação**

Adicionar tratamento de evento para executar a busca ao pressionar a tecla **Enter**.

---

## Melhoria: Exibir mensagem clara quando não houver resultados

**Descrição da melhoria**

Quando a busca não retornar profissionais compatíveis, o sistema deveria exibir uma mensagem informando que nenhum resultado foi encontrado.

**Justificativa**

Evita que a pessoa usuária interprete a ausência de resultados como erro da aplicação.

**Sugestão de implementação**

Exibir mensagem como:

"Nenhum profissional encontrado para o termo pesquisado."

---

## Melhoria: Disponibilizar mecanismo claro para retornar à lista de resultados

**Descrição da melhoria**

Ao acessar o perfil de um profissional a partir da busca, o sistema deveria disponibilizar um botão claro para retornar à lista de resultados.

**Justificativa**

Facilita a navegação entre diferentes profissionais e melhora a experiência de exploração da plataforma.

**Sugestão de implementação**

Adicionar botão **“Voltar para resultados”** na página de perfil do profissional.

---

# Funcionalidade: Contato com profissional

## Melhoria: Permitir nova tentativa após erro de comunicação

**Descrição da melhoria**

Quando ocorre falha de comunicação com o servidor durante a validação do código SMS, o sistema deveria permitir nova tentativa de validação ou reenvio do código.

**Justificativa**

Evita que a pessoa usuária fique bloqueada no fluxo de contato com o profissional.

**Sugestão de implementação**

Exibir opções como:

- **Tentar novamente**
- **Reenviar código**

---

## Melhoria: Informar claramente o status do envio do código SMS

**Descrição da melhoria**

Após solicitar o envio do código de verificação, o sistema deveria apresentar mensagens claras indicando se o envio foi realizado com sucesso.

**Justificativa**

Aumenta a transparência do processo e reduz dúvidas sobre o funcionamento da etapa de verificação.

**Sugestão de implementação**

Apresentar mensagens de status como:

"Código enviado com sucesso para o número informado."
