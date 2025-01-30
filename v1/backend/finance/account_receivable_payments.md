---
title: 'Account receivable payments'
parent: 'Finance'
nav_order: 2
---

# Accounts Receivable Payments (Pagamentos de Contas a Receber)

Tabela que registra os pagamentos efetuados para contas a receber.

| Campo                      | Tipo      | Descrição |
|----------------------------|----------|-----------|
| id (PK)                   | UUID     | Identificador único |
| accounts_receivable_id (FK) | UUID    | Relacionamento com a conta a receber |
| value                     | Float    | Valor pago |
| installment_total         | Int      | Número total de parcelas (se houver) |
| payment_method            | Enum     | Método de pagamento (CASH, CREDIT_CARD, BANK_TRANSFER, etc.) |
| card_flag                 | String   | Bandeira do cartão (se aplicável) |
| due_date                  | Date     | Data do pagamento |
| created_by_id (FK)        | UUID     | ID do usuário que criou o pagamento |
| updated_by_id (FK)        | UUID     | ID do usuário que atualizou o pagamento |
| created_at                | DateTime | Data de criação do registro |
| updated_at                | DateTime | Data de atualização do registro |
| deleted_at                | DateTime | Data de exclusão lógica (soft delete) |
