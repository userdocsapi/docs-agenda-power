---
title: 'Total customer stats'
parent: 'Reports'
nav_order: 2
---

# Total customer stats (Estatísticas Totais de Clientes)

O relatório **Total Customer Stats** fornece uma visão abrangente sobre a base de clientes do sistema, incluindo métricas importantes como número total de clientes cadastrados, taxas de retenção e comportamento ao longo do tempo.

## ➡️ Funcionalidades Principais

- **Número Total de Clientes**  
  Exibe a quantidade total de clientes registrados na plataforma.

- **Taxa de Retenção**  
  Analisa quantos clientes continuam utilizando os serviços após um determinado período.

- **Distribuição de Clientes**  
  Permite segmentação por idade, localização, gênero e outros critérios demográficos.

- **Atividade dos Clientes**  
  Indica quais clientes estão mais ativos e quais estão inativos há um longo período.

## ➡️ Estrutura do Módulo

```bash
/reports/total_customer_stats.md  # Estatísticas gerais dos clientes
```

## ➡️ Benefícios

- Permite entender o crescimento da base de clientes.
- Ajuda na criação de estratégias para retenção e reativação de clientes inativos.
- Fornece insights para melhorar campanhas de marketing e atendimento ao cliente.

## ➡️ Endpoints Relacionados

| Método  | Rota                                  | Descrição |
|---------|--------------------------------------|------------------------------------------|
| `GET`   | `/reports/total-customer-stats`    | Retorna as estatísticas gerais de clientes |
| `GET`   | `/reports/total-customer-stats/{id}` | Exibe dados detalhados de um cliente específico |

Este relatório é essencial para monitorar o comportamento dos clientes e tomar decisões estratégicas para melhorar a retenção e engajamento.