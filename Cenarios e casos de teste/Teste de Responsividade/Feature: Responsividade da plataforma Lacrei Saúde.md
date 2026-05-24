```gherkin id="n4zq7x"
Feature: Responsividade da plataforma Lacrei Saúde

  Background:
    Given que a pessoa usuária acessa a plataforma Lacrei Saúde

  # Responsividade - Tela de Login

  Scenario: Validar layout da tela de login no mobile
    Given que a aplicação está na resolução de até 600px
    When acessar a tela de login
    Then os elementos devem ser exibidos corretamente
    And não deve existir scroll horizontal
    And não deve existir quebra crítica de layout

  Scenario: Validar funcionalidade da tela de login no mobile
    Given que a aplicação está na resolução mobile
    When preencher os campos de login
    And clicar no botão "Entrar"
    Then os campos e botões devem permanecer funcionais

  Scenario: Validar usabilidade da tela de login no mobile
    Given que a aplicação está na resolução mobile
    When interagir com os componentes da tela
    Then os botões devem possuir tamanho adequado para toque
    And os campos devem permanecer legíveis

  Scenario: Validar layout da tela de login no desktop
    Given que a aplicação está na resolução acima de 1024px
    When acessar a tela de login
    Then os componentes devem permanecer alinhados corretamente
    And não deve existir sobreposição de elementos

  # Responsividade - Cadastro

  Scenario: Validar layout da tela de cadastro no mobile
    Given que a aplicação está na resolução mobile
    When acessar a tela de cadastro
    Then os formulários devem se adaptar corretamente à tela
    And os campos devem permanecer visíveis

  Scenario: Validar funcionalidade do cadastro no mobile
    Given que a aplicação está na resolução mobile
    When preencher os campos do cadastro
    And enviar o formulário
    Then o sistema deve permitir concluir o cadastro normalmente

  Scenario: Validar usabilidade do cadastro no mobile
    Given que a aplicação está na resolução mobile
    When navegar pelos campos do formulário
    Then os componentes devem possuir boa legibilidade
    And os elementos clicáveis devem ser acessíveis

  Scenario: Validar layout da tela de cadastro no desktop
    Given que a aplicação está na resolução desktop
    When acessar a tela de cadastro
    Then os elementos devem permanecer organizados corretamente

  # Responsividade - Busca de profissionais

  Scenario: Validar layout da busca de profissionais no mobile
    Given que a aplicação está na resolução mobile
    When acessar a listagem de profissionais
    Then os cards de profissionais devem ser exibidos corretamente
    And não deve existir quebra visual

  Scenario: Validar funcionalidade da busca de profissionais no mobile
    Given que a aplicação está na resolução mobile
    When realizar busca de profissionais
    Then os filtros e resultados devem funcionar corretamente

  Scenario: Validar usabilidade da busca de profissionais no mobile
    Given que a aplicação está na resolução mobile
    When navegar pelos resultados da busca
    Then os textos devem permanecer legíveis
    And os botões devem estar acessíveis para interação

  Scenario: Validar layout da busca de profissionais no desktop
    Given que a aplicação está na resolução desktop
    When acessar os resultados da busca
    Then os componentes devem permanecer alinhados corretamente

  # Responsividade - Contato com profissional

  Scenario: Validar layout da tela de contato no mobile
    Given que a aplicação está na resolução mobile
    When acessar o contato de um profissional
    Then as informações devem permanecer organizadas corretamente

  Scenario: Validar funcionalidade da tela de contato no mobile
    Given que a aplicação está na resolução mobile
    When clicar nas ações de contato
    Then os botões devem responder corretamente

  Scenario: Validar layout da tela de contato no desktop
    Given que a aplicação está na resolução desktop
    When acessar o perfil do profissional
    Then os elementos devem permanecer organizados sem sobreposição

  # Responsividade - Recuperação de senha

  Scenario: Validar layout da recuperação de senha no mobile
    Given que a aplicação está na resolução mobile
    When acessar a tela de recuperação de senha
    Then os componentes devem permanecer ajustados corretamente

  Scenario: Validar funcionalidade da recuperação de senha no mobile
    Given que a aplicação está na resolução mobile
    When solicitar recuperação de senha
    Then o fluxo deve funcionar corretamente

  Scenario: Validar layout da recuperação de senha no desktop
    Given que a aplicação está na resolução desktop
    When acessar o fluxo de recuperação
    Then os componentes devem permanecer alinhados corretamente

  # Comportamentos gerais

  Scenario: Validar ausência de scroll horizontal no mobile
    Given que a aplicação está na resolução mobile
    When navegar pelos fluxos principais
    Then não deve existir scroll horizontal indevido

  Scenario: Validar adaptação dos componentes em diferentes resoluções
    When alterar entre resoluções mobile e desktop
    Then os componentes devem se adaptar corretamente

  Scenario: Validar legibilidade geral da aplicação
    When acessar os fluxos principais da plataforma
    Then os textos devem permanecer legíveis em todas as resoluções

  Scenario: Validar comportamento dos menus no mobile
    Given que a aplicação está na resolução mobile
    When acessar menus e navegação
    Then os menus devem abrir corretamente
    And os itens devem permanecer acessíveis

  Scenario: Validar estabilidade visual da aplicação
    When navegar entre páginas da plataforma
    Then os componentes não devem apresentar desalinhamentos críticos
```
