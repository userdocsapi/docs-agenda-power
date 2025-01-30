---
title: 'User roles'
parent: 'Authentication'
nav_order: 2
---

# User Account Status (Status da Conta do Usuário)

Tabela que armazena informações sobre o status da conta dos usuários.

| Campo                      | Tipo     | Descrição |
|----------------------------|---------|-----------|
| id (PK)                    | UUID    | Identificador único do status |
| company_name               | String  | Nome da empresa do usuário |
| account_type               | Enum    | Tipo de conta (TRIAL, PREMIUM, etc.) |
| trial_expiration_date      | DateTime | Data de expiração do período de teste |
| max_number_users           | Int     | Número máximo de usuários permitidos |
| createdAt                  | DateTime | Data de criação |
| apple_subscription         | Boolean | Indica se tem assinatura Apple |
| android_subscription       | Boolean | Indica se tem assinatura Android |
| paid_grace_period_end_date | DateTime | Data de fim do período de carência |
| subscription_type          | String  | Tipo de assinatura |
| last_paid_at               | DateTime | Última data de pagamento |
| android_product_id         | String  | ID do produto Android |
| can_pay_boleto            | Boolean | Indica se pode pagar via boleto |
| mobile_account            | Boolean | Conta criada no mobile |
| web_account               | Boolean | Conta criada no web |
| paypal                    | Boolean | Integração com PayPal |
| stripe                    | Boolean | Integração com Stripe |
| asaas                     | Boolean | Integração com Asaas |
| boleto                    | Boolean | Opção de boleto disponível |
| premium_activated         | Boolean | Indica se o plano premium foi ativado |
