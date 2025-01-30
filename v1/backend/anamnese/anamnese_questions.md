---
title: 'Anamnese questions'
parent: 'Anamnese'
nav_order: 2
---

# Anamnese Questions (Perguntas da Anamnese)

Tabela que armazena as perguntas associadas aos formulários de anamnese.

## Estrutura da Tabela

| Campo                        | Tipo      | Descrição |
|------------------------------|----------|-----------|
| id (PK)                      | UUID     | Identificador único da pergunta |
| anamnese_form_id (FK → anamnese_forms) | UUID | Relacionamento com o formulário de anamnese |
| title                         | String   | Texto da pergunta |
| section_title (nullable)      | String   | Título da seção (caso aplicável) |
| question_type                 | ENUM     | Tipo de pergunta (BOOLEAN, TEXT, MULTIPLE_CHOICE) |
| boolean_with_details (nullable) | Boolean  | Indica se a pergunta booleana permite detalhes adicionais |
| required                      | Boolean  | Indica se a resposta é obrigatória |
| other_item_id (nullable, FK → anamnese_question_items) | UUID | Identificador do item "Outro" se aplicável |
| section                       | Boolean  | Indica se a pergunta representa uma seção no formulário |
| deleted                       | Boolean  | Indica se a pergunta foi excluída |
| deleted_at (nullable)         | DateTime | Data de exclusão lógica |
| deleted_by_id (nullable)      | UUID     | Identificador do usuário que excluiu a pergunta |
| created_at                    | DateTime | Data de criação |
| updated_at                    | DateTime | Última atualização |
| created_by_id (FK → users)     | UUID     | Identificador do usuário que criou a pergunta |
| updated_by_id (FK → users)     | UUID     | Identificador do usuário que atualizou a pergunta |

