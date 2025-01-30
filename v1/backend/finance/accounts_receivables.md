---
title: 'Accounts receivables'
parent: 'Finance'
nav_order: 2
---

# Accounts Receivables (Contas a Receber)

Tabela que armazena os registros de contas a receber da empresa.

| Campo                               | Tipo     | Descrição |
|------------------------------------|---------|-----------|
| id (PK)                           | UUID    | Identificador único |
| company_id (FK)                   | UUID    | Relacionamento com a empresa |
| customer_id (FK)                   | UUID    | Relacionamento com o cliente |
| date                               | Date    | Data da conta a receber |
| total_before_discount              | Float   | Valor total antes do desconto |
| total                              | Float   | Valor final da conta a receber |
| total_paid                         | Float   | Valor já pago |
| opened                             | Boolean | Indica se a conta ainda está em aberto |
| comments                           | String  | Comentários sobre a conta a receber |
| number_of_appointments_allowed     | Int     | Número de agendamentos permitidos |
| type                               | Enum    | Tipo da conta (NORMAL, PACKAGE) |
| discount                           | Float   | Valor do desconto aplicado |
| discount_in_percentage             | Boolean | Indica se o desconto é percentual |
| commission_done                    | Boolean | Indica se a comissão foi processada |
| created_by_id (FK)                 | UUID    | ID do usuário que criou o registro |
| updated_by_id (FK)                 | UUID    | ID do usuário que atualizou o registro |
| created_at                         | DateTime | Data de criação do registro |
| updated_at                         | DateTime | Data de atualização do registro |
| deleted_at                         | DateTime | Data de exclusão lógica (soft delete) |



