# API de Comércio com Spring Boot

Este repositório contém uma API de Comércio desenvolvida em Java com Spring Boot para gerenciar clientes, produtos e pedidos. A API oferece um conjunto completo de operações CRUD e integra diversas tecnologias e ferramentas para garantir segurança, eficiência e facilidade de uso.

## Funcionalidades

- **Operações CRUD:** Gerenciamento completo de clientes, produtos e pedidos.
- **Autenticação e Autorização:** Utilização de Spring Security e JWT (JSON Web Token) para autenticação e autorização.
- **Validação:** Implementação de Bean Validation para garantir que os dados recebidos nas requisições sejam válidos.
- **Documentação:** Documentação completa da API utilizando Swagger.

## Tecnologias Utilizadas

- Spring Boot
- Spring Data JPA
- Spring Security
- JWT (JSON Web Token)
- MySQL
- Swagger

## Como Executar o Projeto

### Pré-requisitos

- Java 17 ou superior
- Maven
- MySQL

### Passo a Passo

1.**Clone o repositório**

2. **Configure o banco de dados:**  
   Crie um banco de dados MySQL com o nome vendas e configure as credenciais no arquivo `application.properties`:

   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/vendas
   spring.datasource.username=seu-usuario
   spring.datasource.password=sua-senha
   spring.jpa.hibernate.ddl-auto=update


properties
Copiar código
spring.datasource.url=jdbc:mysql://localhost:3306/commerce_db
spring.datasource.username=seu-usuario
spring.datasource.password=sua-senha
spring.jpa.hibernate.ddl-auto=update

3. **Instale as dependências e compile o projeto:**
    ```properties
   mvn clean install

## Endpoints Principais

### Clientes

- **GET /clientes**: Retorna todos os clientes
- **GET /clientes/{id}**: Retorna um cliente específico
- **POST /clientes**: Adiciona um novo cliente
- **PUT /clientes/{id}**: Atualiza um cliente existente
- **DELETE /clientes/{id}**: Remove um cliente

### Produtos

- **GET /produtos**: Retorna todos os produtos
- **GET /produtos/{id}**: Retorna um produto específico
- **POST /produtos**: Adiciona um novo produto
- **PUT /produtos/{id}**: Atualiza um produto existente
- **DELETE /produtos/{id}**: Remove um produto

### Pedidos

- **GET /pedidos**: Retorna todos os pedidos
- **GET /pedidos/{id}**: Retorna um pedido específico
- **POST /pedidos**: Adiciona um novo pedido
- **PUT /pedidos/{id}**: Atualiza um pedido existente
- **DELETE /pedidos/{id}**: Remove um pedido
