# 🌱 Spring Boot Products API

A RESTful CRUD API built with Spring Boot 3, developed while following the course **Spring Boot 3 | Complete Course 2023** by [Michelli Brito](https://www.youtube.com/@MichelliBrito).

---

## 📋 About the Project

This project is a products management API that covers the fundamentals of Spring Boot 3, including REST architecture, JPA/Hibernate integration with PostgreSQL, data validation, and layered architecture.

---

## 🚀 Technologies

- **Java 17**
- **Spring Boot 3**
- **Spring Data JPA**
- **Spring Validation**
- **PostgreSQL**
- **Maven**

---

## 🗂️ Project Structure

```
com.example.springboot
├── controllers
│   └── ProductController.java
├── services
│   └── ProductService.java
├── repositories
│   └── ProductRepository.java
├── models
│   └── ProductModel.java
└── dtos
    └── ProductRecordDto.java
```

---

## ⚙️ Prerequisites

Before running the project, make sure you have installed:

- [Java 17+](https://www.oracle.com/java/technologies/downloads/)
- [Maven](https://maven.apache.org/)
- [PostgreSQL](https://www.postgresql.org/)

---

## 🔧 Configuration

1. Create a database in PostgreSQL:

```sql
CREATE DATABASE products-api;
```

2. Update the `src/main/resources/application.properties` file with your credentials:

```properties
spring.application.name=springboot
spring.datasource.url=jdbc:postgresql://localhost:5432/products-api
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.properties.hibernate.jdbc.lob.non_contextual_creation=true
```

---

## ▶️ Running the Project

```bash
# Clone the repository
git clone https://github.com/your-username/springboot-products.git

# Navigate to the project folder
cd springboot-products

# Run with Maven
./mvnw spring-boot:run
```

The API will be available at: `http://localhost:8080`

---

## 📡 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/products` | Create a new product |
| `GET` | `/products` | List all products |
| `GET` | `/products/{id}` | Get a product by ID |
| `PUT` | `/products/{id}` | Update a product |
| `DELETE` | `/products/{id}` | Delete a product |

---

## 📦 Request Body

### Create / Update Product

```json
{
  "name": "Product Name",
  "value": 99.99
}
```

---

## 📚 Course Reference

- **Course:** Spring Boot 3 | Complete Course 2023
- **Instructor:** Michelli Brito
- **Channel:** [youtube.com/@MichelliBrito](https://www.youtube.com/@MichelliBrito)

---

## 📝 License

This project was developed for study purposes.
