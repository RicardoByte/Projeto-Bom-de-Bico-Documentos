# **Regras de Negócio (Business Rules)**

## Usuário
- **RN-USR-01:** O e-mail de um usuário deve ser único e sua posse deve ser verificada através de um link de confirmação enviado após o cadastro.
- **RN-USR-02:** O usuário deve declarar ter no mínimo 18 anos no momento do cadastro para utilizar a plataforma.

## Comprador
- **RN-CPR-01:** Um comprador tem até 7 dias corridos após o recebimento para abrir uma disputa ou solicitar uma devolução.

## Vendedor
- **RN-VND-01:** Para se tornar um vendedor, o usuário deve fornecer documentos válidos, como Cartão CNPJ e um comprovante de endereço recente (ex: conta de consumo dos últimos 3 meses).
- **RN-VND-02:** Um vendedor só pode ter um anúncio ativo por produto (evitar spam).
- **RN-VND-03:** A reputação de um vendedor será calculada com base na média das avaliações recebidas. Para vendedores novos, a reputação será exibida como "Vendedor Novo".

## Produtos
- **RN-PRD-01:** Um produto não pode ser anunciado sem pelo menos uma foto com resolução mínima (ex: 800x800 pixels), nítida e que represente fielmente o item.
- **RN-PRD-02:** O preço de um produto deve ser sempre maior que R$ 0,00.
- **RN-PRD-03:** Apenas usuários que concluíram a compra de um produto podem deixar uma avaliação sobre ele.

## Pedidos
- **RN-PED-01:** Um pedido só é considerado "confirmado" e notificado ao vendedor após a aprovação do pagamento.
- **RN-PED-02:** O vendedor tem um prazo de 3 dias úteis para postar o produto após a confirmação do pedido.
- **RN-PED-03:** Caso o vendedor não cumpra o prazo de postagem, o pedido será automaticamente cancelado e o comprador, integralmente reembolsado.

## Plataforma
- **RN-PLT-01:** A plataforma reterá uma comissão de 10% sobre o valor de cada produto vendido.
- **RN-PLT-02:** O pagamento só será liberado ao vendedor 7 dias após a confirmação de entrega pelo comprador.
- **RN-PLT-03:** Comentários ou perguntas com linguagem de cunho ofensivo serão removidos pela moderação.
- **RN-PLT-04:** A plataforma manterá uma lista explícita e pública de categorias e produtos proibidos em seus "Termos de Uso".

## Logística e Entrega

#### Modelo 1: Logística Integrada (Etiqueta gerada pela Plataforma)
- **RN-LOG-01A:** O valor do frete será calculado dinamicamente com base nas tabelas das transportadoras parceiras, considerando CEP de origem, destino, dimensões e peso do produto.
- **RN-LOG-02A:** O vendedor deve utilizar exclusivamente a etiqueta de envio gerada e pré-paga pela plataforma para garantir o rastreamento automático e a segurança da transação.
- **RN-LOG-03A:** Quando um cupom de frete grátis for oferecido pela plataforma, o custo do envio será integralmente subsidiado por ela.

#### Modelo 2: Logística Própria (Gerenciada pelo Vendedor)
- **RN-LOG-01B:** Vendedores com estrutura própria podem solicitar o uso deste modelo, sujeito à aprovação pela plataforma.
- **RN-LOG-02B:** O vendedor é responsável por cadastrar e manter sua própria tabela de fretes na plataforma, definindo custos, prazos e áreas de cobertura.
- **RN-LOG-03B:** O vendedor é obrigado a atualizar manualmente o status do pedido em cada etapa chave (`Em preparação`, `Saiu para entrega`, `Entregue`).
- **RN-LOG-04B:** A entrega será considerada concluída somente após a confirmação de recebimento pelo comprador na plataforma, para fins de liberação de pagamento.
- **RN-LOG-05B:** A responsabilidade pela operação de entrega é exclusivamente do vendedor, e falhas impactarão sua reputação.