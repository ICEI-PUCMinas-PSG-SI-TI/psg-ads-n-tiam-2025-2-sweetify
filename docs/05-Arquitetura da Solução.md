# Arquitetura da Solução

<span style="color:red">Pré-requisitos: <a href="3-Projeto de Interface.md"> Projeto de Interface</a></span>

Optamos por utilizar o Modelo C4 para descrever a arquitetura do nosso sistema, fornecendo visões detalhadas nos níveis de Contexto e Container.

### Nível de Contexto

Esta seção apresenta a visão geral do nosso sistema.

O Aplicativo Sweetify é utilizado pelo Usuário (Confeiteiro). O principal objetivo do sistema é automatizar e simplificar dois processos críticos para o usuário: a gestão da produção e o processo de precificação de produtos de confeitaria.

![Modelo C4 Nível Contexto](img/C4-Contexto.jpg)

### Nível de Container

A visão de Container detalha a arquitetura interna do nosso aplicativo, mostrando as principais aplicações e armazenamentos de dados que compõem o sistema. O Usuário interage diretamente com a Interface de Usuário (Mobile App), que será desenvolvida utilizando React Native. Esta interface, por sua vez, se comunica com a API de Backend. A API é o componente responsável por toda a lógica de negócio e pelo gerenciamento do acesso aos dados, sendo desenvolvida em C# com o framework ASP.NET Core. Complementando o backend, o Banco de Dados é responsável por persistir e armazenar todas as informações críticas da aplicação. A comunicação e o gerenciamento dos dados do banco são feitos exclusivamente pela API.

![Modelo C4 Nível Container](img/C4-Container.jpg)


## Diagrama de Classes

![Diagrama de classes](img/C4-Diagrama-de-classes.png)

## Modelo ER

O Modelo ER representa através de um diagrama como as entidades (coisas, objetos) se relacionam entre si na aplicação interativa.]

As referências abaixo irão auxiliá-lo na geração do artefato “Modelo ER”.

> - [Como fazer um diagrama entidade relacionamento | Lucidchart](https://www.lucidchart.com/pages/pt/como-fazer-um-diagrama-entidade-relacionamento)

## Esquema Relacional

O Esquema Relacional corresponde à representação dos dados em tabelas juntamente com as restrições de integridade e chave primária.
 
As referências abaixo irão auxiliá-lo na geração do artefato “Esquema Relacional”.

> - [Criando um modelo relacional - Documentação da IBM](https://www.ibm.com/docs/pt-br/cognos-analytics/10.2.2?topic=designer-creating-relational-model)

## Modelo Físico

Entregar um arquivo banco.sql contendo os scripts de criação das tabelas do banco de dados. Este arquivo deverá ser incluído dentro da pasta src\bd.

## Tecnologias Utilizadas

### Frontend (Interface de Usuário)
Plataforma: React Native (para o desenvolvimento da interface mobile).
Estilização: CSS e o framework Tailwind CSS (para aceleração e consistência do design).

### Backend (API e Dados)
Linguagem da API: C#.
Framework da API: ASP.NET Core.
Banco de Dados: SQL Server (tipo relacional, utilizado para persistência de dados).

### Ferramentas de Desenvolvimento e Processo
Ambiente de Desenvolvimento (IDE): Visual Studio Code (VS Code).
Controle de Versão: GitHub (para versionamento e colaboração).
Testes de API e Documentação: Swagger (para documentação de endpoints) e Postman (para testes manuais e funcionais na API).

Apresente também uma figura explicando como as tecnologias estão relacionadas ou como uma interação do usuário com o sistema vai ser conduzida, por onde ela passa até retornar uma resposta ao usuário.

## Hospedagem

Explique como a hospedagem e o lançamento da plataforma foi feita.

> **Links Úteis**:
>
> - [Website com GitHub Pages](https://pages.github.com/)
> - [Programação colaborativa com Repl.it](https://repl.it/)
> - [Getting Started with Heroku](https://devcenter.heroku.com/start)
> - [Publicando Seu Site No Heroku](http://pythonclub.com.br/publicando-seu-hello-world-no-heroku.html)

## Qualidade de Software

Conceituar qualidade de fato é uma tarefa complexa, mas ela pode ser vista como um método gerencial que através de procedimentos disseminados por toda a organização, busca garantir um produto final que satisfaça às expectativas dos stakeholders.

No contexto de desenvolvimento de software, qualidade pode ser entendida como um conjunto de características a serem satisfeitas, de modo que o produto de software atenda às necessidades de seus usuários. Entretanto, tal nível de satisfação nem sempre é alcançado de forma espontânea, devendo ser continuamente construído. Assim, a qualidade do produto depende fortemente do seu respectivo processo de desenvolvimento.

A norma internacional ISO/IEC 25010, que é uma atualização da ISO/IEC 9126, define oito características e 30 subcaracterísticas de qualidade para produtos de software.
Com base nessas características e nas respectivas sub-características, identifique as sub-características que sua equipe utilizará como base para nortear o desenvolvimento do projeto de software considerando-se alguns aspectos simples de qualidade. Justifique as subcaracterísticas escolhidas pelo time e elenque as métricas que permitirão a equipe avaliar os objetos de interesse.

> **Links Úteis**:
>
> - [ISO/IEC 25010:2011 - Systems and software engineering — Systems and software Quality Requirements and Evaluation (SQuaRE) — System and software quality models](https://www.iso.org/standard/35733.html/)
> - [Análise sobre a ISO 9126 – NBR 13596](https://www.tiespecialistas.com.br/analise-sobre-iso-9126-nbr-13596/)
> - [Qualidade de Software - Engenharia de Software 29](https://www.devmedia.com.br/qualidade-de-software-engenharia-de-software-29/18209/)
