# Freelance Platform

This is a backend solution for a freelance marketplace platform, built with Java, Spring Boot, and MySQL. The platform allows clients to post projects and receive offers from qualified experts across various tech fields. It includes core features like **user authentication**, **project management**, **offer and contract management**, and **category management**.

## Features

- **User Management**:
  - Register new user (Client/Experts/Admin)
  - User authentication and role-based authorization
  - Update user profile

- **Project Management**:
  - Clients can create new projects (title, description, budget, and deadline)
  - Experts can retrieve available projects with pagination and filtering
  - View project details
  - Edit or delete a project (by project owner)

- **Offer (Proposal) Management**:
  - Experts can submit offers (proposals) for posted projects (custom price, delivery timeline, and message)
  - Clients can retrieve offers with pagination and filtering
  - Update Offer status (pending, accepted, rejected)

- **Contract Management**:
  - Clients can retrieve accepted offers as active contracts
  - Update contract status (in progress, completed, canceled)

- **Category Management**:
  - Admin can create and manage categories (e.g., Web Development, Data Science, UI/UX)
  - Retrieve categories with pagination and filtering
  - Update or delete existing categories

## Technologies Used

- Java 21 – Core programming language
- Spring Boot – Framework for building RESTful APIs
- Spring Data JPA – ORM layer for interacting with the database
- Spring Security – Authentication and authorization
- Bean Validation (JSR 380) – Input validation using annotations
- MySQL – Relational database used for persistence
- JPA (Hibernate) – ORM provider for database access
- Lombok – Reduces boilerplate code for models and DTOs
- JUnit 5 (Jupiter) – Unit testing framework
- Spring Boot Test – Testing support for Spring Boot applications
- Maven – Build and dependency management
