# ZephyraTech Backend

Spring Boot backend for the ZephyraTech project, featuring JWT-based authentication and SQLite integration for local development.

**Live API**: [https://zephyratech-task-backend.onrender.com](https://zephyratech-task-backend.onrender.com)

## 🚀 Features

- **JWT Authentication**: Secure stateless authentication using JSON Web Tokens.
- **User Management**: Signup and Signin endpoints with BCrypt password hashing.
- **Database Integration**: Local file-based storage using SQLite for easy setup and development.

## 🛠️ Tech Stack

- Java 17
- Spring Boot 3.2.2
- Spring Security
- Spring Data JPA
- SQLite JDBC Driver
- Hibernate Community Dialects
- JJWT (Java JWT Library)
- Lombok

## 📋 API Endpoints

### Auth
- `POST /api/auth/signup`: Register a new user.
- `POST /api/auth/signin`: Authenticate and receive a JWT.

## ⚙️ Configuration

The application is pre-configured to use a local SQLite database (`zephyratech.db`).

- `spring.datasource.url`: `jdbc:sqlite:zephyratech.db`
- `spring.datasource.driver-class-name`: `org.sqlite.JDBC`
- `spring.jpa.properties.hibernate.dialect`: `org.hibernate.community.dialect.SQLiteDialect`

## 🏗️ Getting Started

### Prerequisites

- JDK 17 or higher
- Maven 3.x

### Running the Application

1. Navigate to the `backend` directory:
   ```bash
   cd backend
   ```
2. Build the project:
   ```bash
   mvn clean install
   ```
3. Run the application:
   ```bash
   mvn spring-boot:run
   ```

The backend server will start on [https://zephyratech-task-backend.onrender.com](https://zephyratech-task-backend.onrender.com) (or http://localhost:8080 locally).
