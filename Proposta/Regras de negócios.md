# **Regras de Negócio (Business Rules)**

Regras de negócio são as políticas e restrições específicas que governam como sua plataforma irá operar. Elas ditam o que pode ou não ser feito. 

## Usuário
- Um usuário deve ter no mínimo 18 anos para se cadastrar.
- Usuários menores de idade devem ter vinculado ao menos o CPF de um responsável legal para realizar compras.
- O e-mail de um usuário deve ser único na plataforma.

## Comprador
- Um comprador tem até 7 dias corridos após o recebimento para abrir uma disputa ou solicitar uma devolução. 

## Vendedor
- Para se tornar um vendedor, o usuário deve fornecer um comprovante CPF ou CNPJ e endereço.
- Um vendedor só pode ter um anúncio ativo por produto idêntico (evitar spam).
- A reputação de um vendedor será calculada com base na média das notas dos últimos 100 pedidos.

## Produtos
- Um produto não pode ser anunciado sem pelo menos uma foto de boa qualidade.
- O preço de um produto deve ser sempre maior que R$ 0,00. 
- Apenas usuários que concluíram a compra de um produto podem deixar uma avaliação sobre ele.

## Plataforma
- A plataforma reterá uma comissão de 10% sobre o valor de cada produto vendido.
- O pagamento só será liberado ao vendedor 7 dias após a confirmação de entrega pelo comprador.
- Comentários ou perguntas com linguagem de cunho ofensivo serão removidos pela moderação.
- É proibido anunciar produtos de categorias restritas (ex: produtos não relacionados aos serviços do marketplace, produtos ilegais).

## ## Logística e Entrega

- O valor do frete será calculado dinamicamente no momento da compra, com base nas tabelas de preços fornecidas pelas transportadoras parceiras, considerando o CEP de origem (vendedor), CEP de destino (comprador), dimensões e peso do produto.
- O vendedor deve utilizar exclusivamente a etiqueta de envio gerada e pré-paga pela plataforma para garantir o rastreamento e a segurança da transação.
- O repasse dos valores de frete para as transportadoras parceiras será realizado em ciclos de faturamento mensais, após a conciliação das entregas efetivamente postadas.
- Quando um cupom de frete grátis for oferecido pela **plataforma** (como ação de marketing), o custo do envio será integralmente subsidiado pela plataforma, não sendo descontado do repasse do vendedor.
- Vendedores que possuem uma estrutura de logística própria podem solicitar o uso deste modelo (etiqueta pré-paga). A aprovação dependerá de uma análise da capacidade operacional do vendedor.
- O vendedor é responsável por cadastrar e manter atualizada sua própria tabela de fretes na plataforma, definindo os custos, prazos e áreas de cobertura (por exemplo, por faixa de CEP, bairro ou cidade). O valor do frete calculado por esta tabela será o cobrado do comprador.
- Uma vez que a plataforma não tem rastreamento automático, o vendedor é obrigado a atualizar manualmente (ou via integração) o status do pedido na plataforma em cada etapa chave, no mínimo: `Em preparação`, `Saiu para entrega` e `Entregue`.
- A entrega será considerada oficialmente concluída somente após a **confirmação de recebimento pelo comprador** dentro da plataforma. O prazo de liberação do pagamento ao vendedor (definido nas regras da Plataforma) começará a contar a partir desta confirmação.
- Toda a responsabilidade pela operação de entrega — incluindo o cumprimento de prazos, a integridade do produto durante o transporte, a comunicação com o cliente e eventuais extravios — é **exclusivamente do vendedor**. Falhas nesta operação impactarão diretamente a reputação do vendedor e estarão sujeitas à mediação de disputas pela plataforma.