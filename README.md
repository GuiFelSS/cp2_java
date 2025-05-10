# API de Gerenciamento de Brinquedos

**Checkpoint 2 - Programação Spring Boot com Persistência**

Este projeto é uma API REST desenvolvida em **Spring Boot** para gerenciar brinquedos de uma empresa, com operações básicas de **CRUD** (Create e Read) e persistência em um banco de dados **Oracle**.

## 📌 Tecnologias Utilizadas
- **Java 21**
- **Spring Boot 3.4.5**
- **Spring Data JPA**
- **Oracle Database** (via JDBC)
- **Lombok** (para redução de boilerplate)
- **Maven** (gerenciamento de dependências)

## ⚙️ Configuração do Projeto

### Pré-requisitos
1. **Oracle Database**
2. **JDK 21+**
3. **Maven**

### Configuração do Banco de Dados
Edite o arquivo `src/main/resources/application.properties`:
```properties
spring.application.name=brinquedos-api
spring.datasource.url=jdbc:oracle:thin:@oracle.fiap.com.br:1521:ORCL
spring.datasource.username=****
spring.datasource.password=****
spring.datasource.driver-class-name=oracle.jdbc.OracleDriver
spring.jpa.show-sql=true
spring.jpa.hibernate.ddl-auto=update
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.OracleDialect
