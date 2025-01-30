---
title: 'Service package items'
parent: 'Services'
nav_order: 2
---

# Service Package Items (Itens do Pacote de Serviços)

Tabela que gerencia os serviços incluídos nos pacotes de serviços.

| Campo                | Tipo     | Descrição |
|----------------------|---------|-----------|
| id (PK)             | UUID    | Identificador único do item no pacote |
| service_package_id (FK) | UUID | Identificador do pacote de serviços |
| service_id (FK)     | UUID    | Identificador do serviço incluído no pacote |
| quantity            | Int     | Quantidade do serviço no pacote |
| price               | Float   | Preço individual do serviço no pacote |
| created_by_id (FK)  | UUID    | Usuário que adicionou o serviço ao pacote |
| updated_by_id (FK)  | UUID    | Usuário que fez a última atualização no item |
| deleted             | Boolean | Indica se o item foi excluído (soft delete) |
| deleted_at          | DateTime | Data de exclusão lógica (opcional) |
| created_at          | DateTime | Data de criação |
| updated_at          | DateTime | Última atualização |
