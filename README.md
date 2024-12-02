# Projeto-ecommerce
O projeto seguinte visou o refinamento do modelo lógico de vendas e-commerce, conforme desafio proposto pelo BootCamp da DIO.
O processo de modelagem conceitual do projeto levou em consideração o cenário de vendas e-commerce, cujo as entidades inicialmente selecionadas para modelagem foram: produto, cliente, pedido, estoque e fornecedor. Foi desenvolvido o relacionamento entre cada entidade durante o projeto conceitual, até a execução do projeto lógico no MySQL Workbench. 
# Requisitos:
- Os produtos são vendidos por uma única plataforma online que loja possui atendentes para contato com cliente. Cada produto possui um ou mais fornecedor.
- O cliente pode se cadastrar no site a partir de contas com CPF ou CNPJ. O endereço do cliente determinará o valor do frete; Um cliente pode fazer mais de um pedido.
- Os pedidos são criados por clientes e possuem o id do cliente, bem como id do endereço, além da descrição dos produtos contidos, status da entrega, valor e frete. Um ou mais produtos podem compor o pedido; Um pedido pode ser cancelado; 
Para as demais entidades os requisitos foram sendo criados conforme as relações se desenvolviam.
# Resultados:
- Criei outras entidades para devido refinamento do modelo, sendo estas: Conta, Pagamento e Entrega. 
- A entidade Conta foi criada para atender clientes que possuem mais de uma conta, sendo elas de razão social CPF ou CPNPJ. Um cliente pode ter duas contas na mesma loja. A mesma entidade possui relacionamento de herança com a entidade cliente pelo modelo EER.
- A entidade Pagamento foi criada para se relacionar com a entidade Conta, para as contas de clientes que possuem mais de uma forma de pagamento, contendo os dados bancários dos mesmos caso estes solicitem por extorno do pedido. 
- A entidade Entrega se relaciona diretamente com Pedido, exibinxo o status e código de rastreio. Contudo, me mantenho em dúvida se a criação da entidade foi mesmo necessária e se a mesm não poderia ter sido feita como atributo em Pedido.
