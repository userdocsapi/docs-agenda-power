---
title: 'User roles permissions'
parent: 'Authentication'
nav_order: 2
---

# Role Permissions (Relacionamento entre Perfis e Permissões)

Tabela que gerencia a associação entre perfis de usuários e permissões.

| Campo               | Tipo      | Descrição |
|--------------------|----------|-----------|
| role_id (FK)      | UUID     | Identificador do perfil de usuário (roles.id) |
| permission_id (FK) | UUID    | Identificador da permissão associada (permissions.id) |
