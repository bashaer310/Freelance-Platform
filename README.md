# Freelance Platform

This is a backend solution for a freelance marketplace platform, built with Java, Spring Boot, and MySQL. The platform allows clients to post projects and receive offers from qualified experts across various tech fields. It includes core features like **user authentication**, **project management**, **offer management**, and **category management**.

## Features

- **User Management**:
  - **User Registration** - users can create account (Client/Expert)
  - **Authentication & Authorization** - users can login with role-based access
  - **Profile Management** - users can update their profile

- **Project Management**:
  - **Project Management** - clients can create, edit or delete projects (title, description, budget, and deadline)
  - **Project Browsing** - experts can retrieve available projects with pagination and filtering
  - **Project Details View** - users can view project details
    
- **Category Management (types of project)**:
  - **Category Management** - admin can create, update, and delete categories (e.g., Web Development, Data Science, UI/UX)
  - **Category Retrieval** - users can retrieve categories with pagination and filtering
  
- **Offer Management**:
  - **Offer Creation** - experts can submit offers for projects (custom price, delivery timeline, and message)
  - **Offer Retrieval** - clients can retrieve offers with pagination and filtering
  - **Offer Status Management** - clients can update Offer status (pending, accepted, rejected)

## Technologies Used
- Languages
    - Java 21 – Programming language
- Frameworks
    - Spring Boot – RESTful API framework
- Datebase
    - MySQL – Relational database
- Dependencies
    - Spring Data JPA (Hibernate) – ORM for database access
    - Spring Security (JWT) – Authentication and authorization
    - Bean Validation – Input validation
    - Lombok – Reduces boilerplate code
    - JUnit 5 – Testing framework
    - Spring Boot Test – Test support for Spring apps
- Dependency manger
    - Maven – Dependency and build management
- Tools
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
│   │   │       ├── controller/       # API controllers for handling requests and responses
│   │   │       ├── config/           # Security and application configurations
│   │   │       ├── dto/              # Data Transfer Objects
│   │   │       ├── model/            # JPA entities (models)
│   │   │       ├── advice/           # Custom exceptions and hanling
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
