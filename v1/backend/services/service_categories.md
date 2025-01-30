---
title: 'Service categories'
parent: 'Services'
nav_order: 2
---

# Service Categories (Categorias de Serviços)

Tabela que armazena as categorias dos serviços oferecidos.

| Campo             | Tipo     | Descrição |
|------------------|---------|-----------|
| id (PK)         | UUID    | Identificador único |
| company_id (FK) | UUID    | Identificador da empresa |
| created_by_id (FK) | UUID | Usuário que criou a categoria |
| updated_by_id (FK) | UUID | Usuário que fez a última atualização |
| name            | String  | Nome da categoria |
| deleted         | Boolean | Indica se a categoria foi excluída (soft delete) |
| deleted_at      | DateTime | Data de exclusão lógica (opcional) |
| created_at      | DateTime | Data de criação |
| updated_at      | DateTime | Última atualização |

