# ZephyraTech Backend

Spring Boot backend for the ZephyraTech project, featuring JWT-based authentication and PostgreSQL integration.

## 🚀 Features

- **JWT Authentication**: Secure stateless authentication using JSON Web Tokens.
- **User Management**: Signup and Signin endpoints with BCrypt password hashing.
- **Database Integration**: Seamless connection to PostgreSQL (Supabase).
- **Security**: Pre-configured CORS and Spring Security filters.
- **RESTful API**: Clean API structure for frontend integration.

## 🛠️ Tech Stack

- Java 17
- Spring Boot 3.2.2
- Spring Security
- Spring Data JPA
- PostgreSQL Driver
- JJWT (Java JWT Library)
- Lombok

## 📋 API Endpoints

### Auth
- `POST /api/auth/signup`: Register a new user.
- `POST /api/auth/signin`: Authenticate and receive a JWT.

## ⚙️ Configuration

The application requires the following environment variables or `application.properties` settings:

- `DB_URL`: JDBC URL for your PostgreSQL database.
- `DB_USERNAME`: Database username.
- `DB_PASSWORD`: Database password.

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

The backend server will start on [http://localhost:8080](http://localhost:8080).
