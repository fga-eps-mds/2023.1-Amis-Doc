# Análise de Front-end
Esse documento tem como objetivo identificar falhas no repositório responsável pelo front-end do semestre 2022.2.
<br></br>
<div style="display: flex; justify-content: center; align-items:center;">
    <img src="./assets/analyze/client-side.svg">
</div>


## 1. Site não responsivo
<p align="justify">Com mais pessoas usando smartphones e tablets para tarefas que antes eram possíveis apenas no desktop, é cada vez mais importante criar um site que funcione em várias plataformas e atenda às necessidades e requisitos dos clientes.</p>

<p align="justify">Neste cenário, o <em>site responsivo</em> é um método de projetar e codificar um site de forma que ele forneça uma experiência de visualização privilegiada em uma ampla gama de dispositivos, de telefones celulares a computadores desktop.</p>

<p align="justify">Portanto ao aplicar no site a <i>responsividade</i> a partir do  <i>front-end</i>, pode-se facilitar a inclusão de ferramentas de acessibilidade para os usuários, facilitando a navegação em telas de diferentes tamanhos.</p>


## 2. Features Incompletas
<p align="justify">Uma feature incompleta é um termo utilizado no desenvolvimento de software para descrever uma funcionalidade que não está totalmente implementada ou que não atende completamente às necessidades do usuário final. Isso pode ocorrer por uma série de motivos, como falta de tempo, recursos ou compreensão inadequada dos requisitos do usuário..</p>

<p align="justify">No projeto <i>front-end</i> atual é possível identificar features incompletas problemáticas, que levam o software a não atender as expectativas do usuário. Além disso, dificulta o desenvolvimento de outras partes do software que dependem dela para funcionar.</p>

<p align="justify">Um exemplo de feature incompleta é a funcionalidade que permite ao usuário a recuperação de sua senha pessoal na área de acesso a conta, que é representada no <i>front-end</i>, mas não possui funcinalidade alguma implementada. Segue imagem ilustrativa que indica o local sem a funcionalidade implementada.</p>

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

<p align="justify"> Criar um site que funcione sem erros e preveja as ações do usuário é uma tarefa complexa, e é comum ocorrerem erros de requisição para o backend e problemas de usabilidade. Esses erros podem prejudicar a experiência do usuário e afetar a impressão geral do site.

<p align="justify"> Para melhorar a usabilidade do site e ajudar a aumentar a satisfação do usuário, reduzir a taxa de abandono e facilitar a identificação de bugs pelos desenvolvedores, é recomendado implementar algumas funcionalidades. Uma delas é utilizar toasts de sucesso/erro para indicar quando ocorrem requisições para o backend. Isso permite que os usuários e desenvolvedores estejam cientes do funcionamento da plataforma e possam identificar problemas com mais facilidade.

<p align="justify"> Outra funcionalidade importante é criar páginas de erro personalizadas 404 para quando o usuário acessa uma URL inexistente. Essas páginas fornecem uma mensagem mais amigável e útil para o usuário, em vez de apenas uma mensagem genérica de erro. Isso ajuda a melhorar a experiência do usuário e pode incentivá-lo a continuar navegando pelo site.

<p align="justify"> Em resumo, ao implementar essas funcionalidades, é possível melhorar a usabilidade do site, reduzir a taxa de abandono e aumentar a satisfação do usuário. Além disso, os desenvolvedores podem identificar bugs com mais facilidade, o que ajuda a manter a plataforma funcionando corretamente.

## 5. Acessibilidade UI/UX
<p align="justify">Acessibilidade UI/UX refere-se ao design de experiência do usuário e interface do usuário com o objetivo de tornar o produto digital acessível a todos os usuários, independentemente de suas habilidades, limitações ou deficiências. Isso envolve garantir que as pessoas possam acessar e usar um produto digital sem obstáculos ou dificuldades adicionais.</p>

<p align="justify">Para projetar uma experiência UI/UX acessível, é importante que os designers e desenvolvedores considerem as necessidades e limitações de todos os usuários. O desenvolvimento de.</p>

<p align="justify">Garantir a acessibilidade UI/UX em um produto não é apenas uma questão de responsabilidade social, mas também pode ser uma vantagem competitiva para as empresas. Produtos digitais que são acessíveis a todos os usuários podem aumentar a base de usuários e a satisfação do cliente.</p>

<p align="justify">O desenvolvimento do projeto AMIS, não tem abordado a problemática problemática de acessibilidade UI/UX. Tendo em vista o público da aplicação a ser desenvolvida é possível considerar de suma importância a necessidade de uma atenção maior a esse tema.</p>

## 6. Guia de estilo

<p align="justify"> Com base em uma análise inicial do produto foi possível perceber que não foi definido um guia de estilo para ser seguido. Um guia de estilo é uma importante ferramenta para auxiliar na construção de um serviço digital consistente, independente do seu alcance, número de páginas ou micro serviços. Além disso, um guia de estilo pode servir como uma ferramenta de comunicação entre os membros da equipe de design e a equipe de desenvolvimento (Barbosa e Silva, 2010).</p>

Pensando-se nesse notoriedade será criado um guia de estilo para o site que pode ser acessado na aba [Visual](/visual/guia-estilo). 

## 7. Má gerência em gerenciar usuários logados
<p>Na autenticação por <i>token</i>, o usuário insere login e senha na plataforma, o que gera um token —certificado digital— que o permite navegar pelos recursos do seu interesse, dentro de um prazo determinado, sem a necessidade de utilizar os dados do login novamente.</p>

 <p align="justify">Nela o <i>token</i> funciona como um mecanismo que facilita o controle de acesso. Uma vez que os tokens trazem uma série de benefícios para o usuário, por exemplo, a possibilidade de salvar as informações do cliente no próprio <i>token</i>, e não no servidor, o que dificulta o acesso de pessoas não autorizadas.</p>

<p align="justify">O token pode ser configurado de acordo com as suas necessidades, podendo conceder as autorizações devidas, pelo prazo de que necessfor necessario. Após o período de vencimento, o token para de funcionar, impedindo que o usuário continue acessando o sistema.</p>

<p align="justify">Neste sentido, o <i>front-end</i> pode desempenhar um papel na geração de tokens, o que geralmente envolve apenas a captura das credenciais de login do usuário e o envio dessas informações para o servidor para processamento. Depois que o <i>token<i> é gerado no servidor, ele pode ser retornado ao <i>front-end</i> e armazenado de forma segura para uso posterior em solicitações subsequentes.</p>

 

## Referencial teórico
* MANNING, Jeff. Incomplete feature. In: LiveBook. Disponível em: https://livebook.manning.com/concept/agile/incomplete-feature. Acesso em: 12 abr. 2023.

* MARCOTTE, Ethan. Responsive Web Desing. New York: A Book Apart, 2011.

* Mesquita, V.; Alencar, F. M.; Cavalcanti, Y. (2016). Testes unitários em aplicações web utilizando mocks. Revista de Informática Teórica e Aplicada, 23(2), 37-51.

* Freeman, S.; Robson, E. (2016). Head First JavaScript Programming: A Brain-Friendly Guide. O'Reilly Media.

* Hand Talk. (2022). UX/UI design acessível: tudo o que você precisa saber. https://www.handtalk.me/br/blog/uxui-design-acessivel-tudo-o-que-voce-precisa-saber/. Acesso em: 12 abr. 2023.

* STALLINGS, W. Criptografia e segurança de redes: princípios e práticas. 6. ed. São Paulo: PEARSON, 2014.

* ZEMEL, Tárcio. Web Design Responsivo: páginas adaptáveis para todos os dispositivos. São Paulo: Casado Código, 2013.

* BARBOSA, S. D. J.; SILVA, B. S. Interação Humano-Computador. Rio de Janeiro: Elsevier, 2010.


## Histórico de versões

Data | Versão | Descrição | Autor(es) 
---- | ----------- | ------ | ---------
10/04/2023 | 1.0 | Adicionando tópicos| [@dansousamelo](http://github.com/dansousamelo)|
11/04/2023 | 1.1 | Adicionando tópico 3| [@dansousamelo](http://github.com/dansousamelo)|
12/04/2023 | 1.2 |Adicionando tópico 1| [@malu214](http://github.com/marialuisa214)
12/04/2023 | 1.3 |Adicionando tópico 2| [@gaubiela](https://github.com/gaubiela)
12/04/2023 | 1.4 |Adicionando tópico 5| [@gaubiela](https://github.com/gaubiela)
12/04/2023 | 1.5 |Adicionando tópico 7| [@malu214](http://github.com/marialuisa214)
16/04/2023 | 1.6 |Adicionando tópico 6| [@Peh099](https://github.com/Peh099)
18/04/2023 | 1.7 |Adicionando tópico 4| [@FHansen98](https://github.com/FHansen98)
