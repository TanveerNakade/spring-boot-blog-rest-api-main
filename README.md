# Spring Boot Blog REST API

A RESTful API for a blog platform built with Spring Boot. This project demonstrates best practices in REST API development, including authentication, CRUD operations for posts and comments, and clear code organization.

---

## Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Endpoints](#endpoints)
  - [Auth](#auth)
  - [Post](#post)
  - [Comment](#comment)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

---

## Features

- User registration and authentication (JWT-based)
- Create, read, update, and delete blog posts
- Comment on posts
- RESTful API design
- Exception handling and validation

---

## Tech Stack

- Java 17+
- Spring Boot
- Spring Data JPA
- Spring Security
- H2 Database (for development)
- Maven

---

## Endpoints

### Auth

- **POST** `/api/v1/auth/signin` — Sign in with email and password
- **POST** `/api/v1/auth/signup` — Register a new user

### Post

- **GET** `/api/v1/posts` — Get all posts
- **GET** `/api/v1/posts/{postId}` — Get post by ID
- **POST** `/api/v1/posts` — Create a new post
- **PUT** `/api/v1/posts/{postId}` — Update a post
- **DELETE** `/api/v1/posts/{postId}` — Delete a post

### Comment

- **GET** `/api/v1/posts/{postId}/comments` — Get all comments for a post
- **GET** `/api/v1/posts/{postId}/comments/{commentId}` — Get a specific comment
- **POST** `/api/v1/posts/{postId}/comments` — Add a comment to a post
- **PUT** `/api/v1/posts/{postId}/comments/{commentId}` — Update a comment
- **DELETE** `/api/v1/posts/{postId}/comments/{commentId}` — Delete a comment

---

## Installation

1. **Install Java:**  
   Download and install Java from the [official website](https://www.java.com/en/download/).

2. **Install an IDE:**  
   - [IntelliJ IDEA](https://www.jetbrains.com/idea/download/)  
   - [Visual Studio Code](https://code.visualstudio.com/Download)

3. **Clone the repository:**
   ```sh
   git clone https://github.com/TanveerNakade/spring-boot-blog-rest-api-main
   ```

4. **Navigate to the project directory:**
   ```sh
   cd spring-boot-blog-rest-api-main
   ```

---

## Usage

1. **Run the application:**
   - In your IDE, open the project and run the `SpringBootBlogRestApiApplication` main class.
   - Or use Maven from the terminal:
     ```sh
     mvn spring-boot:run
     ```

2. **Access the API:**  
   The API will be available at `http://localhost:8080/`.  
   Use tools like [Postman](https://www.postman.com/) or `curl` to interact with the endpoints.

---

## Project Structure

```
spring-boot-blog-rest-api-main
├── src
│   ├── main
│   │   ├── java
│   │   │   └── com
│   │   │       └── example
│   │   │           └── blog
│   │   │               ├── controller
│   │   │               ├── model
│   │   │               ├── repository
│   │   │               ├── service
│   │   │               └── SpringBootBlogRestApiApplication.java
│   │   └── resources
│   │       ├── application.properties
│   │       └── static
│   └── test
│       └── java
│           └── com
│               └── example
│                   └── blog
├── pom.xml
└── README.md
```

---

## Contributing

Contributions are welcome!  
Fork the repository, make your changes, and submit a pull request.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

