# Barber Shop API

## Descrição
Este projeto é uma API para gerenciamento de uma barbearia, desenvolvida utilizando Java, Spring Boot, e Gradle. A API permite o gerenciamento de clientes e agendamentos.

## Tecnologias Utilizadas
- Java
- Spring Boot
- Gradle
- SQL
- MapStruct

## Estrutura do Projeto
- `src/main/java`: Contém o código fonte principal da aplicação.
  - `br/com/dio/barbershopui/controller`: Contém os controladores REST.
  - `br/com/dio/barbershopui/entity`: Contém as entidades JPA.
  - `br/com/dio/barbershopui/mapper`: Contém os mapeadores MapStruct.
  - `br/com/dio/barbershopui/repository`: Contém os repositórios JPA.
  - `br/com/dio/barbershopui/service`: Contém as classes de serviço.
- `src/main/resources`: Contém os arquivos de configuração.
  - `application.yml`: Configurações do Spring Boot.

## Configuração
1. Clone o repositório:
   ```sh
   git clone <URL_DO_REPOSITORIO>
   ```
2. Navegue até o diretório do projeto:
   ```sh
   cd barber-shop-api
   ```
3. Configure as variáveis de ambiente no arquivo `application.yml`:
   ```yaml
   spring:
     datasource:
       url: ${DB_URL}
       username: ${DB_USER}
       password: ${DB_PASSWORD}
   ```

## Executando a Aplicação
Para executar a aplicação, utilize o comando:
```sh
./gradlew bootRun
```

## Endpoints Principais
- **Clientes**
  - `POST /clients`: Cria um novo cliente.
  - `GET /clients`: Lista todos os clientes.
  - `GET /clients/{id}`: Obtém os detalhes de um cliente específico.
  - `PUT /clients/{id}`: Atualiza um cliente existente.
  - `DELETE /clients/{id}`: Remove um cliente.

- **Agendamentos**
  - `POST /schedules`: Cria um novo agendamento.
  - `GET /schedules`: Lista todos os agendamentos.
  - `GET /schedules/{id}`: Obtém os detalhes de um agendamento específico.
  - `PUT /schedules/{id}`: Atualiza um agendamento existente.
  - `DELETE /schedules/{id}`: Remove um agendamento.

## Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests.

## Licença
Este projeto está licenciado sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.
