# Library Management System

A backend-focused **Library Management System** developed using Java and Spring Boot to manage library-related data and operations through RESTful APIs.

The project demonstrates practical use of **Spring Boot, Spring Data JPA, Hibernate, PostgreSQL, REST APIs, JWT Authentication, CRUD operations, and Maven**.

## 🚀 Features

* User authentication using **JWT**
* Secure authentication and authorization for protected API endpoints
* CRUD operations for library-related data
* RESTful API development using Spring Boot
* Database persistence using **PostgreSQL**
* Object-relational mapping using **Spring Data JPA and Hibernate**
* Layered backend application structure
* Maven-based project and dependency management

## 🛠️ Technologies Used

| Technology      | Purpose                               |
| --------------- | ------------------------------------- |
| Java            | Backend programming                   |
| Spring Boot     | Backend application development       |
| Spring Data JPA | Data access and repository operations |
| Hibernate       | ORM / database mapping                |
| PostgreSQL      | Relational database                   |
| REST API        | Client-server communication           |
| JWT             | Authentication and secure API access  |
| Maven           | Dependency and build management       |
| Eclipse         | Development environment               |

## 🏗️ Application Architecture

The application follows a layered backend architecture:

```text
Client
  |
  v
REST Controller
  |
  v
Service Layer
  |
  v
Repository Layer
  |
  v
Spring Data JPA / Hibernate
  |
  v
PostgreSQL Database
```

### Authentication Flow

```text
User Login
    |
    v
Authentication Request
    |
    v
Spring Boot Backend
    |
    v
Credentials Validation
    |
    v
JWT Token Generated
    |
    v
Client Stores Token
    |
    v
Protected API Request
    |
    v
JWT Validation
    |
    v
Authorized Request
```

## 🔐 JWT Authentication

The application uses JWT-based authentication to secure protected API endpoints.

The general authentication flow is:

1. User sends login credentials.
2. The backend validates the credentials.
3. A JWT token is generated after successful authentication.
4. The client sends the token with subsequent protected requests.
5. The backend validates the JWT.
6. Valid requests are allowed to access protected resources.

This provides stateless authentication for the REST API.

## 🔄 CRUD Operations

The application implements standard CRUD operations:

* **Create** — Add new records
* **Read** — Retrieve existing records
* **Update** — Modify existing records
* **Delete** — Remove records

These operations are exposed through REST API endpoints and connected to PostgreSQL through Spring Data JPA and Hibernate.

## 🗄️ Database

**PostgreSQL** is used as the relational database.

Spring Data JPA and Hibernate are used to map Java objects to database tables and perform database operations without requiring SQL for every standard data-access operation.

## 📂 Project Structure

A typical layered structure used by the application is:

```text
LibraryManagement
│
├── src
│   ├── main
│   │   ├── java
│   │   │   └── ...
│   │   └── resources
│   │       └── application.properties
│   │
│   └── test
│
├── pom.xml
└── README.md
```

## ⚙️ Prerequisites

Before running the project, make sure you have:

* Java installed
* Maven installed
* PostgreSQL installed and running
* Eclipse or another Java IDE
* A PostgreSQL database configured for the application

## ▶️ Running the Project

### 1. Clone the repository

```bash
git clone https://github.com/Sonalisahu728/Library-Management-System.git
```

### 2. Open the project

Open the project in Eclipse or another Java IDE.

### 3. Configure PostgreSQL

Create the required PostgreSQL database and update the application's database configuration in:

```text
src/main/resources/application.properties
```

Configure the database URL, username, and password according to your local PostgreSQL setup.

### 4. Build the project

```bash
mvn clean install
```

### 5. Run the application

Run the Spring Boot application from Eclipse or using Maven.

```bash
mvn spring-boot:run
```

The REST APIs can then be tested using a tool such as Postman.

## 🧪 API Testing

The REST APIs can be tested using **Postman**.

Testing can include:

* Authentication requests
* JWT-protected requests
* Create operations
* Read operations
* Update operations
* Delete operations
* Invalid request handling
* Unauthorized access attempts

## 📌 Project Highlights

* Developed a Java backend using Spring Boot.
* Implemented RESTful APIs for application operations.
* Used Spring Data JPA and Hibernate for database persistence.
* Integrated PostgreSQL as the relational database.
* Implemented JWT-based authentication.
* Implemented CRUD functionality.
* Used Maven for dependency and build management.
* Followed a structured backend architecture for separation of responsibilities.

## 👩‍💻 Author

**Sonali Sahu**

GitHub: [Sonalisahu728](https://github.com/Sonalisahu728)

LinkedIn: [Sonali Sahu](https://www.linkedin.com/in/sonalisahu02)
