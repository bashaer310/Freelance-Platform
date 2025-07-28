# Freelance Platform

This is a backend solution for a freelance marketplace platform, built with Java, Spring Boot, and MySQL. The platform allows clients to post projects and receive offers from qualified experts across various tech fields. It includes core features like **user authentication**, **project management**, **offer and contract management**, and **category management**.

## Features

- **User Management**:
  - Register new user (Client/Expert/Admin)
  - User authentication and role-based authorization
  - Update user profile

- **Project Management**:
  - Clients can create, edit or delete projects (title, description, budget, and deadline)
  - Experts can retrieve available projects with pagination and filtering
  - View project details

- **Offer (Proposal) Management**:
  - Experts can submit offers for projects (custom price, delivery timeline, and message)
  - Clients can retrieve offers with pagination and filtering
  - Clients can update Offer status (pending, accepted, rejected)

- **Contract Management**:
  - Accepted offers are converted into active contracts
  - Clients and experts can view contract details
  - Clients can update contract status (in progress, completed, canceled)

- **Category Management**:
  - Admin can create, update, and delete categories (e.g., Web Development, Data Science, UI/UX)
  - Retrieve categories with pagination and filtering

## Technologies Used
- Java 21 – Programming language
- Spring Boot – RESTful API framework
- Spring Data JPA (Hibernate) – ORM for database access
- Spring Security (JWT) – Authentication and authorization
- Bean Validation – Input validation
- MySQL – Relational database
- Lombok – Reduces boilerplate code
- JUnit 5 – Testing framework
- Spring Boot Test – Test support for Spring apps
- Maven – Dependency and build management
- Postman – API testing

## Getting Started

1. Clone the repository:
  ```bash
  git clone https://github.com/bashaer310/Freelance-Platform
  ```

2. Navigate to the project folder:
  ```bash
  Freelance-Platform
  ```

3. Configure Database:
- Ensure MySQL is running.
- Create tables for all the models in your DB.
- Open `src/main/resources/application.properties` and update the DB config:

```bach
  spring.datasource.url=jdbc:mysql://localhost:3306/yourDB
  spring.datasource.username=yourUsername
  spring.datasource.password=yourPassword
```

- Run the application:

  Use your IDE or run via command line:
```bash
./mvnw spring-boot:run
```
5. Test the API

    Use tools like Postman to test the endpoints.


## Project structure
```bash
Freelance-Platform/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/example/freelance/
│   │   │       ├── controller/       # REST controllers (API endpoints)
│   │   │       ├── config/           # Security and application configurations
│   │   │       ├── dto/              # Data Transfer Objects
│   │   │       ├── model/            # JPA entities (models)
│   │   │       ├── advice/           # Custom exceptions
│   │   │       ├── api/              # Custom hanling exceptions
│   │   │       ├── repository/       # Spring Data JPA repositories
│   │   │       ├── service/          # Business logic and services
│   │   │       └── FreelanceApplication.java  # Application entry point
│   │   ├── resources/
│   │   ├── application.properties    # App configuration and DB connection
├── pom.xml                           # Maven configuration file
```

## API Endpoints
All the API endpoints are documented and can be accessed at:

## Deployment

The application is deployed and can be accessed at: 

## License

This project is licensed under the MIT License.
