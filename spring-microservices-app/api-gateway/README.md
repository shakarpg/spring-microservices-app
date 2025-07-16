# API Gateway

Este documento fornece uma visão geral do API Gateway do projeto de microsserviços. O API Gateway atua como um ponto de entrada único para os clientes interagirem com os diferentes serviços do sistema.

## Funcionalidade

O API Gateway é responsável por:

- Roteamento de requisições para os serviços apropriados.
- Agregação de respostas de múltiplos serviços, se necessário.
- Implementação de autenticação e autorização, se aplicável.
- Monitoramento e registro de chamadas de API.

## Rotas

As rotas disponíveis no API Gateway são configuradas no arquivo `application.yml`. As rotas principais incluem:

- `/products`: Rota para acessar o serviço de catálogo de produtos.
- `/orders`: Rota para acessar o serviço de simulação de pedidos.

## Configuração

A configuração do API Gateway é realizada no arquivo `src/main/resources/application.yml`. Este arquivo contém as definições de rotas, informações de serviço e outras configurações necessárias para o funcionamento do gateway.

## Execução

Para executar o API Gateway, siga os passos abaixo:

1. Certifique-se de que o Java e o Maven estão instalados em sua máquina.
2. Navegue até o diretório do API Gateway.
3. Execute o comando:

   ```
   mvn spring-boot:run
   ```

4. O API Gateway estará disponível em `http://localhost:8080`.

## Contribuição

Sinta-se à vontade para contribuir com melhorias ou correções. Para isso, faça um fork do repositório, crie uma branch para sua feature e envie um pull request.

## Licença

Este projeto está licenciado sob a MIT License - consulte o arquivo LICENSE para mais detalhes.