# Análise de Back-end

Esse documento tem como objetivo identificar falhas no repositório responsável pelo back-end do semestre 2022.2.


<div style="display: flex; justify-content: center; align-items:center;">
    <img src="./assets/analyze/backend.png" style="width: 30%;">
</div>

## Histórico de versões

| Data       | Versão | Descrição           | Autor(es)                               |
| ---------- | ------ | ------------------- | --------------------------------------- |
| 14/04/2023 | 1.0    | Adicionando tópicos | [@gpersijn](http://github.com/gpersijn) |
| 15/04/2023 | 1.1    | Adicionando tópico de arquitetura de microsserviços| [@lorranyoliveira](https://github.com/lorranyoliveira)[@biancasofia](https://github.com/biancasofia) |
| 16/04/2023 | 1.2    | Adicionando tópico de testes|[@biancasofia](https://github.com/biancasofia) e [@lorranyoliveira](https://github.com/lorranyoliveira) |


## 1. Problema de Execução

<p align="justify">

</p>

## 2. Arquitetura de microsserviços
<p align="justify">
O microsserviços é um tipo de arquitetura de software que visa a construção de pequenos serviços que são independentes entre si, mas que se comunicam uns com os outros utilizando APIs bem definidas. Nesse tipo de arquitetura, cada serviço realiza uma única função.
</p>

<p align="justify">
Nesse caso, o atual projeto poderia ser melhor dividido em relação a abordagem de microsserviços. Como por exemplo, atualmente a relação de cadastro de turmas, alunas, receitas, são todas realizadas em uma única API, e segundo a arquitetura de microsserviços seria melhor explorada, sendo cada uma dividida em um serviço. Isso traria uma melhor flexibilidade, escalabilidade, além de diminuir o acoplamento.
</p>


## 3. Testes

<p align="justify">
O processo de teste de software consiste em uma série de etapas para garantir que o código do programa execute sua função corretamente e não exiba um comportamento inesperado. É importante que o software seja confiável, previsível e evite surpresas desagradáveis ​​para o usuário. Os autores também definem teste como "o processo de executar um programa com a intenção de encontrar erros" (MYERS; SANDLER; BADGETT, 2011). 

Nesse sentido, os testes existentes são úteis e relevantes para testar o código da API. No entanto, por problemas de configurações do projeto, a cobertura de testes unitários não é gerada. Analisando o código, é possível notar que não há cobertura de todas as linhas, também faltam testes para o serviço de login.
</p>

## 4. Clean Code
<p align="justify">
Clean code é um conjunto de técnicas de programação, onde o código fonte fica fácil de ler, entender e manter. Ele é escrito de forma clara e concisa, seguindo boas práticas de programação, como utilizar nomes de variáveis descritivas, evitar duplicação de código e manter a simplicidade. O objetivo do clean code é maximizar a legibilidade do código e minimizar a probabilidade de erros. Um código limpo é mais fácil de manter e modificar, tornando-o mais eficiente e produtivo no longo prazo.
</p>
<p align="justify">
Nesse projeto existem diversas falhas quando falamos de clean code, existem várias linhas
duplicadas, código com uma sintaxe de dificil entendimento e mal estruturado. Uma possível
solução é reestruturar o cógigo pensando em boas práticas de programação.

</p>

## 5. Banco de Dados

## 6. Branches

## 7. Segurança e Autenticação

## Referencial teórico

MYERS, G. J.; SANDLER, C.; BADGETT, T. The art of software testing. [S.l.]: John
Wiley & Sons, 2011.
