---
title: 'Products'
parent: 'Products'
nav_order: 2
---

# Products (Produtos)

Tabela que armazena os produtos vendidos ou utilizados no sistema.

| Campo                | Tipo     | Descrição |
|----------------------|---------|-----------|
| id (PK)             | UUID    | Identificador único do produto |
| company_id (FK)     | UUID    | Identificador da empresa |
| created_by_id (FK)  | UUID    | Usuário que criou o produto |
| updated_by_id (FK)  | UUID    | Usuário que fez a última atualização |
| name               | String  | Nome do produto |
| sale_price         | Float   | Preço de venda do produto |
| product_category_id (FK) | UUID | Categoria do produto |
| desired_stock_amount | Int  | Quantidade desejada em estoque |
| image_url          | String  | URL da imagem do produto (opcional) |
| deleted            | Boolean | Indica se o produto foi excluído (soft delete) |
| deleted_at         | DateTime | Data de exclusão lógica (opcional) |
| created_at         | DateTime | Data de criação |
| updated_at         | DateTime | Última atualização |