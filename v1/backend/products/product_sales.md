---
title: 'Product sales'
parent: 'Products'
nav_order: 2
---

# Product Sales (Vendas de Produtos)

Tabela que registra as vendas de produtos realizadas por uma empresa.

| Campo                 | Tipo     | Descrição |
|----------------------|---------|-----------|
| id (PK)            | UUID    | Identificador único da venda |
| company_id (FK)    | UUID    | Identificador da empresa |
| customer_id (FK)   | UUID    | Identificador do cliente |
| sale_date         | Date    | Data da venda |
| comments         | String  | Comentários sobre a venda |
| discount        | Float   | Valor do desconto aplicado |
| discount_in_percentage | Boolean | Indica se o desconto é percentual |
| created_by_id (FK) | UUID  | Usuário que registrou a venda |
| updated_by_id (FK) | UUID  | Usuário que fez a última atualização |
| created_at       | DateTime | Data de criação |
| updated_at       | DateTime | Última atualização |

