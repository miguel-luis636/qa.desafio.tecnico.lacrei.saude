# 🏗️ Critérios de Aceite — Desafio QA | Lacrei Saúde

Esta seção define os critérios utilizados para avaliação do projeto de Quality Assurance, garantindo padronização, rastreabilidade e clareza na entrega dos testes, automações e documentações.

Cada critério possui um peso específico, representando sua importância dentro do contexto geral do desafio.

---

# 📊 Matriz de Avaliação

| Critério | Peso (%) | Descrição |
|---|---|---|
| Casos de Teste (Gherkin) | 15% | Cobertura completa dos fluxos críticos da aplicação com cenários claros, reutilizáveis e bem estruturados |
| Documentação no GitHub | 10% | Organização do repositório, clareza do README e estrutura de pastas padronizada |
| Teste de Acessibilidade | 10% | Validação com Lighthouse ≥ 90 e checklist manual (teclado, leitor de tela, contraste e semântica) |
| Teste de Desempenho | 10% | Validação de performance com tempo de resposta < 500ms em fluxos críticos |
| Teste de Responsividade | 10% | Garantia de usabilidade sem quebras críticas em dispositivos mobile e desktop |
| Automação e Pipeline (CI/CD) | 20% | Implementação de testes automatizados de cadastro com Cypress + execução via GitHub Actions |
| Gestão de Bugs e Melhorias | 15% | Registro estruturado de bugs com evidências, severidade, prioridade e sugestões de melhoria |
| Qualidade da Documentação Geral | 10% | Clareza, organização e centralização das informações no GitHub |

---

# 🎯 Regras Gerais de Aceite

Para que o projeto seja considerado completo, os seguintes requisitos devem ser atendidos:

## ✔️ Cobertura Funcional
- Todos os fluxos principais devem possuir testes documentados em Gherkin
- Cenários devem contemplar casos positivos e negativos

## ✔️ Automação
- Pelo menos o fluxo de cadastro deve estar automatizado
- Execução deve ocorrer via Cypress
- Pipeline CI/CD deve estar funcional no GitHub Actions

## ✔️ Qualidade Não Funcional
- Acessibilidade deve atingir nota mínima de 90 no Lighthouse
- Performance deve atender tempo de resposta definido
- Responsividade não pode apresentar quebras críticas

## ✔️ Documentação
- README completo e atualizado
- Estrutura clara de diretórios no GitHub
- Evidências organizadas e versionadas

## ✔️ Gestão de Defeitos
- Bugs devem conter:
  - Título claro
  - Passos para reprodução
  - Evidência (print/vídeo)
  - Severidade e prioridade
  - Sugestão de melhoria

---

# 📌 Critério de Qualidade Final

O projeto será considerado **aprovado** quando:

- Todos os fluxos críticos estiverem cobertos por testes
- A automação estiver integrada ao CI/CD
- Os testes não funcionais atenderem os thresholds definidos
- A documentação estiver completa e organizada no GitHub
- Os bugs estiverem documentados de forma rastreável

---

# 💡 Observação

A avaliação não considera apenas execução de testes, mas principalmente:

- Clareza na documentação
- Pensamento crítico de QA
- Estrutura de automação
- Organização do projeto
- Capacidade de identificar riscos e propor melhorias
