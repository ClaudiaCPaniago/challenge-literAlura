## Challenge LiterAlura

O **LiterAlura** é um sistema de catálogo de livros interativo, desenvolvido em Java com **Spring Boot**, que realiza consultas em tempo real à **API Gutendex** para buscar informações de mais de 70 mil obras do Projeto Gutenberg. Os dados são armazenados em um banco **PostgreSQL** e manipulados por meio de uma interface textual (via console).


##  Funcionalidades

-  Buscar livro pelo título  
-  Listar livros registrados  
-  Listar autores registrados  
-  Listar autores vivos em um determinado ano  
- Listar livros por idioma



##  Tecnologias Utilizadas

- Java 17+  
- Spring Boot 3.2.3  
- Spring Data JPA  
- PostgreSQL 16+  
- Jackson Databind  
- Maven 4+  


##  Requisitos para Executar

Antes de iniciar, verifique se você tem o ambiente configurado:

1. **Java JDK 17 ou superior**
2. **Maven 4 ou superior**
3. **Spring Boot 3.2.3**
4. **PostgreSQL 16 ou superior**


##  Instruções de Instalação

### 1. Clone o repositório:

```bash
git clone https://github.com/seu-usuario/literalura.git
cd literalura
```

### 2. Configure o banco de dados PostgreSQL:

Crie um banco de dados chamado `literalura`.

### 3. Atualize o arquivo `src/main/resources/application.properties` com suas credenciais:

```properties
spring.datasource.url=jdbc:postgresql://localhost/literalura
spring.datasource.username=SEU_USUARIO
spring.datasource.password=SUA_SENHA
spring.datasource.driver-class-name=org.postgresql.Driver

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true
spring.jpa.database-platform=org.hibernate.dialect.PostgreSQLDialect
```

### 4. Instale as dependências:

```bash
mvn clean install
```

### 5. Execute a aplicação:

```bash
mvn spring-boot:run
```



