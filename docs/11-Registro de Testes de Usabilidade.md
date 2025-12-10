# Registro de Testes de Usabilidade

Este documento serve como o Registro Oficial dos Testes de Usabilidade realizados no aplicativo de gerenciamento e precificação. Ele apresenta as evidências, observações e feedback qualitativo dos participantes, conforme o Plano de Testes de Usabilidade estabelecido no documento inicial.

---

### Detalhes do Teste

| Item | Descrição |
| :--- | :--- |
| **Aplicativo Testado** | Telas de Cadastro e Página Inicial/Gerenciamento |
| **Testador Responsável** | Matheus Dias |
| **Referência** | Plano de Testes de Usabilidade (Documento Base) |

### Perfil dos Participantes

| Participante | Perfil/Ocupação | Nível de Familiaridade com a Plataforma |
| :--- | :--- | :--- |
| **Usuário 1** | Proprietário de Empresa (Público-Alvo) | Nenhuma (Primeiro Contato) |
| **Usuário 2** | Proprietário de Empresa (Público-Alvo) | Nenhuma (Primeiro Contato) |
| **Usuário 3** | Proprietário de Empresa (Público-Alvo) | Nenhuma (Primeiro Contato) |

---

### Evidências dos Casos de Teste

#### Cenário 1: Fluxo de Cadastro e Compreensão da Dinâmica de Dados

**Objetivo:** Analisar a facilidade de aprendizado e compreensão da dinâmica de componentes e subcomponentes para o gerenciamento e precificação (Ingredientes $\rightarrow$ Receitas $\rightarrow$ Produtos $\rightarrow$ Encomendas).

| Tarefa | Status | Compreensão Autônoma |
| :--- | :--- | :--- |
| Cadastrar Ingrediente, Serviço | Sucesso | Sim |
| Cadastrar Receita | Sucesso | Sim |
| Cadastrar Produto | Sucesso | Sim |
| Cadastrar Encomenda (Fechamento do Ciclo) | Sucesso | Sim |

**Observações de Usabilidade:**

* **Facilidade de Aprendizado:** Os usuários conseguiram concluir todas as etapas de cadastro sem assistência. A estrutura sequencial das telas de cadastro guiou os usuários através da hierarquia de entidades.
* **Evidência:** O funcionamento das telas de cadastro foi bem compreendido, indicando uma **boa usabilidade** nesta etapa crucial para a precificação. 

**Relato Comum:** "Eu entendi que tinha que cadastrar o pequeno (ingrediente) antes do grande (receita)."

#### Cenário 2: Página Inicial e Gerenciamento de Entidades

**Objetivo:** Avaliar a usabilidade da página inicial, a autonomia na navegação e o destaque visual das informações financeiras (Custo, Preço de Venda e Lucro).

| Ação Avaliada | Status | Destaque Visual (Cores) |
| :--- | :--- | :--- |
| Acesso e Navegação Autônoma | Sucesso | N/A |
| Identificação do Lucro (Cor Verde) | Imediata | Eficaz |
| Identificação do Custo (Cor Vermelha) | Imediata | Eficaz |
| Ações de Edição/Exclusão (Botões) | Sucesso, mas com Fricção | N/A |

**Observações de Usabilidade:**

* **Autonomia:** Os usuários conseguiram manipular (editar/excluir) e acessar as informações cadastradas sem auxílio, confirmando a boa usabilidade da navegação principal.
* **Clareza Visual:** O uso das cores **Verde** para lucro e **Vermelho** para custo foi **altamente eficaz** em colocar o preço de venda, o custo de produção e o lucro obtido "em evidência", atingindo o objetivo principal desta seção.

---

### *Feedback* Qualitativo e Pontos de Fricção (Melhorias)

O *feedback* geral foi positivo, com satisfação em relação ao design e à funcionalidade. Os problemas identificados são de "micro-usabilidade" e acessibilidade visual.

| Tipo de Melhoria | Descrição do Problema (Relato do Usuário) | Ação de Correção Gerada |
| :--- | :--- | :--- |
| **Visual/Acessibilidade** | Algumas letras em informações secundárias nos *cards* estavam muito pequenas, dificultando a leitura rápida. | **Aumentar o tamanho de algumas letras** e deixar informações mais evidentes. |
| **Design de Interação (Ícones)** | Os ícones de edição e exclusão nas páginas de detalhes estavam "muito pequenos" e muito próximos dos botões de seleção. | **Alterar o posicionamento** e **aumentar o *touch target*** dos ícones de edição e exclusão. |
| **Design de Ícones** | Sugestão de alteração das cores de alguns ícones para melhor diferenciação ou contraste. | **Alterar cores de ícones** pontuais para otimizar a usabilidade visual. |

### Plano de Implementação de Melhorias

Com base nos resultados, as seguintes ações foram priorizadas para aprimorar a usabilidade:

1.  Revisão da tipografia dos *cards* de listagem para melhor legibilidade.
2.  Redesenho da área de ações em massa (selecionar/editar/excluir) nas telas de detalhes para aumentar o tamanho e separação dos botões e ícones.
3.  Ajustes finos nas cores dos ícones para melhor clareza.

