---
title: 'Anamnese forms'
parent: 'Anamnese'
nav_order: 1
---

# Anamnese Forms (Formulários de Anamnese)

Tabela que armazena os formulários de anamnese utilizados pelas empresas.

## Estrutura da Tabela

| Campo                        | Tipo      | Descrição |
|------------------------------|----------|-----------|
| id (PK)                      | UUID     | Identificador único do formulário |
| company_id (FK → companies)   | UUID     | Relacionamento com a empresa proprietária do formulário |
| name                          | String   | Nome do formulário |
| description (nullable)        | Text     | Descrição do formulário |
| terms (nullable)              | Text     | Termos e condições aplicáveis |
| deleted                       | Boolean  | Indica se o formulário foi excluído |
| deleted_at (nullable)         | DateTime | Data de exclusão lógica |
| deleted_by_id (nullable)      | UUID     | Identificador do usuário que excluiu o formulário |
| created_at                    | DateTime | Data de criação |
| updated_at                    | DateTime | Última atualização |
| created_by_id (FK → users)     | UUID     | Identificador do usuário que criou o formulário |
| updated_by_id (FK → users)     | UUID     | Identificador do usuário que atualizou o formulário |


