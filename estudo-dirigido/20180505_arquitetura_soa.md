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

## O que é Pub/Sub?

## O que é uma API?

## REFERÊNCIAS

ALVES, Luís Cézar Darienzo. **O impacto da virtualização no desempenho de aplicações distribuídas baseadas em SOA e a sua influência nos modelos de desempenho**. Orientador: Marcos José Santana. Tese de doutorado. Universidade de São Paulo. 2013.

SOMMERVILLE, Ian. **Engenharia de software**. 9ª ed. São Paulo: Pearson Prentice Hall, 2011.

TECMUNDO. **O que é mashup?**. Disponível em: <<https://www.tecmundo.com.br/twitter/1401-o-que-e-mashup-.htm>>. Acesso em: 20 mai. 2018.

TROYER, J. **Understanding full virtualization, paravirtualization, and hardware assist**. VMWare White Paper, VMWare, Palo Alto, CA, 2007.