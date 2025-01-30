---
title: 'Application roles'
parent: 'Authentication'
nav_order: 2
---

# Permissions (Restrições Específicas)

Tabela que define permissões específicas para controle de acesso no sistema.

| Campo               | Tipo      | Descrição |
|--------------------|----------|-----------|
| id (PK)           | UUID     | Identificador único da permissão |
| value            | String   | Código da permissão (ex: CANNOT_EDIT_APPOINTMENTS) |
| name             | String   | Nome da permissão visível no sistema |
| description      | Text (nullable) | Explicação detalhada da permissão |
| sorting_order    | Int (nullable) | Define a ordem de exibição das permissões |
| internal         | Boolean  | Indica se é uma permissão interna do sistema |
| professional     | Boolean  | Indica se a permissão se aplica a profissionais |
| active          | Boolean  | Indica se a permissão está ativa |
| created_at       | DateTime | Data de criação |
| updated_at       | DateTime | Última atualização |

