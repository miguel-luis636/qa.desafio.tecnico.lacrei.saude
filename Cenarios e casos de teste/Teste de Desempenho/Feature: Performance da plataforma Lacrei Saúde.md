```gherkin id="r6kq9m"
Feature: Performance da plataforma Lacrei Saúde

  Background:
    Given que a pessoa usuária acessa a plataforma Lacrei Saúde
    And o ambiente de testes está disponível

  # Performance - Tela inicial e login

  Scenario: Validar tempo de carregamento da tela de login
    When acessar a página de login
    Then a aplicação deve carregar dentro do tempo esperado
    And o Lighthouse deve apresentar métricas aceitáveis de performance

  Scenario: Validar estabilidade da tela de login sob múltiplos acessos
    Given que existem 30 usuários simultâneos acessando a tela de login
    When a aplicação receber múltiplas requisições simultâneas
    Then o sistema deve permanecer estável
    And não deve apresentar indisponibilidade

  # Performance - Cadastro

  Scenario: Validar tempo de resposta do cadastro de pessoa usuária
    When realizar cadastro com dados válidos
    Then o sistema deve concluir a operação em tempo aceitável
    And o tempo de resposta deve ser inferior a 500ms

  Scenario: Validar estabilidade do cadastro sob carga simultânea
    Given que existem 30 usuários simultâneos realizando cadastro
    When os formulários forem enviados simultaneamente
    Then o sistema deve processar as requisições sem falhas críticas

  Scenario: Validar carregamento da tela de cadastro
    When acessar a tela de cadastro
    Then os componentes devem carregar corretamente
    And não deve existir lentidão excessiva

  # Performance - Busca de profissionais

  Scenario: Validar tempo de resposta da busca de profissionais
    Given que a pessoa usuária está autenticada
    When realizar busca de profissionais
    Then os resultados devem ser exibidos em tempo aceitável
    And o tempo de resposta deve ser inferior a 500ms

  Scenario: Validar estabilidade da busca sob carga simultânea
    Given que existem 30 usuários simultâneos realizando buscas
    When múltiplas pesquisas forem executadas simultaneamente
    Then o sistema deve permanecer responsivo
    And os resultados devem ser carregados corretamente

  Scenario: Validar carregamento dos resultados da busca
    When acessar a listagem de profissionais
    Then os cards e informações devem carregar sem atrasos críticos

  # Performance - Recuperação de senha

  Scenario: Validar tempo de resposta da recuperação de senha
    When solicitar recuperação de senha
    Then o sistema deve processar a solicitação em tempo aceitável

  Scenario: Validar estabilidade da recuperação de senha sob múltiplas solicitações
    Given que existem múltiplas solicitações simultâneas de recuperação
    When o sistema receber requisições concorrentes
    Then o fluxo deve permanecer estável

  # Lighthouse

  Scenario: Validar métricas Lighthouse da tela de login
    When executar análise Lighthouse na tela de login
    Then a aplicação deve apresentar métricas satisfatórias de performance

  Scenario: Validar métricas Lighthouse da tela de cadastro
    When executar análise Lighthouse na tela de cadastro
    Then o desempenho da página deve permanecer aceitável

  Scenario: Validar métricas Lighthouse da busca de profissionais
    When executar análise Lighthouse na tela de busca
    Then a aplicação deve manter boa performance durante navegação

  # Recursos e estabilidade

  Scenario: Validar estabilidade geral da aplicação durante navegação
    When navegar pelos fluxos principais da plataforma
    Then o sistema não deve apresentar travamentos
    And a navegação deve permanecer fluida

  Scenario: Validar comportamento da aplicação em conexões lentas
    Given que a aplicação está sob simulação de rede limitada
    When acessar os fluxos principais
    Then a aplicação deve permanecer funcional

  Scenario: Validar carregamento dos componentes visuais
    When acessar páginas principais da plataforma
    Then imagens e componentes devem carregar corretamente

  Scenario: Validar ausência de falhas críticas sob carga
    Given que existem múltiplos usuários simultâneos utilizando a plataforma
    When ocorrer uso concorrente das funcionalidades críticas
    Then o sistema não deve apresentar erros críticos

  # Registro de problemas de performance

  Scenario: Registrar problemas de desempenho encontrados
    When identificar lentidão ou falha de estabilidade
    Then o problema deve ser documentado com evidências
    And o impacto deve ser classificado corretamente
```
