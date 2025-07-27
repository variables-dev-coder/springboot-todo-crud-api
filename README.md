# springboot-todo-crud-api
📝 Todo List CRUD API using Spring Boot  Simple and clean RESTful API for managing Todo tasks. Built with Java 17, Spring Boot, Spring Data JPA, and MySQL.

# ✅ Todo CRUD API (Spring Boot + MySQL + H2)

A simple RESTful **CRUD API for managing tasks (todos)** built using **Spring Boot**, **Spring Data JPA**, and **MySQL** (with optional H2 in-memory database for testing).

---

## 🚀 Features

- Create, Read, Update, and Delete (CRUD) operations for tasks
- Validation using `jakarta.validation`
- Swagger/OpenAPI support (optional)
- Uses MySQL or in-memory H2 DB
- Clean architecture with layered structure (Controller, Service, Repository)

---

## 🧰 Tech Stack

- Java 17
- Spring Boot 3.x
- Spring Web
- Spring Data JPA
- MySQL & H2 Database
- Lombok
- Spring devtool
- Maven

---

## 📁 Project Structure

src/
├── main/
│ ├── java/com/example/todo/
│ │ ├── controller/
│ │ ├── model/
│ │ ├── repository/
│ │ └── service/
│ └── resources/
│ ├── application.properties

---

## 🧑‍💻 Setup Instructions

### ✅ 1. Clone the repository
```bash
git clone https://github.com/your-username/todo-crud-api.git
cd todo-crud-api

✅ 2. Configure MySQL
Make sure MySQL is running

Create a database:
CREATE DATABASE tododb;
Update credentials in src/main/resources/application.properties:

spring.datasource.url=jdbc:mysql://localhost:3306/tododb
spring.datasource.username=root
spring.datasource.password=****
✅ Alternatively, use H2 (enabled by default). Just access /h2-console.

▶️ Run the App
Using Maven:
./mvnw spring-boot:run
Or run from your IDE (e.g. IntelliJ or STS).

🧪 API Endpoints
Base URL: http://localhost:8080/api/tasks

Method	Endpoint	Description
GET	/api/tasks	Get all tasks
GET	/api/tasks/{id}	Get task by ID
POST	/api/tasks	Create a new task
PUT	/api/tasks/{id}	Update existing
DELETE	/api/tasks/{id}	Delete a task

📌 All endpoints consume and return JSON (application/json)

🧪 Sample Request – Create Task (POST)

POST /api/tasks
Content-Type: application/json

{
  "title": "Learn Spring Boot",
  "description": "Practice daily and build projects",
  "completed": false
}
🌐 H2 Console (Optional)
URL: http://localhost:8080/h2-console

JDBC URL: jdbc:h2:mem:todo-db

Username: sa, Password: (leave blank)

🧑 Author
Munna Aziz Mondal

LinkedIn: https://www.linkedin.com/in/munna-aziz-mondal-061b95212/
