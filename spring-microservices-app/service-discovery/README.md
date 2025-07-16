# Serviço de Descoberta

Este repositório contém a implementação do serviço de descoberta, que é uma parte fundamental da arquitetura de microsserviços. O serviço de descoberta permite que os microsserviços se registrem e descubram uns aos outros, facilitando a comunicação entre eles.

## Estrutura do Projeto

O serviço de descoberta é implementado utilizando o Spring Boot e está organizado da seguinte forma:

```
service-discovery
├── src
│   └── main
│       ├── java
│       │   └── com
│       │       └── example
│       │           └── servicediscovery
│       │               └── ServiceDiscoveryApplication.java
│       └── resources
│           └── application.yml
└── README.md
```

## Configuração

Para configurar o serviço de descoberta, você deve editar o arquivo `application.yml` localizado em `src/main/resources/`. Este arquivo contém as configurações necessárias para o registro e descoberta de serviços.

## Execução

Para executar o serviço de descoberta, você pode usar o comando:

```
mvn spring-boot:run
```

Certifique-se de que todas as dependências estão corretamente configuradas no seu arquivo `pom.xml`.

## Dependências

O serviço de descoberta utiliza as seguintes dependências:

- Spring Boot
- Spring Cloud
- Eureka Server

## Contribuição

Sinta-se à vontade para contribuir com melhorias ou correções. Para isso, faça um fork do repositório e envie um pull request com suas alterações.

## Licença

Este projeto está licenciado sob a MIT License. Veja o arquivo LICENSE para mais detalhes.