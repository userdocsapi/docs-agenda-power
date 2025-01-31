---
title: 'Appointment tags'
parent: 'Appointments'
nav_order: 2
---

# Appointment tags

## Estrutura da Tabela

| Campo          | Tipo       | Descrição |
|---------------|-----------|-----------|
| `id`         | `UUID`    | Identificador único da tag. |
| `appointment_id` | `UUID`    | Identificador do agendamento associado. |
| `name`       | `STRING`  | Nome da tag atribuída ao agendamento. |
| `color`      | `STRING`  | Código hexadecimal da cor da tag. |
| `created_at` | `DATETIME` | Data e hora da criação da tag. |
| `updated_at` | `DATETIME` | Data e hora da última atualização. |

