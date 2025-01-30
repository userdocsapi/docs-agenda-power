---
title: 'Product categories'
parent: 'Products'
nav_order: 2
---


# Product Categories (Categorias de Produtos)

Tabela que armazena as categorias dos produtos.

| Campo              | Tipo     | Descrição |
|-------------------|---------|-----------|
| id (PK)          | UUID    | Identificador único da categoria |
| company_id (FK)  | UUID    | Identificador da empresa |
| created_by_id (FK) | UUID  | Usuário que criou a categoria |
| updated_by_id (FK) | UUID  | Usuário que fez a última atualização |
| name            | String  | Nome da categoria |
| deleted         | Boolean | Indica se a categoria foi excluída (soft delete) |
| deleted_at      | DateTime | Data de exclusão lógica (opcional) |
| created_at      | DateTime | Data de criação |
| updated_at      | DateTime | Última atualização |


