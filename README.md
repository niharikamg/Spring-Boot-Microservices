# Spring Boot Microservices Project

## 📌 Overview
This project demonstrates a **Spring Boot Microservices Architecture** with multiple services communicating with each other using **Spring Cloud Components**.

### ✅ Features:
- **Service Discovery** (Eureka Server)
- **API Gateway** (Spring Cloud Gateway)
- **Configuration Management** (Spring Cloud Config)
- **RESTful Microservices** (User, Order, Product Services)
- **Inter-Service Communication** (Feign Client & RestTemplate)
- **JWT Authentication & Security**
- **Logging & Monitoring** (Spring Boot Actuator, Zipkin, Sleuth)
- **Containerization** (Docker & Kubernetes)

---
## 🏗 Architecture Diagram
```plaintext
 ┌───────────────┐      ┌────────────────┐
 │ Client (UI)   │ ---> │ API Gateway    │
 └───────────────┘      └────────────────┘
         |                     |
 ┌───────────────┐  ┌───────────────┐  ┌───────────────┐
 │ User Service  │  │ Order Service │  │ Product Service │
 └───────────────┘  └───────────────┘  └───────────────┘
         |                     |
 ┌──────────────────────────────┐
 │ Eureka Discovery Service     │
 └──────────────────────────────┘
```

---
## 🚀 Setup & Run Instructions
### 1️⃣ Clone the Repository
```sh
git clone https://github.com/your-username/SpringBootMicroservices.git
cd SpringBootMicroservices
```

### 2️⃣ Start Eureka Server
```sh
cd eureka-server
mvn spring-boot:run
```

### 3️⃣ Start API Gateway
```sh
cd api-gateway
mvn spring-boot:run
```

### 4️⃣ Start Config Server
```sh
cd config-server
mvn spring-boot:run
```

### 5️⃣ Start Microservices
```sh
cd user-service && mvn spring-boot:run &
cd order-service && mvn spring-boot:run &
cd product-service && mvn spring-boot:run &
```

---
## 🐳 Running with Docker
Build & Run Services:
```sh
docker-compose up --build
```

---
## ☸️ Deploying to Kubernetes
```sh
kubectl apply -f k8s-manifests/
```

---
## 📬 API Endpoints
| Service | Endpoint |
|---------|---------|
| User Service | `http://localhost:8081/users` |
| Order Service | `http://localhost:8082/orders` |
| Product Service | `http://localhost:8083/products` |
| API Gateway | `http://localhost:8080/` |

---
## 🛠 Technologies Used
- **Spring Boot 3**
- **Spring Cloud** (Eureka, Gateway, Config Server)
- **Spring Security & JWT**
- **Docker & Kubernetes**
- **MySQL, JPA, Hibernate**
- **Maven & Lombok**
- **Zipkin, Sleuth for Tracing**

---
## 📜 License
This project is licensed under the MIT License - see the LICENSE file for details.

---
## 📩 Contribution
Feel free to fork this repo, create a feature branch, and submit a PR! 😊

