# Arquitetura SOA

 - Líder
	 - Eduardo
 - Secretário
	 - Leonardo
 - Referências do professor
	 - Larman, Pressman, Sommerville.
	 - Fox, Armando e Paterson, David. Construindo Software como Serviço – Uma Abordagem Ágil Usando Computação em Nuvem, Strawberry Canyon LLC, 2015.

## O que é SOA?

### O básico

SOA é um estilo de arquitetura de TI que dá suporte à transformação de um negócio em um conjunto de serviços, encadeados, que podem ser acessados através de uma rede. (ALVES, 2013, p. 8).

SOA se apresenta como uma evolução da orientação a objetos e da componentização dos mesmos e caracteriza-se pelo **fraco acoplamento**, **transparência de localização** e **independência de protocolos**. (ALVES, 2013, p. 8).

É importante observar que SOA é uma arquitetura conceitual, que **define serviço como um processo de negócio implementado em software**, que a partir de um **conjunto de entradas** fornece um **conjunto de saídas**, baseado em uma **função de transformação**. Esta função de transformação é conhecida pelo solicitante, uma vez que é descrita através de uma **interface formal**. (ALVES, 2013, p. 8).

As arquiteturas orientadas a serviços (SOA, no inglês *service-oriented architectures*) são uma forma de desenvolvimento de sistemas distribuídos em que os componentes de sistema são **serviços autônomos**, executando em **computadores geograficamente distribuídos**. Protocolos-padrão baseados em XML, SOAP e WSDL foram projetados para oferecer suporte à comunicação de serviço e à troca de informações. Consequentemente, os serviçõs são plataforma e implementação indepentes de linguagem. Os sistemas de software podem ser construídos pela composição de serviços locais e serviços externos de provedores diferentes, com interação perfeita entre os serviços no sistema. (SOMMERVILLE, 2011; p. 356).

Um serviço possui três camadas: (ALVES, 2013, p. 8).

*  **CAMADA DE NEGÓCIOS**: define os serviços mediante as necessidades da organização, independente das tecnologias que serão utilizadas. É nesta camada que é realizada a descrição das composições dos serviços.
*  **CAMADA DE INTERFACE**: descrevem o serviço, sendo estas publicadas em um serviço de registro, tornando-se disponível para os consumidores.
*  **CAMADA DE IMPLEMENTAÇÃO**: contém a implementação do software posteriormente mapeado em serviço. Tais aplicações podem ser desenvolvidas em diferentes plataformas de desenvolvimento e estar distribuídas em diferentes provedores.

### Conceitos de *web service* e *serviço*

Um *web service* é uma instância de uma ideia mais geral de um serviço, que é definido como: (SOMMERVILLE, 2011; p. 355).

> um ato ou desempenho oferecido de uma parte para outra. Embora o processo possa ser vinculado a um produto físico, o desempenho é essencialmente intangível e normalmente não resulta na posse de qualquer um dos fatores de produção. (SOMMERVILLE, 2011; p. 355).

Portanto, a essência de um serviço é que **o fornecimento de serviço é independente da aplicação que o usa**. Os provedores de serviços podem desenvolver serviços especializados e oferecê-los para uma variedade de usuários de serviço de diferentes organizações.

### SOA x SaaS

A noção de *SaaS* e as arquiteturas orientadas a serviço (*SOA*s) relacionam-se, obviamente, mas não são as mesmas: (SOMMERVILLE, 2011; p. 350):

1.  O **SaaS** é uma forma de fornecer funcionalidade em um servidor remoto com acesso de clientes por meio de um browser de Web. O servidor mantém os dados e o estado do usuário durante uma sessão de interação. Geralmente, as transações são longas (por exemplo, edição de um documento).
1.  A **SOA** é uma abordagem para a estruturação de um sistema de software como **um conjunto de serviços separados, sem estado**. Estes podem ser fornecidos por vários provedores e podem ser distribuídos. Normalmente, tratam-se de transações curtas, em que um serviço é chamado, faz alguma coisa e, em seguirda, retorna um resultado.

O SaaS é uma maneira de entregar a funcionalidade de aplicação para os usuários, enquanto a SOA é uma tecnologia de implementação para sistemas de aplicações. A funcionalidade implementada pelo uso da SOA precisa aparecer para usuários como serviços. Da mesma forma, os serviços de usuário não precisam ser implementados pelo uso da SOA. No entando, se o SaaS é implementado usando a SOA, torna-se possível para aplicações usarem APIs de serviço para acessar a funcionalidade de outras aplicações. Em seguida, estas podem ser integradas em sistemas mais complexos; são chamados ***mashups*** e representam outra abordagem para reúso de software e desenvolvimento rápido de software. (SOMMERVILLE, 2011; p. 350).

Só por curisidade, *mashup* se resume a diferentes serviços que podem funcionar simultaneamente. Mashup significa *misturar*: a combinação de dois aplicativos que podem complementar e melhorar a oferta de determinado serviço. Você já deve ter visto sites de notícias com conteúdo do *YouTube* ou sites de compartilhamento de imagens com conteúdo do *Google Maps*. Se sua resposta foi sim, você está usando mashups mesmo sem saber. (SOMMERVILLE, 2011; p. 350).

## O que é CORBA?

O conteúdo abaixo foi retirado de CORBA (2018).

### Conceitos básicos

**CORBA** é o acrônimo para **Common Object Request Broker Architecture** (*arquitetura comum de agente de solicitação de objeto*, em uma tradução livre). É uma arquitetura e infraestrutura do OMG aberta e independente de vendedores que aplicações usam para trabalhar juntas usando redes de computadores. Utilizando o protocolo padrão IIOP, um programa baseado em CORBA de qualquer vendedor, em quase qualquer computador, sistema operacional, linguagem de programação e rede pode interoperar com um programa baseado em CORBA do mesmo ou de outro vendedor, em quase que qualquer outro computador, sistema operacional, linguagem de programação e rede.

### Utilidade

CORBA é útil em muitas situações. Em virtude da forma fácil como CORBA integra máquinas de tantos vendedores, com tamanhos variando de mainframes até sistemas pequenos e desktops até hand-helds e sistemas embarcados, esse é o middleware escolhido por grandes (e mesmo não tão grandes) empresas. Um de seus mais importantes, e também mais frequentes, usos é em servidores que precisam manipular um grande número de clientes, em altas taxas de acerto, com alta confiabilidade. CORBA trabalha por trás das cenas em salas de computador de muitos dos maiores websites do mundo; alguns dos quais o público em geral usa todos os dias. Especializações para escalabilidade e tolerância a falhas dão suporte a esses sistemas. Contudo, CORBA não é utilizada somente por grandes aplicações: versões especializadas de CORBA rodam em sistemas de tempo real e pequenos sistemas embarcados.

### Visão geral mais técnica

Os quatro conceitos chave da orientação a objetos são:

*  Encapsulamento
*  Polimorfismo
*  Herança
*  Instanciação

Aplicações CORBA são compostas de objetos, unidades individuais de software rodando que combinam funcionalidade e dados e, com frequência (mas não sempre) representam algo do mundo real. Tipicamente há muitas instâncias de um objeto de um determinado tipo - por exemplo, um site de e-commerce pode ter muitas instâncias de carrinhos de compras, todas idênticas em termos de funcionalidade mas diferentes sob o ponto de vista de que cada uma está associada a um cliente diferente e contém dados representando mercadorias que um cliente em particular selecionou. Quando uma aplicação legada, como um sistema de contabilidade, é envolvido (*wrapped*) no código com interfaces CORBA e aberto para clientes na rede, existe normalmente somente uma instância dele.

Para cada tipo de objeto, como o carrinho de compras mencionado a pouco, define-se uma interface OMG IDL. A interface é a parte da sintaxe do contrato que o objeto servidor oferece aos clientes que o invocam. Qualquer cliente que quer invocar uma operação no objeto deve utilizar essa interface IDL para especificar a operação que ele quer realizar e para empacotar os argumentos que ele envia. Quando a invocação alcança o objeto alvo, a mesma definição de interface é utilizada para desempacotar os resultados da viagem de volta e para desempacotar quando eles encontram seu destino.

A definição da interface IDL é independente de linguagem de programação, mas mapeia para todas as linguagens populares de programação através de padrões OMG: OMG tem padronizado o mapeamento de IDL para C, C++, C++11, Java, Ruby, COBOL, Smalltalk, Ada, Lisp, Python e IDLscript.

A separação entre interface e implementação, permitida pelo OMG IDL, é a essência de CORBA - como isso permite interoperabilidade, com toda a transparência que se almeja. A interface de cada objeto é definida de forma muito estrita. Em contraste, a implementação de um objeto - seu código rodando e seus dados - está oculta do resto do sistema (que está encapsulado) atrás de uma fronteira que o cliente não pode passar. Os clientes acessam os objetos somente através de sua interface anunciada, invocando somente aquelas operações que o objeto expõe através de sua interface IDL, com somente aqueles parâmetros (entradas e saídas) que estão incluidas na invocação.

## O que é Pub/Sub?

## O que é uma API?

Segundo FOLDOC (2018),

API, or "application programming interface" é uma interface (convenções de chamadas) pela qual uma aplicação acessa o sistema operacional e outros serviços. Uma API é definida em nível de código fonte e fornece um nível de abstração entre a aplicação e o kernel (ou outras utilidades privilegiadas) para assegurar a portabilidade do código.

Uma API também pode prover uma interface entre uma linguagem de alto nível e funcionalidades de nível mais baixo e serviços que foram escritos sem considerar convenções de chamada suportadas por linguagens compiladas. Nesse caso, a tarefa principal da API pode ser a tradução da lista de parâmetros de um formato para outro e a interpretação de argumentos chamados por valor e chamados por referência em uma ou em ambas as direções.

Segundo COMPUTERWORLD (2018),

Todo software tem que requisitar a outro software para fazer coisas para si. Para alcançar esse objetivo, o programa que requisita usa um grupo de requisições padronizadas, chamadas de application programming interface (API), que foram definidas pelo programa que está sendo chamado.

Quase toda aplicação depende de APIs de seu sistema operacional subjacente para realizar funções básicas como o acesso ao sistema de arquivos. Na essência, uma API de programa define a maneira adequada de um desenvolvedor requisitar serviços do programa.

## REFERÊNCIAS

ALVES, Luís Cézar Darienzo. **O impacto da virtualização no desempenho de aplicações distribuídas baseadas em SOA e a sua influência nos modelos de desempenho**. Orientador: Marcos José Santana. Tese de doutorado. Universidade de São Paulo. 2013.

COMPUTERWORLD. **Application Programming Interface**. Disponível em: <<https://www.computerworld.com/article/2593623/app-development/application-programming-interface.html>>. Acesso em: 21 mai. 2018.

CORBA. **CORBA FAQ**. Disponível em: <<http://www.corba.org/faq.htm>>. Acesso em: 20 mai. 2018.

FOLDOC. **Application Program Interface**. Disponível em: <<http://foldoc.org/Application+Program+Interface>>. Acesso em: 21 mai. 2018.

SOMMERVILLE, Ian. **Engenharia de software**. 9ª ed. São Paulo: Pearson Prentice Hall, 2011.

TECMUNDO. **O que é mashup?**. Disponível em: <<https://www.tecmundo.com.br/twitter/1401-o-que-e-mashup-.htm>>. Acesso em: 20 mai. 2018.

TROYER, J. **Understanding full virtualization, paravirtualization, and hardware assist**. VMWare White Paper, VMWare, Palo Alto, CA, 2007.