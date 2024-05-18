# Project Management System

## Overview
This Project Management System is a RESTful API built using Java 17 and Spring Boot. It allows users to perform CRUD (Create, Read, Update, Delete) operations on projects. The application uses an H2 in-memory database for data storage and management.

## Features
- Create a new project
- Retrieve all projects
- Retrieve a single project by ID
- Update an existing project
- Delete a project by ID

## Technologies Used
- Java 17
- Spring Boot
- Spring Data JPA
-  MYSQL 
- Spring Web
- Spring Validation
- Swagger for API documentation

## Project Setup

### Prerequisites
- Java 17
- Maven

### Initialization
1. Clone the repository:
    ```bash
    git clone <repository-url>
    cd project-management-system
    ```

2. Build the project using Maven:
    ```bash
    mvn clean install
    ```

3. Run the application:
    ```bash
    mvn spring-boot:run
    ```

The application will start on `http://localhost:8080`.

## Configuration
The MYSQL database is configured in the `src/main/resources/application.properties` file:
`
spring.application.name=Project-Management
spring.datasource.Driver-class-name=com.mysql.cj.jdbc.Driver
spring.datasource.url=jdbc:mysql://localhost:3306/Projectdb
spring.datasource.username=root
spring.datasource.password=root
spring.jpa.hibernate.ddl-auto=update
spring.jpa.properties.hibernate.format_sql=true
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect = org.hibernate.dialect.MySQL8Dialect
spring.mvc.pathmatch.matching-strategy=ant-path-matcher


