# Modelagem inicial de dados — Doce Encanto

## 1. Objetivo

Descrever as principais informações que o aplicativo precisa representar para permitir a consulta de produtos e a montagem de pedidos.

## 2. Entidades previstas

### Produto
- id_produto: identificador único.
- nome: nome do cupcake.
- descricao: descrição do produto.
- preco: preço unitário.
- imagem: referência da imagem ilustrativa.
- disponivel: indica se o produto está disponível no catálogo.

### Cliente
- id_cliente: identificador único.
- nome: nome informado pelo cliente.
- telefone: telefone para contato.

### Pedido
- id_pedido: identificador único.
- id_cliente: referência ao cliente.
- data_pedido: data e hora do pedido, se suportadas pela plataforma.
- endereco_entrega: endereço informado.
- forma_pagamento: opção selecionada.
- valor_total: total do pedido.
- status: situação demonstrativa do pedido.

### ItemPedido
- id_item: identificador único.
- id_pedido: referência ao pedido.
- id_produto: referência ao produto.
- quantidade: quantidade escolhida.
- preco_unitario: preço do produto no momento do pedido.
- subtotal: quantidade multiplicada pelo preço unitário.

## 3. Relacionamentos

- Um cliente pode realizar vários pedidos.
- Um pedido pertence a um cliente.
- Um pedido possui um ou mais itens.
- Cada item de pedido referencia um produto.
- Um produto pode aparecer em vários itens de pedidos diferentes.

## 4. Regras de integridade previstas

- Todo produto deve possuir identificador, nome e preço válido.
- A quantidade de cada item deve ser maior que zero.
- O pedido deve possuir ao menos um item.
- O valor total deve corresponder à soma dos subtotais.
- Os dados de demonstração devem ser fictícios.

## 5. Situação

Esta é a modelagem lógica inicial. O modelo físico, os tipos de dados, as chaves e as restrições serão ajustados conforme o SGBD ou o recurso de dados da plataforma escolhida. Não há banco de dados implementado neste momento.
