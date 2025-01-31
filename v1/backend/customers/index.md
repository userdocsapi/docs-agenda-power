---
title: 'Customers'
parent: 'Backend'
nav_order: 1
---

# Módulo: Customers

O módulo **Customers** gerencia as informações e interações dos clientes dentro do sistema, permitindo um controle eficiente dos dados e histórico de cada usuário.

## ➡️ Funcionalidades Principais

- **Cadastro e Gestão de Clientes**  
  Registro e atualização das informações dos clientes.

- **Histórico de Agendamentos**  
  Visualização de serviços agendados e concluídos pelo cliente.

- **Anotações sobre o Cliente**  
  Adição de observações e informações complementares sobre os clientes.

## ➡️ Estrutura do Módulo

```bash
/customers
│── index.md                   # Página inicial do módulo
│── customer_appointments.md    # Histórico de agendamentos
│── customer_notes.md           # Notas e observações sobre clientes
│── customers.md                # Gerenciamento de clientes
```

## ➡️ Regras de Negócio

- Cada cliente deve ter um e-mail ou telefone cadastrado para contato.
- As informações dos clientes devem ser mantidas em conformidade com a LGPD.
- Clientes podem ter status diferenciados como "ativo", "inativo" ou "bloqueado".

## ➡️ Endpoints Relacionados

| Método  | Rota                          | Descrição |
|---------|-------------------------------|----------------------------------|
| `GET`   | `/customers`                  | Lista todos os clientes |
| `POST`  | `/customers`                  | Cadastra um novo cliente |
| `PUT`   | `/customers/{id}`             | Atualiza os dados de um cliente |
| `DELETE`| `/customers/{id}`             | Remove um cliente |
| `GET`   | `/customers/{id}/appointments`| Retorna o histórico de agendamentos do cliente |
| `POST`  | `/customers/{id}/notes`       | Adiciona uma nota ao cliente |

