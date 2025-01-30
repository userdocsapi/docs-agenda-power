---
title: 'User roles'
parent: 'Authentication'
nav_order: 2
---

# Roles (Perfis de Usuário)

Tabela que gerencia os diferentes perfis de usuários no sistema.

| Campo               | Tipo      | Descrição |
|--------------------|----------|-----------|
| id (PK)           | UUID     | Identificador único do perfil |
| value            | String   | Código interno do perfil (ex: EMPLOYEE_INDEPENDENT) |
| name             | String   | Nome do perfil visível no sistema |
| description      | Text     | Explicação detalhada do perfil |
| description_new  | Text (nullable) | Nova descrição do perfil |
| internal         | Boolean  | Indica se é um perfil interno do sistema |
| professional     | Boolean  | Indica se o perfil se aplica a profissionais |
| active          | Boolean  | Indica se o perfil está ativo |
| sorting_order    | Int      | Define a ordem de exibição dos perfis |
| created_at       | DateTime | Data de criação |
| updated_at       | DateTime | Última atualização |
