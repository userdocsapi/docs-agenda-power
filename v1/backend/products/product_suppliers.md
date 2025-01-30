---
title: 'Product suppliers'
parent: 'Products'
nav_order: 2
---

# Product Suppliers (Fornecedores de Produtos)

Tabela que gerencia os fornecedores de produtos cadastrados por uma empresa.

| Campo              | Tipo     | Descrição |
|-------------------|---------|-----------|
| id (PK)          | UUID    | Identificador único do fornecedor |
| company_id (FK)  | UUID    | Identificador da empresa |
| created_by_id (FK) | UUID  | Usuário que cadastrou o fornecedor |
| updated_by_id (FK) | UUID  | Usuário que fez a última atualização |
| name            | String  | Nome do fornecedor |
| deleted         | Boolean | Indica se o fornecedor foi excluído (soft delete) |
| deleted_at      | DateTime | Data de exclusão lógica (opcional) |
| created_at      | DateTime | Data de criação |
| updated_at      | DateTime | Última atualização |

