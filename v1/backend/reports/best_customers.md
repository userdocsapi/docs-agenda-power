---
title: 'Best customers'
parent: 'Reports'
nav_order: 2
---

# Best customers (Melhores clientes)

O módulo **Best Customers** fornece relatórios detalhados sobre os clientes mais ativos e valiosos para o negócio, auxiliando na identificação de padrões de consumo e fidelização.

## ➡️ Funcionalidades Principais

- **Identificação dos Clientes Mais Frequentes**  
  Lista os clientes que realizam mais agendamentos dentro de um período específico.

- **Análise de Ticket Médio**  
  Exibe os clientes com maior valor gasto em serviços e produtos.

- **Segmentação por Período**  
  Permite a análise dos melhores clientes por semana, mês ou ano.

- **Exportação de Relatórios**  
  Geração de relatórios em formatos como PDF ou CSV para análise externa.

## ➡️ Estrutura do Módulo

```bash
/reports/best_customers.md     # Relatório dos melhores clientes
```

## ➡️ Benefícios

- Ajuda a criar estratégias de fidelização com base no comportamento do cliente.
- Facilita a segmentação para campanhas de marketing personalizadas.
- Identifica os clientes que mais geram receita para a empresa.

## ➡️ Endpoints Relacionados

| Método  | Rota                            | Descrição |
|---------|---------------------------------|----------------------------------|
| `GET`   | `/reports/best-customers`      | Retorna a lista dos melhores clientes |
| `GET`   | `/reports/best-customers/{id}` | Detalhes de um cliente específico |

Esses relatórios são essenciais para otimizar estratégias de retenção de clientes e melhorar o relacionamento com o público-alvo.