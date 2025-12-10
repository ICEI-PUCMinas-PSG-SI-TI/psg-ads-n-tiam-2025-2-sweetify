# Plano de Testes de Usabilidade e Relatório de Resultados

Este documento apresenta a metodologia e os resultados dos testes de usabilidade realizados para avaliar a experiência do usuário com o aplicativo de gerenciamento e precificação de empresas.

---

### Objetivo

O principal objetivo dos testes foi avaliar a **facilidade de aprendizado**, **eficiência de uso** e **satisfação** geral dos usuários-alvo (proprietários de pequenas empresas) com o aplicativo, identificando áreas que necessitam de melhoria na usabilidade.

### Participantes

* **Número de Usuários:** 3
* **Perfil:** Usuários que gerenciam suas próprias empresas, alinhados ao público-alvo do aplicativo.

---

### Testes Realizados

Os testes foram divididos em duas etapas principais, ambas realizadas sem qualquer instrução prévia dos desenvolvedores para garantir uma avaliação da usabilidade orgânica.

#### 1. Telas de Cadastro e Fluxo de Dados

**Foco:** Compreensão da dinâmica de cadastro e da hierarquia de entidades:

* **Entidades:** Ingredientes, Serviços, Receitas, Produtos e Encomendas.
* **Complexidade Avaliada:** Capacidade do usuário de entender a relação de componentes e subcomponentes (ex: uma Receita usa Ingredientes e Serviços; um Produto usa Receitas, e uma Encomenda usa Produtos). Este é um passo **imprescindível** para a correta precificação.
* **Metodologia:** Observação da interação do usuário ao tentar realizar o cadastro completo do ciclo de produção.
* ****

**Resultados:**
* **Avaliação:** **Muito Bom**. Os usuários conseguiram cadastrar as entidades e compreenderam o fluxo e a interdependência entre as telas de cadastro de forma autônoma.
* **Conclusão:** O *design* da informação e o fluxo de cadastro são intuitivos e possuem boa usabilidade.

#### 2. Página Inicial e Gerenciamento de Entidades

**Foco:** Usabilidade da interface de gerenciamento, acesso a dados e destaque de informações cruciais.

* **Ações Avaliadas:** Acesso e visualização de entidades cadastradas, uso de botões para cadastrar novas entidades, edição e exclusão.
* **Destaque Prioritário:** Avaliação da visualização do **Preço de Venda**, **Custo de Produção** e **Lucro Obtido**.
* **Recursos Avaliados:** Uso de cores (**Verde** para Lucro, **Vermelho** para Custo) para rápida identificação.
* **Metodologia:** Observação da navegação e das tentativas de gerenciamento e alteração dos dados após o cadastro.

**Resultados:**
* **Avaliação:** **Boa Usabilidade**. Os usuários demonstraram autonomia na navegação da página inicial e no gerenciamento das entidades (acesso, edição, exclusão).
* **Destaque:** O uso estratégico de cores para **Lucro** e **Custo** foi eficaz para evidenciar as informações financeiras de forma imediata.

---

### Resultados e Melhorias Identificadas

Os testes confirmaram a **facilidade de uso** e o **design agradável** do aplicativo. No entanto, o *feedback* qualitativo dos usuários indicou pontos de fricção importantes relacionados à clareza visual e posicionamento de elementos.

| Categoria | *Feedback* do Usuário | Ação de Melhoria (Pós-Teste) |
| :--- | :--- | :--- |
| **Acessibilidade Visual** | Necessidade de **aumentar o tamanho de algumas letras** para melhor leitura. | Ajuste da hierarquia tipográfica e aumento das fontes em áreas de texto denso. |
| **Clareza da Informação** | Deixar **informações mais evidentes** nos *cards* de entidades (na página inicial). | Revisão do *design* dos *cards* para priorizar e evidenciar dados essenciais (e.g., nome da entidade, preço final). |
| **Posicionamento de Ícones** | Ícones de **edição/exclusão** na página de detalhes estavam **muito pequenos** e próximos dos botões "selecionar" e "selecionar todos". | **Movimentação e Redimensionamento** dos ícones de ação (Edição/Exclusão) para uma área mais destacada e com maior *touch target*, separando-os dos botões de seleção em lote. |
| **Design de Interação** | Necessidade de **alterar cores de ícones** para melhor distinção de função ou estado. | Alteração pontual das cores de ícones para reforçar sua função e *affordance* (convite à ação). |

### Conclusão

O processo de teste de usabilidade foi **fundamental** para aprimorar a experiência do usuário. Embora o aplicativo apresente um bom fluxo de trabalho e seja intuitivo nas etapas críticas de cadastro (confirmando a lógica de negócio), o *feedback* dos usuários permitiu a identificação e correção de problemas de **micro-usabilidade** (tamanho da fonte, posicionamento de *touch targets*) que afetam diretamente a autonomia e a satisfação.

As alterações implementadas após os testes resultaram em uma interface mais acessível e com maior autonomia para o usuário final.

--
> * [Planejando testes de usabilidade: o que (e o que não) fazer | iMasters](https://imasters.com.br/design-ux/planejando-testes-de-usabilidade-o-que-e-o-que-nao-fazer/)
> * [Ferramentas de Testes de Usabilidade | Usability.gov](https://www.usability.gov/how-to-and-tools/resources/templates.html)
