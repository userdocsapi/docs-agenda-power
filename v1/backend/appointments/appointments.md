---
title: 'Appointments'
parent: 'Appointments'
nav_order: 2
---

# Appointments (Agendamentos)

Tabela que gerencia os agendamentos no sistema.

| Campo                    | Tipo     | Descrição |
|--------------------------|---------|-----------|
| id (PK)                 | UUID    | Identificador único |
| company_id (FK)         | UUID    | Identificador da empresa |
| user_id (FK)           | UUID    | Identificador do usuário responsável |
| customer_id (FK)       | UUID    | Identificador do cliente |
| service_id (FK)        | UUID    | Identificador do serviço agendado |
| date                   | DateTime | Data do agendamento |
| start_time             | Time     | Horário de início |
| end_time               | Time     | Horário de término |
| duration               | Int      | Duração do serviço (em minutos) |
| price                  | Float    | Preço do serviço agendado |
| total_paid             | Float    | Valor total pago pelo cliente |
| payment_method         | Enum     | Método de pagamento (CASH, CARD, etc.) |
| tag                    | Enum     | Status do agendamento (CANCELED, CONFIRMED, etc.) |
| non_paid               | Boolean  | Indica se o pagamento não foi realizado |
| accounts_receivable_id (FK) | UUID | Conta a receber vinculada (opcional) |
| commission_rate        | Float    | Percentual de comissão associado |
| color_id (FK)         | UUID    | Cor associada ao serviço |
| discount              | Float    | Valor do desconto aplicado |
| discount_in_percentage | Boolean  | Indica se o desconto é percentual |
| total_before_discount  | Float    | Valor total antes do desconto |
| installment_total      | Float    | Valor total das parcelas |
| card_flag             | Enum     | Bandeira do cartão de crédito |
| commission_done       | Boolean  | Indica se a comissão já foi paga |
| created_at            | DateTime | Data de criação |
| updated_at            | DateTime | Última atualização |
| deleted               | Boolean  | Indica se o agendamento foi excluído |
| deleted_at            | DateTime | Data de exclusão lógica |
