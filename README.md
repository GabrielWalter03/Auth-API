# Login-Auth-API

API de autenticação e registro de usuários utilizando Spring Boot, com suporte a JWT e banco de dados H2.

## Endpoints Principais
- **POST /auth/register**: Registro de novos usuários.
  - **Exemplo de JSON**:
    ```json
    {
      "name": "John Doe",
      "email": "john.doe@example.com",
      "password": "senha123"
    }
    ```
- **POST /auth/login**: Autenticação de usuários.
  - **Exemplo de JSON**:
    ```json
    {
      "email": "john.doe@example.com",
      "password": "senha123"
    }
    ```

## Tecnologias Utilizadas
- **Spring Boot**: Framework principal.
- **Spring Security**: Gerenciamento de autenticação e autorização.
- **JWT**: Tokens para autenticação.
- **H2 Database**: Banco de dados em memória para testes.

## Como Rodar Localmente
1. Clone o repositório.
2. Configure o ambiente com Java 17.
3. Rode o comando: `./mvnw spring-boot:run`.
4. Acesse a aplicação em `http://localhost:8080`.
5. Para acessar o H2 Console: `http://localhost:8080/h2-console` (URL JDBC: `jdbc:h2:mem:testdb`).

## Autor
Projeto desenvolvido por Gabriel Walter Arantes.

