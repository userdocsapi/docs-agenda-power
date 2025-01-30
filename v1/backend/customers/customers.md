---
title: 'Customers'
parent: 'Customers'
nav_order: 2
---

# Customers (Clientes)

Tabela que armazena os dados dos clientes.

| Campo        | Tipo     | Descrição |
|-------------|---------|-----------|
| id (PK)     | UUID    | Identificador único |
| company_id (FK) | UUID | Identificador da empresa |
| created_by_id (FK) | UUID | Usuário que criou o cliente |
| updated_by_id (FK) | UUID | Última alteração feita por |
| name        | String  | Nome do cliente |
| phone1      | String  | Telefone principal |
| phone2      | String  | Telefone secundário (opcional) |
| address     | String  | Endereço do cliente |
| cpf         | String  | CPF do cliente (opcional) |
| cnpj        | String  | CNPJ do cliente (opcional) |
| birth_date  | DateTime | Data de nascimento |
| email       | String  | E-mail do cliente (opcional) |
| noted       | Boolean | Indica se há observação importante |
| deleted     | Boolean | Indica exclusão lógica |
| deleted_at  | DateTime | Data de exclusão lógica |
| created_at  | DateTime | Data de criação |
| updated_at  | DateTime | Última atualização |



