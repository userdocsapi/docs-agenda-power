---
title: 'Company page bio Instagram'
parent: 'Companies'
nav_order: 2
---

# Company Page Bio Instagram (Instagram do Perfil Público)

Tabela que armazena as contas do Instagram associadas ao perfil público da empresa.

## Estrutura da Tabela

| Campo                     | Tipo      | Descrição |
|---------------------------|----------|-----------|
| id (PK)                   | UUID     | Identificador único do Instagram |
| company_page_bio_id (FK → company_page_bio) | UUID | Relacionamento com o perfil público da empresa |
| instagram_user            | String   | Nome de usuário do Instagram |
| instagram_title (nullable) | String   | Título associado ao Instagram |
| created_at                | DateTime | Data de criação |
| updated_at                | DateTime | Última atualização |
