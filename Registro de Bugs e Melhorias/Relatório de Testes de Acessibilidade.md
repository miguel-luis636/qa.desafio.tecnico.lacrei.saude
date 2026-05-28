# ♿ 📋 Relatório de Testes de Acessibilidade — Lacrei Saúde

## 📌 Informações Gerais

| Item        | Detalhe                           |
| ----------- | --------------------------------- |
| Projeto     | Lacrei Saúde                      |
| Ambiente    | Staging                           |
| Escopo      | Acessibilidade Web                |
| Ferramentas | Lighthouse, DevTools, NVDA        |
| Execução    | Manual + Ferramentas de auditoria |
| Responsável | Miguel Luis de Ataíde Ferreira    |
| Data        | 28/05/2026                        |

---

# 📊 Resultados Lighthouse (Acessibilidade)

## 🔍 Tela de Login

* Performance: **78**
* Accessibility: **90**
* Best Practices: **77**
* SEO: **82**

## 🔍 Tela de Cadastro

* Performance: **81**
* Accessibility: **96**
* Best Practices: **77**
* SEO: **82**

## 🔍 Busca de Profissionais

* Performance: **73**
* Accessibility: **96**
* Best Practices: **77**
* SEO: **82**

---

# 🧪 Execução dos Testes

## ♿ Navegação via teclado

### Resultado

* ✔ Elementos acessíveis via TAB
* ✔ Ordem de navegação funcional
* ❌ Em algumas telas, foco visual inconsistente

---

## 🧏 Leitores de tela (NVDA)

### Resultado

* ✔ Campos possuem labels na maioria dos fluxos
* ✔ Botões são anunciados corretamente
* ❌ Algumas informações da busca não são suficientemente descritivas

---

## 🎨 Contraste e legibilidade

### Resultado

* ✔ Boa legibilidade geral
* ✔ Texto adequado em telas principais
* ❌ Alguns componentes secundários apresentam contraste abaixo do ideal

---

## 🧱 Estrutura semântica

### Resultado

* ✔ Uso parcial correto de headings
* ✔ Inputs com labels associados
* ❌ Hierarquia HTML poderia ser mais consistente (headings e landmarks)

---

## 📱 Responsividade acessível

### Resultado

* ✔ Navegação funcional no mobile
* ❌ Problemas de layout em tablets impactam acessibilidade
* ✔ Desktop estável

---

# ⚠️ Problemas Encontrados (Acessibilidade)

## 🐞 A11Y-001 — Foco visual inconsistente

* Impacto: Médio
* Descrição: Alguns elementos perdem destaque de foco ao navegar via teclado

## 🐞 A11Y-002 — Descrição insuficiente na busca de profissionais

* Impacto: Médio
* Descrição: Informações exibidas não são totalmente claras para leitores de tela

## 🐞 A11Y-003 — Estrutura semântica inconsistente

* Impacto: Médio
* Descrição: Hierarquia de títulos e landmarks poderia ser melhor estruturada

## 🐞 A11Y-004 — Problemas de contraste em componentes secundários

* Impacto: Médio
* Descrição: Alguns textos e botões apresentam contraste abaixo do ideal

---

# 📈 Insights de Acessibilidade

## ✔ Pontos positivos

* Excelente pontuação geral (até 96)
* Boa compatibilidade com NVDA
* Fluxos principais acessíveis
* Boa base de estrutura de formulários

## ⚠️ Pontos de melhoria

* Melhorar consistência de foco visual
* Refinar semântica HTML
* Melhorar descrição da busca de profissionais
* Revisar contraste de elementos secundários

---

# 🎯 Conclusão — Acessibilidade

A plataforma apresenta **bom nível de acessibilidade geral (90–96)**, com base sólida em:

* Navegação por teclado
* Compatibilidade com leitor de tela
* Estrutura funcional

Porém, ainda existem oportunidades de melhoria principalmente em:

* Semântica HTML
* Clareza da informação na busca
* Consistência visual de foco
* Contraste em componentes secundários
---
