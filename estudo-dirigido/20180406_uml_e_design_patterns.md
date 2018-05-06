# UML e DESIGN PATTERNS

***

## O que é UML?

A UML, Linguagem Unificada de Modelagem, é uma **linguagem gráfica** para **visualização, especificação, construção e documentação** de artefatos de sistemas complexos de software. (BOOK, RUMBAUGH, JACOBSON; pág. VII).

A UML (Unified Modeling Language) é uma **linguagem-padrão para a elaboração da estrutura de projetos de software**. Ela poderá se empregada para a visualização, a especificação, a construção e a documentação de artefatos que façam uso de sistemas complexos de software. (BOOK, RUMBAUGH, JACOBSON; pág. 14).

Aprender a aplicar a UML de maneira efetiva tem início com a formação de um **modelo conceitual da linguagem**, o que pressupõe o entendimento de três principais elementos: (BOOK, RUMBAUGH, JACOBSON; pág. 14).

* Os blocos básicos de construção da UML.
* As regras que determinam como esses blocos de construção deverão ser combinados; e
* Alguns mecanismos básicos que se aplicam a toda a linguagem.

A UML é apenas uma linguagem e, portanto, é somente uma parte de um método para desenvolvimento de software. A UML **é independente do processo**, apesar de ser perfeitamente utilizada em processo orientado a casos de usos, centrado na arquitetura, iterativo e incremental. (BOOK, RUMBAUGH, JACOBSON; pág. 14).

A UML **é uma linguagem para construção**; **não é uma linguagem visual de programação**, mas seus modelos podem ser diretamente conectados a várias linguagens de programação. Isso significa que é possível mapear os modelos da UML em linguagens de programação tais como Java, C++, Visual Basic ou até tabelas de bancos de dados relacionais ou o armazenamento de dados persistentes de um banco de dados orientado a objetos. (BOOK, RUMBAUGH, JACOBSON; pág. 16-17).

A UML **é capaz de representar tudo que possa ser mais bem expresso em termos gráficos**, enquanto as linguagens de programação representam o que é mais bem expresso em termos textuais. (BOOK, RUMBAUGH, JACOBSON; pág. 17).

A UML **não está restrita à modelagem de software**. Na verdade, a UML é suficientemente expressiva para modelar sistemas que não sejam de software, como o fluxo de trabalho no sistema legal, a estrutura e o comportamento de sistemas de saúde e o projeto de hardware. (BOOK, RUMBAUGH, JACOBSON; pág. 18).

### Blocos de construção da UML

O vocabulário da UML abrange três tipos de blocos de construção: (BOOK, RUMBAUGH, JACOBSON; pág. 19).

* **Itens**: abstrações identificadas como cidadãos de primeira classe em um modelo;
* **Relacionamentos**: reúnem os itens UML;
* **Diagramas**: agrupam coleções interessantes de ítens.

### Itens da UML

Existem quatro tipos de itens na UML:  (BOOK, RUMBAUGH, JACOBSON; pág. 19).

* **Itens estruturais**: substantivos utilizados em modelos da UML. São as partes mais estáticas do modelo, representando elementos conceituais ou físicos;
    * Coletivamente, os itens estruturais são chamados de **classificadores**;
    * **Classes** são descrições de conjuntos de objetos que **compartilham os mesmos atributos, operações, relacionamentos e semântica**;
    * Graficamente, **as classes são representadas por retângulos**, geralmente incluindo seu **nome, atributos e operações**;
    * Uma **interface é uma coleção de operações** que **especificam serviços de uma classe ou componente**;
    * Uma interface descreve o **comportamento externamente visível** desse elemento;
    * A declaração de uma interface é semelhante a uma classe mas com a palavra-chave <<interface>> acima do nome; os atributos não são relevantes, exceto, às vezes, para mostrar as constantes.
    * Uma interface raramente aparece sozinha.
* **Itens comportamentais**;
* **Itens de agrupamentos**;
* **Itens anotacionais**.

São os **blocos de construção básicos orientados a objeto**s da UML.  (BOOK, RUMBAUGH, JACOBSON; pág. 19).

***

## O que é a OMG?

O Object Management Group, ou OMG, é uma organização internacional que aprova padrões abertos para aplicações orientadas a objetos. Esse grupo define também a OMA (Object Management Architecture), um modelo padrão de objeto para ambientes distribuídos. (WIKIPEDIA, 2018a).

Site: https://www.omg.org/

***

## Quais os diferentes diagramas UML e quais são suas divisões?

Um diagrama é uma apresentação gráfica de um conjunto de elementos, geralmente representada como um gráfico conectado de vértices (itens) e arcos (relacionamentos). Um diagrama é uma projeção em um sistema. A UML inclui 12 desses diagramas.

_Obs.:_ os tipos de diagramas híbridos são permitidos; não há separação estrita entre elementos de modelo.

1. **Diagrama de Classes**
    * Um diagrama estrutural que mostra um conjunto de classes, interfaces, colaborações e seus relacionamentos.
1. **Diagrama de Objetos**
    * Um diagrama estrutural que mostra um conjunto de objetos e seus relacionamentos.
1. **Diagrama de Componentes**
    * Um diagrama estrutural que mostra as interfaces externas, incluindo portas e a composição interna de um componente.
1. **Diagrama de Estrutura Composta**
    * Um diagrama estrutural que mostra as interfaces externas e a composição interna de uma classe estruturada. Neste livro, combinamos o tratamento do diagrama de estrutura composta com o diagrama de componentes.
1. **Diagrama de Casos de Uso**
    * Um diagrama comportamental que mostra um conjunto de  casos de uso e atores e seus relacionamentos.
1. **Diagrama de Sequências**
    * Um diagrama comportamental que mostra uma interação, dando ênfase à ordenação temporal das mensagens.
1. **Diagrama de Comunicação**
    * Um diagrama comportamental que mostra uma interação, dando ênfase à organização estrutural de objetos que enviam e recebem mensagens.
1. **Diagrama de Estados**
    * Um diagrama comportamental que mostra uma máquina de estados, dando ênfase ao comportamento ordenado por eventos de um objeto.
1. **Diagrama de Atividades**
    * Um diagrama comportamental que mostra um processo computacional, dando ênfase ao fluxo de uma atividade para outra.
1. **Diagrama de Implantação**
    * Um diagrama estrutural que mostra os relacionamentos entre um conjunto de nós, artefatos e classes manifestadas e componentes.
1. **Diagrama de Pacotes**
    * Um diagrama estrutural que mostra a organização do modelo em pacotes.
1. **Diagrama de Temporização**
    * Um diagrama comportamental que mostra uma interação com mensagens em momentos específicos.
1. **Diagrama de Visão Geral da Interação**
    * Um diagrama comportamental que combina aspectos dos diagramas de atividades e dos diagramas de sequências.

***

## O que é um padrão ISO?

Segundo Significados (2018a),

ISO é a sigla de International Organization for Standardization, ou Organização Internacional para Padronização, em português. A ISO é uma entidade de padronização e normatização, e foi criada em Genebra, na Suiça, em 1947.

A sigla para International Organization for Standardization deveria ser IOS e não ISO. No entanto, como em cada país de línguas diferentes existiria uma sigla diferente, os fundadores decidiram escolher uma só sigla para todos os países: ISO. Esta foi a sigla escolhida porque em grego isos significa "igual", o que se enquadra com o propósito da organização em questão.

A ISO tem como objetivo principal aprovar normas internacionais em todos os campos técnicos, como normas técnicas, classificações de países, normas de procedimentos e processos, e etc. No Brasil, a ISO é representada pela ABNT (Associação Brasileira de Normas Técnicas).

A ISO promove a normatização de empresas e produtos, para manter a qualidade permanente. Suas normas mais conhecidas são a ISO 9000, ISO 9001, ISO 14000 e ISO 14064. As ISO 9000 e 9001 são um sistema de gestão de qualidade aplicado em empresas, e ISO 14000 e ISO 14064 são um sistema de gestão ambiental.

***

## O que são design patterns?

Christopher Alexander afirma: (GAMMA, 2000, p. 19).

> Cada padrão descreve um problema no nosso ambiente e o cerne da sua solução, de tal forma que você possa usar essa solução mais de um milhão de vezes, sem nunca fazê-lo da mesma maneira. (GAMMA, 2000, p. 19).

Muito embora Alexander estivesse falando acerca de padrões em construções e cidades, o que ele diz é verdadeiro em relação aos padrões de projeto orientados a objeto. Nossas soluções são expressas em termos de objetos e interfaces em vez de paredes e portas, mas no cerne de ambos os tipos de padrões está a solução para um problema em um determinado contexto.  (GAMMA, 2000, p. 19).

Em geral, um padrão tem quatro elementos essenciais:  (GAMMA, 2000, p. 19).

* Nome do padrão para referência;
* O problema descreve em que situação aplicar o padrão;
* A solução; e
* As consequências de seu uso.

***

## Quais são os padrões GOF?

A lista abaixo foi obtida de Gamma (2000, capa).

### Padrões de Criação

* Abstract Factory
* Builder
* Factory Method
* Prototype
* Singleton

### Padrões Estruturais

* Adapter
* Bridge
* Composite
* Decorator
* Façade
* Flyweight
* Proxy

### Padrões Comportamentais

* Chain of Responsibility
* Command
* Interpreter
* Iterator
* Mediator
* Memento
* Observer
* State
* Strategy
* Template Method
* Visitor

***

## Por que contratar mais de um programador atrasa ainda mais o projeto de acordo com o artigo "no silver bullet"?

***

## Por que a OO não está relacionada a uma linguagem de programação e a nenhuma ferramenta de desenvolvimento?

***

## REFERÊNCIAS

BOOCK, Grady; RUMBAUGH, James; JACOBSON, Ivar. **UML**: guia do usuário. 2ª ed. Rio de Janeiro: Elsevier, 2012.

GAMMA, Erich; HELM, Richard; JOHNSON, Ralph; VLISSIDES, John. Padrões de projeto: soluções reutilizáveis de software orientado a objetos. Porto Alegre: Bookman, 2000.

SIGNIFICADOS. **Significado de ISO**. Disponível em: <<https://www.significados.com.br/iso/>>. Acesso em 04 mai. 2018a.

WIKIPEDIA. Object Management Group. Disponível em: <<https://pt.wikipedia.org/wiki/Object_Management_Group>>. Acesso em 24 abr. 2018a.