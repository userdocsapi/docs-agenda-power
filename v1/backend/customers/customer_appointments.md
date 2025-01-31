---
title: 'Customer Appointments'
parent: 'Customers'
nav_order: 2
---

# Customer Appointments (Agendamentos de Clientes)

O módulo **Customer Appointments** gerencia os agendamentos dos clientes, garantindo o controle e organização das marcações de serviços no sistema.

## ➡️ Tabela de Estrutura

| Campo        | Tipo                | Descrição                                        |
|-------------|-------------------|------------------------------------------------|
| `id`        | UUID               | Identificador único do agendamento            |
| `customer_id` | UUID              | Identificador do cliente associado             |
| `service_id` | UUID              | Serviço relacionado ao agendamento            |
| `date`      | DateTime           | Data e hora do agendamento                    |
| `status`    | ENUM               | Status do agendamento (pendente, confirmado, cancelado) |
| `created_at` | DateTime          | Data de criação do registro                    |
| `updated_at` | DateTime          | Data da última atualização                     |
| `deleted_at` | DateTime (nullable) | Data de exclusão (soft delete)                 |

## ➡️ Endpoints Relacionados

| Método  | Rota                                      | Descrição                                 |
|---------|------------------------------------------|-------------------------------------------|
| `GET`   | `/customers/appointments`              | Lista todos os agendamentos dos clientes  |
| `GET`   | `/customers/appointments/{id}`         | Retorna detalhes de um agendamento       |
| `POST`  | `/customers/appointments`              | Cria um novo agendamento                 |
| `PUT`   | `/customers/appointments/{id}`         | Atualiza informações de um agendamento   |
| `DELETE`| `/customers/appointments/{id}`         | Remove um agendamento registrado         |

