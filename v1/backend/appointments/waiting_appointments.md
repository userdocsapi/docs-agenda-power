---
title: 'Waiting appointments'
parent: 'Appointments'
nav_order: 2
---

# Waiting Appointments (Fila de Espera de Agendamentos)

Tabela que gerencia os agendamentos em fila de espera.

| Campo                              | Tipo     | Descrição |
|------------------------------------|---------|-----------|
| id (PK)                           | UUID    | Identificador único |
| company_id (FK)                    | UUID    | Identificador da empresa |
| customer_id (FK)                   | UUID    | Identificador do cliente |
| service_id (FK)                    | UUID    | Identificador do serviço |
| waiting_appointment_has_service     | Boolean | Indica se há um serviço vinculado |
| preference_order                    | Int     | Ordem de preferência na fila |
| comments                            | String  | Comentários sobre o agendamento |
| created_by_id (FK)                  | UUID    | Usuário que criou o agendamento |
| updated_by_id (FK)                  | UUID    | Usuário que atualizou o agendamento |
| deleted                             | Boolean | Indica se o agendamento foi excluído |
| deleted_at                          | DateTime | Data de exclusão lógica |
| created_at                          | DateTime | Data de criação |
| updated_at                          | DateTime | Última atualização |

