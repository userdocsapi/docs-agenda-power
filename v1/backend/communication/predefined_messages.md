---
title: 'Predefined messages'
parent: 'Communication'
nav_order: 2
---

# Predefined Messages (Mensagens Predefinidas)

Tabela que armazena mensagens padrão cadastradas pelos usuários.

| Campo                     | Tipo      | Descrição |
|---------------------------|----------|-----------|
| id (PK)                  | UUID     | Identificador único |
| company_id (FK)          | UUID     | Relacionamento com a empresa |
| user_id (FK)            | UUID     | Relacionamento com o usuário que cadastrou a mensagem |
| name                     | String   | Nome da mensagem |
| text                     | Text     | Conteúdo da mensagem |
| deleted                  | Boolean  | Indica se a mensagem foi excluída |
| deleted_at (nullable)    | DateTime | Data de exclusão lógica (soft delete) |
| deleted_by_id (FK)       | UUID     | ID do usuário que excluiu a mensagem |
| created_by_id (FK)       | UUID     | ID do usuário que criou a mensagem |
| created_at               | DateTime | Data de criação do registro |
| updated_by_id (FK)       | UUID     | ID do usuário que atualizou a mensagem |
| updated_at               | DateTime | Data de atualização do registro |

