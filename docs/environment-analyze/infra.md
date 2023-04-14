# Análise de infra inical

## Histórico de versões

Data | Versão | Descrição | Autor(es) 
---- | ----------- | ------ | ---------
13/04/2023 | 1.0 | Adicionando tópicos 1| [@iagorrr04](http://github.com/iagorrr04)|

## 1 Pontos críticos

### 1.1 Microsserviços mal estruturados
- Dois microsserviços acessando um único banco.
- Autenticação redundante a cada requisição.

<div align="center">
<img src="assets/pain-points/fluxogram_services.png" width="400px">
</div>

- Como visualizado na imagem independente do login ou não toda requisição passava pelo processo de login novamente, comprometendo o balanceamento de carga proposto pelos microsserviços. Fora isso outro ponto é que como ambos os servições de login e <i>back-end</i> no geral acessavam o mesmo banco de dados, logo a distribuição de carga se torna ineficiente uma vez que a maior parte do tempo requisição se dá na consulta do banco.

- Devido ao ``connection pool`` ser um recurso limitado, ao ser fazer um número alto de conexões os bancos criam um sistema de `queue` e processa as conexões linearmente, o cenário se agrava ainda mais quando se tem poucas conexões, tornando o tempo de resposta de cada requisição  mais alto.


## Referencial teórico

* WIKIPEDIA Connection pool. Disponível em: https://en.wikipedia.org/wiki/Connection_pool . Acesso em 13 abr. 2023 