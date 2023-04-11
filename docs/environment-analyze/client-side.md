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


## 1. Site não responsivo
## 2. Features Incompletas

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

* Mesquita, V.; Alencar, F. M.; Cavalcanti, Y. (2016). Testes unitários em aplicações web utilizando mocks. Revista de Informática Teórica e Aplicada, 23(2), 37-51.

* Freeman, S.; Robson, E. (2016). Head First JavaScript Programming: A Brain-Friendly Guide. O'Reilly Media.
