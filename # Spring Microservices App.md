# Spring Microservices App

Este projeto é um sistema simples de catálogo de produtos e simulação de pedidos, desenvolvido como parte do desafio da DIO. Ele utiliza arquitetura de microsserviços com Spring Boot e Spring Cloud, integrando API Gateway e Service Discovery.

## Funcionalidades

- Cadastro, consulta, atualização e remoção de produtos via API REST.
- Simulação de pedidos em microsserviço separado.
- Descoberta de serviços com Service Discovery (Eureka).
- Roteamento de requisições via API Gateway.
- Persistência dos dados utilizando Spring Data JPA e banco H2 (memória).
- Estrutura pronta para expansão.

## Estrutura do Projeto

```
spring-microservices-app/
├── product-catalog-service/
│   ├── src/main/java/com/example/productcatalog/
│   │   ├── controller/ProductController.java
│   │   ├── model/Product.java
│   │   └── repository/ProductRepository.java
│   └── src/main/resources/application.properties
├── order-simulator-service/
│   ├── src/main/java/com/example/ordersimulator/
│   │   ├── controller/OrderController.java
│   │   ├── model/Order.java
│   │   └── repository/OrderRepository.java
│   └── src/main/resources/application.properties
├── api-gateway/
│   ├── src/main/java/com/example/apigateway/
│   │   └── ApiGatewayApplication.java
│   └── src/main/resources/application.properties
├── service-discovery/
│   ├── src/main/java/com/example/servicediscovery/
│   │   └── ServiceDiscoveryApplication.java
│   └── src/main/resources/application.properties
├── target/
├── pom.xml
└── README.md
```

## Como executar

1. Clone o repositório:
   ```shell
   git clone https://github.com/seu-usuario/spring-microservices-app.git
   ```
2. Entre na pasta de cada microsserviço e execute:
   ```shell
   mvn spring-boot:run
   ```
3. Acesse a API Gateway em: [http://localhost:8080](http://localhost:8080)

## Exemplos de Endpoints

- `GET /products` - Lista todos os produtos
- `GET /orders` - Lista todos os pedidos
- Outros endpoints conforme documentação dos microsserviços

## Tecnologias Utilizadas

- Java 11
- Spring Boot 2.5.4
- Spring Cloud (Eureka, Gateway)
- Spring Data JPA
- H2 Database
- Maven

---

Sinta-se livre para modificar e expandir este projeto conforme sua criatividade!