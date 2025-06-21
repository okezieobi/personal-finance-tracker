# Personal Finance Tracker

Personal Finance Tracker is a Java Spring Boot application designed to help users manage and track their personal finances efficiently. The project leverages modern Java frameworks and tools to provide a robust backend for user management and financial data storage.

## Features

- User management with roles (username, password, email, role)
- Secure authentication and authorization
- In-memory H2 database for easy development and testing
- JPA/Hibernate for object-relational mapping and automatic schema updates
- H2 web console for inspecting and managing the database

## Technologies Used

- Java 17+
- Spring Boot
- Spring Data JPA (Hibernate)
- H2 Database
- Lombok

## Getting Started

### Prerequisites

- Java 17 or higher
- Maven

### Running the Application

Clone the repository and run:

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