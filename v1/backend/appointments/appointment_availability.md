---
title: 'Appointment availability'
parent: 'Appointments'
nav_order: 2
---

# Appointment Availability (Disponibilidade de Agendamentos)

Tabela que gerencia a disponibilidade para agendamentos.

| Campo        | Tipo     | Descrição |
|-------------|---------|-----------|
| id (PK)     | UUID    | Identificador único |
| date        | DateTime | Data de disponibilidade |
| start_time  | Time     | Horário de início |
| end_time    | Time     | Horário de término |
| employee_id (FK) | UUID | Identificador do profissional disponível |
| company_id (FK) | UUID | Identificador da empresa |
| created_at  | DateTime | Data de criação |
| updated_at  | DateTime | Última atualização |

