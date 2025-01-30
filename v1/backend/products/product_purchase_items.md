---
title: 'Product purchase items'
parent: 'Products'
nav_order: 2
---

# Product Purchase Items (Itens de Compras de Produtos)

Tabela que armazena os itens de cada compra de produtos realizada por uma empresa.

## Estrutura da Tabela

| Campo                        | Tipo      | Descrição |
|------------------------------|----------|-----------|
| id (PK)                      | UUID     | Identificador único do item da compra |
| product_purchase_id (FK → product_purchases) | UUID | Relacionamento com a compra associada |
| product_id (FK → products)    | UUID     | Relacionamento com o produto adquirido |
| quantity                      | Integer  | Quantidade do produto comprado |
| unit_price                    | Decimal  | Preço unitário do produto na compra |
| total_price                   | Decimal  | Valor total do item (quantity × unit_price) |
| created_at                    | DateTime | Data de criação |
| updated_at                    | DateTime | Última atualização |

