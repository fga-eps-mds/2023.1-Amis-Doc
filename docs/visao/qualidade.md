# Planejamento de Qualidade

## 1. Introdução
De acordo com a ISO/IEC 25010, a qualidade de um sistema é medida pelo seu grau de atendimento às necessidades declaradas e implícitas das partes interessadas, proporcionando valor. Essas necessidades dos stakeholders abrangem funcionalidade, desempenho, segurança, manutenibilidade e outros aspectos, os quais são representados no modelo de qualidade por meio de características e subcaracterísticas. Com o intuito de identificar não conformidades no projeto e estabelecer ações corretivas e preventivas, visando entregar um produto altamente satisfatório para o usuário final, este Planejamento de Qualidade abordará práticas, modelos e parâmetros que possibilitam a equipe alcançar esse objetivo.

Este documento utiliza as métricas de qualidade do SonarCloud como suporte para alcançar a qualidade do projeto, visando interpretar dados brutos e selecionar métricas relevantes para o mesmo. Além disso, estão planejados testes a serem executados, como testes unitários, de aceitação e de funcionalidade.

## 2. SonarCloud
O SonarCloud é uma plataforma de análise de código em nuvem que visa medir e melhorar a qualidade do código. Com recursos abrangentes, como verificações de código estático, análise de segurança, métricas de qualidade e integração com o GitHub, o SonarCloud é baseado no projeto de código aberto SonarQube. Ele oferece uma solução fácil de usar na nuvem, adequada para equipes de todos os tamanhos.

No contexto deste projeto, foram coletadas métricas após cada *Pull Request* submetido e mergeado. Essas métricas são combinadas para calcular os aspectos de qualidade relevantes, divididos em mantenabilidade do código e confiabilidade. Esses aspectos são essenciais para garantir a qualidade do código e auxiliar na criação de um software robusto e confiável, e conseguimos importá-los do SonarCloud buscando pelos termos *files,functions, complexity, comment_lines_density, duplicated_lines_density, coverage, ncloc, tests, test_errors, test_failures, test_execution_time, security_rating*.

### 2.1. Mantenabilidade
#### Fator *Code Quality*
Esse aspecto é importante, pois nos permite avaliar a facilidade de realizar a manutenção no código do projeto. Serão coletadas as métricas a seguir relacionadas ao fator de qualidade "Code Quality", que compõe o aspecto de manutenibilidade, a fim de avaliar a manutenibilidade do código do projeto.

**Complexidade**: Esta métrica tem como objetivo identificar a densidade de arquivos de baixa complexidade, ou seja, aqueles que estão abaixo do limite de complexidade ciclomática estabelecido (por padrão, 10). Para isso, é calculada a *Densidade de arquivos não complexos*.

**Comentários**: Esta métrica tem como objetivo avaliar a densidade de arquivos comentados. Um arquivo é considerado comentado quando a proporção de linhas comentadas está dentro do limite estabelecido (por padrão, entre 10% e 30%). Para isso, é calculada a *Densidade de arquivos comentados* e a *Densidade de linhas comentadas*.

**Duplicidade**: Esta métrica avalia a quantidade de arquivos que estão abaixo do limite estabelecido para a porcentagem de linhas duplicadas. Um arquivo é considerado sem duplicações quando a sua densidade de duplicação é, por padrão, menor que 5%. Para isso, é calculada a *Ausência de duplicações* e *Densidade de duplicação*.

### 2.2. Confiabilidade
A mensuração desse aspecto requer o cálculo do fator de qualidade chamado Testing Status. Este aspecto é importante para avaliar o quão confiável o código é em realizar as funcionalidades que se propõe.

#### Fator *Testing Status*
São necessárias três métricas para mensurar esse aspecto: *Passed Tests*, *Fast Test Builds* e *Test Coverage*. Essas métricas fornecem informações importantes para avaliar a confiabilidade do código.

- **Passed tests:** Calcula a densidade de testes unitários com sucesso. 
- **Fast Test Builds:** Tem como objetivo o cálculo das builds de teste cuja duração esteja abaixo do limite definido (300 segundos).
- **Test Coverage:** Avalia a cobertura de código do Projeto considerando os arquivos de teste unitários que estejam acima do limite definido (60% por padrão).

## 3. Testes

### 3.1. Testes Unitários
Testes unitários são pequenos blocos de código que verificam o funcionamento correto de partes específicas do programa. Eles são escritos pelos desenvolvedores para testar individualmente funções, métodos ou classes isoladas. Os testes unitários ajudam a identificar e corrigir erros de forma rápida, melhoram a qualidade do código e facilitam a manutenção e refatoração.

### Ferramentas
#### PyTest
PyTest é uma ferramenta em Python para escrever testes de forma simples e escalável. É amplamente utilizado para testar APIs, bancos de dados e interfaces do usuário. Suas vantagens incluem uma sintaxe fácil de aprender, a capacidade de executar testes em paralelo, a detecção automática de testes e ser uma ferramenta de código aberto.

#### JestJS
O Jest é uma poderosa ferramenta baseada em JavaScript utilizada para testar aplicações React, React Native e outras aplicações JavaScript. Ele resolve o problema de obter resultados precisos nos testes de unidade executados no front-end do software, proporcionando testes front-end mais rápidos e eficazes. Além disso, o Jest é capaz de validar uma ampla variedade de aspectos relacionados ao JavaScript, incluindo a renderização de aplicativos web no navegador. Com uma API intuitiva, configuração e instalação simplificadas, o Jest se tornou uma das frameworks de testes JavaScript mais populares atualmente disponíveis.

### 3.2. Teste de aceitação
O teste de aceitação é realizado para verificar se o sistema atende às expectativas do cliente ou usuário final em relação às funcionalidades e requisitos. Ele é conduzido pelo cliente ou pelo time de teste, em colaboração com o cliente, e tem como objetivo garantir que o software seja aceito e funcione corretamente antes de ser entregue para uso. Os testes são planejados e projetados com o mesmo cuidado e detalhes que o teste do sistema, utilizando casos de teste selecionados a partir do teste do sistema. É importante seguir rigorosamente os casos de teste escolhidos. Em muitas organizações, o teste de aceitação formal é automatizado.

### 3.3. Teste de funcionalidade
Os testes de funcionalidade têm como objetivo avaliar o correto funcionamento das funções do sistema, incluindo testes de unidade, integração, sistema, entre outros. Eles são especialmente focados na navegação e interações do usuário, priorizando a validação da funcionalidade do software.

## 4. Referências
> LENILDO. Qualidade de Software - Engenharia de Software 29. DEVMEDIA, 2010. Disponível em: https://www.devmedia.com.br/qualidade-de-software-engenharia-de-software-29/18209. Acesso em: 25 de maio de 2023.


> ASSOCIAÇÃO BRASILEIRA DE NORMAS TÉCNICAS. NBR ISO/IEC 25010: Systems and software engineering — Systems and software Quality Requirements and Evaluation (SQuaRE) — System and software quality models, 2011.

> Definição Pytest: Disponível em: guru99.com. Acesso em 25 de maio de 2023.

> Definição Jest. Disponível em: lambdatest.com. Acesso em 25 de maio de 2023.


### Histórico de versões

| Data | Versão | Descrição | Autor(es) |
|:- |:- |:- |:- |
| 26/05/2023 | 1.0 | Criação do documento | [@lorraynecardozo](https://github.com/LorrayneCardozo) 