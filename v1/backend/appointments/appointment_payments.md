---
title: 'Appointment payments'
parent: 'Appointments'
nav_order: 2
---

# Appointment payments (Pagamentos de Agendamentos)

O módulo **Appointment Payments** gerencia os pagamentos relacionados aos agendamentos, garantindo o controle financeiro das transações associadas aos serviços prestados.

## ➡️ Funcionalidades Principais

- **Registro de Pagamentos**  
  Armazena informações detalhadas sobre pagamentos efetuados para cada agendamento.

- **Métodos de Pagamento**  
  Suporte a diversas formas de pagamento, como cartão de crédito, débito, boleto, e Pix.

- **Consulta de Histórico**  
  Permite visualizar pagamentos realizados, pendentes e cancelados.

- **Reembolsos e Ajustes**  
  Suporte a estornos e ajustes de valores caso necessário.

## ➡️ Estrutura do Módulo

```bash
/appointments/appointment_payments.md  # Documentação sobre pagamentos de agendamentos
```

## ➡️ Benefícios

- Facilita a gestão financeira dos pagamentos vinculados aos serviços.
- Proporciona transparência no controle de valores recebidos.
- Integra-se a outros módulos financeiros para relatórios consolidados.

## ➡️ Endpoints Relacionados

| Método  | Rota                                  | Descrição |
|---------|--------------------------------------|----------------------------------|
| `GET`   | `/appointments/payments`           | Lista todos os pagamentos de agendamentos |
| `GET`   | `/appointments/payments/{id}`      | Retorna detalhes de um pagamento específico |
| `POST`  | `/appointments/payments`           | Registra um novo pagamento |
| `PUT`   | `/appointments/payments/{id}`      | Atualiza informações de um pagamento |
| `DELETE`| `/appointments/payments/{id}`      | Remove um pagamento registrado |

Este módulo é essencial para manter o controle dos pagamentos e garantir a confiabilidade nas transações financeiras da plataforma.