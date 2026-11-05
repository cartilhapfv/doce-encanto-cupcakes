# Modelagem inicial de dados — Doce Encanto

## 1. Objetivo

Registrar uma proposta inicial das informações que o aplicativo precisa organizar para atender ao escopo descrito no PIT I: vitrine virtual, pedidos eletrônicos, pagamentos e entregas.

## 2. Entidades propostas

### Produto
- **id_produto:** identificador do produto.
- **nome:** nome do cupcake.
- **descricao:** descrição do produto.
- **preco:** preço do produto.
- **imagem:** referência da imagem de apresentação.
- **disponivel:** indica se o produto está disponível.

### Cliente
- **id_cliente:** identificador do cliente.
- **nome:** nome do cliente.
- **telefone:** contato do cliente.

### Pedido
- **id_pedido:** identificador do pedido.
- **id_cliente:** cliente relacionado ao pedido.
- **data_pedido:** data do pedido.
- **endereco_entrega:** informação necessária para entrega.
- **forma_pagamento:** forma de pagamento informada.
- **valor_total:** valor total do pedido.

### ItemPedido
- **id_item:** identificador do item.
- **id_pedido:** pedido ao qual o item pertence.
- **id_produto:** produto selecionado.
- **quantidade:** quantidade solicitada.
- **preco_unitario:** preço do produto considerado no pedido.
- **subtotal:** resultado da quantidade multiplicada pelo preço unitário.

## 3. Relacionamentos propostos

- Um cliente pode realizar vários pedidos.
- Cada pedido está relacionado a um cliente.
- Um pedido possui um ou mais itens.
- Cada item de pedido referencia um produto.
- Um produto pode estar presente em vários pedidos.

## 4. Regras de integridade propostas

- Cada produto deve possuir identificador, nome e preço.
- Cada pedido deve estar relacionado a um cliente.
- Cada item deve estar relacionado a um pedido e a um produto.
- A quantidade solicitada deve ser maior que zero.
- O valor total do pedido deve corresponder à soma dos subtotais dos itens.

## 5. Situação e limites

Este documento registra uma proposta conceitual inicial para orientar a organização dos dados. 

