---
title: 'Product sale items'
parent: 'Products'
nav_order: 2
---

# Product Sale Items (Itens Vendidos)

Tabela que armazena os itens vendidos em cada venda de produtos.

| Campo               | Tipo     | Descrição |
|--------------------|---------|-----------|
| id (PK)          | UUID    | Identificador único do item vendido |
| product_sale_id (FK) | UUID  | Identificador da venda à qual o item pertence |
| product_id (FK)   | UUID    | Identificador do produto vendido |
| quantity        | Int     | Quantidade vendida |
| value          | Float   | Valor unitário do produto na venda |
| created_at     | DateTime | Data de criação |
