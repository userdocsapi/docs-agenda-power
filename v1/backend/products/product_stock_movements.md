---
title: 'Product stock movements'
parent: 'Products'
nav_order: 2
---

# Product Stock Movements (Movimentações de Estoque de Produtos)

Tabela que armazena os registros de movimentação de estoque dos produtos.

| Campo              | Tipo     | Descrição |
|-------------------|---------|-----------|
| id (PK)          | UUID    | Identificador único da movimentação |
| product_id (FK)  | UUID    | Identificador do produto movimentado |
| quantity        | Int     | Quantidade movimentada |
| description     | String  | Descrição da movimentação |
| date           | Date    | Data da movimentação |
| movement_type  | Enum    | Tipo de movimentação (ADD, REMOVE) |
| created_at     | DateTime | Data de criação |

