---
title: 'Services'
parent: 'Backend'
nav_order: 1
---

# Services (Serviços)

Tabela que gerencia os serviços oferecidos pelas empresas.

| Campo                      | Tipo     | Descrição |
|----------------------------|---------|-----------|
| id (PK)                   | UUID    | Identificador único |
| company_id (FK)           | UUID    | Identificador da empresa |
| created_by_id (FK)        | UUID    | Usuário que criou o serviço |
| updated_by_id (FK)        | UUID    | Usuário que fez a última atualização |
| name                      | String  | Nome do serviço |
| duration                  | Int     | Duração do serviço (em minutos) |
| price                     | Float   | Preço do serviço |
| price_cost                | Float   | Custo do serviço |
| color_id (FK)             | UUID    | Identificador da cor associada |
| service_category_id (FK)  | UUID    | Categoria do serviço |
| description               | String  | Descrição do serviço |
| promo_price_description   | String  | Descrição da promoção |
| image_url                 | String  | URL da imagem do serviço |
| online_scheduling_enabled | Boolean | Disponível para agendamento online |
| deleted                   | Boolean | Indica se o serviço foi excluído |
| deleted_at                | DateTime | Data de exclusão lógica |
| created_at                | DateTime | Data de criação |
| updated_at                | DateTime | Última atualização |

