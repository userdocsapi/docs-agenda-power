---
title: 'Company page bio'
parent: 'Companies'
nav_order: 2
---

# Company Page Bio (Perfil Público da Empresa)

Tabela que define as informações da página pública da empresa.

| Campo                              | Tipo      | Descrição |
|-----------------------------------|----------|-----------|
| slug                              | String   | Identificador único da página |
| background_color_id (FK) (nullable) | UUID    | Cor de fundo da página |
| border_color_id (FK) (nullable)  | UUID    | Cor da borda da página |
| avatar_url (nullable)             | String   | URL da imagem de avatar |
| name                              | String   | Nome da empresa ou perfil |
| header_text (nullable)            | String   | Texto do cabeçalho da página |
| address (nullable)                | String   | Endereço da empresa |
| locale                            | String   | Localização padrão da página (ex: PT_BR) |
| online_scheduling_available       | Boolean  | Indica se o agendamento online está disponível |
| online_scheduling_slug (nullable) | String   | Slug para a página de agendamento online |
| created_at                        | DateTime | Data de criação |
| updated_at                        | DateTime | Última atualização |


# Company Page Bio Links (Links do Perfil Público)

Tabela que armazena links externos adicionados ao perfil público da empresa.

## Estrutura da Tabela

| Campo                    | Tipo      | Descrição |
|--------------------------|----------|-----------|
| id (PK)                 | UUID     | Identificador único do link |
| company_page_bio_id (FK → company_page_bio) | UUID | Relacionamento com o perfil público da empresa |
| title                   | String   | Título do link (ex: Meu Portfólio, Canal do YouTube) |
| url                     | String   | URL do link externo |
| created_at              | DateTime | Data de criação |
| updated_at              | DateTime | Última atualização |



# WhatsApp Contact Information (Informações de Contato WhatsApp)

Tabela que armazena os números de WhatsApp e mensagens personalizadas.

| Campo                                  | Tipo      | Descrição |
|---------------------------------------|----------|-----------|
| whats_number (nullable)               | String   | Número principal do WhatsApp |
| whats_title (nullable)                 | String   | Título para o WhatsApp principal |
| whats_message (nullable)               | String   | Mensagem personalizada para o WhatsApp principal |
| whats_number_2 (nullable)              | String   | Segundo número do WhatsApp |
| whats_title_2 (nullable)               | String   | Título para o segundo WhatsApp |
| whats_message_2 (nullable)             | String   | Mensagem personalizada para o segundo WhatsApp |
| whats_number_3 (nullable)              | String   | Terceiro número do WhatsApp |
| whats_title_3 (nullable)               | String   | Título para o terceiro WhatsApp |
| whats_message_3 (nullable)             | String   | Mensagem personalizada para o terceiro WhatsApp |
| whats_number_with_country_code (nullable) | String | Número do WhatsApp com código do país |
| whats_number_2_with_country_code (nullable) | String | Segundo número do WhatsApp com código do país |
| whats_number_3_with_country_code (nullable) | String | Terceiro número do WhatsApp com código do país |



# Social Media Links (Links de Redes Sociais)

Tabela que armazena os links e informações das redes sociais da empresa.

| Campo                      | Tipo      | Descrição |
|---------------------------|----------|-----------|
| instagram_user (nullable)  | String   | Nome de usuário do Instagram |
| instagram_title (nullable) | String   | Título do Instagram |
| instagram_user_2 (nullable) | String  | Segundo nome de usuário do Instagram |
| instagram_title_2 (nullable) | String | Segundo título do Instagram |
| external_link_title (nullable) | String | Título do link externo |
| external_link_url (nullable)   | String | URL do link externo |


Este modelo de bio permite que empresas personalizem suas páginas públicas, adicionando contatos, redes sociais e informações institucionais de forma organizada e acessível.
