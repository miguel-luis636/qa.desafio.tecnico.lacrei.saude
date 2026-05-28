# ⚠️ Gestão de Riscos — Estratégia de QA Baseada em Risco

## 📌 Visão Geral

A estratégia de qualidade aplicada neste projeto foi baseada em uma abordagem orientada a risco, priorizando funcionalidades críticas da plataforma Lacrei Saúde considerando:

- Impacto para a pessoa usuária
- Criticidade do fluxo
- Probabilidade de falha
- Impacto operacional
- Impacto na experiência de uso
- Impacto em acessibilidade e inclusão
- Possível impacto reputacional da plataforma

A proposta não foi apenas executar testes, mas apoiar decisões relacionadas à qualidade e ao risco do produto.

A priorização dos cenários foi definida considerando:

- Fluxos mais utilizados
- Funcionalidades essenciais para navegação
- Funcionalidades diretamente relacionadas à jornada da pessoa usuária
- Possíveis falhas que poderiam impedir uso da plataforma

---

# 🧠 Mentalidade Aplicada

A execução dos testes foi guiada pelo conceito de:

> “Testar não é apenas executar cenários, mas reduzir incertezas e apoiar decisões sobre risco.”

Dessa forma, a estratégia priorizou:

- Identificação de riscos críticos
- Validação dos fluxos de maior impacto
- Cobertura de cenários negativos
- Testes exploratórios
- Validação de acessibilidade
- Estabilidade da experiência da pessoa usuária

---

# 🎯 Objetivos da Gestão de Riscos

A gestão de riscos deste projeto possui os seguintes objetivos:

- Identificar funcionalidades críticas da plataforma
- Priorizar testes com maior valor de negócio
- Reduzir probabilidade de falhas críticas
- Garantir experiência consistente para pessoas usuárias
- Minimizar impactos relacionados à acessibilidade e usabilidade
- Apoiar tomada de decisão sobre qualidade da entrega

---

# 📊 Critérios Utilizados para Priorização

Os riscos foram analisados considerando:

| Critério | Descrição |
|---|---|
| Impacto no usuário | Consequência da falha para utilização da plataforma |
| Frequência de uso | Frequência esperada de uso da funcionalidade |
| Complexidade | Complexidade técnica ou funcional |
| Probabilidade de falha | Chance da funcionalidade apresentar defeitos |
| Impacto reputacional | Impacto na confiança e experiência da plataforma |
| Dependência de fluxo | Impacto em funcionalidades dependentes |
| Acessibilidade | Impacto para pessoas com deficiência |
| Usabilidade | Impacto na navegação e entendimento da interface |

---

# 📊 Matriz de Riscos 

| ID | Funcionalidade | Descrição do Risco | Impacto | Probabilidade | Nível de Risco | Consequência | Mitigação Aplicada |
|---|---|---|---|---|---|---|---|
| RSK-01 | Cadastro de pessoa usuária | Falha ao realizar cadastro | Alto | Alto | Crítico | Impede entrada de novas pessoas usuárias | Testes funcionais, negativos e automação E2E |
| RSK-02 | Login | Falha de autenticação | Alto | Alto | Crítico | Bloqueia acesso à plataforma | Testes de login válidos e inválidos |
| RSK-03 | Recuperação de senha | Fluxo de redefinição não funcional | Alto | Médio | Alto | Pessoa usuária não consegue recuperar acesso | Testes completos de recuperação |
| RSK-04 | Busca de profissionais | Busca não retorna resultados corretamente | Alto | Alto | Crítico | Compromete funcionalidade principal | Testes funcionais e exploratórios |
| RSK-05 | Contato com profissional | Falha ao iniciar contato | Alto | Médio | Alto | Interrompe jornada principal | Testes de navegação e interação |
| RSK-06 | Validação de formulários | Campos aceitam dados inválidos | Alto | Alto | Crítico | Possível inconsistência de dados | Testes negativos e validações |
| RSK-07 | Responsividade mobile | Layout quebrado em telas pequenas | Médio | Alto | Alto | Má experiência mobile | Testes responsivos em múltiplas resoluções |
| RSK-08 | Responsividade desktop | Sobreposição ou desalinhamento visual | Médio | Médio | Médio | Dificulta uso da plataforma | Testes visuais e exploratórios |
| RSK-09 | Navegação via teclado | Componentes inacessíveis via TAB | Alto | Médio | Alto | Barreira de acessibilidade | Testes com navegação por teclado |
| RSK-10 | Compatibilidade com leitor de tela | Leitor não interpreta elementos corretamente | Alto | Médio | Alto | Impacto em acessibilidade | Testes com NVDA |
| RSK-11 | Contraste de cores | Baixa legibilidade da interface | Médio | Médio | Médio | Dificulta leitura | Lighthouse e DevTools |
| RSK-12 | Estrutura semântica | HTML sem semântica adequada | Médio | Médio | Médio | Impacta acessibilidade | Validação de headings e landmarks |
| RSK-13 | Performance do login | Lentidão no carregamento | Médio | Médio | Médio | Frustração da pessoa usuária | Lighthouse |
| RSK-14 | Performance do cadastro | Tempo de resposta elevado | Alto | Médio | Alto | Abandono de fluxo | Testes de performance |
| RSK-15 | Performance da busca | Lentidão ao buscar profissionais | Alto | Médio | Alto | Impacta experiência principal | Simulação de carga |
| RSK-16 | Estabilidade sob carga | Instabilidade com múltiplos acessos | Alto | Médio | Alto | Queda ou lentidão do sistema | Testes com múltiplos usuários |
| RSK-17 | Mensagens de erro inadequadas | Feedback pouco claro | Médio | Médio | Médio | Confusão da pessoa usuária | Testes exploratórios |
| RSK-18 | Scroll horizontal no mobile | Layout ultrapassa largura da tela | Médio | Alto | Alto | Navegação prejudicada | Testes em resoluções mobile |
| RSK-19 | Botões pequenos no mobile | Dificuldade de interação touch | Médio | Médio | Médio | Problema de usabilidade | Testes de usabilidade |
| RSK-20 | Falhas em automação | Testes automatizados instáveis | Médio | Médio | Médio | Falsos positivos/negativos | Melhorias de estabilidade |
| RSK-21 | Pipeline CI/CD | Pipeline não executa corretamente | Alto | Baixo | Médio | Perda de validação contínua | GitHub Actions |
| RSK-22 | Dependência do ambiente staging | Ambiente indisponível ou instável | Alto | Médio | Alto | Bloqueia execução de testes | Planejamento de execução |
| RSK-23 | Dados persistidos incorretamente | Dados inconsistentes após ações | Alto | Médio | Alto | Problemas funcionais | Testes exploratórios e funcionais |
| RSK-24 | Sessão da pessoa usuária | Sessão expira incorretamente | Médio | Médio | Médio | Perda de navegação | Testes de autenticação |
| RSK-25 | Quebra de fluxo pós-cadastro | Usuária não consegue continuar jornada | Alto | Médio | Alto | Interrupção da experiência | Testes E2E completos |

# 📱 Riscos Prioritários Mobile

Considerando o comportamento atual de uso de aplicações web, o mobile foi tratado como prioridade de risco.

## Principais riscos mobile

- Quebra de layout
- Elementos sobrepostos
- Botões inacessíveis
- Scroll horizontal
- Problemas de usabilidade
- Lentidão em conexões móveis

---

# ♿ Riscos de Acessibilidade

A acessibilidade foi considerada um dos pilares críticos do projeto.

## Principais riscos avaliados

- Falta de navegação via teclado
- Ausência de labels
- Baixo contraste
- Falta de semântica HTML
- Incompatibilidade com leitores de tela

---

# ⚡ Riscos de Performance

Os testes de performance priorizaram:

- Tempo de carregamento
- Tempo de resposta
- Estabilidade
- Comportamento sob múltiplos acessos

## Cenários críticos

- Cadastro
- Busca de profissionais
- Login
- Recuperação de senha

---

# 🔄 Riscos Relacionados à Automação

| Risco | Mitigação |
|---|---|
| Falhas intermitentes | Uso de waits adequados e validações estáveis |
| Dependência do ambiente staging | Execução controlada via pipeline |
| Regressões | Execução automática em PRs e commits |

---

# 📋 Critérios de Aceitação de Risco

Os riscos foram considerados aceitáveis quando:

- Não bloqueiam fluxos críticos
- Possuem work around conhecido
- Não comprometem acessibilidade mínima
- Não afetam segurança ou autenticação
- Não impedem navegação principal

---

# 📈 Resultado Esperado da Estratégia

A abordagem orientada a risco busca:

- Maior eficiência dos testes
- Melhor priorização
- Redução de falhas críticas
- Melhor experiência da pessoa usuária
- Maior confiança na entrega
- Melhor rastreabilidade da qualidade

---

# 🎯 Conclusão

A gestão de riscos aplicada neste projeto teve como foco principal apoiar decisões de qualidade com base no impacto real para as pessoas usuárias da plataforma Lacrei Saúde.

Mais do que executar testes, a estratégia buscou identificar:

- Onde a aplicação possui maior criticidade
- Quais falhas possuem maior impacto
- Quais áreas exigem maior cobertura
- Como reduzir riscos para a experiência final

Essa abordagem permite que o processo de QA atue de forma estratégica, direcionando esforços para os pontos de maior valor e maior risco da aplicação.
