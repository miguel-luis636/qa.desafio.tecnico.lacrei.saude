```gherkin
Feature: Recuperação de senha

  Background:
    Given que a pessoa usuária acessa a tela de login

  Scenario: Solicitar recuperação de senha com sucesso
    When clicar em "Esqueci minha senha"
    And preencher um e-mail válido
    And solicitar recuperação
    Then o sistema deve exibir mensagem de envio da recuperação

  Scenario: Tentar recuperação com e-mail inválido
    When acessar o fluxo de recuperação de senha
    And preencher um e-mail inválido
    And clicar em recuperar senha
    Then o sistema deve exibir mensagem de e-mail inválido

  Scenario: Tentar recuperação com campo vazio
    When acessar a recuperação de senha
    And clicar em recuperar senha sem preencher o e-mail
    Then o sistema deve validar o campo obrigatório

  Scenario: Validar retorno para e-mail não cadastrado
    When solicitar recuperação utilizando um e-mail não cadastrado
    Then o sistema deve exibir mensagem apropriada conforme regra de negócio

  Scenario: Validar acesso ao fluxo de redefinição
    Given que a pessoa usuária recebeu o e-mail de recuperação
    When acessar o link de redefinição
    Then o sistema deve permitir cadastrar uma nova senha

  Scenario: Validar redefinição de senha com sucesso
    Given que a pessoa usuária acessou a redefinição de senha
    When informar uma nova senha válida
    And confirmar a nova senha
    And salvar alteração
    Then o sistema deve atualizar a senha com sucesso

  Scenario: Validar divergência entre senhas
    When preencher senha e confirmação diferentes
    And tentar salvar alteração
    Then o sistema deve exibir mensagem de divergência entre senhas

  Scenario: Validar responsividade da recuperação de senha no mobile
    Given que a aplicação está em resolução mobile
    When acessar o fluxo de recuperação
    Then os elementos devem permanecer acessíveis
    And não deve existir quebra crítica de layout

  Scenario: Validar responsividade da recuperação de senha no desktop
    Given que a aplicação está em resolução desktop
    When acessar o fluxo de recuperação
    Then os elementos devem ser exibidos corretamente
```
