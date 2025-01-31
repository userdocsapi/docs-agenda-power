---
title: 'Finance'
parent: 'Backend'
nav_order: 1
---

# Módulo: Finance

O módulo **Finance** gerencia todas as transações financeiras, incluindo pagamentos, contas a receber e despesas, garantindo um controle detalhado do fluxo financeiro do sistema.

## ➡️ Funcionalidades Principais

- **Gestão de Contas a Receber**  
  Controle de pagamentos pendentes e recebimentos de clientes.

- **Pagamentos e Métodos de Pagamento**  
  Registro de pagamentos e suporte a diferentes métodos, como PIX, cartão de crédito e boleto.

- **Gerenciamento de Despesas**  
  Registro e categorização de despesas da empresa.

- **Relatórios Financeiros**  
  Geração de relatórios de fluxo de caixa e análise financeira.

## ➡️ Estrutura do Módulo

```bash
/finance
│── index.md                         # Página inicial do módulo
│── account_receivable_payments.md   # Pagamentos de contas a receber
│── accounts_receivables.md          # Gestão de contas a receber
│── accounts_receivables_items.md    # Itens detalhados das contas a receber
│── cash_flow_reports.md             # Relatórios de fluxo de caixa
│── commission_payments.md           # Pagamentos de comissões
│── expense_categories.md            # Categorização de despesas
│── expenses.md                      # Controle de despesas
│── payment_methods.md               # Métodos de pagamento disponíveis
│── payments.md                      # Registro de pagamentos
```

## ➡️ Regras de Negócio

- Todas as transações devem ser registradas com um identificador único e data de criação.
- Contas a receber podem ser associadas a diferentes métodos de pagamento.
- Despesas devem ser categorizadas corretamente para análise financeira.
- Relatórios financeiros devem exibir uma visão consolidada do fluxo de caixa.

## ➡️ Endpoints Relacionados

| Método  | Rota                                      | Descrição |
|---------|-------------------------------------------|----------------------------------|
| `GET`   | `/finance/accounts-receivables`          | Lista todas as contas a receber |
| `POST`  | `/finance/accounts-receivables`          | Cria uma nova conta a receber |
| `GET`   | `/finance/payments`                      | Lista todos os pagamentos registrados |
| `POST`  | `/finance/payments`                      | Registra um novo pagamento |
| `GET`   | `/finance/expenses`                      | Lista todas as despesas |
| `POST`  | `/finance/expenses`                      | Registra uma nova despesa |
| `GET`   | `/finance/cash-flow-reports`             | Gera um relatório de fluxo de caixa |
