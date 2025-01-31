---
title: 'Payment methods'
parent: 'Finance'
nav_order: 2
---

# Payment Methods (Métodos de Pagamento)

O módulo Payment Methods gerencia os diferentes métodos de pagamento aceitos pelo sistema, garantindo flexibilidade e segurança nas transações financeiras. Ele permite a configuração de opções como cartão de crédito, boleto bancário, Pix e outras formas de pagamento utilizadas pelos clientes.

| Campo              | Tipo                | Descrição                                        |
| ------------------ | ------------------- | ------------------------------------------------ |
| `id`               | UUID                | Identificador único do método de pagamento     |
| `name`             | String              | Nome do método de pagamento                     |
| `type`             | ENUM                | Tipo de pagamento (cartão, boleto, pix, etc.)    |
| `active`           | Boolean             | Indica se o método de pagamento está ativo      |
| `created_at`       | DateTime            | Data de criação do registro                    |
| `updated_at`       | DateTime            | Data da última atualização                     |
| `deleted_at`       | DateTime (nullable) | Data de exclusão (soft delete)                   |





