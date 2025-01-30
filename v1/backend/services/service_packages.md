---
title: 'Service packages'
parent: 'Services'
nav_order: 2
---

# Service Packages (Pacotes de Serviços)

Tabela que armazena os pacotes de serviços oferecidos pelas empresas.

| Campo            | Tipo     | Descrição |
|-----------------|---------|-----------|
| id (PK)        | UUID    | Identificador único do pacote de serviços |
| company_id (FK) | UUID    | Identificador da empresa |
| created_by_id (FK) | UUID | Usuário que criou o pacote de serviços |
| updated_by_id (FK) | UUID | Usuário que fez a última atualização |
| name           | String  | Nome do pacote de serviços |
| price          | Float   | Preço total do pacote |
| deleted        | Boolean | Indica se o pacote foi excluído (soft delete) |
| deleted_at     | DateTime | Data de exclusão lógica (opcional) |
| created_at     | DateTime | Data de criação |
| updated_at     | DateTime | Última atualização |

