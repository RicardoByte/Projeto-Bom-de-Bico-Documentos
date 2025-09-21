___

Estes requisitos descrevem **como** o sistema deve operar, definindo seus atributos de qualidade.

#### **Categoria: Segurança**

| Requisito n.º         | RNF-SEG-001                                                                                                      | **Título:** Segurança de Comunicação |                    |
| :-------------------- | :--------------------------------------------------------------------------------------------------------------- | :----------------------------------- | ------------------ |
| **Descrição**         | Toda a comunicação entre o cliente (navegador) e o servidor deve ser criptografada utilizando o protocolo HTTPS. |                                      |                    |
| **Prioridade**        | Essencial                                                                                                        | **Dependências:** N/A                | **Conflitos:** N/A |
| **Material de Apoio** | Certificado SSL/TLS.                                                                                             |                                      |                    |

| Requisito n.º         | RNF-SEG-002                                                                                    | **Título:** Armazenamento Seguro de Senhas |                    |
| :-------------------- | :--------------------------------------------------------------------------------------------- | :----------------------------------------- | ------------------ |
| **Descrição**         | As senhas dos usuários devem ser armazenadas no banco de dados utilizando um algoritmo de hash |                                            |                    |
| **Prioridade**        | Essencial                                                                                      | **Dependências:** N/A                      | **Conflitos:** N/A |
| **Material de Apoio** | Política de Segurança da Informação.                                                           |                                            |                    |

| Requisito n.º | RNF-SEG-003 | **Título:** Mitigação de Riscos de Segurança |
| :--- | :--- | :--- |
| **Descrição** | O sistema deve ser desenvolvido seguindo as recomendações do OWASP Top 10 para mitigar os riscos de segurança mais comuns em aplicações web. |
| **Prioridade** | Essencial | **Dependências:** N/A | **Conflitos:** N/A |
| **Material de Apoio** | Relatórios de ferramentas de análise de vulnerabilidades. |

#### **Categoria: Desempenho** 

| Requisito n.º         | RNF-DES-001                                                                                                                                             | **Título:** Desempenho de Carregamento |                    |
| :-------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------ | :------------------------------------- | ------------------ |
| **Descrição**         | As páginas principais do site (home, busca, produto) devem ter seu conteúdo principal renderizado em menos de 3 segundos em uma conexão de internet 3G. |                                        |                    |
| **Prioridade**        | Alta                                                                                                                                                    | **Dependências:** N/A                  | **Conflitos:** N/A |
| **Material de Apoio** | Relatórios de ferramentas como Google PageSpeed.                                                                                                        |                                        |                    |

#### **Categoria: Usabilidade**

| Requisito n.º         | RNF-USA-001                                                                                                                                  | **Título:** Design Responsivo |                    |
| :-------------------- | :------------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------- | ------------------ |
| **Descrição**         | A interface do sistema deve se adaptar e ser plenamente funcional em diferentes tamanhos de tela, incluindo desktops, tablets e smartphones. |                               |                    |
| **Prioridade**        | Alta                                                                                                                                         | **Dependências:** N/A         | **Conflitos:** N/A |
| **Material de Apoio** | Protótipos para diferentes breakpoints (mobile, desktop).                                                                                    |                               |                    |

#### **Categoria: Confiabilidade e Disponibilidade **

| Requisito n.º | RNF-DIS-001 | **Título:** Disponibilidade do Sistema |
| :--- | :--- | :--- |
| **Descrição** | O sistema deve estar disponível para os usuários 99.8% do tempo, medido mensalmente. |
| **Prioridade** | Alta | **Dependências:** N/A | **Conflitos:** N/A |
| **Material de Apoio** | Relatórios da plataforma de monitoramento (uptime). |

| Requisito n.º | RNF-CON-002 | **Título:** Logs e Monitoramento |
| :--- | :--- | :--- |
| **Descrição** | O sistema deve registrar logs detalhados de eventos críticos e erros da aplicação. Deve haver um painel de monitoramento para acompanhar a saúde do sistema (uso de CPU, memória, etc.). |
| **Prioridade** | Alta | **Dependências:** N/A | **Conflitos:** N/A |
| **Material de Apoio** | N/A |