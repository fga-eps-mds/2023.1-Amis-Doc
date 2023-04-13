# Análise de Front-end
Esse documento tem como objetivo identificar falhas no repositório responsável pelo front-end do semestre 2022.2.
<br></br>
<div style="display: flex; justify-content: center; align-items:center;">
    <img src="./assets/analyze/client-side.svg">
</div>

## Histórico de versões

Data | Versão | Descrição | Autor(es) 
---- | ----------- | ------ | ---------
10/04/2023 | 1.0 | Adicionando tópicos| [@dansousamelo](http://github.com/dansousamelo)|
11/04/2023 | 1.1 | Adicionando tópico 3| [@dansousamelo](http://github.com/dansousamelo)|
12/04/2023 | 1.2 |Adicionando tópico 1| [@malu214](http://github.com/marialuisa214)
12/04/2023 | 1.3 |Adicionando tópico 2| [@gaubiela](https://github.com/gaubiela)


## 1. Site não responsivo
<p align="justify">Com mais pessoas usando smartphones e tablets para tarefas que antes eram possíveis apenas no desktop, é cada vez mais importante criar um site que funcione em várias plataformas e atenda às necessidades e requisitos dos clientes.</p>

<p align="justify">Neste cenário, o <em>site responsivo</em> é um método de projetar e codificar um site de forma que ele forneça uma experiência de visualização privilegiada em uma ampla gama de dispositivos, de telefones celulares a computadores desktop.</p>

<p align="justify">Portanto ao aplicar no site a <i>responsividade</i> a partir do  <i>front-end</i>, pode-se facilitar a inclusão de ferramentas de acessibilidade para os usuários, facilitando a navegação em telas de diferentes tamanhos.</p>


## 2. Features Incompletas
<p align="justify">Uma feature incompleta é um termo utilizado no desenvolvimento de software para descrever uma funcionalidade que não está totalmente implementada ou que não atende completamente às necessidades do usuário final. Isso pode ocorrer por uma série de motivos, como falta de tempo, recursos ou compreensão inadequada dos requisitos do usuário..</p>

<p align="justify">No projeto front-end atual é possível identificar features incompletas problemáticas, que levam o software a não atender as expectativas do usuário. Além disso, dificulta o desenvolvimento de outras partes do software que dependem dela para funcionar.</p>

<p align="justify">Um exemplo de feature incompleta é a funcionalidade que permite ao usuário a recuperação de sua senha pessoal na área de acesso a conta, que é representada no front-end, mas não possui funcinalidade alguma implementada. Segue imagem ilustrativa que indica o local sem a funcionalidade implementada.</p>

<div width="100%" display = "flex" align="center">
<img src="./assets/pain-points/imagem_indicativa_featureincompleta1.jpg" width="450">
</div>

<p align="justify">Há também botões não funcionais na página home.
Segue imagem indicativa.</p>

<div width="100%" display = "flex" align="center">
<img src="./assets/pain-points/imagem_indicativa_featureincompleta2.png" width="450">
</div>


## 3. Alta dependência de um backend real

<p align="justify">Para que possamos entender o que está acontecendo dentro do sistema precisamos que o <i>back-end</i> esteja funcionando perfeitamente, para resolver esse problema podemos utilizar <i>mocks</i> além de auxiliar na elaboração de testes.</p>

<p align="justify"><i>Mocks</i> são utilizados para simular comportamentos de objetos ou funções, de modo a garantir a consistência e a qualidade do <i>software</i>. No contexto do <i>front-end</i>, os <i>mocks</i> podem ser utilizados para simular a comunicação com a <i>API</i> ou com outros serviços externos, por exemplo.</p>

<p align="justify">Ao utilizar <i>mocks</i> no <i>front-end</i>, é possível testar a lógica da aplicação sem a necessidade de executar todos os serviços externos que a aplicação precisa se comunicar, o que pode ser demorado e propenso a erros. Além disso, os <i>mocks</i> permitem que o desenvolvedor teste cenários específicos, como falhas de conexão ou respostas inesperadas do servidor, que podem ser difíceis de simular de outra forma.</p>

<p align="justify">Em resumo, utilizar <i>mocks</i> no <i>front-end</i> pode ajudar a aumentar a eficiência e a qualidade dos testes automatizados, permitindo que o desenvolvedor teste a lógica da aplicação de forma mais rápida e precisa.</p>

## 4. Padrões de usabilidade incompletos

Ex: Não existe página 404, 500, por exemplo, toast e etc.

## 5. Acessibilidade

## 6. Guia de estilo

## 7. Má gerência em gerenciar usuários logados

## Referencial teórico

* MARCOTTE, Ethan. Responsive Web Desing. New York: A Book Apart, 2011.

* Mesquita, V.; Alencar, F. M.; Cavalcanti, Y. (2016). Testes unitários em aplicações web utilizando mocks. Revista de Informática Teórica e Aplicada, 23(2), 37-51.

* Freeman, S.; Robson, E. (2016). Head First JavaScript Programming: A Brain-Friendly Guide. O'Reilly Media.

* ZEMEL, Tárcio. Web Design Responsivo: páginas adaptáveis para todos os dispositivos. São Paulo: Casado Código, 2013.

* MANNING, Jeff. Incomplete feature. In: LiveBook. Disponível em: https://livebook.manning.com/concept/agile/incomplete-feature. Acesso em: 12 abr. 2023.
