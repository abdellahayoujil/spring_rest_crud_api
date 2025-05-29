# Spring REST CRUD API

A minimal and extensible **Spring Boot** project that provides a fully functional **RESTful CRUD API** for managing `Product` entities. This application uses **Spring Web**, **Spring Data JPA**, and supports standard HTTP operations.

## 🛠️ Technologies Used

- **Java 17+**
- **Spring Boot**
- **Spring Web (REST)**
- **Spring Data JPA**
- **H2 / MySQL** (easily switchable)
- **Maven**

## 📁 Project Structure

spring_rest_crud_api/
├── controller/
│ └── ProductController.java # Handles HTTP requests
├── model/
│ └── Product.java # JPA entity
├── repository/
│ └── ProductRepository.java # JPA data access layer
└── SpringRestCrudApiApplication.java # Application bootstrap


## ⚙️ Configuration

### `application.properties`

properties
spring.application.name=spring_rest_crud_api
server.port=8082
server.servlet.context-path=/abdellahayj

spring.datasource.url=jdbc:mysql://localhost:3306/productsdb
spring.datasource.username=root
spring.datasource.password=0240133

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect

🚀 Getting Started
Prerequisites
Java 17+

Maven

MySQL installed and running with a database named productsdb

#Run the Project

git clone https://github.com/abdellahayoujil/spring_rest_crud_api.git
cd spring_rest_crud_api
mvn spring-boot:run

The app will be available at:
http://localhost:8082/abdellahayj

| Method | Endpoint         | Description                |
| ------ | ---------------- | -------------------------- |
| GET    | `/products/`     | Retrieve all products      |
| GET    | `/products/{id}` | Get a product by ID        |
| POST   | `/products/`     | Create a new product       |
| PUT    | `/products/`     | Update an existing product |
| DELETE | `/products/{id}` | Delete a product by ID     |


#🔖 Sample JSON (POST or PUT)

{
  "id": 1,
  "name": "Bluetooth Speaker",
  "price": 39.99
}


🧑‍💻 Author
Abdellah Ayoujil
📎 [GitHub Profile](https://github.com/abdellahayoujil)

