---
title: 'Anamnese answers details'
parent: 'Anamnese'
nav_order: 1
---

# Anamnese Answers Details (Detalhes das Respostas da Anamnese)

Tabela que armazena detalhes das respostas fornecidas pelos clientes aos formulários de anamnese.

## Estrutura da Tabela

| Campo                        | Tipo      | Descrição |
|------------------------------|----------|-----------|
| id (PK)                      | UUID     | Identificador único do detalhe da resposta |
| anamnese_answer_id (FK → anamnese_answers) | UUID | Relacionamento com a resposta da anamnese |
| anamnese_question_id (FK → anamnese_questions) | UUID | Relacionamento com a pergunta respondida |
| boolean_answer (nullable)     | Boolean  | Resposta booleana (sim/não) |
| text_answer (nullable)        | String   | Resposta em formato de texto |
| anamnese_question_item_ids (nullable) | Array[UUID] | Lista de IDs das opções escolhidas (para múltipla escolha) |
| created_at                    | DateTime | Data de criação |
| updated_at                    | DateTime | Última atualização |
| created_by_id (FK → users)     | UUID     | Identificador do usuário que criou o detalhe da resposta |
| updated_by_id (FK → users)     | UUID     | Identificador do usuário que atualizou o detalhe da resposta |

