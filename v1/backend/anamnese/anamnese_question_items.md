# Anamnese Question Items (Opções de Perguntas da Anamnese)

Tabela que armazena as opções de resposta associadas às perguntas dos formulários de anamnese.

## Estrutura da Tabela

| Campo                        | Tipo      | Descrição |
|------------------------------|----------|-----------|
| id (PK)                      | UUID     | Identificador único da opção de resposta |
| anamnese_question_id (FK → anamnese_questions) | UUID | Relacionamento com a pergunta da anamnese |
| label                        | String   | Texto da opção de resposta |
| deleted                       | Boolean  | Indica se a opção foi excluída |
| deleted_at (nullable)         | DateTime | Data de exclusão lógica |
| deleted_by_id (nullable)      | UUID     | Identificador do usuário que excluiu a opção |
| created_at                    | DateTime | Data de criação |
| updated_at                    | DateTime | Última atualização |
| created_by_id (FK → users)     | UUID     | Identificador do usuário que criou a opção |
| updated_by_id (FK → users)     | UUID     | Identificador do usuário que atualizou a opção |
