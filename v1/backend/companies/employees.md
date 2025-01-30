---
title: 'Employees'
parent: 'Companies'
nav_order: 2
---

# Employees (Funcionários)

Tabela que armazena os dados dos funcionários da empresa.

| Campo                  | Tipo     | Descrição |
|------------------------|---------|-----------|
| id (PK)               | UUID    | Identificador único |
| company_id (FK)       | UUID    | Identificador da empresa |
| name                  | String  | Nome do funcionário |
| cpf                   | String  | CPF do funcionário (opcional) |
| cnpj                  | String  | CNPJ do funcionário (opcional) |
| email                 | String  | E-mail do funcionário (opcional) |
| temp_password         | String  | Senha temporária (opcional) |
| professional          | Boolean | Indica se é um profissional da beleza |
| commission            | Float   | Percentual de comissão (ex: 1 = 100%) |
| color_id              | UUID    | Identificador da cor associada |
| enabled               | Boolean | Funcionário ativo |
| roles                 | JSON    | Funções atribuídas |
| master                | Boolean | Acesso administrativo |
| revenue_excluded      | Boolean | Receita excluída do financeiro |
| without_login_credentials | Boolean | Indica se tem login no sistema |
| is_cnpj               | Boolean | Indica se o funcionário usa CNPJ |
| role_ids              | JSON    | Lista de IDs de papéis vinculados |
| deleted               | Boolean | Indica exclusão lógica |
| deleted_at            | DateTime | Data de exclusão lógica |
| created_at            | DateTime | Data de criação |
| updated_at            | DateTime | Última atualização |

