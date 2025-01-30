---
title: 'Users'
parent: 'Authentication'
nav_order: 2
---

# Users (Usuários)

Tabela que armazena os dados dos usuários do sistema.

| Campo         | Tipo     | Descrição |
|--------------|---------|-----------|
| id (PK)      | UUID    | Identificador único do usuário |
| email        | String  | E-mail do usuário |
| password     | String  | Senha (hash) |
| role_id (FK) | UUID    | Relacionado a roles (CLIENT, PROFESSIONAL, ADMIN) |
| theme_id (FK) | UUID   | Relacionado a user_themes |
| company_id (FK) | UUID | Relacionado a companies |
| createdAt    | DateTime | Data de criação |
| updatedAt    | DateTime | Última atualização |
| deletedAt    | DateTime | Data de exclusão lógica |










