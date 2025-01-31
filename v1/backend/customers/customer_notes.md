---
title: 'Customer notes'
parent: 'Customers'
nav_order: 2
---

# Customer notes

Descrição sobre `customer_notes`.

| Campo          | Tipo                | Descrição                                        |
|---------------|-------------------|------------------------------------------------|
| `id`          | UUID                | Identificador único da nota do cliente         |
| `customer_id` | UUID                | Identificador do cliente associado             |
| `note`        | Text                | Conteúdo da anotação registrada                |
| `created_by`  | UUID                | Identificador do usuário que criou a nota      |
| `created_at`  | DateTime            | Data e hora de criação da nota                 |
| `updated_at`  | DateTime            | Data da última atualização                     |
| `deleted_at`  | DateTime (nullable) | Data de exclusão da nota (soft delete)         |