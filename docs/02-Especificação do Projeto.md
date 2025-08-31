# Especificações do Projeto

## Personas

**Persona 1 – Mariana Oliveira (Confeiteira Autônoma Iniciante)**
- **Idade:** 23 anos
- **Profissão:** Estudante de gastronomia 
- **Contexto:** Mariana começou a vender doces durante a faculdade para complementar a renda. Trabalha de casa, recebe encomendas pelo WhatsApp e Instagram, mas ainda tem dificuldade em organizar os pedidos e calcular preços de forma justa.
- **Necessidades:**
  - Não sabe precificar corretamente seus doces.
  - Se perde com as encomendas, às vezes esquece prazos.
  - Quer transmitir mais profissionalismo para os clientes.
- **Como o Sweetify ajuda:**
  - Automatiza o cálculo de preços com base nos custos e margem de lucro.
  - Organiza os pedidos por ordem de entrega.
  - Gera um catálogo bonito e compartilhável para enviar aos clientes.

**Persona 2 – Carlos Mendes (Confeiteiro Experiente e Empreendedor)**
- **Idade:** 35 anos
- **Profissão:** Dono de uma pequena confeitaria de bairro
- **Contexto:** Carlos já vive da confeitaria há anos, mas gerencia tudo em cadernos e planilhas. Quer expandir o negócio, atender mais clientes e evitar erros na produção, mas tem dificuldade em ter um controle eficiente dos ingredientes e da produção.
- **Necessidades/Dores:**
  - Precisa de controle sobre os ingredientes para evitar desperdícios.
  - Quer facilitar o gerenciamento de muitos pedidos ao mesmo tempo.
  - Precisa manter seu catálogo sempre atualizado de forma rápida.
- **Como o Sweetify ajuda:**
  - Mostra a quantidade exata de ingredientes para cada produção.
  - Ajuda a acompanhar pedidos em andamento e já concluídos.
  - Permite atualizar receitas e preços facilmente.


**Persona 3 – Juliana Santos (Cliente de Doces)**
- **Idade:** 29 anos
- **Profissão:** Analista de Marketing
- **Contexto:** Juliana adora encomendar doces para festas de amigos e eventos da família. Costuma buscar opções em redes sociais, mas muitas vezes se sente perdida porque os catálogos não são claros e os preços variam muito.
- **Necessidades/Dores:**
  - Quer visualizar facilmente as opções de doces e preços.
  - Deseja praticidade na hora de encomendar.
  - Gosta de ter segurança de que o pedido será entregue no prazo.
 - **Como o Sweetify ajuda:**
  - Disponibiliza um catálogo online organizado e confiável.
  - Dá clareza sobre preços e produtos disponíveis.
  - Aumenta a confiança no trabalho do confeiteiro.


## Histórias de Usuários

|EU COMO... `PERSONA`| QUERO/PRECISO ... `FUNCIONALIDADE` |PARA ... `MOTIVO/VALOR`                 |
|--------------------|------------------------------------|----------------------------------------|
| Confeiteiro | Cadastrar minhas informações pessoais e criar meu catálogo | Organizar minhas receitas e pedidos de forma prática |
| Confeiteiro | Cadastrar os preços dos ingredientes que uso | Calcular os valores das encomendas |
| Confeiteiro | Registrar as encomendas recebidas e suas datas | Cumprir os prazos corretamente |
| Confeiteiro | Dividir a margem de luvro de cada pedido | Garantir que estou lucrando de forma justa e transparente |
| Confeiteiro | Visualizar todos os pedidos em ordem de prioridade (prazo) | Conseguir organizar minha rotina de produção |
| Confeiteiro | Ver a lista de ingredientes necessários para cada pedido | saber exatamente as quantidade e me organizar para comprar os produtos |
| Confeiteiro | Consultar o histórico de pedidos concluídos | Ter um registro de encomendas já feitas e analisar meu desempenho |
| Cliente | Acessar o catálogo online | vizualizar com maior facilidade e poder realizar pedidos |


## Indicadores de Desempenho

Apresente aqui os principais indicadores de desempenho e algumas metas para o processo. Atenção: as informações necessárias para gerar os indicadores devem estar contempladas no diagrama de classe. Colocar no mínimo 5 indicadores. 

Usar o seguinte modelo: 

![Indicadores de Desempenho](img/02-indic-desemp.png)
Obs.: todas as informações para gerar os indicadores devem estar no diagrama de classe a ser apresentado a posteriori. 

## Requisitos

### Requisitos Funcionais

|ID    | Descrição do Requisito |Teste | Critério | Prioridade |
|------|-----------------------------------------|---|------------------------------------------|---|
|RF-001|UC-001 - Login no Sistema|TC-001 - Teste de autenticação| O usuário consegue acessar o sistema com credenciais válidas.| Alta |
|RF-002|UC-002 - Cadastro de Catálogo|TC-002 - Teste de cadastro de produtos| O usuário consegue cadastrar produtos com nome, descrição, preço e imagens.| Alta |
|RF-003|UC-003 - Listar Encomendas|TC-003 - Teste de listagem de encomendas| Listagem completa de encomendas com os campos definidos.| Média |
|RF-004|UC-004 - Priorizar Pedidos|TC-004 - Teste de ordenação por prazo| Pedidos exibidos em ordem de prazo crescente.| Média |
|RF-005|UC-005 - Gerenciar Receitas|TC-005 - Teste de criação e edição de receitas| O usuário consegue criar, salvar e alterar receitas existentes.| Alta |
|RF-006|UC-006 - Sugestão de Preços|TC-006 - Teste de precificação automática| Sugestões de preços apresentadas com base em dados externos ou históricos.| Média |
|RF-007|UC-007 - Controle de Estoque|TC-007 - Teste de atualização automática do estoque| O estoque é atualizado automaticamente após cada pedido confirmado.| Baixa |
|RF-008|UC-008 - Relatórios Financeiros|TC-008 - Teste de geração de relatórios| Relatórios são gerados corretamente e exibem dados consolidados.| Média |

### Requisitos não Funcionais

|ID     | Descrição do Requisito  | Tipo |
|-------|-------------------------|----|
|RNF-001|O sistema deve seguir as regras de privacidade LGPD.|Segurança|Dados do usuário tratados de acordo com a legislação vigente.|
|RNF-002|O sistema deve ser responsivo.|Usabilidade|Interface se adapta a dispositivos móveis, tablets e desktops.|
|RNF-003|O sistema deve estar disponível 24/7.|Disponibilidade|Testes confirmam uptime contínuo.|
|RNF-004|Tempo de carregamento menor que 3 segundos.|Desempenho|Páginas principais carregam em até 3 segundos em ambiente de produção.|
 

## Restrições

|ID| Restrição                                             |
|--|-------------------------------------------------------|
|RN-01|Senhas devem ter no mínimo 8 caracteres, incluindo letras e números.|
|RN-02|Relatórios só podem ser gerados por usuários com perfil de administrador.|

## Diagrama de Casos de Uso

O diagrama de casos de uso é o próximo passo após a elicitação de requisitos, que utiliza um modelo gráfico e uma tabela com as descrições sucintas dos casos de uso e dos atores. Ele contempla a fronteira do sistema e o detalhamento dos requisitos funcionais com a indicação dos atores, casos de uso e seus relacionamentos. 

As referências abaixo irão auxiliá-lo na geração do artefato “Diagrama de Casos de Uso”.

> **Links Úteis**:
> - [Criando Casos de Uso](https://www.ibm.com/docs/pt-br/elm/6.0?topic=requirements-creating-use-cases)
> - [Como Criar Diagrama de Caso de Uso: Tutorial Passo a Passo](https://gitmind.com/pt/fazer-diagrama-de-caso-uso.html/)
> - [Lucidchart](https://www.lucidchart.com/)
> - [Astah](https://astah.net/)
> - [Diagrams](https://app.diagrams.net/)

# Matriz de Rastreabilidade

A matriz de rastreabilidade é uma ferramenta usada para facilitar a visualização dos relacionamento entre requisitos e outros artefatos ou objetos, permitindo a rastreabilidade entre os requisitos e os objetivos de negócio. 

A matriz deve contemplar todos os elementos relevantes que fazem parte do sistema, conforme a figura meramente ilustrativa apresentada a seguir.

![Exemplo de matriz de rastreabilidade](img/02-matriz-rastreabilidade.png)

> **Links Úteis**:
> - [Artigo Engenharia de Software 13 - Rastreabilidade](https://www.devmedia.com.br/artigo-engenharia-de-software-13-rastreabilidade/12822/)
> - [Verificação da rastreabilidade de requisitos usando a integração do IBM Rational RequisitePro e do IBM ClearQuest Test Manager](https://developer.ibm.com/br/tutorials/requirementstraceabilityverificationusingrrpandcctm/)
> - [IBM Engineering Lifecycle Optimization – Publishing](https://www.ibm.com/br-pt/products/engineering-lifecycle-optimization/publishing/)


# Gerenciamento de Projeto

Todo o gerenciamento do projeto será feito através do worksplace do [Sweetify no Clickup](https://app.clickup.com/90132328478/v/li/901319034147).

Somente o [planejamento de custos](img/02-orcamento.png](https://docs.google.com/spreadsheets/d/1Kk22LDt9Ccu2w5gTrt0UidkCqqAYLPMlzvw2s77rH5c/edit?usp=sharing)) foi feito em outra plataforma (Google Sheets)
