Projeto: Vendas de Informática
Descrição

Este projeto utiliza o banco de dados vendas_informatica para cadastrar clientes, produtos e registrar vendas utilizando comandos SQL.

1. Cadastro de Cliente

O primeiro comando realiza o cadastro de um cliente na tabela cliente.

Dados cadastrados:

Nome: Rubervaldo Sesiano
E-mail: ruber.sesi@gmail.com
Cidade: Jaguariúna
Estado: São Paulo
Data de cadastro: 28/10/2026
sql
````
USE vendas_informatica;

INSERT INTO cliente(nome_cliente, email, cidade, estado, data_cadastro)
VALUES ("Rubervaldo Sesiano", "ruber.sesi@gmail.com", "Jaguariuna", "São Paulo", "2026-10-28");
````
2. Cadastro de Produto

O segundo comando adiciona um produto à tabela produto.

Dados cadastrados:

Produto: MousePad 5POL
Marca: LUMIX
Preço unitário: R$ 59,98
Estoque: 35 unidades
Ativo: Sim
Data de cadastro: 28/10/2026
sql
````
USE vendas_informatica;

INSERT INTO produto(nome_produto, marca, preco_unitario, estoque, ativo, data_cadastro)
VALUES ("MousePad 5POL", "LUMIX", 59.98, 35, 1, "2026-10-28");
````
3. Registro de Venda

O terceiro comando registra uma venda na tabela venda, relacionando um cliente a um produto.

Dados da venda:

ID do cliente: 101
ID do produto: 21
Data da venda: 28/10/2026
Quantidade: 10 unidades
Valor antes do desconto: R$ 599,80
Desconto: 1,33%
Forma de pagamento: PIX
Status: Concluída
sql
````
USE vendas_informatica;

INSERT INTO venda(id_cliente, id_produto, data_venda, quantidade, preco_unitario_venda, desconto_percentual, forma_pagamento, status_venda)
VALUES (101, 21, "2026-10-28", 10, 599.80, 1.33, "PIX", "Concluida");
````
Objetivo do Projeto

Praticar operações de inserção de dados (INSERT INTO) em um banco de dados relacional, trabalhando com cadastro de clientes, produtos e registro de vendas.

Tecnologias Utilizadas
SQL
MySQL
Observação

Para que o registro da venda funcione corretamente, os IDs 101 e 21 devem corresponder a um cliente e a um produto existentes no banco de dados.
