# ⚡ 📋 Relatório de Testes de Performance

## 📌 Informações Gerais

| Item        | Detalhe                        |
| ----------- | ------------------------------ |
| Projeto     | Lacrei Saúde                   |
| Ambiente    | Staging                        |
| Escopo      | Performance Web                |
| Ferramenta  | Lighthouse                     |
| Execução    | Manual                         |
| Responsável | Miguel Luis de Ataíde Ferreira |
| Data        | 28/05/2026                     |

---

# 📊 Resultados Lighthouse (Performance)

## 🔍 Login

* Performance: **78**
* Accessibility: 90
* Best Practices: 77
* SEO: 82

## 🔍 Cadastro

* Performance: **81**
* Accessibility: 96
* Best Practices: 77
* SEO: 82

## 🔍 Busca de Profissionais

* Performance: **73**
* Accessibility: 96
* Best Practices: 77
* SEO: 82

---

# 🧪 Análise de Performance

## ⏱️ Tempo de resposta percebido

### Fluxos críticos analisados:

* Login
* Cadastro
* Busca de profissionais

### Resultado:

* ✔ Tempo aceitável em desktop
* ❌ Queda perceptível em busca de profissionais
* ❌ Performance mais baixa na página de busca (73)

---

## 📦 Carregamento de componentes

### Resultado:

* ✔ Componentes principais carregam corretamente
* ❌ Cards da busca têm maior custo de renderização
* ❌ Layout mais pesado na listagem de profissionais

---

## 📱 Performance mobile

### Resultado:

* ✔ Funciona em dispositivos móveis
* ❌ Sensação de lentidão em telas de busca
* ✔ Cadastro e login mais estáveis

---

## 🌐 Estabilidade geral

### Resultado:

* ✔ Sem crashes ou falhas críticas
* ✔ Fluxos principais estáveis
* ❌ Performance inconsistente entre páginas

---

# ⚠️ Problemas Identificados (Performance)

## 🐞 PERF-001 — Baixa performance na busca de profissionais

* Impacto: Alto
* Score: 73
* Causa provável: carga de dados e renderização dos cards

## 🐞 PERF-002 — Performance abaixo do ideal em algumas páginas

* Impacto: Médio
* Descrição: variação entre 73 e 81 nos fluxos principais

---

# 📈 Insights de Performance

## ✔ Pontos positivos

* Fluxos principais funcionam sem travamento
* Login e cadastro com performance aceitável
* Estabilidade geral da aplicação

## ⚠️ Pontos de melhoria

* Otimização da página de busca
* Redução de custo de renderização de cards
* Melhor carregamento progressivo (lazy loading)
* Otimização de assets

---

# 🎯 Conclusão — Performance

A plataforma apresenta desempenho **aceitável, porém não consistente**, com destaque para:

* Boa performance em login e cadastro
* Queda significativa na busca de profissionais (73)

A principal área de melhoria é:

* Otimização da listagem de profissionais
* Redução do custo de renderização
* Melhoria na experiência mobile em páginas mais pesadas
