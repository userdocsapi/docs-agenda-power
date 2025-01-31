---
title: 'Cash Flow Reports'
parent: 'Reports'
nav_order: 2
---

# **Cash Flow Reports (Relatórios de Fluxo de Caixa)**

O módulo **Cash Flow Reports** fornece insights detalhados sobre a movimentação financeira da empresa, permitindo um acompanhamento preciso das entradas e saídas de recursos.

## ➞ **Funcionalidades Principais**

- **Monitoramento de Entradas e Saídas**  
  Exibe o fluxo de caixa diário, semanal ou mensal, categorizando receitas e despesas.

- **Relatórios Personalizados**  
  Filtragem por data, tipo de transação e categoria financeira.

- **Análise de Saldo Disponível**  
  Indica a posição financeira da empresa em períodos específicos.

- **Exportação de Dados**  
  Possibilidade de exportar relatórios em formatos como **PDF** e **CSV**.

## ➞ **Estrutura do Módulo**

```bash
/reports/cash_flow_reports.md     # Relatório de fluxo de caixa
```

## ➞ **Benefícios**

- Facilita a tomada de decisão baseada na saúde financeira da empresa.  
- Melhora o controle financeiro ao visualizar padrões de receita e despesa.  
- Identifica possíveis déficits ou períodos de menor liquidez.

## ➞ **Endpoints Relacionados**

| Método  | Rota                              | Descrição |
|---------|----------------------------------|--------------------------------------------|
| `GET`   | `/reports/cash-flow`            | Retorna o fluxo de caixa geral |
| `GET`   | `/reports/cash-flow?period=30d` | Relatório de fluxo de caixa dos últimos 30 dias |
| `GET`   | `/reports/cash-flow/{id}`       | Detalhes de uma transação específica |

Os relatórios de **Fluxo de Caixa** são essenciais para um planejamento financeiro eficiente, garantindo uma visão clara da sustentabilidade e rentabilidade do negócio.