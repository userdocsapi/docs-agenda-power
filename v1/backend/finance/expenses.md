---
title: 'Expenses'
parent: 'Finance'
nav_order: 2
---

# Expenses (Despesas)

Tabela que gerencia as despesas de uma empresa.

| Campo                        | Tipo      | Descrição |
|------------------------------|----------|-----------|
| id (PK)                     | UUID     | Identificador único |
| company_id (FK)             | UUID     | Identificador da empresa |
| employee_id (FK, opcional)  | UUID     | Identificador do funcionário relacionado |
| name                        | String   | Nome da despesa |
| value                       | Float    | Valor da despesa |
| date                        | Date     | Data da despesa |
| category                    | Enum     | Categoria da despesa (ADVANCE_MONEY, COSTS, etc.) |
| expense_category_id (FK, opcional) | UUID | Identificador da categoria da despesa |
| type                        | Enum     | Tipo de despesa (REGULAR, INSTALLMENT) |
| start_date (nullable)       | Date     | Data de início (se for parcelada) |
| end_date (nullable)         | Date     | Data de término (se for parcelada) |
| installment_number (nullable) | Int     | Número da parcela (se parcelada) |
| installment_total (nullable) | Int     | Total de parcelas (se parcelada) |
| total_value (nullable)      | Float    | Valor total da despesa parcelada |
| parent_expense_id (FK, opcional) | UUID | Relacionamento com outra despesa (se for parte de um conjunto) |
| paid                        | Boolean  | Indica se a despesa já foi paga |
| attachment_source_type (nullable) | String | Tipo da fonte do anexo |
| attachment_source_object_id (nullable) | UUID | Identificador do objeto do anexo |
| deleted                     | Boolean  | Indica se a despesa foi excluída |
| deleted_at (nullable)       | DateTime | Data de exclusão lógica (soft delete) |
| deleted_by_id (FK, opcional) | UUID | ID do usuário que excluiu o registro |
| created_by_id (FK)          | UUID     | ID do usuário que criou a despesa |
| created_at                  | DateTime | Data de criação do registro |
| updated_by_id (FK)          | UUID     | ID do usuário que atualizou a despesa |
| updated_at                  | DateTime | Data de atualização do registro |

