---
title: 'Anamnese answers'
parent: 'Anamnese'
nav_order: 2
---

# Anamnese Answers (Respostas da Anamnese)

Tabela que armazena as respostas dos clientes aos formulários de anamnese.

## Estrutura da Tabela

| Campo                        | Tipo      | Descrição |
|------------------------------|----------|-----------|
| id (PK)                      | UUID     | Identificador único da resposta |
| anamnese_form_id (FK → anamnese_forms) | UUID | Relacionamento com o formulário de anamnese |
| company_id (FK → companies)   | UUID     | Relacionamento com a empresa |
| customer_id (FK → customers)  | UUID     | Relacionamento com o cliente |
| date                          | Date     | Data da resposta |
| comments (nullable)           | Text     | Comentários adicionais |
| signed_at (nullable)          | DateTime | Data de assinatura do formulário |
| signed_local_file_path (nullable) | String | Caminho do arquivo de assinatura no dispositivo |
| signed_device_info (nullable) | String   | Informações do dispositivo usado para assinatura |
| signed_device_model (nullable) | String  | Modelo do dispositivo usado para assinatura |
| signed_platform (nullable)    | String   | Plataforma do dispositivo (ex: iOS, Android) |
| created_at                    | DateTime | Data de criação |
| updated_at                    | DateTime | Última atualização |
| created_by_id (FK → users)     | UUID     | Identificador do usuário que criou a resposta |
| updated_by_id (FK → users)     | UUID     | Identificador do usuário que atualizou a resposta |


