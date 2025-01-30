---
title: 'Appointment repeat info'
parent: 'Appointments'
nav_order: 2
---

# Appointment Repeat Info (Repetição de Agendamentos)

Tabela que gerencia a repetição dos agendamentos.

| Campo              | Tipo     | Descrição |
|--------------------|---------|-----------|
| id (PK)           | UUID    | Identificador único |
| appointment_id (FK) | UUID  | Identificador do agendamento |
| repeat_style      | Enum    | Estilo de repetição (DAILY, WEEKLY, etc.) |
| repeat_interval   | Int     | Intervalo de repetição (exemplo: 15 dias) |
| number_of_occurrences | Int | Número de repetições |
| end_date          | DateTime | Data final da repetição |
| days_of_week      | JSON    | Dias da semana para repetição |
| created_at        | DateTime | Data de criação |
| updated_at        | DateTime | Última atualização |

