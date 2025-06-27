# Book Management System 
    A Spring Boot REST API to manage books with JWT-based authentication and MySQL integration.

## Features
- CRUD operations for books
- JWT login for secured access
- MySQL database with Spring Data JPA
- Global exception handling
- Unit testing with JUnit + MockMvc

## Setup
- Java 17, Spring Boot 3.x
- MySQL DB: bookdb
- Run: mvn spring-boot:run

## Login
POST `/auth/login`
json
{ "username": "admin", "password": "password" }

## Book APIs

Method            Endpoint               Description
- GET               /books                 Get all books
- GET               /books/{isbn}          Get book by ISBN
- POST              /books                 Add new book
- PUT               /books/{isbn}          Update book
- DELETE            /books/{isbn}          Delete book

All endpoint's require a bearer token in the header



