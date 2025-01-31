---
title: 'Daily performance reports'
parent: 'Reports'
nav_order: 2
---

# Daily Performance Reports (Relatórios de Desempenho Diário)

O módulo **Daily Performance Reports** fornece um panorama detalhado do desempenho diário da empresa, permitindo acompanhar métricas essenciais para a gestão e otimização dos processos.

## ➡️ Funcionalidades Principais

- **Resumo Diário de Atendimentos**  
  Exibe a quantidade de serviços realizados no dia.

- **Faturamento Diário**  
  Relatório com a receita gerada no dia, segmentado por tipo de serviço e profissional.

- **Métricas de Eficiência**  
  Comparação entre agendamentos marcados, realizados e cancelados.

- **Análise de Ocupação**  
  Identifica horários mais e menos movimentados, auxiliando na otimização da agenda.

## ➡️ Estrutura do Módulo

```bash
/reports/daily_performance_reports.md  # Relatório de desempenho diário
```

## ➡️ Benefícios

- Monitoramento contínuo da performance da empresa.
- Identificação de padrões de demanda para melhor planejamento.
- Otimização da ocupação de profissionais e horários.
- Geração de insights para estratégias de crescimento.

## ➡️ Endpoints Relacionados

| Método  | Rota                                       | Descrição |
|---------|-------------------------------------------|----------------------------------|
| `GET`   | `/reports/daily-performance`             | Retorna o resumo diário de desempenho |
| `GET`   | `/reports/daily-performance/{date}`      | Detalhes do desempenho de um dia específico |

Os relatórios de desempenho diário são fundamentais para manter um acompanhamento preciso das operações e garantir a eficiência dos serviços prestados.

