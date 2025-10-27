# Programação de Funcionalidades

# Especificação de Requisitos Funcionais

Este documento descreve os **Requisitos Funcionais (RF)** e **Casos de Uso (UC)** do sistema de gestão de confeitaria, com foco em controle de produtos, receitas, custos e encomendas.

## RF-001 / UC-001 — Login com e-mail e senha

**Descrição:**  
O sistema deve permitir que o usuário faça login com e-mail e senha.

**Implementação:**  
- Foi criada uma tela de login e cadastro.  
- O usuário pode escolher entre fazer login ou cadastro.  
- Utiliza comunicação assíncrona com o nosso banco de dados via backend
- Hooks do **React Native** são usados para controle de estado e autenticação.

## RF-002 / UC-002 — Gerenciamento de usuários, produtos, receitas, encomendas e custos de produção

**Descrição:**  
O sistema deve permitir o gerenciamento de usuários, produtos, receitas, encomendas e custos de produção.

**Implementação:**  
- Criado um **menu de gerenciamento** que redireciona para telas de controle (Produtos, Receitas, Encomendas, Itens de Custos).  
- As informações são armazenadas em **objetos e listas**.  
- Cada entidade é manipulada com funções **CRUD** (Criar, Listar, Atualizar, Excluir).

## RF-003 / UC-003 — Cálculo de rendimento total de um produto

**Descrição:**  
O sistema deve ser capaz de calcular o rendimento total de um produto.

**Implementação:**  
- Criada uma função que recebe os dados do produto (quantidade produzida, insumos e custos) e retorna o **rendimento total**.

## RF-004 / UC-004 — Cadastro de produto com múltiplas receitas

**Descrição:**  
O sistema deve permitir o cadastro de produtos com múltiplas receitas.

**Implementação:**  
- O formulário de cadastro permite vincular **mais de uma receita** a um produto.  
- Utiliza **array de objetos** para associar várias receitas.  
- O componente **“Adicionar Receita”** usa **FlatList** e **useState** para manipular os dados dinamicamente.  
- A verificação pode ser feita criando um novo produto e adicionando múltiplas receitas.

## RF-005 / UC-005 — Gerenciar receitas

**Descrição:**  
O sistema deve ser capaz de gerenciar receitas.

**Implementação:**  
- Tela dedicada para **listar, cadastrar e excluir receitas**.  
- Receitas armazenadas como **objetos** com propriedades: `nome`, `ingredientes`, `rendimento`, `custo`.  
- Utiliza comunicação assíncrona com o nosso banco de dados via backend

## RF-006 / UC-006 — Sugerir preços de produtos

**Descrição:**  
O sistema deve ser capaz de sugerir preços de produtos.

**Implementação:**  
- Função que calcula automaticamente o **preço sugerido** com base no **custo e margem de lucro**.  
- O resultado é exibido no campo **“Preço Sugerido”** do formulário antes da confirmação do cadastro.

## RF-007 / UC-007 — Alterar preços de venda sugeridos

**Descrição:**  
O sistema deve permitir que o usuário altere os preços de venda sugeridos pela plataforma.

**Implementação:**  
- Na tela de edição de produto, o campo de preço é **editável**.  
- O usuário pode **modificar manualmente** o valor antes de salvar.  
- Utiliza comunicação assíncrona com o nosso banco de dados via backend

## RF-008 / UC-008 — Controle de insumos

**Descrição:**  
O sistema deve permitir o controle de insumos.

**Implementação:**  
- Tela para **cadastrar e listar insumos** usados nas receitas.  
- Cada insumo possui: `nome`, `quantidade`, `unidade de medida`, `custo`.  
- Dados armazenados via **AsyncStorage**.  
- A listagem permite **visualizar, editar e excluir** insumos.

## RF-009 / UC-009 — Visualizar todas as informações cadastradas

**Descrição:**  
O sistema deve permitir que o usuário visualize todas as informações cadastradas.

**Implementação:**  
- Tela de **resumo** exibe informações de usuários, produtos, receitas, encomendas e insumos.  
- Utiliza comunicação assíncrona com o nosso banco de dados via backend
- Exibição em **listas agrupadas por categoria**, com expansão de itens para detalhes.

## RF-010 / UC-010 — Fornecer preço de venda, custo e lucro das encomendas

**Descrição:**  
O sistema deve fornecer o preço de venda, custo e lucro das encomendas.

**Implementação:**  
- A tela de encomendas **calcula automaticamente** custo, preço e lucro com base nos produtos selecionados.  
- Exibição em **cards**, com atualização dinâmica conforme os itens são adicionados.

## RF-011 / UC-011 — Notificação ao tentar adicionar itens não cadastrados

**Descrição:**  
O sistema deve notificar o usuário quando tentar adicionar itens não cadastrados.

**Implementação:**  
- Verificação condicional antes de salvar receitas ou encomendas.  
- Caso o item (produto, insumo, etc.) não exista, o sistema exibe um **alerta (Alert)** informando a necessidade de cadastro prévio.

## RF-012 / UC-012 — Aplicação de templates pré-definidos

**Descrição:**  
O sistema deve permitir ao usuário aplicar **templates pré-definidos** no momento do cadastro.

**Implementação:**  
- Durante o cadastro de produtos e receitas, o usuário pode escolher **modelos prontos** armazenados em arquivo JSON.  
- Templates carregados dinamicamente e modificáveis antes do salvamento.  
- Utiliza **useState** e **Dropdown** para seleção dos templates.

## 🧭 Tecnologias utilizadas
- **React Native**
- **React Native Paper**
- **Styled Components**
- **API C#**

