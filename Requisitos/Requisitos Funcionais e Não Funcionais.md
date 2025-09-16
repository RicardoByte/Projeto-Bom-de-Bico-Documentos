___
### **Requisitos Funcionais (Functional Requirements)**

- O sistema deve permitir que usuários se cadastrem usando e-mail e senha.
    
- O sistema deve permitir o login com e-mail e senha.
    
- O sistema deve permitir a busca de produtos por texto.
    
- O sistema deve permitir filtrar e ordenar os resultados da busca (por preço, relevância, etc.).
    
- O sistema deve exibir uma página de detalhes para cada produto.
    
- O sistema deve permitir que o comprador adicione e remova itens de um carrinho de compras.
    
- O sistema deve permitir ao comprador selecionar um endereço de entrega.
    
- O sistema deve permitir que o comprador realize o pagamento via Cartão de Crédito, Debito, PIX e Boleto.
    
- O sistema deve permitir ao comprador visualizar seu histórico de pedidos.
    
- O sistema deve permitir que o comprador deixe uma avaliação em um pedido concluído.
    
- O sistema deve permitir que um usuário se torne um vendedor através de um cadastro complementar.
    
- O sistema deve permitir ao vendedor criar, editar e excluir anúncios de produtos.
    
- O sistema deve permitir ao vendedor gerenciar o estoque de seus produtos.
    
- O sistema deve exibir um painel (dashboard) com o histórico de vendas.
    
- O sistema deve notificar o vendedor sobre novas vendas.
    
- O sistema deve permitir ao vendedor informar o código de rastreio de um envio.
    
- O sistema deve permitir ao vendedor responder às perguntas dos compradores em seus anúncios.
    
- O sistema deve permitir ao administrador visualizar e gerenciar todos os usuários.
    
- O sistema deve permitir ao administrador aprovar ou reprovar novos anúncios.
    
- O sistema deve permitir ao administrador moderar avaliações e perguntas.
    
- O sistema deve permitir ao administrador mediar disputas entre compradores e vendedores.
    
- O sistema deve gerar relatórios de vendas e comissões da plataforma.



---
### **Requisitos Não Funcionais (Non-Functional Requirements)**

- As páginas do site devem carregar em menos de 3 segundos.
    
- O resultado de uma busca deve ser retornado em menos de 1 segundo.
    
- O sistema deve suportar 10.000 usuários simultâneos sem degradação de performance.
    
- O sistema deve usar criptografia HTTPS em todas as comunicações.
    
- As senhas dos usuários devem ser armazenadas utilizando um algoritmo de hash seguro (ex: Argon2, bcrypt).
    
- O sistema deve ser protegido contra ataques comuns (SQL Injection, Cross-Site Scripting - XSS, Ataques DDos).
    
- O sistema deve estar em conformidade com a Lei Geral de Proteção de Dados (LGPD).
    
- A interface deve ser intuitiva e fácil de usar para pessoas com pouca experiência em tecnologia.
    
- O design do site deve ser responsivo, adaptando-se a desktops, tablets e smartphones.
    
- O processo de checkout deve ser concluído em, no máximo, 5 passos.
     
- O sistema deve ter uma disponibilidade (uptime) de 99.8% do tempo.
    
- Backups diários do banco de dados devem ser realizados automaticamente.
    
- A arquitetura do sistema deve permitir o aumento da capacidade (de processamento e armazenamento) para acompanhar o crescimento do número de usuários e produtos.