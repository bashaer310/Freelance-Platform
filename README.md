# Freelance Platform

This is a backend solution for a freelance marketplace platform, built with Java, Spring Boot, and MySQL. The platform allows clients to post projects and receive offers from qualified experts across various tech fields. It includes core features like **user authentication**, **project management**, **offer and contract management**, and **category management**.

## Features

- **User Management**:
  - Register new user (Client/Experts/Admin)
  - User authentication and role-based authorization
  - Update user profile

- **Project Management**:
  - Clients can create new projects (title, description, budget, and deadline)
  - Experts can retrieve available projects and project details with handling pagination and filtering
  - Edit or delete a project (by project owner)

- **Offer (Proposal) Management**:
  - Freelancers can submit offers (proposals) for posted projects (custom price, delivery timeline, and message)
  - Clients can retrieve offers with handling pagination and filtering
  - Offer status tracking (pending, accepted, rejected)

- **Contract Management**:
  - Track accepted offers as active contracts
  - Update contract status (in progress, completed, canceled)

- **Category Management**:
  - Admin can create and manage categories (e.g., Web Development, Data Science, UI/UX)
  - Retrieve categories with handling pagination and filtering
  - Update or delete existing categories

## Technologies Used

- Java 21
- Spring Boot
- Spring Security (JWT-based authentication)
- MySQL
- JPA (Hibernate)
- ModelMapper (for DTO conversion)
- Maven
- Postman (for API testing)
