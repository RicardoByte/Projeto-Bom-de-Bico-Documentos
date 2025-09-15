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