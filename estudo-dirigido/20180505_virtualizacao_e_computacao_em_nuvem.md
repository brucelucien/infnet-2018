
# Virtualização e Computação em Nuvem

 - Líder
	 - Bruce
 - Secretário
	 - Anderson
 - Referências do professor
	 - https://www.redhat.com/pt-br/topics/virtualization
	 - https://www.vmware.com/br/solutions/virtualization.html
	 - https://www.infowester.com/virtualizacao.php

## Qual é a diferença entre máquina virtual e container?

A tecnologia de máquinas virtuais, frequentemente chamada de "virtualização", tem mais de 40 anos. Essa tecnologia permite que um único computador hospede múltiplas máquinas virtuais, cada uma rodando potencialmente diferentes sistemas operacionais. A vantagem dessa abordagem é que a falha em uma máquina virtual não causa a queda automática das outras máquinas virtuais. Em um sistema virtualizado diferentes servidores podem rodar em diferentes máquinas virtuais, mantendo assim um modelo de falha parcial, da mesma forma que uma abordagem com vários computadores físicos teria, mas com custo muito menor e com manutenção mais fácil. (TANEMBAUM, 2009, p. 567).

Máquinas virtuais são uma abstração de hardware físico, transformando um servidor em muitos servidores. O hypervisor permite que múltiplas máquinas virtuais rodem em uma única máquina física.  Cada máquina virtual inclui uma cópia de um sistema operacional, uma ou mais aplicações, arquivos binários e bibliotecas necessárias, ocupando dezenas de GBs e, além disso, máquinas virtuais também podem ser lentas no processo de boot. (DOCKER, 2018).

Containers são uma abstração na camada da aplicação que empacota código e dependências juntos. Multiplos containers podem rodar na mesma máquina e compartilhar o kernel do sistema operacional com outros containers, cada um rodando como um processo isolado, em um espaço de usuário separado dos demais. Containers ocupam menos espaço do que máquinas virtuais (imagens de containers tem tipicamente dezenas de MBs em tamanho) e a inicialização deles é quase que instantânea. (DOCKER, 2018).

Um *Docker container*, por exemplo, é uma instância executável de uma imagem Docker. Você pode rodar, inicializar, parar, mover ou excluir um container usando a API do Docker ou comandos via CLI. Quando você roda um container, você pode providenciar metadados de configuração como informações sobre a rede e variáveis de ambiente. Cada container é uma plataforma de aplicação isolada e segura mas pode ter acesso a recursos rodando em diferentes hosts ou containers, bem como a armazenamentos persistentes ou bancos de dados. (ACADGILD, 2018).

Complementando o parágrafo anterior, uma *imagem Docker* é um template somente leitura com instruções para criar um container Docker. Por exemplo, uma imagem pode conter um sistema operacional Ubuntu com um servidor web Apache e sua aplicação instalada. Você pode construir ou atualizar imagens do zero ou fazer o download de imagens usadas por outros. Uma imagem pode ser baseada ou extender uma ou mais outras imagens. Uma imagem Docker é descrita como um arquivo texto conhecido como *Docker file*, o qual tem uma simples e bem definida sintaxe. (ACADGILD, 2018).

## Qual a diferença entre um host físico e um virtual?

Um host físico é um host comum, servindo uma única aplicação em um único servidor web. Um host virtual utiliza a abordagem conhecida como *Virtual Hosts*.

O termo **Virtual Hosts** (ou *hosts virtuais*, em uma tradução livre) refere-se à prática de rodar mais de um site (como `company1.example.com` e `company2.example.com`, por exemplo) em uma única máquina. Virtual hosts podem ser **IP-based**, significando que você tem um IP diferente para cada web site, or **name-based**, significando que você tem múltiplos nomes rodando em cada endereço IP. O fato de que eles estão rodando no mesmo servidor físico não é perceptível para o usuário final. (APACHE, 2018)

Os Virtual Hosts (no contexto do servidor Apache) são apelidos dados ao caminho onde está rodando seu site ou aplicação web. Geralmente isso é feito em servidores de desenvolvimento para facilitar o acesso ao projeto. Por exemplo, em vez de colocar `http://localhost/sites2015/joomla3/sitesdeloja/loja10` você pode configurar o Virtual Host do servidor para simplesmente acessar com o endereço `http://loja10`. (TABLELESS, 2018).

Os hosts virtuais funcionam da seguinte forma: (ALURA, 2018).

*  Um computador faz a requisição para acessar um site pelo seu nome de domínio;
*  Esse pedido chega ao nosso servidor web que encaminha para o host virtual da requisitção, podendo ser uma pasta ou outro servidor. O servidor recebe a requisição e encaminha para o diretório que está configurado.

Uma alternativa ao Virtual Hosts (que pode ser implementando com o *Apache* ou com outro servidor web, como o *nginx*, por exemplo), seria utilizar um virtualizador, como o *VMware*, que possibilita que outros sistemas operacionais rodem em uma única máquina, de forma que seja possível colocar para rodar mais de um *servidor virtual* por máquina. (ALURA, 2018).

## O que é e como funciona o Hipervisor?

*Hypervisor* é uma camada de software entre o hardware e o sistema operacional. O hypervisor é responsável por fornecer ao sistema operacional visitante a abstração da máquina virtual. E é ele que controla o acesso dos sistemas operacionais visitantes aos dispositivos de hardware. Existem tecnologias de hardware que optimizam a execução de máquinas virtuais, dentre essas tecnologias estão *VT-d* e *AMD-V*. (GETCARD, 2018).

Existem diversos hypervisors no mercado, tanto open source quanto pago. Alguns exemplos de hypervisor são *kvm*, *hyper-v*, *vmware* e *xen*, cada um com seus prós e contras e seus custos; cabendo a um especialista ajudá-lo na decisão de qual hardware e hypervisor se enquadra melhor no seu cenário. (GETCARD, 2018).

## Quais são as vantagens e desvantagens da computação em nuvem?

### Vantagens

A maior vantagem da computação em nuvem é a **possibilidade de utilizar softwares sem que estes estejam instalados no computador**, mas há outras vantagens: (WIKIPEDIA, 2018).

* Na maioria das vezes **o usuário não precisa se preocupar com o sistema operacional e hardware que está usando em seu computador pessoal**, podendo acessar seus dados na *nuvem computacional* independentemente disso.
*  As **atualizações dos softwares são feitas de forma automática**, sem necessidade de intervenção do usuário.
*  O trabalho corporativo e o comartilhamento de arquivos se tornam mais fáceis, uma vez que **todas as informações se encontram em um mesmo *lugar***, ou seja, na *nuvem computacional*.
*  Os **softwares e os dados podem ser acessados em qualquer lugar**, basta apenas que haja acesso à internet, não são mais restritos ao ambiente local de computação, nem dependem da sincronização de mídias removíveis.
*  O usuário tem um **melhor controle de gastos** ao usar aplicativos, pois a maioria dos sistemas de computação em nuvem fornece aplicações gratuitamente e, quando não gratuitas, são pagas somente pelo tempo de utilização dos recursos. Não é necessário pagar por uma licença integral de uso de software.
*  **Diminui a necessidade de manutenção** da infraestrutura física de redes locais cliente/servidor, bem como da instalação dos softwares nos computadores corporativos, pois esta fica a cargo do provedor do software em nuvem, bastando que os computadores clientes tenham acesso à internet.
*  **A infraestrutura necessária para uma solução de computação em nuvem é bem mais enxuta do que uma solução tradicional** de hospedagem ou alojamento, consumindo menos energia, refrigeração e espaço físico e, consequentemente, contribuindo para a preservação e o uso racional dos recursos naturais.

### Desvantagens

A maior desvantagem da computação em nuvem vem de fora do propósito desta, que é o **acesso à internet**. Caso você perca o acesso, comprometerá todos os sistemas embarcados. Outras desvantagens são: (WIKIPEDIA, 2018).

*  **Velocidade de processamento**: caso seja necessária uma grande taxa de transferência, se a internet não possuir uma banda de qualidade, o sistema pode ser comprometido. Um exemplo típico é com mídias digitais ou jogos.
*  Assim como todo tipo de serviço, ele é **custeado**.

No que se refere ao custo, para cada ação realizada pela empresa, existe um custo a ser adicionado no orçamento. No caso da computação em nuvem não seria diferente, já que você terá de contratar um servidor para atender especificamente às necessidades de seus colaboradores e da organização como um todo. Assim, é importante verificar qual a solução ideal, para não gastar excessivamente. (MARQUES, 2018).

Outra desvantagem referese à **segurança**. Apesar dos arquivos serem criptografados, a partir do momento em que são armazenados na nuvem, muitas pessoas ainda sentem-se inseguras ao salvarem seus dados nestas ferramentas. Isso porque, seus usuários podem sofrer ataques de cibercriminosos e ter logins e senhas capturados, o que pode gerar um grande transtorno para a empresa no futuro. (MARQUES, 2018).

## Qual é a associação entre computação em nuvem e virtualização?

## Faça uma analogia entre virtualização e contêiner.

## REFERÊNCIAS

ACADGILD. **What is Docker container - an introduction**. Disponível em: <<https://acadgild.com/blog/what-is-docker-container-an-introduction>>. Acesso em: 20 mai. 2018.

ALURA. **Como configurar Virtual Hosts no Apache**. Disponível em: <<http://blog.alura.com.br/como-configurar-virtual-hosts-no-apache/>>. Acesso em: 20 mai. 2018.

APACHE. **Apache Virtual Host documentation**. Disponível em: <<https://httpd.apache.org/docs/2.4/vhosts/>>. Acesso em: 20 mai. 2018.

DOCKER. **What is a container**: a standardized unit of software. Disponível em: <<https://www.docker.com/what-container>>. Acesso em: 20 mai. 2018.

GETCARD. **O que é um hypervisor?**. Disponível em: <<http://www.getcard.com.br/novo/o-que-e-um-hypervisor/>>. Acesso em: 20 mai. 2018.

MARQUES, **Marcus. Vantagens e desvantagens da computação em nuvem para o seu negócio**. Disponível em: <<http://marcusmarques.com.br/estrategias-de-negocio/vantagens-desvantagens-computacao-em-nuvem-negocio/>>. Acesso em: 20 mai. 2018.

TABLELESS. **Como automatizar a criação de Virtual Hosts**. Disponível em: <<https://tableless.com.br/como-automatizar-criacao-de-virtual-hosts/>>. Acesso em: 20 mai. 2018.

TANENBAUM, Andrew S. **Modern operating systems**. 3ª ed. Upper Saddle River: Pearson Prentice Hall, 2009.

WIKIPEDIA. **Computação em nuvem**. Disponível em: <<https://pt.wikipedia.org/wiki/Computa%C3%A7%C3%A3o_em_nuvem>>. Acessível em: 20 mai. 2018.





