# 🧪 Plano de Testes – Plataforma Lacrei Saúde

## 📌 1. Identificação

* **Projeto**: Desafio Técnico QA – Lacrei Saúde

* **Aplicação**: Plataforma Web de atendimento e busca de profissionais de saúde

* **Ambiente de Testes**: Ambiente Staging disponibilizado para validação do desafio técnico

* **URL da aplicação**:

  https://paciente-staging.lacreisaude.com.br/login/

* **Tipos de Teste**:

  * Testes Funcionais
  * Testes Exploratórios
  * Testes Negativos
  * Testes de Validação de Formulários
  * Testes de Responsividade
  * Testes de Acessibilidade
  * Testes de Performance
  * Testes Automatizados E2E
  * Testes de Usabilidade

* **Data de Atualização**: 22/05/2026

* **Responsável**: Miguel Luis de Ataíde Ferreira

---

# 🎯 2. Objetivo

Garantir a qualidade funcional e não funcional da plataforma Lacrei Saúde, validando os principais fluxos da aplicação relacionados à jornada da pessoa usuária.

O objetivo dos testes é identificar falhas, validar regras de negócio, avaliar experiência de uso e garantir estabilidade da aplicação em diferentes cenários de utilização.

Os testes possuem foco principal nos seguintes fluxos:

* Cadastro de pessoa usuária
* Pós-cadastro
* Busca de profissionais de saúde
* Contato com profissionais
* Recuperação de senha
* Responsividade da interface
* Acessibilidade da aplicação
* Performance dos fluxos críticos
* Estabilidade da automação E2E

A execução busca simular comportamentos reais de usuários finais, garantindo que a plataforma apresente comportamento confiável, acessível e consistente.

---

# 🧠 3. Abordagem de Teste

A estratégia de testes utilizada neste desafio foi baseada em análise exploratória inicial da plataforma, seguida pela definição de cenários estruturados priorizando os fluxos críticos da aplicação.

A abordagem considera:

---

### 🔹 Exploração Inicial da Plataforma

Inicialmente foi realizada uma exploração do ambiente staging para compreender:

* Fluxos disponíveis
* Navegação da aplicação
* Comportamento dos formulários
* Regras de validação
* Estrutura das páginas
* Fluxo de autenticação
* Fluxo de recuperação de senha

Essa etapa permitiu identificar os pontos críticos que necessitam maior cobertura de testes.

---

### 🔹 Testes Baseados em Fluxos Principais

Os testes foram priorizados considerando as funcionalidades principais da plataforma:

* Cadastro da pessoa usuária
* Busca de profissionais
* Contato com profissionais
* Recuperação de senha

Esses fluxos representam as funcionalidades de maior impacto para a experiência da pessoa usuária.

---

### 🔹 Testes Negativos

Também foram definidos cenários inválidos para avaliar o comportamento do sistema diante de entradas incorretas.

Exemplos:

* Campos obrigatórios vazios
* E-mails inválidos
* Senhas inválidas
* Dados incompletos
* Campos com caracteres especiais
* Tentativas de envio inválidas

O objetivo desses testes é validar as regras de negócio e a robustez das validações implementadas.

---

### 🔹 Testes Exploratórios

Durante a execução também foram realizadas sessões de testes exploratórios visando identificar:

* Comportamentos inesperados
* Problemas visuais
* Bugs não previstos inicialmente
* Inconsistências de navegação
* Problemas de usabilidade

Esse tipo de abordagem auxilia na identificação de falhas difíceis de detectar apenas com cenários estruturados.

---

### 🔹 Testes Não Funcionais

Além dos testes funcionais, também foram realizados testes relacionados à qualidade não funcional da aplicação:

* Responsividade
* Acessibilidade
* Performance
* Compatibilidade básica entre navegadores

---

# 🧩 4. Escopo

## ✅ Incluído no escopo

### Fluxos Funcionais

* Cadastro de pessoa usuária
* Login
* Recuperação de senha
* Busca de profissionais
* Contato com profissionais
* Validação dos formulários
* Mensagens de erro e feedback visual

### Testes Não Funcionais

* Responsividade mobile e desktop
* Navegação via teclado
* Compatibilidade com leitor de tela
* Contraste e legibilidade
* Performance dos fluxos críticos
* Testes automatizados E2E

### Gestão de Qualidade

* Registro de bugs
* Registro de melhorias
* Coleta de evidências
* Organização da documentação no GitHub

---

## ❌ Fora do escopo

* Testes de invasão (pentest)
* Testes avançados de segurança
* Testes de APIs internas não expostas
* Testes de banco de dados
* Testes de infraestrutura
* Testes de carga em ambiente produtivo
* Testes mobile nativos

---

# ⚖️ 5. Ferramentas Utilizadas

Durante a execução dos testes foram utilizadas as seguintes ferramentas:

---

## Navegadores Utilizados

Os testes foram executados utilizando versões estáveis recentes dos navegadores:

- Google Chrome
- Mozilla Firefox
- Microsoft Edge

---

## Sistemas Operacionais

- Windows 11

---

## Ferramentas de Apoio

| Ferramenta | Finalidade |
|---|---|
| Cypress | Automação E2E |
| Cucumber | Escrita BDD/Gherkin |
| GitHub | Repositório e documentação |
| GitHub Actions | Pipeline CI/CD |
| Lighthouse | Performance e acessibilidade |
| Chrome DevTools | Debug e análise |
| NVDA | Testes de leitor de tela |
| Ferramenta de captura | Evidências visuais |

---

# 🧪 6. Técnicas de Teste Utilizadas

---

## Observação sobre a estratégia

A estratégia deste desafio priorizou cobertura dos fluxos principais da aplicação, execução manual exploratória e validações não funcionais.

Os testes foram estruturados principalmente com foco em:

* Fluxos críticos da pessoa usuária
* Validação de regras de negócio
* Testes positivos e negativos
* Testes exploratórios
* Testes de acessibilidade
* Testes de responsividade
* Testes automatizados E2E

---

### 🔹 Testes Funcionais

Validação das funcionalidades principais da plataforma.

Fluxos testados:

* Cadastro completo
* Login
* Recuperação de senha
* Busca de profissionais
* Contato com profissionais

---

### 🔹 Testes Negativos

Testes realizados para validar comportamento do sistema diante de entradas inválidas.

Exemplos:

* Campos vazios
* Senha inválida
* E-mail inválido
* Tentativas incompletas de cadastro
* Dados inconsistentes

---

### 🔹 Testes Exploratórios

Sessões livres de exploração visando identificar:

* Bugs inesperados
* Problemas visuais
* Problemas de navegação
* Inconsistências de UX

---

### 🔹 Testes de Responsividade

Validação da interface em diferentes resoluções:

#### Mobile
- Até 600px

#### Desktop
- Acima de 1024px

Itens avaliados:

* Quebra de layout
* Usabilidade
* Navegação
* Comportamento dos componentes

---

### 🔹 Testes de Acessibilidade

Validações realizadas:

* Navegação via teclado
* Ordem de foco
* Compatibilidade com NVDA
* Contraste de cores
* Hierarquia semântica
* Labels de formulário

Meta definida:

* Lighthouse Accessibility ≥ 90

---

### 🔹 Testes de Performance

Avaliação de:

* Tempo de carregamento
* Tempo de resposta
* Estabilidade do sistema
* Lighthouse Performance

Cenários avaliados:

* Cadastro
* Busca de profissionais

---

### 🔹 Testes Automatizados

Automação do fluxo crítico:

* Cadastro completo de pessoa usuária

Tecnologias utilizadas:

* Cypress
* Cucumber
* GitHub Actions

---

# ⏱️ 7. Cronograma de Testes

| Atividade | Frequência | Observação |
|---|---|---|
| Exploração inicial da aplicação | Início do desafio | Compreensão dos fluxos |
| Criação dos cenários | Após análise inicial | Baseado nos fluxos críticos |
| Execução manual | Durante o desafio | Validação funcional |
| Execução automatizada | Após implementação | Execução via CI |
| Registro de bugs | Durante execução | Documentação contínua |
| Coleta de evidências | Durante execução | Prints e vídeos |
| Testes não funcionais | Após validação funcional | Performance e acessibilidade |

---

# 📋 8. Módulos e Prioridades

| Código | Módulo | Prioridade |
|---|---|---|
| RF01 | Cadastro de pessoa usuária | Alta |
| RF02 | Login | Alta |
| RF03 | Recuperação de senha | Alta |
| RF04 | Busca de profissionais | Alta |
| RF05 | Contato com profissionais | Alta |
| RF06 | Responsividade | Média |
| RF07 | Acessibilidade | Média |
| RF08 | Performance | Média |
| RF09 | Usabilidade | Média |
| RF10 | Automação E2E | Alta |

---

# 🐞 9. Gestão de Defeitos

Todos os defeitos encontrados durante os testes são registrados contendo:

* ID do defeito
* Título
* Descrição
* Passos para reprodução
* Resultado esperado
* Resultado obtido
* Severidade
* Prioridade
* Evidência (print/vídeo)
* Sugestão de melhoria

---

## Classificação de Severidade

| Severidade | Descrição |
|---|---|
| Crítica | Sistema indisponível ou fluxo bloqueado |
| Alta | Funcionalidade principal comprometida |
| Média | Impacto moderado na experiência |
| Baixa | Problema visual ou comportamento secundário |

---

# ⚠️ 10. Análise de Risco

A priorização dos testes foi definida considerando:

* Impacto da funcionalidade para a pessoa usuária
* Frequência de uso
* Probabilidade de falha
* Criticidade do fluxo
* Impacto na acessibilidade e experiência

---

## Fluxos de Maior Risco

Os fluxos considerados críticos para o sistema são:

* Cadastro de pessoa usuária
* Login
* Recuperação de senha
* Busca de profissionais
* Contato com profissionais

Falhas nesses pontos podem impedir utilização da plataforma.

---

# 📄 11. Documentação dos Testes

Toda a documentação do projeto está centralizada no GitHub.

A documentação contém:

* Casos de teste
* Cenários Gherkin
* Bugs encontrados
* Evidências
* Relatórios Lighthouse
* Resultados da automação
* Relatórios CI/CD

---

# 🔄 12. Estratégia de Automação

A automação foi implementada visando validar continuamente os fluxos críticos da aplicação.

---

## Fluxo Automatizado

* Cadastro completo da pessoa usuária

---

## Objetivos da Automação

* Validar regressões
* Garantir estabilidade
* Executar testes automaticamente via CI/CD
* Reduzir falhas manuais repetitivas

---

## Pipeline CI/CD

A pipeline executa automaticamente:

* Instalação das dependências
* Execução dos testes Cypress
* Geração de relatórios
* Armazenamento de evidências

---

# 📌 13. Critérios de Aceite dos Testes

Os testes são considerados aprovados quando:

* Fluxos críticos executam sem falhas bloqueantes
* Responsividade não apresenta quebras críticas
* Lighthouse Accessibility ≥ 90
* Performance atende os thresholds definidos
* Pipeline executa com sucesso
* Evidências estão documentadas
* Bugs estão registrados adequadamente

---

# 🎯 Nota Final

Este plano de testes foi elaborado com o objetivo de estruturar a estratégia de qualidade aplicada à plataforma Lacrei Saúde.

A abordagem prioriza:

* Cobertura dos fluxos críticos
* Qualidade da experiência da pessoa usuária
* Inclusão e acessibilidade
* Organização da documentação
* Rastreabilidade dos defeitos
* Automação contínua

Toda a documentação, evidências, bugs e automações estão organizados no repositório GitHub do projeto.
