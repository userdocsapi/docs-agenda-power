---
title: 'Expense categories'
parent: 'Finance'
nav_order: 2
---

# Expense Categories (Categorias de Despesas)

Tabela que armazena as categorias de despesas de uma empresa.

| Campo                     | Tipo      | Descrição |
|---------------------------|----------|-----------|
| id (PK)                  | UUID     | Identificador único |
| company_id (FK)          | UUID     | Relacionamento com a empresa |
| name                     | String   | Nome da categoria de despesa |
| description (nullable)   | Text     | Descrição da categoria |
| category_group_id (nullable) | UUID | Referência a um agrupamento de categorias |
| category_group_name (nullable) | String | Nome do grupo da categoria |
| deleted                  | Boolean  | Indica se a categoria foi excluída |
| deleted_at (nullable)    | DateTime | Data de exclusão lógica (soft delete) |
| deleted_by_id (FK)       | UUID     | ID do usuário que excluiu a categoria |
| created_by_id (FK)       | UUID     | ID do usuário que criou a categoria |
| created_at               | DateTime | Data de criação do registro |
| updated_by_id (FK)       | UUID     | ID do usuário que atualizou a categoria |
| updated_at               | DateTime | Data de atualização do registro |
