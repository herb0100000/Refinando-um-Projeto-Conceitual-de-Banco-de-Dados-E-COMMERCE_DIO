
# Refinando-um-Projeto-Conceitual-de-Banco-de-Dados-E-COMMERCE_DIO

## 🎯 Descrição
Este projeto foi desenvolvido como parte prática do curso **Randstad - Análise de Dados**, utilizando o MySQL Workbench para construir o modelo de um sistema de e-commerce.

O objetivo foi representar de forma estruturada os principais processos de um ambiente de vendas online, incluindo cadastro de clientes, pedidos, pagamentos e entregas.

## 🧩 Estrutura Geral do Modelo
O modelo contempla as seguintes entidades principais:

* Cliente

* Pedido

* Pagamento

* Entrega

* Produto

* Item do Pedido

## 🛠️ Refinamentos Implementados
Durante o desafio prático, foram realizados os seguintes refinamentos no modelo:

#### ✅ Cliente PF e PJ
Uma conta pode ser do tipo Pessoa Física ou Pessoa Jurídica, mas não ambas ao mesmo tempo.

A modelagem foi feita usando especialização (herança), garantindo exclusividade entre os dois tipos de cliente.

#### ✅ Pagamento com múltiplas formas
Um pedido pode ter mais de uma forma de pagamento associada.

Cada forma de pagamento (Cartão, Boleto, Pix, etc.) possui atributos próprios, organizados por especialização.

A tabela base Pagamento centraliza os dados.

#### ✅ Entrega com status e rastreio
A entrega contém os atributos:

* status 

* codigo_rastreio

Isso permite acompanhar o progresso logístico do pedido.

