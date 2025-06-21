# Personal Finance Tracker

A Spring Boot application for tracking personal finances.

## Features

- User management with roles
- In-memory H2 database for development and testing
- JPA/Hibernate for ORM and schema management
- H2 console for database inspection

## Application Properties

```properties
spring.application.name=personal-finance-tracker

# H2 Database Configuration
spring.h2.console.enabled=true
spring.h2.console.path=/h2-console
spring.datasource.url=jdbc:h2:mem:financetrackerdb;DB_CLOSE_DELAY=-1;DB_CLOSE_ON_EXIT=FALSE
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=

# JPA/Hibernate Configuration
spring.jpa.hibernate.ddl-auto=update # Automatically create/update schema based on entities
spring.jpa.show-sql=true 
spring.jpa.properties.hibernate.format_sql=true # Format logged SQL for readability
```

## Getting Started

### Prerequisites

- Java 17+
- Maven

### Running the Application

```sh
./mvnw spring-boot:run
```

The application will start at [http://localhost:8080](http://localhost:8080).

### Accessing the H2 Console

- URL: [http://localhost:8080/h2-console](http://localhost:8080/h2-console)
- JDBC URL: `jdbc:h2:mem:financetrackerdb`
- Username: `sa`
- Password: *(leave blank)*

## Project Structure

- `src/main/java/com/finance/tracker` - Main application code
- `src/main/resources/application.properties` - Application configuration
- `src/test/java/com/finance/tracker` - Test code

## License

This project is licensed under the GNU General Public License v3.0. See the LICENSE file for