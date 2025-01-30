---
title: 'Accounts receivables'
parent: 'Finance'
nav_order: 2
---

# Accounts Receivable Items (Itens das Contas a Receber)

Tabela que armazena os serviços ou pacotes adquiridos em uma conta a receber.

| Campo                      | Tipo      | Descrição |
|----------------------------|----------|-----------|
| id (PK)                   | UUID     | Identificador único |
| accounts_receivable_id (FK) | UUID    | Relacionamento com a conta a receber |
| service_id (FK)           | UUID     | Relacionamento com um serviço |
| service_package_id (FK)   | UUID     | Relacionamento com um pacote de serviços |
| quantity                  | Int      | Quantidade do serviço/pacote adquirido |
| price                     | Float    | Preço unitário do serviço/pacote |
| created_by_id (FK)        | UUID     | ID do usuário que criou o registro |
| updated_by_id (FK)        | UUID     | ID do usuário que atualizou o registro |
| created_at                | DateTime | Data de criação do registro |
| updated_at                | DateTime | Data de atualização do registro |
| deleted_at                | DateTime | Data de exclusão lógica (soft delete) |
