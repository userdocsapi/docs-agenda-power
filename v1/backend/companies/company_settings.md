---
title: 'Company settings'
parent: 'Companies'
nav_order: 2
---

# Company Online Scheduling Settings (Configurações de Agendamento Online da Empresa)

Tabela que gerencia as configurações de agendamento online dos serviços de uma empresa.

| Campo                              | Tipo     | Descrição |
|-----------------------------------|---------|-----------|
| id (PK)                          | UUID    | Identificador único |
| company_id (FK)                   | UUID    | Identificador da empresa |
| service_id (FK)                   | UUID    | Identificador do serviço configurado para agendamento online |
| online_scheduling_enabled         | Boolean | Indica se o serviço pode ser agendado online |
| online_scheduling_price_display   | Enum    | Tipo de exibição do preço no agendamento online (FIXED, VARIABLE, etc.) |
