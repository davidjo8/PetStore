Overview

The Pet Store API is a backend application designed to manage a virtual pet store. It supports operations for managing pets, customers, and transactions. This project demonstrates the implementation of CRUD operations, relational database management, and RESTful design using Java, Spring Boot, and MySQL.

# **Features**

1. **Pet Management**

- Add, update, retrieve, and delete pet entries.

- Track details such as breed, age, and availability.

2. **Customer Management**

- Manage customer details including contact information.

- Associate customers with their purchases.

3. **Transaction Management**

- Record and manage pet purchases.

- Generate transaction histories for customers.

4. **Search Functionality**

- Search pets by breed, age, or availability status.

# **Technologies Used**

- Programming Language: Java

- Framework: Spring Boot

- Database: MySQL

- Logging: SLF4J with Logback

# **Setup Instructions**

## Prerequisites

- JDK 17 or higher

- Maven

- MySQL Server

- An IDE such as IntelliJ IDEA or Eclipse

## Steps to Run the Application

1. Clone the repository:

git clone <repository_url>
cd pet-store-api

2. Configure the database:

- Create a new MySQL database named pet_store.

- Update the application.properties file with your MySQL credentials:

  spring.datasource.url=jdbc:mysql://localhost:3306/pet_store
  spring.datasource.username=<your_username>
  spring.datasource.password=<your_password>
  spring.jpa.hibernate.ddl-auto=update

3. Build and run the application:

mvn clean install
mvn spring-boot:run

4. Access the API:

The API will be accessible locally at http://localhost:8080.

# API Endpoints

## Pet Endpoints

- GET /pets: Retrieve all pets.

- GET /pets/{id}: Retrieve a specific pet by ID.

- POST /pets: Add a new pet.

- PUT /pets/{id}: Update an existing pet.

- DELETE /pets/{id}: Delete a pet.

## Customer Endpoints

- GET /customers: Retrieve all customers.

- GET /customers/{id}: Retrieve a specific customer by ID.

- POST /customers: Add a new customer.

- PUT /customers/{id}: Update an existing customer.

- DELETE /customers/{id}: Delete a customer.

## Transaction Endpoints

- GET /transactions: Retrieve all transactions.

- GET /transactions/{id}: Retrieve a specific transaction by ID.

- POST /transactions: Record a new transaction.

# Database Schema

## Tables

1. Pet: Stores pet details such as breed, age, and availability.

2. Customer: Stores customer information like name and contact details.

3. Transaction: Stores transaction details including pet and customer references.

## Relationships

- Customer and Transaction: One-to-Many

- Pet and Transaction: Many-to-One

# Future Enhancements

- Implement user authentication and roles (e.g., admin, employee).

- Add pet adoption requests and status tracking.

- Develop a front-end interface for pet browsing and management.

- Add support for payment gateway integration.

# License

MIT License

Copyright (c) 2025 David Joseph Jay Song Albuquerque Canarsky

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

# Contact

For questions or contributions, please contact David Canarsky at davidjosephgpa@gmail.com.

