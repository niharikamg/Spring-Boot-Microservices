# 🌟 Spring Boot Microservices Project

## 🚀 What’s This Project About?
This is a **Spring Boot Microservices** project showcasing how different services interact using **Spring Cloud Components**. It’s a great starting point for learning **microservices architecture** with practical examples.

### ✅ What’s Inside?
- 🛠 **Service Discovery** (Eureka Server)
- 🔀 **API Gateway** (Spring Cloud Gateway)
- 🎛 **Centralized Config Management** (Spring Cloud Config)
- 📡 **RESTful Microservices** (User, Order, Product Services)
- 🔗 **Communication Between Services** (Feign Client & RestTemplate)
- 🔑 **Authentication & Security** (JWT)
- 📊 **Logging & Monitoring** (Spring Boot Actuator, Zipkin, Sleuth)
- 🐳 **Containerization** (Docker & Kubernetes)

---
## 🏗 How Does It Work?
Imagine an **online shopping system** where different services handle different tasks:

```
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
## 🛠 Getting Started
### 1️⃣ Clone This Repository
```sh
git clone https://github.com/your-username/SpringBootMicroservices.git
cd SpringBootMicroservices
```

### 2️⃣ Start the Eureka Server
```sh
cd eureka-server
mvn spring-boot:run
```

### 3️⃣ Start the API Gateway
```sh
cd api-gateway
mvn spring-boot:run
```

### 4️⃣ Start the Config Server
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
To run everything in **Docker**, just execute:
```sh
docker-compose up --build
```

---
## ☸️ Deploying on Kubernetes
```sh
kubectl apply -f k8s-manifests/
```

---
## 🌍 API Endpoints
| Service | Endpoint |
|---------|---------|
| 👤 User Service | `http://localhost:8081/users` |
| 📦 Order Service | `http://localhost:8082/orders` |
| 🏬 Product Service | `http://localhost:8083/products` |
| 🌍 API Gateway | `http://localhost:8080/` |

---
## 🛠 Technologies Used
- 🌱 **Spring Boot 3**
- ☁️ **Spring Cloud** (Eureka, Gateway, Config Server)
- 🔐 **Spring Security & JWT**
- 🐳 **Docker & Kubernetes**
- 💾 **MySQL, JPA, Hibernate**
- ⚙️ **Maven & Lombok**
- 🔎 **Zipkin & Sleuth for Tracing**

---
## 📜 License
This project is under the **MIT License**. Check the LICENSE file for details.

---
## 🤝 Want to Contribute?
Fork this repo, create a feature branch, and submit a PR! 🚀 Let's build something amazing together! 😊

