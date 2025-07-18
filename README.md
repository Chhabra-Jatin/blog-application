# 📝 Spring Boot Blog REST API

A secure and scalable RESTful blog application built with **Spring Boot**. It features **JWT-based authentication** and **role-based authorization**, allowing users to register, login, and perform CRUD operations on blog posts, categories, and comments. The API also supports **pagination, sorting**, and robust validation, making it suitable for production-grade backend systems for blogs or content platforms.

---

## 🚀 Features

- ✅ JWT Authentication & Role-Based Access Control
- ✍️ CRUD operations on Posts, Categories, and Comments
- 🔒 Secure endpoints with Spring Security
- 📄 Input validation and exception handling
- 🔁 Pagination & Sorting support
- 🧪 Unit-tested and modular codebase

---

## 🛠️ Tech Stack

- ![Java](https://img.shields.io/badge/Java-17-blue?logo=java)
- ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.0-green?logo=springboot)
- ![Spring Security](https://img.shields.io/badge/Spring%20Security-yellowgreen?logo=spring)
- ![JWT](https://img.shields.io/badge/JWT-authentication-red?logo=jsonwebtokens)
- ![Maven](https://img.shields.io/badge/Maven-Build-blue?logo=apachemaven)
- ![MySQL](https://img.shields.io/badge/MySQL-Database-blue?logo=mysql)
- ![Lombok](https://img.shields.io/badge/Lombok-Annotation-red?logo=lombok)
- ![ModelMapper](https://img.shields.io/badge/ModelMapper-ObjectMapping-orange)

---

## 📁 Project Structure

springboot-blog-rest-api

├── config

├── controller

├── dto

├── entity

├── exception

├── payload

├── repository

├── security

├── service

└── utils


---

## 📦 Installation Instructions

### 1. Clone the repository

git clone https://github.com/Chhabra-Jatin/blog-application.git
cd blog-application/springboot-blog-rest-api

### 2. Configure the application

Update application.properties with your own database and JWT settings:

spring.datasource.url=jdbc:mysql://localhost:3306/blogdb

spring.datasource.username=root

spring.datasource.password=yourpassword

app.jwt-secret=your_jwt_secret

app-jwt-expiration-milliseconds=86400000

### 3. Install dependencies and build the project

./mvnw clean install
or 

if Maven is installed

mvn clean install

### 4. Run the application

./mvnw spring-boot:run
or
mvn spring-boot:run


## 🎯 API Endpoints Overview

| Method | Endpoint              | Description                   |
|--------|-----------------------|-------------------------------|
| POST   | `/api/auth/register`  | Register a new user           |
| POST   | `/api/auth/login`     | Login and receive JWT         |
| GET    | `/api/posts`          | List all blog posts           |
| POST   | `/api/posts`          | Create a new post (auth req)  |
| PUT    | `/api/posts/{id}`     | Update post (auth req)        |
| DELETE | `/api/posts/{id}`     | Delete post (auth req)        |
| GET    | `/api/categories`     | List all categories           |


