# Spring Cloud Gateway

A simple Java project using Spring Cloud Gateway to manage routing and secure endpoints with OAuth2, designed to work
with other Spring-based projects.

**Note: This project requires another repository to be set up and running for the OAuth2 Authorization
Server. [OAuth2 Authorization Server Repository](https://github.com/CarinaPorumb/spring-oauth2)**

---

## Features

- API Gateway using Spring Cloud Gateway
- Secure endpoints with OAuth2 and JWT
- Configurable routes for various microservices

---

## Technologies Used

- Java 21
- Spring Boot 3.3.0
- Spring Cloud Gateway
- Spring Security
- OAuth2 Authorization Server

--- 

## Getting Started

### Prerequisites

Make sure you have the following installed on your system:

- Java 21
- Maven

---

### Installation

- #### 1. Clone and Set Up the OAuth2 Authorization Server Project

This Cloud Gateway project relies on a separate OAuth2 Authorization Server project for authentication and
authorization.

Clone and set up the OAuth2 project first:

```bash
git clone https://github.com/CarinaPorumb/spring-oauth2
cd spring-oauth2
```

<br>

Build the project using Maven:

```bash
mvn clean install
```

<br>

You can run the application using your IDE or from the command line:

```bash
mvn spring-boot:run
```

Once the application is running, it will be available at http://localhost:9000.

<br>

- #### 2. Clone and Set up the Spring Cloud Gateway Project

After setting up the OAuth2 Authorization Server, clone and set up the Spring Cloud Gateway project:

```bash
git clone https://github.com/CarinaPorumb/spring-cloud-gateway
```

<br>

Build the project using Maven:

```bash
mvn clean install
```

<br>

You can run the application using your IDE or from the command line:

```bash
mvn spring-boot:run
```

Once the application is running, it will be available at http://localhost:8080.

**Ensure the OAuth2 Authorization Server is running on http://localhost:9000 before using this project.**