# Aplicação CRUD com Spring Boot e PostgreSQL
Este repositório contém uma aplicação simples de CRUD (Create, Read, Update, Delete) desenvolvida usando Spring Boot e PostgreSQL. O projeto é baseado em um tutorial da Fernanda Kipper e tem como objetivo demonstrar as operações fundamentais de uma API RESTful com um banco de dados relacional.

## Funcionalidades
- Spring Boot: Framework utilizado para criar aplicações Spring autônomas e prontas para produção.
- PostgreSQL: Banco de dados relacional usado para armazenar e gerenciar dados.
- Operações CRUD: Implementação de operações básicas para criar, ler, atualizar e deletar registros.
- API RESTful: Princípios REST são utilizados para expor as operações CRUD como endpoints.

## Começando
### Pré-requisitos
- Java 17
- Maven 3.6+
- PostgreSQL 12+
- Git

### Instalação
1. Clone o repositório:
```
git clone https://github.com/juanmatias1/crud-spring-boot.git
```
```
cd crud-spring-boot
```
2. Configure o banco de dados PostgreSQL:
##### Certifique-se de que você tem o PostgreSQL instalado e em execução. Crie um novo banco de dados para este projeto.
```
CREATE DATABASE product;
```
3. Atualize o application.properties:
##### Atualize o arquivo src/main/resources/application.properties com as credenciais do seu banco de dados PostgreSQL:
```
spring.datasource.url=jdbc:postgresql://localhost:5432/product
spring.datasource.username=usuario_db
spring.datasource.password=senha_db
```

4. Construa e execute a aplicação:
```
mvn clean install
mvn spring-boot:run
```

### Uso
#### Uma vez que a aplicação esteja em execução, você pode interagir com ela através dos seguintes endpoints:

- Criar: POST /product - Adicionar uma nova entidade.
- Ler Todas: GET /product - Recuperar todas as entidades.
- Atualizar: PUT /product - Atualizar uma entidade existente pelo ID no JSON.
- Deletar: DELETE /product{id} - Deletar uma entidade pelo ID.

### Contribuindo
#### Sinta-se à vontade para fazer um fork deste repositório e enviar pull requests. Quaisquer melhorias, correções de bugs ou sugestões são bem-vindas.

### Agradecimentos
- Fernanda Kipper pelo tutorial que guiou o desenvolvimento deste projeto.
