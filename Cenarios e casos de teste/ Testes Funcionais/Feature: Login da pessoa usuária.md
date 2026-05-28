```gherkin
Feature: Login da pessoa usuária

  Background:
    Given que a pessoa usuária acessa a tela de login

  Scenario: Realizar login com sucesso [PASSOU]
    When preencher e-mail válido
    And preencher senha válida
    And clicar no botão "Entrar"
    Then o sistema deve autenticar a pessoa usuária com sucesso

  Scenario: Tentar login com senha inválida [PASSOU]
    When preencher e-mail válido
    And preencher senha inválida
    And clicar no botão "Entrar"
    Then o sistema deve exibir mensagem de credenciais inválidas

  Scenario: Tentar login com campos vazios [PASSOU]
    When clicar no botão "Entrar" sem preencher os campos
    Then o sistema deve validar os campos obrigatórios

  Scenario: Validar mensagem de erro para e-mail inválido [PASSOU]
    When preencher um e-mail inválido
    And preencher uma senha qualquer
    And clicar no botão "Entrar"
    Then o sistema deve exibir mensagem de e-mail inválido

  Scenario: Validar responsividade da tela de login no mobile [ NÃO PASSOU] (mesmo problema da tela de respomsividade)
    Given que a aplicação está em resolução mobile
    When acessar a tela de login
    Then os elementos da interface devem permanecer acessíveis
    And não deve existir quebra crítica de layout

  Scenario: Validar responsividade da tela de login no desktop [PASSOU]
    Given que a aplicação está em resolução desktop
    When acessar a tela de login
    Then os elementos devem ser exibidos corretamente
```
