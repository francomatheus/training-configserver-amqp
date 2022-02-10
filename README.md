# Como atualizar arquivo de configuração do Spring


>Este projeto foi construido para entender o processo de atualização dos arquivos de configurações das aplicações spring boot e a aplicação em tempo de execução atualizar as configuração sem a necessidade de reiniciar.

## O que contém: 

- Spring cloud config server
- spring cloud config client

## Como funciona:

- Há duas formas de atualizar o arquivo de configuração: 
  - Forma manual
  - Utilizando message-broker

## Explicação das formas de atualização: 

### Forma Manual

- Entenda como forma manual, há necessidade de ir serviço por serviço e realizar uma requisição para o serviço atualizar.

A seguir uma imagem para representar: 

![](https://github.com/francomatheus/training-configserver-amqp/blob/main/image/processo-manual.png)


### Utilizando message-broker

- Essa forma facilita um pouco quando se tem vários microsserviços no seu ambiente. Através da utilização de um message-broker, pode ser RabbitMQ ou Kafka, haverá uma comunicação com os microsserviços que irá consequentemente atualizar as propriedades

A seguir uma imagem para representar a estrutura: 

![](https://github.com/francomatheus/training-configserver-amqp/blob/main/image/spring-cloud-config-rabbitmq.png)
