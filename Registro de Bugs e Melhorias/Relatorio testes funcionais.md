# 📋 Relatório de Execução dos Testes — Lacrei Saúde

## 📌 Informações Gerais

| Item             | Detalhe                                                                                                  |
| ---------------- | -------------------------------------------------------------------------------------------------------- |
| Projeto          | Lacrei Saúde                                                                                             |
| Ambiente         | Staging                                                                                                  |
| URL              | [https://paciente-staging.lacreisaude.com.br/login/](https://paciente-staging.lacreisaude.com.br/login/) |
| Tipo de Teste    | Funcional, Responsividade e Usabilidade                                                                  |
| Plataforma       | Web                                                                                                      |
| Execução         | Manual                                                                                                   |
| Responsável      | Miguel Luis de Ataíde Ferreira                                                                           |
| Data da Execução | 28/05/2026                                                                                               |

---

# 📊 Resumo Geral da Execução

| Feature                    | Total  | Passou | Falhou |
| -------------------------- | ------ | ------ | ------ |
| Cadastro de pessoa usuária | 8      | 7      | 1      |
| Login da pessoa usuária    | 6      | 5      | 1      |
| Busca de profissionais     | 8      | 7      | 1      |
| Recuperação de senha       | 9      | 8      | 1      |
| **TOTAL**                  | **31** | **27** | **4**  |

---

# ✅ Resultado Geral

| Status     | Quantidade |
| ---------- | ---------- |
| PASSOU     | 27         |
| NÃO PASSOU | 4          |

---

# 🧪 Execução — Cadastro de Pessoa Usuária

## Resultado da Execução

| Cenário                                 | Resultado    | Observação                            |
| --------------------------------------- | ------------ | ------------------------------------- |
| Realizar cadastro com sucesso           | ✅ PASSOU     | Fluxo executado corretamente          |
| Cadastro com campos obrigatórios vazios | ✅ PASSOU     | Validações funcionando                |
| Cadastro com e-mail inválido            | ✅ PASSOU     | Mensagem exibida corretamente         |
| Cadastro com senha inválida             | ✅ PASSOU     | Regra validada                        |
| Obrigatoriedade de aceite dos termos    | ✅ PASSOU     | Cadastro bloqueado corretamente       |
| Redirecionamento pós-cadastro           | ✅ PASSOU     | Fluxo concluído corretamente          |
| Responsividade no mobile                | ❌ NÃO PASSOU | Quebra de layout em resoluções tablet |
| Responsividade no desktop               | ✅ PASSOU     | Layout estável                        |

---

## 🐞 Problema Encontrado — Cadastro Responsivo

### ID

BUG-RESP-001

### Severidade

Média

### Descrição

Foi identificada quebra de layout na tela de cadastro em resoluções intermediárias de tablet.

### Impacto

Os campos apresentam desalinhamento e comprometem parcialmente a experiência da pessoa usuária.

### Resultado Esperado

A interface deveria adaptar corretamente os componentes em resoluções mobile/tablet.

### Resultado Obtido

Campos e botões apresentaram desalinhamento visual.

---

# 🔐 Execução — Login da Pessoa Usuária

## Resultado da Execução

| Cenário                  | Resultado    | Observação                             |
| ------------------------ | ------------ | -------------------------------------- |
| Login com sucesso        | ✅ PASSOU     | Fluxo funcional                        |
| Login com senha inválida | ✅ PASSOU     | Mensagem correta exibida               |
| Login com campos vazios  | ✅ PASSOU     | Campos obrigatórios validados          |
| E-mail inválido          | ✅ PASSOU     | Validação funcionando                  |
| Responsividade mobile    | ❌ NÃO PASSOU | Mesmo problema responsivo identificado |
| Responsividade desktop   | ✅ PASSOU     | Interface estável                      |

---

## 🐞 Problema Encontrado — Login Responsivo

### ID

BUG-RESP-002

### Severidade

Média

### Descrição

A tela de login apresentou inconsistências visuais em resoluções tablet/mobile.

### Impacto

Experiência visual comprometida em determinados dispositivos móveis.

### Resultado Esperado

Layout adaptável sem quebra visual.

### Resultado Obtido

Elementos desalinhados em resoluções intermediárias.

---

# 🔎 Execução — Busca de Profissionais

## Resultado da Execução

| Cenário                             | Resultado    | Observação                             |
| ----------------------------------- | ------------ | -------------------------------------- |
| Buscar profissional com sucesso     | ✅ PASSOU     | Resultados exibidos corretamente       |
| Buscar profissional por localização | ❌ NÃO PASSOU | Sistema retornou localização incorreta |
| Buscar sem filtros                  | ✅ PASSOU     | Fluxo funcional                        |
| Busca inexistente                   | ✅ PASSOU     | Mensagem exibida corretamente          |
| Contato com profissional            | ✅ PASSOU     | Fluxo funcionando                      |
| Carregamento da listagem            | ✅ PASSOU     | Cards carregados corretamente          |
| Responsividade mobile               | ✅ PASSOU     | Sem quebra crítica                     |
| Responsividade desktop              | ✅ PASSOU     | Layout funcional                       |

---

## 🐞 Problema Encontrado — Busca por Localização

### ID

BUG-BUSCA-001

### Severidade

Alta

### Descrição

A funcionalidade de busca por localização retornou profissionais incompatíveis com a região pesquisada.

### Impacto

Compromete diretamente a principal funcionalidade da plataforma.

### Resultado Esperado

O sistema deveria listar profissionais compatíveis com a localização informada.

### Resultado Obtido

Foram exibidos profissionais de regiões diferentes da pesquisada.

---

## 🐞 Problema Encontrado — Experiência da Busca de Profissionais

### ID

BUG-UX-001

### Severidade

Média

### Descrição

Durante a utilização do fluxo de busca de profissionais, foi identificado que a experiência possui poucas informações relacionadas às especialidades médicas e ao problema de saúde da pessoa usuária.

Além disso, foi observado um foco excessivo em filtros relacionados à sexualidade e identidade, enquanto informações mais relevantes para tomada de decisão clínica aparecem com menor destaque visual.

### Impacto

A experiência de busca pode gerar dificuldade para pessoas usuárias que desejam encontrar rapidamente profissionais adequados para resolução do seu problema de saúde.

Isso pode:

* Dificultar tomada de decisão
* Tornar a busca menos objetiva
* Gerar excesso de navegação
* Reduzir eficiência da jornada principal da plataforma

### Resultado Esperado

A busca deveria priorizar de forma mais clara:

* Especialidade médica
* Sintomas ou necessidades da pessoa usuária
* Experiência do profissional
* Informações clínicas relevantes
* Facilidade para encontrar atendimento adequado

### Resultado Obtido

O fluxo apresenta maior destaque para informações relacionadas à identidade e sexualidade do que para critérios clínicos e especialidades.

### Sugestão de Melhoria

* Melhorar priorização visual das especialidades
* Destacar sintomas e necessidades da pessoa usuária
* Melhorar filtros clínicos
* Exibir mais informações profissionais relevantes
* Facilitar entendimento do perfil do profissional
* Tornar a busca mais orientada à resolução do problema da pessoa usuária

---

# 🔑 Execução — Recuperação de Senha

## Resultado da Execução

| Cenário                         | Resultado    | Observação                               |
| ------------------------------- | ------------ | ---------------------------------------- |
| Solicitação de recuperação      | ✅ PASSOU     | Fluxo funcionando                        |
| Recuperação com e-mail inválido | ✅ PASSOU     | Validação correta                        |
| Recuperação com campo vazio     | ✅ PASSOU     | Campo obrigatório validado               |
| E-mail não cadastrado           | ✅ PASSOU     | Regra de negócio respeitada              |
| Acesso ao fluxo de redefinição  | ✅ PASSOU     | Fluxo funcional                          |
| Redefinição de senha            | ✅ PASSOU     | Senha alterada corretamente              |
| Divergência entre senhas        | ✅ PASSOU     | Validação funcionando                    |
| Responsividade mobile           | ❌ NÃO PASSOU | Quebra visual semelhante aos formulários |
| Responsividade desktop          | ✅ PASSOU     | Layout funcional                         |

---

## 🐞 Problema Encontrado — Recuperação Responsiva

### ID

BUG-RESP-003

### Severidade

Média

### Descrição

A tela de recuperação de senha apresentou problemas responsivos em resoluções tablet/mobile.

### Impacto

Compromete parcialmente a usabilidade do fluxo.

### Resultado Esperado

Interface adaptável em diferentes tamanhos de tela.

### Resultado Obtido

Formulários apresentaram desalinhamento visual.

---

# 🎨 Problemas Visuais e de Design Identificados

Durante a execução dos testes também foram identificados alguns problemas relacionados à consistência visual e dimensionamento dos componentes da interface.

## Problemas observados

* Componentes com tamanhos inconsistentes
* Espaçamentos irregulares
* Elementos desalinhados em algumas resoluções
* Quebras visuais em telas intermediárias
* Formulários com adaptação parcial em tablets
* Hierarquia visual pouco clara em alguns fluxos

## Impacto

Embora não impeçam totalmente o uso da plataforma, esses problemas afetam:

* Experiência da pessoa usuária
* Clareza visual
* Navegação
* Percepção de qualidade da interface

---

# 📈 Análise Geral da Execução

## Pontos Positivos

* Fluxos principais funcionando corretamente
* Validações de formulário implementadas
* Mensagens de erro funcionando
* Fluxos de autenticação estáveis
* Busca funcional em cenários gerais
* Navegação desktop estável

---

## Pontos de Atenção

### 🔴 Responsividade

Foi identificado um padrão de falha relacionado à responsividade em resoluções intermediárias (tablet), impactando:

* Cadastro
* Login
* Recuperação de senha

### 🔴 Busca por localização

A funcionalidade apresentou comportamento inconsistente e possui impacto elevado na experiência principal da plataforma.

### 🔴 Experiência da busca

Foi observado que o fluxo de busca poderia priorizar melhor informações clínicas e especialidades profissionais, tornando a jornada mais objetiva para pessoas usuárias buscando resolução de problemas de saúde.

---

# ⚠️ Riscos Identificados

| Risco                                         | Impacto |
| --------------------------------------------- | ------- |
| Quebra de layout mobile/tablet                | Médio   |
| Resultado incorreto na busca por localização  | Alto    |
| Comprometimento parcial da usabilidade mobile | Médio   |
| Pouca clareza na busca por especialidades     | Médio   |
| Hierarquia visual inconsistente               | Médio   |

---

# 🎯 Conclusão

A execução dos testes demonstrou que os fluxos principais da plataforma apresentam comportamento funcional estável na maior parte dos cenários validados.

Entretanto, foram identificados pontos de atenção relacionados à:

* Responsividade em dispositivos tablet/mobile
* Precisão da busca por localização
* Hierarquia visual da interface
* Clareza das informações exibidas na busca de profissionais

Os problemas encontrados não impedem totalmente o uso da plataforma, porém impactam diretamente a experiência da pessoa usuária e devem ser priorizados para correção e melhoria contínua.

A cobertura dos testes contemplou:

* Fluxos principais
* Cenários positivos
* Cenários negativos
* Responsividade
* Usabilidade funcional
* Avaliação exploratória da experiência de navegação

Os defeitos encontrados foram devidamente registrados para acompanhamento e priorização.

