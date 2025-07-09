# Microservices Architecture Demo

## 🚀 Enterprise-Grade Microservices Ecosystem

A comprehensive demonstration of modern microservices architecture patterns, inspired by my experience building scalable systems at **Bank of America** and **Marriott International**. This project showcases distributed systems design, service mesh implementation, and cloud-native development practices.

## 🏗️ System Architecture 
┌─────────────────┐
                       │   React Client  │
                       │   (Port 3000)   │
                       └─────────┬───────┘
                                 │
                       ┌─────────▼───────┐
                       │  API Gateway    │
                       │ (Spring Cloud)  │
                       │   (Port 8080)   │
                       └─────────┬───────┘
                                 │
     ┌───────────────────────────┼───────────────────────────┐
     │                           │                           │
     ┌─────────────────┐    ┌─────────────────┐
         │   Config Server │    │ Service Registry│
         │   (Port 8888)   │    │ Eureka (8761)   │
         └─────────────────┘    └─────────────────┘

┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│    Zipkin       │    │   Prometheus    │    │     Grafana     │
│  (Port 9411)    │    │   (Port 9090)   │    │   (Port 3001)   │
└─────────────────┘    └─────────────────┘    └─────────────────┘ 
## 🎯 Key Features

### 🔧 Core Microservices
- **API Gateway** - Single entry point with routing, rate limiting, and authentication
- **User Service** - User management, authentication, and authorization
- **Product Service** - Product catalog and inventory management
- **Order Service** - Order processing and transaction management
- **Notification Service** - Email, SMS, and push notification handling

### 🌐 Infrastructure Services
- **Service Registry** - Eureka server for service discovery
- **Config Server** - Centralized configuration management
- **Circuit Breaker** - Resilience patterns with Hystrix/Resilience4J
- **Distributed Tracing** - Request tracking with Zipkin
- **Monitoring Stack** - Prometheus metrics and Grafana dashboards

### ☁️ Cloud-Native Features
- **Docker Containerization** - All services containerized
- **Kubernetes Deployment** - Production-ready K8s manifests
- **Health Checks** - Comprehensive health monitoring
- **Auto-Scaling** - Horizontal pod autoscaling
- **Service Mesh** - Istio integration ready

## 🛠️ Technology Stack

### Backend Services
- **Java 11** with Spring Boot 2.7
- **Spring Cloud** (Gateway, Config, Netflix stack)
- **Spring Security** with JWT authentication
- **Spring Data JPA** and Spring Data MongoDB
- **Apache Kafka** for event-driven communication
- **Redis** for caching and session management

### Databases
- **PostgreSQL** - User service data
- **MongoDB** - Product catalog and analytics
- **MySQL** - Order transaction data
- **Redis** - Caching and session storage

### Monitoring & Observability
- **Prometheus** - Metrics collection
- **Grafana** - Visualization and dashboards
- **Zipkin** - Distributed tracing
- **ELK Stack** - Centralized logging
- **Micrometer** - Application metrics

### DevOps & Deployment
- **Docker** & **Docker Compose**
- **Kubernetes** with Helm charts
- **GitHub Actions** CI/CD
- **SonarQube** for code quality
- **Testcontainers** for integration testing

## 🚀 Quick Start

### Prerequisites
- Java 11+
- Docker & Docker Compose
- Node.js 16+ (for frontend)
- kubectl (for Kubernetes deployment)
