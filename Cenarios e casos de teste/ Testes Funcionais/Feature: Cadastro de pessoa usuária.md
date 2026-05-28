```gherkin
Feature: Cadastro de pessoa usuária

  Background:
    Given que a pessoa usuária acessa a página de cadastro da Lacrei Saúde

  Scenario: Realizar cadastro com sucesso []
    When preencher todos os campos obrigatórios com dados válidos
    And aceitar os termos da plataforma
    And clicar no botão "Cadastrar"
    Then o sistema deve criar a conta com sucesso
    And a pessoa usuária deve ser redirecionada para o fluxo pós-cadastro

  Scenario: Tentar realizar cadastro com campos obrigatórios vazios []
    When clicar no botão "Cadastrar" sem preencher os campos obrigatórios
    Then o sistema deve exibir mensagens de validação nos campos obrigatórios

  Scenario: Tentar realizar cadastro com e-mail inválido []
    When preencher o campo e-mail com um formato inválido
    And preencher os demais campos corretamente
    And clicar no botão "Cadastrar"
    Then o sistema deve exibir mensagem de e-mail inválido

  Scenario: Tentar realizar cadastro com senha inválida []
    When preencher o campo senha fora do padrão exigido
    And preencher os demais campos corretamente
    And clicar no botão "Cadastrar"
    Then o sistema deve exibir mensagem de senha inválida

  Scenario: Validar obrigatoriedade de aceite dos termos []
    When preencher todos os campos corretamente
    But não aceitar os termos da plataforma
    And clicar no botão "Cadastrar"
    Then o sistema deve impedir o cadastro da pessoa usuária

  Scenario: Validar redirecionamento após cadastro []
    When realizar cadastro com sucesso
    Then a pessoa usuária deve acessar o fluxo pós-cadastro

  Scenario: Validar comportamento responsivo da tela de cadastro no mobile []
    Given que a aplicação está em resolução mobile
    When acessar a tela de cadastro
    Then os campos e botões devem permanecer visíveis e utilizáveis
    And não deve existir quebra crítica de layout

  Scenario: Validar comportamento responsivo da tela de cadastro no desktop []
    Given que a aplicação está em resolução desktop
    When acessar a tela de cadastro
    Then os componentes devem ser exibidos corretamente
    And não deve existir sobreposição de elementos

```
