```gherkin
Feature: Busca de profissionais de saúde

  Background:
    Given que a pessoa usuária está autenticada na plataforma

  Scenario: Buscar profissional com sucesso
    When preencher o campo de busca com uma especialidade válida
    And executar a pesquisa
    Then o sistema deve exibir profissionais relacionados à busca

  Scenario: Buscar profissional utilizando localização
    When preencher a busca utilizando localização válida
    Then o sistema deve exibir profissionais compatíveis com a região pesquisada

  Scenario: Buscar profissional sem preencher filtros
    When executar a busca sem preencher filtros
    Then o sistema deve exibir resultados disponíveis ou comportamento esperado pela regra de negócio

  Scenario: Validar retorno para busca inexistente
    When pesquisar uma especialidade inexistente
    Then o sistema deve informar que não foram encontrados resultados

  Scenario: Contatar profissional com sucesso
    Given que existem profissionais listados na busca
    When acessar o perfil de um profissional
    And clicar em "Entrar em contato"
    Then o sistema deve permitir iniciar contato com o profissional

  Scenario: Validar carregamento da listagem de profissionais
    When realizar uma busca válida
    Then os cards de profissionais devem carregar corretamente
    And as informações devem permanecer legíveis

  Scenario: Validar responsividade da busca de profissionais no mobile
    Given que a aplicação está em resolução mobile
    When acessar a listagem de profissionais
    Then os filtros e resultados devem permanecer utilizáveis
    And não deve existir quebra crítica de layout

  Scenario: Validar responsividade da busca de profissionais no desktop
    Given que a aplicação está em resolução desktop
    When acessar a listagem de profissionais
    Then os componentes devem ser exibidos corretamente
```
---

