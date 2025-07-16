# Product Catalog Service

O serviço de catálogo de produtos é um dos componentes principais da aplicação de microsserviços. Ele é responsável por gerenciar as informações dos produtos disponíveis, permitindo operações como criação, listagem e busca de produtos.

## Estrutura do Projeto

A estrutura do serviço de catálogo de produtos é organizada da seguinte forma:

```
product-catalog-service
├── src
│   └── main
│       ├── java
│       │   └── com
│       │       └── example
│       │           └── productcatalog
│       │               ├── ProductCatalogApplication.java  # Classe principal do serviço
│       │               ├── controller
│       │               │   └── ProductController.java      # Controlador para gerenciar produtos
│       │               ├── model
│       │               │   └── Product.java               # Modelo de dados do produto
│       │               └── repository
│       │                   └── ProductRepository.java      # Repositório para operações de persistência
│       └── resources
│           └── application.yml                              # Configurações do serviço
```

## Funcionalidades

- **Criar Produto**: Permite adicionar um novo produto ao catálogo.
- **Listar Produtos**: Retorna uma lista de todos os produtos disponíveis.
- **Buscar Produto**: Permite buscar um produto específico pelo seu ID.

## Configuração

As configurações do serviço, incluindo informações de conexão ao banco de dados, estão localizadas no arquivo `application.yml`. Certifique-se de ajustar as configurações conforme necessário para o seu ambiente.

## Execução

Para executar o serviço de catálogo de produtos, você pode usar o comando:

```
mvn spring-boot:run
```

Certifique-se de que todas as dependências estão corretamente configuradas no seu `pom.xml`.

## Contribuição

Sinta-se à vontade para contribuir com melhorias ou correções. Para isso, faça um fork do repositório e envie um pull request com suas alterações.

## Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).