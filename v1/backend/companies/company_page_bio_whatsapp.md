---
title: 'Company page bio WhatsApp'
parent: 'Companies'
nav_order: 2
---

# Company Page Bio WhatsApp (WhatsApp do Perfil Público)

Tabela que armazena os números de WhatsApp vinculados ao perfil público da empresa.

## Estrutura da Tabela

| Campo                               | Tipo      | Descrição |
|-------------------------------------|----------|-----------|
| id (PK)                            | UUID     | Identificador único do número de WhatsApp |
| company_page_bio_id (FK → company_page_bio) | UUID | Relacionamento com o perfil público da empresa |
| whatsapp_number                     | String   | Número do WhatsApp sem código de país |
| whatsapp_number_with_country_code    | String   | Número do WhatsApp com código do país |
| whatsapp_title (nullable)            | String   | Título associado ao número de WhatsApp |
| whatsapp_message (nullable)          | String   | Mensagem personalizada para o WhatsApp |
| created_at                           | DateTime | Data de criação |
| updated_at                           | DateTime | Última atualização |
