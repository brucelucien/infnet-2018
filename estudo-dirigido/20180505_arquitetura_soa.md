# Arquitetura SOA

 - Líder
	 - Eduardo
 - Secretário
	 - Leonardo
 - Referências do professor
	 - Larman, Pressman, Sommerville.
	 - Fox, Armando e Paterson, David. Construindo Software como Serviço – Uma Abordagem Ágil Usando Computação em Nuvem, Strawberry Canyon LLC, 2015.

## O que é SOA?

SOA é um estilo de arquitetura de TI que dá suporte à transformação de um negócio em um conjunto de serviços, encadeados, que podem ser acessados através de uma rede. (ALVES, 2013, p. 8).

SOA se apresenta como uma evolução da orientação a objetos e da componentização dos mesmos e caracteriza-se pelo fraco acomplamento, transparência de localização e independência de protocolos. (ALVES, 2013, p. 8).

É importante observar que SOA é uma arquitetura conceitual, que **define serviço como um processo de negócio implementado em software**, que a partir de um **conjunto de entradas** fornece um **conjunto de saídas**, baseado em uma **função de transformação**. Esta função de transformação é conhecida pelo solicitante, uma vez que é descrita através de uma **interface formal**. (ALVES, 2013, p. 8).

Um serviço possui três camadas: (ALVES, 2013, p. 8).

*  **CAMADA DE NEGÓCIOS**: define os serviços mediante as necessidades da organização, independente das tecnologias que serão utilizadas. É nesta camada que é realizada a descrição das composições dos serviços.
*  **CAMADA DE INTERFACE**: descrevem o serviço, sendo estas publicadas em um serviço de registro, tornando-se disponível para os consumidores.
*  **CAMADA DE IMPLEMENTAÇÃO**: contém a implementação do software posteriormente mapeado em serviço. Tais aplicações podem ser desenvolvidas em diferentes plataformas de desenvolvimento e estar distribuídas em diferentes provedores.

## O que é CORBA?

## O que é Pub/Sub?

## O que é uma API?

## REFERÊNCIAS

ALVES, Luís Cézar Darienzo. O impacto da virtualização no desempenho de aplicações distribuídas baseadas em SOA e a sua influência nos modelos de desempenho. Orientador: Marcos José Santana. Tese de doutorado. Universidade de São Paulo. 2013.

TROYER, J. **Understanding full virtualization, paravirtualization, and hardware assist**. VMWare White Paper, VMWare, Palo Alto, CA, 2007.