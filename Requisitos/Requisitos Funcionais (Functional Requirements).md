___
Estes requisitos descrevem o **que** o sistema deve fazer.

#### **Módulo: Usuários e Autenticação**

| Requisito n.º         | RF-USR-001                                                                                              | **Título:** Cadastro de Comprador |                    |
| :-------------------- | :------------------------------------------------------------------------------------------------------ | :-------------------------------- | ------------------ |
| **Descrição**         | O sistema deve permitir que novos usuários se cadastrem na plataforma utilizando um e-mail e uma senha. |                                   |                    |
| **Prioridade**        | Essencial                                                                                               | **Dependências:** N/A             | **Conflitos:** N/A |
| **Material de Apoio** | Protótipo da tela de cadastro.                                                                          |                                   |                    |

| Requisito n.º | RF-USR-002 | **Título:** Login de Usuário |
| :--- | :--- | :--- |
| **Descrição** | O sistema deve permitir que um usuário cadastrado acesse sua conta utilizando e-mail e senha. |
| **Prioridade** | Essencial | **Dependências:** RF-USR-001 | **Conflitos:** N/A |
| **Material de Apoio** | Protótipo da tela de login. |

| Requisito n.º | RF-USR-003 | **Título:** Histórico e Acompanhamento de Pedidos |
| :--- | :--- | :--- |
| **Descrição** | O usuário deve poder visualizar seu histórico de pedidos. Ao clicar em um pedido, deve ver os detalhes, status do pagamento e, se enviado, o código de rastreio e o status da entrega. |
| **Prioridade** | Alta | **Dependências:** RF-CHK-002 | **Conflitos:** N/A |
| **Material de Apoio** | Protótipo da tela "Meus Pedidos". |

| Requisito n.º | RF-USR-004 | **Título:** Recuperação de Senha ** (NOVO) ** |
| :--- | :--- | :--- |
| **Descrição** | O sistema deve permitir que um usuário que esqueceu sua senha possa solicitar a redefinição através de um link seguro enviado para seu e-mail de cadastro. |
| **Prioridade** | Essencial | **Dependências:** RF-USR-001 | **Conflitos:** N/A |
| **Material de Apoio** | Fluxograma de recuperação de senha. |

| Requisito n.º | RF-USR-005 | **Título:** Gerenciamento de Perfil de Usuário ** (NOVO) ** |
| :--- | :--- | :--- |
| **Descrição** | O usuário deve possuir uma área de perfil onde possa visualizar e editar seus dados pessoais (nome, e-mail, senha) e gerenciar seus endereços de entrega. |
| **Prioridade** | Alta | **Dependências:** RF-USR-001 | **Conflitos:** N/A |
| **Material de Apoio** | Protótipo da tela de perfil. |

#### **Módulo: Produtos e Busca**

| Requisito n.º | RF-PRD-001 | **Título:** Busca de Produtos |
| :--- | :--- | :--- |
| **Descrição** | O sistema deve prover um campo de busca textual para que usuários encontrem produtos. |
| **Prioridade** | Essencial | **Dependências:** RF-VND-002 | **Conflitos:** N/A |
| **Material de Apoio** | N/A |

| Requisito n.º | RF-PRD-002 | **Título:** Filtro e Ordenação de Resultados |
| :--- | :--- | :--- |
| **Descrição** | Na página de resultados da busca, o sistema deve permitir filtrar (por categoria, faixa de preço, etc.) e ordenar (por relevância, preço, mais recentes) os produtos. |
| **Prioridade** | Alta | **Dependências:** RF-PRD-001, RF-ADM-003 | **Conflitos:** N/A |
| **Material de Apoio** | Protótipo da página de busca. |

#### **Módulo: Checkout e Pagamento**

| Requisito n.º | RF-CHK-001 | **Título:** Carrinho de Compras |
| :--- | :--- | :--- |
| **Descrição** | O sistema deve permitir que o usuário adicione e remova produtos de um carrinho de compras virtual. |
| **Prioridade** | Essencial | **Dependências:** N/A | **Conflitos:** N/A |
| **Material de Apoio** | Fluxograma do carrinho. |

| Requisito n.º | RF-CHK-002 | **Título:** Processamento de Pagamento |
| :--- | :--- | :--- |
| **Descrição** | O sistema deve permitir ao comprador realizar o pagamento via Cartão de Crédito, Débito, PIX e Boleto. O sistema deve processar a transação e atualizar o status do pedido. |
| **Prioridade** | Essencial | **Dependências:** RF-CHK-001 | **Conflitos:** N/A |
| **Material de Apoio** | Diagrama de sequência do pagamento. |

| Requisito n.º | RF-CHK-003 | **Título:** Expiração de QR Code PIX |
| :--- | :--- | :--- |
| **Descrição** | Ao selecionar PIX como método de pagamento, o QR Code gerado deve ter um tempo de expiração definido (ex: 5 minutos). |
| **Prioridade** | Essencial | **Dependências:** RF-CHK-002 | **Conflitos:** N/A |
| **Material de Apoio** | Regra de negócio do gateway de pagamento. |

| Requisito n.º | RF-CHK-004 | **Título:** Cancelamento por Não Pagamento (PIX) |
| :--- | :--- | :--- |
| **Descrição** | Se um pagamento via PIX não for confirmado dentro do tempo de expiração do QR Code, o pedido deve ser automaticamente cancelado e o estoque liberado. |
| **Prioridade** | Essencial | **Dependências:** RF-CHK-003, RF-VND-003 | **Conflitos:** N/A |
| **Material de Apoio** | N/A |

#### **Módulo: Vendedor**

| Requisito n.º | RF-VND-001 | **Título:** Cadastro de Vendedor |
| :--- | :--- | :--- |
| **Descrição** | Um usuário comprador deve poder realizar um cadastro complementar para se tornar um vendedor, informando dados adicionais (CPF/CNPJ, endereço, etc.). |
| **Prioridade** | Essencial | **Dependências:** RF-USR-001 | **Conflitos:** N/A |
| **Material de Apoio** | Protótipo do fluxo de cadastro de vendedor. |

| Requisito n.º | RF-VND-002 | **Título:** Gerenciamento de Anúncios |
| :--- | :--- | :--- |
| **Descrição** | O vendedor deve poder criar, visualizar, editar e excluir anúncios de seus produtos. |
| **Prioridade** | Essencial | **Dependências:** RF-VND-001 | **Conflitos:** N/A |
| **Material de Apoio** | Protótipo da tela de gerenciamento de produtos. |

| Requisito n.º | RF-VND-003 | **Título:** Gerenciamento de Estoque |
| :--- | :--- | :--- |
| **Descrição** | O vendedor deve poder definir e atualizar a quantidade em estoque de seus produtos. O estoque deve ser debitado automaticamente após a confirmação de uma venda. |
| **Prioridade** | Essencial | **Dependências:** RF-VND-002 | **Conflitos:** N/A |
| **Material de Apoio** | N/A |

| Requisito n.º | RF-VND-004 | **Título:** Gestão Financeira do Vendedor ** (NOVO) ** |
| :--- | :--- | :--- |
| **Descrição** | O vendedor deve ter um painel financeiro exibindo o saldo de suas vendas, as comissões da plataforma, e o histórico de repasses. O sistema deve permitir que ele solicite o saque dos valores disponíveis para sua conta bancária. |
| **Prioridade** | Essencial | **Dependências:** RF-CHK-002, RF-ADM-004 | **Conflitos:** N/A |
| **Material de Apoio** | Protótipo do painel financeiro. |

#### **Módulo: Administrador**

| Requisito n.º | RF-ADM-001 | **Título:** Gerenciamento de Usuários |
| :--- | :--- | :--- |
| **Descrição** | O administrador deve poder visualizar, buscar, bloquear e desbloquear usuários (compradores e vendedores) na plataforma. |
| **Prioridade** | Essencial | **Dependências:** N/A | **Conflitos:** N/A |
| **Material de Apoio** | Protótipo do painel de administração. |

| Requisito n.º | RF-ADM-002 | **Título:** Moderação de Conteúdo |
| :--- | :--- | :--- |
| **Descrição** | O administrador deve poder aprovar/reprovar novos anúncios e moderar avaliações e perguntas de usuários que violem os termos de uso. |
| **Prioridade** | Alta | **Dependências:** N/A | **Conflitos:** N/A |
| **Material de Apoio** | N/A |

| Requisito n.º | RF-ADM-003 | **Título:** Gerenciamento de Categorias ** (NOVO) ** |
| :--- | :--- | :--- |
| **Descrição** | O administrador deve ter uma interface para criar, editar, reordenar e excluir as categorias de produtos do site. |
| **Prioridade** | Alta | **Dependências:** N/A | **Conflitos:** N/A |
| **Material de Apoio** | N/A |

| Requisito n.º | RF-ADM-004 | **Título:** Configurações da Plataforma ** (NOVO) ** |
| :--- | :--- | :--- |
| **Descrição** | O administrador deve poder gerenciar configurações gerais do sistema, como o valor da comissão padrão, textos de e-mails transacionais e integrações com serviços de terceiros. |
| **Prioridade** | Alta | **Dependências:** N/A | **Conflitos:** N/A |
| **Material de Apoio** | N/A |

---