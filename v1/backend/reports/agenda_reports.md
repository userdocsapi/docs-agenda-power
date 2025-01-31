---
title: 'Agenda reports'
parent: 'Reports'
nav_order: 2
---

# Agenda Reports (Relatórios de Agenda)

O módulo **Agenda Reports** fornece relatórios detalhados sobre os agendamentos registrados no sistema, permitindo análises e acompanhamento de métricas relacionadas a atendimentos e serviços prestados.

## ➡️ Funcionalidades Principais

- **Relatório de Agendamentos**  
  Exibe todos os agendamentos realizados dentro de um período específico.

- **Filtragem Avançada**  
  Permite segmentação por cliente, profissional, serviço ou status do agendamento.

- **Métricas de Desempenho**  
  Fornece insights sobre volume de atendimentos, horários mais movimentados e taxa de cancelamentos.

- **Exportação de Dados**  
  Possibilidade de exportação dos relatórios em formatos como CSV ou PDF para análise externa.

## ➡️ Estrutura do Módulo

```bash
/reports
│── agenda_reports.md            # Relatórios de agendamentos
```

## ➡️ Endpoints Relacionados

| Método  | Rota                                   | Descrição |
|---------|--------------------------------------|----------------------------------|
| `GET`   | `/reports/agenda`                   | Retorna o relatório de agendamentos |
| `GET`   | `/reports/agenda/export`            | Exporta relatório de agendamentos em CSV ou PDF |
| `GET`   | `/reports/agenda/metrics`           | Obtém métricas relacionadas a agendamentos |

## ➡️ Regras de Negócio

- Apenas administradores e profissionais autorizados podem acessar os relatórios completos.
- Os relatórios devem refletir apenas os agendamentos ativos e concluídos.
- Cancelamentos são incluídos para análise de desempenho, mas não afetam a contagem total de atendimentos ativos.

## ➡️ Considerações Finais

O **Agenda Reports** é essencial para o acompanhamento da eficiência operacional e para ajustes estratégicos baseados no volume e comportamento dos agendamentos. Ele auxilia a tomada de decisão e otimiza o fluxo de atendimento dentro do sistema.

