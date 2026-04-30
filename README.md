🧩 First REST API with Spring Boot
📘 Overview
This project implements a fully functional RESTful API using Spring Boot 3.2 and Java 17.
It demonstrates clean architecture, dependency injection, and data persistence with an H2 in‑memory database.
The API exposes endpoints for managing products, including creation, retrieval, update, and deletion.

| Layer | Technology | Purpose |
| --- | --- | --- |
| Backend | **Spring Boot 3.2** | Application framework |
| Web | **Spring Web MVC** | REST API endpoints |
| Data | **Spring Data JPA** | ORM and repository abstraction |
| Database | **H2 Database** | Lightweight in‑memory storage |
| Documentation | **SpringDoc OpenAPI 2.0** | Swagger UI integration |
| Build | **Maven** | Dependency management |
| Language | **Java 17** | Core implementation |


🏗️ Project Structure
Code
pl.edu.vistula.firstrestapispring
 └── product
      ├── api
      │    ├── ProductController.java
      │    ├── request
      │    │    └── ProductRequest.java
      │    └── response
      │         └── ProductResponse.java
      ├── domain
      │    └── Product.java
      ├── repository
      │    └── ProductRepository.java
      ├── service
      │    └── ProductService.java
      └── support
           └── ProductMapper.java
🚀 Getting Started
1️⃣ Clone the repository
bash
git clone https://github.com/PJYRomE/First_Rest-Api-Spring.git
cd FirstRestAPI
2️⃣ Build and run
bash
mvn clean install
mvn spring-boot:run
3️⃣ Access the application
Feature	URL
API Root	http://localhost:8080/api/v1/products
Swagger UI	http://localhost:8080/swagger-ui/index.html
H2 Console	http://localhost:8080/console


🧠 Example Endpoints
➕ Create Product
http
POST /api/v1/products
Content-Type: application/json

{
  "name": "panashe"
}
Response
{
"id":1
"name":"Panashe"
}
🗄️ Database Configuration
Type: In‑memory H2
JDBC URL: jdbc:h2:mem:testdb
Accessible via the H2 Console for quick inspection and testing.

SWAGGER
![image.alt](https://github.com/PJYROmE/First_Rest-Api-Spring/blob/442ab9930b1940a3c42228f372d55e3e1a65221e/SWAGGER.png)

H2 DATABASE
![image.alt](https://github.com/PJYROmE/First_Rest-Api-Spring/blob/162773d71d3afad97f304f8dc251566a433863bd/H2%20DATABASE.png)








