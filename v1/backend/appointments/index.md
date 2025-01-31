---
title: 'Appointments'
parent: 'Backend'
nav_order: 1
---

# Módulo: Appointments

O módulo **Appointments** gerencia os agendamentos de serviços, permitindo que clientes e profissionais organizem horários de forma eficiente.

## ➡️ Funcionalidades Principais

- **Disponibilidade de Agendamentos**  
  Consulta e controle dos horários disponíveis para agendamentos.

- **Criação e Gerenciamento de Agendamentos**  
  Permite a criação, edição e cancelamento de agendamentos.

- **Pagamentos de Agendamentos**  
  Integração com métodos de pagamento para registro e controle financeiro.

- **Lembretes e Notificações**  
  Envio de lembretes automáticos via e-mail ou WhatsApp.

## ➡️ Estrutura do Módulo

```bash
/appointments
│── index.md                        # Página inicial do módulo
│── appointment_availability.md      # Disponibilidade de horários
│── appointment_payments.md          # Gerenciamento de pagamentos
│── appointment_reminders.md         # Notificações e lembretes
│── appointment_repeat_info.md       # Configuração de repetições de agendamentos
│── appointment_tags.md              # Categorização e tags para agendamentos
│── appointments.md                  # Gerenciamento geral de agendamentos
│── waiting_appointments.md          # Lista de espera de agendamentos
```

## ➡️ Regras de Negócio

- Um cliente pode agendar um serviço apenas dentro dos horários disponíveis.
- Cancelamentos devem ser realizados com um tempo mínimo de antecedência.
- Agendamentos podem ser pagos antecipadamente ou no momento do serviço.
- O sistema pode bloquear horários específicos para evitar sobreposição de agendamentos.

## ➡️ Endpoints Relacionados

| Método  | Rota                                 | Descrição |
|---------|--------------------------------------|----------------------------------|
| `GET`   | `/appointments`                     | Lista todos os agendamentos |
| `POST`  | `/appointments`                     | Cria um novo agendamento |
| `PUT`   | `/appointments/{id}`                | Atualiza um agendamento existente |
| `DELETE`| `/appointments/{id}`                | Cancela um agendamento |
| `GET`   | `/appointments/availability`        | Retorna horários disponíveis |
| `GET`   | `/appointments/reminders`           | Lista lembretes de agendamentos |

