---
title: 'Appointment Flow'
parent: 'Flow'
nav_order: 1
---

# Appointment Flow (Fluxo de Agendamento)

Descrição do fluxo de agendamento, desde a escolha do serviço até a confirmação final.

```mermaid
graph TD;
    Start[🚀 Início do Agendamento] --> A[Usuário seleciona serviço e profissional]
    A --> B[Usuário escolhe data e horário]
    B --> C{Horário disponível?}
    C -- Não --> X[Exibe mensagem de erro e retorna]
    C -- Sim --> D[Registra o agendamento no banco de dados]
    D --> E[Envia notificação de confirmação]
    E --> F{Pagamento necessário?}
    F -- Sim --> G[Redireciona para pagamento]
    G --> H{Pagamento aprovado?}
    H -- Não --> Y[Exibe erro e cancela agendamento]
    H -- Sim --> I[Confirma agendamento pago]
    F -- Não --> I
    I --> J[Exibe confirmação ao usuário]
    J --> End[🏁 Fim do processo]
