---
title: 'Product purchases'
parent: 'Products'
nav_order: 2
---

# Product Purchases (Compras de Produtos)

Tabela que armazena as compras de produtos realizadas por uma empresa.

## Estrutura da Tabela

| Campo                        | Tipo      | Descrição |
|------------------------------|----------|-----------|
| id (PK)                      | UUID     | Identificador único da compra de produtos |
| company_id (FK → companies)   | UUID     | Relacionamento com a empresa responsável pela compra |
| product_supplier_id (FK → product_suppliers) | UUID | Relacionamento com o fornecedor do produto |
| description                   | String   | Descrição da compra |
| purchase_date                 | Date     | Data da compra |
| value                         | Decimal  | Valor total da compra |
| payment_method                | ENUM     | Método de pagamento (CASH, CREDIT_CARD, etc.) |
| installment_total (nullable)   | Integer  | Número total de parcelas (caso aplicável) |
| expense_id (FK → expenses, nullable) | UUID | Relacionamento com a despesa associada à compra |
| deleted                       | Boolean  | Indica se a compra foi excluída |
| deleted_at (nullable)         | DateTime | Data de exclusão lógica |
| created_by_id (FK → users)     | UUID     | Identificador do usuário que registrou a compra |
| updated_by_id (FK → users)     | UUID     | Identificador do usuário que atualizou a compra |
| created_at                    | DateTime | Data de criação |
| updated_at                    | DateTime | Última atualização |

