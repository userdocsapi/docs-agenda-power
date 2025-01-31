---
title: 'Appointment reminders'
parent: 'Appointments'
nav_order: 2
---

# Appointment reminders (Lembretes de Agendamentos)

O módulo **Appointment reminders** gerencia o envio automático de lembretes para os clientes sobre seus agendamentos, garantindo maior adesão e redução de faltas. Ele possibilita notificações via e-mail, SMS ou WhatsApp com mensagens personalizadas e programadas conforme a necessidade da empresa.

| Campo                   | Tipo                | Descrição |
|-------------------------|---------------------|--------------------------------|
| `id`                   | UUID                | Identificador único da assinatura |
| `anamnese_form_id`     | UUID                | Referência ao formulário de anamnese |
| `customer_id`          | UUID                | Identificador do cliente |
| `signature_date`       | DateTime            | Data e hora da assinatura |
| `signed_by`            | String              | Nome do assinante |
| `signature_method`     | ENUM                | Método utilizado para assinatura (digital, manual) |
| `signature_data`       | JSON                | Dados da assinatura eletrônica |
| `created_at`           | DateTime            | Data de criação do registro |
| `updated_at`           | DateTime            | Data da última atualização |
| `deleted_at`           | DateTime (nullable) | Data de exclusão (soft delete) |



