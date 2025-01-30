---
title: 'Companies'
parent: 'Companies'
nav_order: 2
---

# Companies (Empresas)

Tabela que armazena as informações das empresas cadastradas no sistema.

| Campo                                 | Tipo     | Descrição |
|--------------------------------------|---------|-----------|
| id (PK)                              | UUID    | Identificador único |
| name                                  | String  | Nome da empresa |
| email                                 | String  | E-mail de contato |
| allow_multiple_appointments_per_hour | Boolean | Permite múltiplos agendamentos por hora |
| allow_overlapping_appointments       | Boolean | Permite agendamentos sobrepostos |
| automatic_appointment_charges        | Boolean | Cobrança automática de agendamentos |
| default_payment_method               | Enum    | Método de pagamento padrão (CASH, CARD, etc.) |
| enable_color_by_tag                  | Boolean | Habilita diferenciação por cor nos agendamentos |
| logo_url                              | String  | URL do logo da empresa |
| locale                                | Enum    | Localização padrão da empresa (PT_BR, EN_US, etc.) |
| target_year                           | Int     | Ano de referência da empresa |
| min_appointment_date                  | DateTime | Data mínima permitida para agendamentos |
| company_page_bio_avatar_url           | String  | URL da imagem de perfil da empresa |
| total_appointments                    | Int     | Número total de agendamentos |
| number_of_distinct_customer_ids       | Int     | Número de clientes únicos atendidos |
| best_services                         | JSON    | Lista de serviços mais agendados |
| total_duration                         | Int     | Tempo total de atendimentos prestados (em minutos) |
| deleted                               | Boolean | Indica se a empresa foi excluída |
| deleted_at                            | DateTime | Data de exclusão lógica |
| created_at                            | DateTime | Data de criação |
| updated_at                            | DateTime | Última atualização |

