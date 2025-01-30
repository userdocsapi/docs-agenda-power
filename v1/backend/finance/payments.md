---
title: 'Payments'
parent: 'Finance'
nav_order: 2
---

# Payments (Pagamentos)

Tabela que gerencia os pagamentos de agendamentos e contas a receber.

| Campo                    | Tipo      | Descrição |
|--------------------------|----------|-----------|
| id (PK)                 | UUID     | Identificador único |
| appointment_id (FK)     | UUID     | Relacionamento com o agendamento |
| accounts_receivable_id (FK) | UUID  | Relacionamento com contas a receber |
| value                   | Float    | Valor do pagamento |
| payment_method          | Enum     | Método de pagamento (CASH, CREDIT_CARD, BANK_TRANSFER, etc.) |
| due_date                | Date     | Data de vencimento do pagamento |
| automatic               | Boolean  | Indica se o pagamento foi automático |
| installment_number      | Int      | Número da parcela (se parcelado) |
| installment_total       | Int      | Total de parcelas (se parcelado) |
| parent_payment_id (FK)  | UUID     | ID do pagamento pai (se for uma subdivisão) |
| expense_id (FK)        | UUID     | Relacionamento com despesas |
| customer_credit_id (FK) | UUID     | Relacionamento com créditos do cliente |
| card_flag               | String   | Bandeira do cartão (se aplicável) |
| created_by_id (FK)      | UUID     | ID do usuário que criou o pagamento |
| updated_by_id (FK)      | UUID     | ID do usuário que atualizou o pagamento |
| created_at              | DateTime | Data de criação do registro |
| updated_at              | DateTime | Data de atualização do registro |
| deleted_at              | DateTime | Data de exclusão lógica (soft delete) |



# Payment Summaries (Resumos de Pagamentos)

Tabela que fornece um resumo dos pagamentos de um agendamento.

| Campo                    | Tipo      | Descrição |
|--------------------------|----------|-----------|
| appointment_id (FK)     | UUID     | Relacionamento com o agendamento |
| price                   | Float    | Valor total do agendamento |
| non_paid                | Boolean  | Indica se o pagamento ainda não foi concluído |
| total_paid              | Float    | Valor total já pago |
| automatic_payment       | Boolean  | Indica se o pagamento foi processado automaticamente |
| total_owned             | Float    | Valor restante a ser pago |
