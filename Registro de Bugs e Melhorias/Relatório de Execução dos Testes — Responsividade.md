# 📋 Relatório de Execução dos Testes — Responsividade 

## 📌 Informações Gerais

| Item             | Detalhe                              |
| ---------------- | ------------------------------------ |
| Projeto          | Lacrei Saúde                         |
| Ambiente         | Staging                              |
| Tipo de Teste    | Responsividade, Usabilidade e Layout |
| Plataforma       | Web                                  |
| Execução         | Manual                               |
| Responsável      | Miguel Luis de Ataíde Ferreira       |
| Data da Execução | 28/05/2026                           |

---

# 📊 Resumo Geral da Execução

| Feature / Área        | Total  | Passou | Falhou |
| --------------------- | ------ | ------ | ------ |
| Login                 | 4      | 3      | 1      |
| Cadastro              | 4      | 3      | 1      |
| Busca                 | 4      | 3      | 1      |
| Contato               | 3      | 3      | 0      |
| Recuperação de senha  | 3      | 3      | 0      |
| Comportamentos gerais | 5      | 4      | 1      |
| **TOTAL**             | **23** | **19** | **4**  |

---

# ✅ Resultado Geral

| Status     | Quantidade |
| ---------- | ---------- |
| PASSOU     | 19         |
| NÃO PASSOU | 4          |

---

# 📱 Execução — Responsividade (Login)

| Cenário                   | Resultado    | Observação                                           |
| ------------------------- | ------------ | ---------------------------------------------------- |
| Layout mobile (até 600px) | ❌ NÃO PASSOU | Quebra de layout em resoluções intermediárias        |
| Funcionalidade no mobile  | ✅ PASSOU     | Fluxo funcional                                      |
| Usabilidade no mobile     | ❌ NÃO PASSOU | Botões com tamanho inadequado em alguns dispositivos |
| Layout desktop            | ✅ PASSOU     | Alinhamento correto                                  |

## 🐞 Bug — Login Responsividade

### ID

RESP-LOGIN-001

### Descrição

Foi identificada quebra de layout e inconsistência de usabilidade em dispositivos mobile/tablet.

### Impacto

Afeta experiência de login em dispositivos móveis.

---

# 🧾 Execução — Responsividade (Cadastro)

| Cenário               | Resultado    | Observação                                    |
| --------------------- | ------------ | --------------------------------------------- |
| Layout mobile         | ❌ NÃO PASSOU | Campos não se ajustam corretamente em tablets |
| Funcionalidade mobile | ✅ PASSOU     | Cadastro funciona corretamente                |
| Usabilidade mobile    | ❌ NÃO PASSOU | Elementos pouco confortáveis para interação   |
| Layout desktop        | ✅ PASSOU     | Estrutura estável                             |

## 🐞 Bug — Cadastro Responsivo

### ID

RESP-CAD-001

### Descrição

Problemas de adaptação visual em resoluções intermediárias.

### Impacto

Compromete a experiência de cadastro em mobile/tablet.

---

# 🔎 Execução — Responsividade (Busca de Profissionais)

| Cenário               | Resultado    | Observação                                         |
| --------------------- | ------------ | -------------------------------------------------- |
| Layout mobile         | ❌ NÃO PASSOU | Cards apresentam desalinhamento em alguns tamanhos |
| Funcionalidade mobile | ✅ PASSOU     | Filtros funcionam corretamente                     |
| Usabilidade mobile    | ❌ NÃO PASSOU | Texto e botões com baixa adaptação                 |
| Layout desktop        | ✅ PASSOU     | Layout consistente                                 |

## 🐞 Bug — Busca Responsiva

### ID

RESP-BUSCA-001

### Descrição

Inconsistência no layout dos cards em dispositivos mobile/tablet.

### Impacto

Dificulta visualização de profissionais.

---

# 💬 Execução — Responsividade (Contato com Profissional)

| Cenário               | Resultado | Observação          |
| --------------------- | --------- | ------------------- |
| Layout mobile         | ✅ PASSOU  | Organização correta |
| Funcionalidade mobile | ✅ PASSOU  | Botões funcionais   |
| Layout desktop        | ✅ PASSOU  | Sem sobreposição    |

---

# 🔑 Execução — Recuperação de Senha

| Cenário               | Resultado    | Observação                                   |
| --------------------- | ------------ | -------------------------------------------- |
| Layout mobile         | ❌ NÃO PASSOU | Problemas semelhantes aos demais formulários |
| Funcionalidade mobile | ✅ PASSOU     | Fluxo funcional                              |
| Layout desktop        | ✅ PASSOU     | Layout correto                               |

## 🐞 Bug — Recuperação Responsiva

### ID

RESP-REC-001

### Descrição

Desalinhamento de campos no fluxo de recuperação em mobile/tablet.

---

# 📊 Execução — Comportamentos Gerais

| Cenário                    | Resultado    | Observação                                    |
| -------------------------- | ------------ | --------------------------------------------- |
| Sem scroll horizontal      | ❌ NÃO PASSOU | Scroll aparece em algumas resoluções          |
| Adaptação entre resoluções | ❌ NÃO PASSOU | Quebras ao alternar tamanhos                  |
| Legibilidade geral         | ✅ PASSOU     | Texto legível                                 |
| Menus no mobile            | ❌ NÃO PASSOU | Menu apresenta inconsistência em alguns casos |
| Estabilidade visual geral  | ❌ NÃO PASSOU | Pequenos desalinhamentos entre páginas        |

---

# 🐞 Bug Geral — Responsividade

### ID

RESP-GERAL-001

### Descrição

Foram identificadas inconsistências de layout ao navegar entre páginas e ao alternar resoluções.

### Impacto

Afeta a consistência visual da plataforma.

---

# 📈 Análise Geral

## ✅ Pontos Positivos

* Funcionalidade geral preservada em todos os fluxos
* Desktop apresenta boa estabilidade
* Navegação funcional em todos os módulos
* Conteúdo legível na maioria dos cenários

---

## ⚠️ Pontos de Atenção

### 🔴 Responsividade (principal risco)

Problemas recorrentes em:

* Tablets
* Mobile intermediário
* Formulários
* Cards de profissionais

### 🔴 Consistência visual

* Desalinhamento entre páginas
* Scroll horizontal em alguns cenários
* Menu mobile instável

---

# 🎯 Conclusão

A análise de responsividade da plataforma Lacrei Saúde identificou que:

* O **funcionamento geral está preservado**
* Porém existem **problemas relevantes de layout e adaptação**
* A inconsistência é mais evidente em dispositivos mobile e tablet

Esses problemas não impedem o uso da plataforma, mas impactam diretamente a experiência da pessoa usuária e devem ser priorizados para correção.

A cobertura de testes garantiu validação de:

* Layout
* Funcionalidade
* Usabilidade
* Estabilidade visual
* Consistência entre resoluções
