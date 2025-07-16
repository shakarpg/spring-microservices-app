# Order Simulator Service

O serviço de simulação de pedidos é um componente essencial do sistema de catálogo de produtos. Ele é responsável por gerenciar a criação e listagem de pedidos, interagindo com o serviço de catálogo de produtos para obter informações sobre os produtos disponíveis.

## Estrutura do Projeto

O serviço de simulação de pedidos é organizado da seguinte forma:

- **OrderSimulatorApplication.java**: Classe principal que inicializa a aplicação Spring Boot.
- **controller**: Pacote que contém a classe `OrderController`, responsável por gerenciar as operações relacionadas a pedidos.
- **model**: Pacote que contém a classe `Order`, que representa o modelo de dados de um pedido.

## API

### Endpoints

- **POST /orders**: Cria um novo pedido.
  - **Request Body**: Um objeto JSON representando o pedido, incluindo informações como produto e quantidade.
  
- **GET /orders**: Lista todos os pedidos.
  - **Response**: Um array de objetos JSON representando os pedidos existentes.

## Configuração

O serviço de simulação de pedidos utiliza um arquivo de configuração `application.yml` para definir as propriedades necessárias, como informações de conexão ao banco de dados e configurações específicas do serviço.

## Execução

Para executar o serviço de simulação de pedidos, siga os passos abaixo:

1. Certifique-se de que o ambiente de desenvolvimento está configurado com o JDK e Maven.
2. Navegue até o diretório do serviço de simulação de pedidos.
3. Execute o comando `mvn spring-boot:run` para iniciar a aplicação.

## Contribuição

Sinta-se à vontade para contribuir com melhorias ou correções. Para isso, faça um fork deste repositório, crie uma nova branch e envie um pull request com suas alterações.

## Licença

Este projeto está licenciado sob a MIT License. Veja o arquivo LICENSE para mais detalhes.