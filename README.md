# 🧪 Desafio Técnico QA — Lacrei Saúde

Projeto desenvolvido como parte do desafio técnico para atuação voluntária em Quality Assurance na plataforma Lacrei Saúde.

O objetivo deste repositório é validar qualidade funcional, acessibilidade, responsividade, desempenho e automação da plataforma, utilizando práticas modernas de QA com documentação centralizada exclusivamente no GitHub.

---

# 📌 Observação sobre Automação e CI/CD

Embora o desafio sugira a implementação de automação utilizando Cypress e integração contínua via GitHub Actions, neste projeto optei por não desenvolver a automação completa e pipeline CI/CD.

A decisão foi tomada de forma estratégica visando aprofundar meus estudos em automação mobile e testes end-to-end utilizando ferramentas como:

* Appium
* Automação mobile híbrida
* Testes cross-platform
* Estratégias de automação orientadas a dispositivos móveis
* Arquitetura de testes automatizados mais escalável

Como foco principal deste desafio, priorizei:

* Estruturação completa da documentação de QA
* Criação detalhada de cenários e casos de teste em Gherkin
* Execução manual dos fluxos críticos
* Testes exploratórios
* Análise de acessibilidade
* Testes de responsividade
* Testes de performance
* Gestão de riscos
* Registro estruturado de bugs e melhorias

Essa abordagem permitiu concentrar esforços na análise crítica da qualidade da aplicação, comportamento do usuário, experiência de navegação e identificação de riscos relevantes para o produto.

Ainda assim, a estrutura do projeto foi organizada considerando futura evolução para automação E2E e integração contínua, mantendo compatibilidade com ferramentas modernas de QA.


# 📌 Objetivos do Projeto

Garantir a qualidade dos principais fluxos da aplicação:

- Cadastro de usuário
- Pós-cadastro
- Busca de profissionais
- Contato com profissional
- Recuperação de senha
- Responsividade
- Acessibilidade
- Performance
- Automação E2E
- Pipeline CI/CD

---

# 🌐 Ambiente Testado

## Ambiente Staging

:contentReference[oaicite:0]{index=0}

---

# 🛠️ Stack Utilizada

| Categoria | Ferramenta |
|---|---|
| Gestão de testes | GitHub |
| Versionamento | GitHub |
| Testes manuais | Gherkin |
| Automação | Cypress |
| BDD | Cucumber |
| Performance | Lighthouse |
| Acessibilidade | Lighthouse + DevTools + NVDA |
| CI/CD | GitHub Actions |

---

# 📋 Escopo dos Testes

## ✅ Testes Funcionais

Fluxos cobertos:

### Cadastro de Usuário

* Cadastro válido
* Validação de campos obrigatórios
* Validação de senha
* Fluxo pós-cadastro

### Busca de Profissionais

* Busca por especialidade
* Busca por localização
* Contato com profissional

### Recuperação de Senha

* Solicitação de recuperação
* Envio de e-mail
* Redefinição de senha

---

# 🧾 Casos de Teste em Gherkin

Os cenários foram desenvolvidos utilizando BDD com Gherkin para garantir clareza, rastreabilidade e entendimento dos fluxos testados.

Exemplo:

```gherkin
Feature: Cadastro de usuário

Scenario: Cadastro realizado com sucesso
Given que a pessoa usuária acessa a tela de cadastro
When preencher os campos obrigatórios corretamente
And clicar em "Cadastrar"
Then o sistema deve criar a conta com sucesso
```

Todos os cenários estão organizados em:


---

# 🐞 Gestão de Bugs e Melhorias

Todos os bugs, inconsistências e sugestões de melhoria foram registrados diretamente no GitHub através de:

* GitHub Issues
* Documentação em Markdown
* Evidências anexadas no repositório

Cada registro contém:

* Descrição detalhada
* Passos para reprodução
* Resultado esperado
* Resultado obtido
* Evidências (prints/vídeos)
* Severidade
* Prioridade
* Sugestão de melhoria

## Classificação utilizada

| Severidade | Descrição                                    |
| ---------- | -------------------------------------------- |
| Crítica    | Impede uso do sistema                        |
| Alta       | Funcionalidade principal comprometida        |
| Média      | Impacto moderado                             |
| Baixa      | Problemas visuais ou pequenos comportamentos |

---

# 📱 Testes de Responsividade

## Resoluções testadas

### Mobile

* 320x568
* 375x667
* 390x844

### Desktop

* 1366x768
* 1920x1080

## Validações realizadas

* Quebra de layout
* Scroll horizontal
* Responsividade dos componentes
* Usabilidade mobile
* Navegação
* Botões e formulários

---

# ♿ Testes de Acessibilidade

## Ferramentas utilizadas

* Lighthouse
* Chrome DevTools
* NVDA

## Itens validados

* Navegação via teclado
* Ordem de foco
* Contraste de cores
* Labels em inputs
* Compatibilidade com leitor de tela
* Hierarquia semântica
* Textos alternativos

## Meta de qualidade

* Lighthouse Accessibility ≥ 90

---

# ⚡ Testes de Performance

## Ferramenta

* Lighthouse

## Cenários avaliados

* Tempo de carregamento da página inicial
* Tempo de resposta no cadastro
* Busca de profissionais

## Critérios esperados

| Métrica                  | Meta    |
| ------------------------ | ------- |
| First Contentful Paint   | < 2s    |
| Largest Contentful Paint | < 2.5s  |
| Tempo de resposta        | < 500ms |

---

# 🤖 Automação de Testes

## Fluxos automatizados

* Cadastro completo de usuário

## Tecnologias utilizadas

* Cypress
* Cucumber
* Mochawesome Reporter

---

# 🔄 Pipeline CI/CD

O projeto possui integração contínua utilizando GitHub Actions.

## O pipeline executa automaticamente:

* Instalação das dependências
* Execução dos testes automatizados
* Geração de relatórios
* Armazenamento de artefatos
* Validação em Pull Requests

---

# 🔐 Checklist de Segurança

## Validações realizadas

* Inputs vulneráveis
* Exposição de dados sensíveis
* Mensagens de erro
* Persistência indevida de dados
* Validações client-side
* Tokens expostos
* Sessão e autenticação

---

# 🔙 Processo de Rollback

Caso os testes automatizados apresentem falhas críticas:

1. Identificar commit responsável
2. Reverter pipeline
3. Restaurar versão estável
4. Executar regressão
5. Validar ambiente novamente

---

# 📌 Organização da Documentação

Toda a documentação do projeto está centralizada exclusivamente no GitHub.

## Estrutura de documentação

| Pasta               | Conteúdo                  |
| ------------------- | ------------------------- |
| CI/CD         | Pipeline          |
| Cenarios e casos de teste | Testes e escritas de cenarios e casos     |
| Registro de bugs e melhorias   | Relatórios e análises     |
| Resultados dos testes |  Relatórios e análises    |
| Cypress | automação |

---


# 🧠 Estratégia de QA Aplicada

O projeto foi desenvolvido utilizando:

* Testes exploratórios
* Testes funcionais
* Testes E2E
* BDD
* Validação visual
* Testes não funcionais
* Análise de acessibilidade
* Testes de performance

---

# 💙 Sobre o Projeto

Este projeto foi desenvolvido com foco em qualidade, acessibilidade e inclusão, contribuindo para uma experiência mais segura e acolhedora para as pessoas usuárias da plataforma Lacrei Saúde.

A documentação, rastreabilidade dos testes, evidências e automações foram organizadas integralmente no GitHub visando transparência, versionamento e facilidade de manutenção.
