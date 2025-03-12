# BookNest Backend - Bookstore Management System

## 📌 Project Overview
BookNest is a **Bookstore Management System** built using **Java and Spring Boot**. It provides RESTful APIs for managing books, customers, orders, and inventory. The backend is designed to be efficient, scalable, and easy to integrate with a frontend or third-party services.

## 🚀 Features
- 📚 **Book Management**: Add, update, delete, and search for books.
- 🛍 **Order Processing**: Manage customer orders and payments.
- 👤 **Customer Management**: Handle customer details and authentication.
- 📦 **Inventory Tracking**: Keep track of book stock levels.
- 🔐 **Authentication & Authorization**: Secure API access using JWT.
- 📊 **API Testing & Documentation**: Tested using **Postman**.

## 🛠 Tech Stack
- **Backend**: Java, Spring Boot, Spring Data JPA
- **Database**: MySQL / PostgreSQL
- **Security**: Spring Security, JWT Authentication
- **API Testing**: Postman
- **Build Tool**: Maven

## 📌 Installation & Setup

### 1️⃣ Clone the Repository
```sh
 git clone https://github.com/yourusername/booknest-backend.git
 cd booknest-backend
```

### 2️⃣ Configure the Database
Update **application.properties** (for MySQL example):
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/booknest
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
```

### 3️⃣ Build & Run the Application
```sh
mvn clean install
mvn spring-boot:run
```

## 📢 API Endpoints

### 📚 Book Management
| Method | Endpoint           | Description |
|--------|-------------------|-------------|
| GET    | `/api/books`      | Get all books |
| GET    | `/api/books/{id}` | Get book by ID |
| POST   | `/api/books`      | Add a new book |
| PUT    | `/api/books/{id}` | Update book details |
| DELETE | `/api/books/{id}` | Delete a book |

### 🛍 Order Management
| Method | Endpoint           | Description |
|--------|-------------------|-------------|
| GET    | `/api/orders`      | Get all orders |
| POST   | `/api/orders`      | Create a new order |
| GET    | `/api/orders/{id}` | Get order details |

### 🔐 Authentication
| Method | Endpoint      | Description |
|--------|-------------|-------------|
| POST   | `/api/auth/register` | Register a new user |
| POST   | `/api/auth/login`    | Authenticate user & get JWT |

## 🛠 API Testing using Postman
1. Import the **Postman Collection** (BookNest.postman_collection.json) into Postman.
2. Set up environment variables (`BASE_URL` = `http://localhost:8080`).
3. Test the endpoints with appropriate request bodies and headers.

## 📜 License
This project is licensed under the MIT License.

## 📞 Contact
For any inquiries or contributions, feel free to reach out:
- ✉ Email: yourname@example.com
- 💻 GitHub: [yourusername](https://github.com/yourusername)

Happy coding! 🚀📚
