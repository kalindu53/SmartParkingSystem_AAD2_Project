# 🚗 Smart Parking Management System (SPMS)

A microservice-based backend system for managing parking space availability, vehicle tracking, user handling, and simulated payments using Spring Boot and Spring Cloud.

---

## 📦 Project Modules (Microservices)

| Service Name        | Description                                      | Default Port |
|---------------------|--------------------------------------------------|--------------|
| `eureka-server`     | Service Discovery with Eureka                    | 8761         |
| `config-server`     | Centralized configuration for all services       | 8888         |
| `api-gateway`       | Gateway to route all client requests             | 8080         |
| `user-service`      | User registration, login, and profiles           | Dynamic      |
| `vehicle-service`   | Vehicle registration and entry/exit tracking     | Dynamic      |
| `parking-service`   | Manage parking spot data and reservations        | Dynamic      |
| `payment-service`   | Simulated payment transactions and receipts      | Dynamic      |

> Dynamic ports are managed via `application.yml` or `application.properties`.

---

## 🔧 Tech Stack

- Java 17+
- Spring Boot
- Spring Cloud (Eureka, Config, Gateway)
- REST APIs
- H2 / MySQL (configurable)
- Maven

---

## ▶️ How to Run the Project

### 🔁 1. Start the Microservices (Order matters!)
Each service is a Maven-based Spring Boot project. Use the terminal in each folder:

```bash
cd config-server
mvn spring-boot:run
