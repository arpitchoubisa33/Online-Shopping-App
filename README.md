# Online-Shopping-App-SpringBoot

## Introduction
This project is a backend-based Online Shopping Application developed using Java and Spring Boot. It provides RESTful APIs to handle essential e-commerce operations such as user registration, product management, cart functionality, and order processing.

The application is designed to simulate how an online shopping system works on the backend, including data storage, request handling, and business logic implementation. It demonstrates the use of Spring Boot for building scalable web applications along with MySQL for database management and Hibernate for object-relational mapping.

**Project Developer:** Arpit Choubisa (24BAI10514)

---

## Entity Relationship Diagram

The following diagram represents the relationship between core entities such as User, Customer, Product, Cart, and Order in the system.

![ER Diagram](https://user-images.githubusercontent.com/101566519/185047965-4bca8f2f-a99b-42bb-98e9-ecd71934242e.png)

---

## Tech Stack & Tools

### Technologies:
- **Java** - Core programming language
- **Spring Framework** - Application framework
- **Spring Boot** - Rapid application development
- **MySQL** - Relational database management
- **Hibernate** - ORM (Object-Relational Mapping)

### Development Tools:
- **Spring Tool Suite (STS)** - IDE for Spring development
- **Swagger** - API documentation and testing
- **Postman** - API testing and debugging

---

## Project Structure

### Model Classes:
1. **User.java** - User authentication and management
2. **Customer.java** - Customer profile information
3. **Address.java** - Delivery address management
4. **Product.java** - Product catalog details
5. **Cart.java** - Shopping cart functionality
6. **MyOrder.java** - Order processing and history
7. **CategoryEnum.java** - Product category enumeration

---

## API Endpoints

### Base URL
```
http://localhost:8088
```

### Swagger Documentation
```
http://localhost:8088/swagger-ui/index.html#/
```

### Key Endpoints:

#### User Management
- **User Registration:** `POST /registration`
- **User Login:** `POST /login`

#### Product Management
- **Add New Products:** `POST /newproducts`

#### Customer Management
- **Get Customer Details:** `GET /{customerId}`

#### Cart Operations
- **Add Product to Cart:** `POST /Cart/addtocart/{id}/{custId}`

#### Address Management
- **Get All Addresses:** `GET /getAll`

---

## Features

- User registration and authentication
- Product catalog management
- Shopping cart functionality
- Order processing and tracking
- Multiple address management
- RESTful API architecture
- Comprehensive API documentation with Swagger

---

## Getting Started

### Prerequisites
- JDK 8 or higher
- MySQL Server
- Maven

### Installation
1. **Clone the repository**
```bash
git clone https://github.com/arpitchoubisa33/Online-Shopping-App-SpringBoot
cd Online-Shopping-App-SpringBoot
```
2. **Configure database**  
Update the database credentials in the `application.properties` file (see Database Configuration section below).

3. **Build the project**
```bash
mvn clean install
```
4. **Run the application**
```bash
mvn spring-boot:run
```
5. **(Optional) Run using JAR file**
```bash
java -jar target/OnlineShoppingApp.jar
```
6. **Access the application**
- Base URL: http://localhost:8088  
- Swagger UI: http://localhost:8088/swagger-ui/index.html
  
---

## Database Configuration

Update the `application.properties` file with your MySQL credentials:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/shopping_db
spring.datasource.username=your_username
spring.datasource.password=your_password
```

---

## Project Status

This project was developed as part of academic coursework to implement backend functionality using Spring Boot and REST APIs.

---

**Developed by:** Arpit Choubisa

**Institution:** VIT Bhopal University

---

## 🚀 Future Improvements

- Add frontend interface  
- Implement product search and filtering  
- Add payment system simulation  
- Improve security using JWT authentication  

---

## License

This project is open for educational purposes.

---

Thank you for checking out this project!
