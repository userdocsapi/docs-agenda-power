---
title: 'Commission payments'
parent: 'Finance'
nav_order: 2
---

# Commission Payments (Pagamentos de Comissão)

Tabela que registra os pagamentos de comissão para funcionários.

| Campo                    | Tipo      | Descrição |
|--------------------------|----------|-----------|
| id (PK)                 | UUID     | Identificador único |
| employee_id (FK)        | UUID     | Relacionamento com o funcionário |
| start_date              | Date     | Data inicial do cálculo da comissão |
| end_date                | Date     | Data final do cálculo da comissão |
| gross_total             | Float    | Valor total bruto da comissão |
| number_of_appointments  | Int      | Número de agendamentos relacionados à comissão |
| created_at              | DateTime | Data de criação do registro |
| updated_at              | DateTime | Data de atualização do registro |
