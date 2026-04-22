# Microservices Docker Compose Project (Skill Test 1: Cloud and Containers)

---
## Overview
This project demonstrates a microservices architecture using Node.js, fully containerized with Docker and orchestrated using Docker Compose.

## Services
1. User Service → 3000
2. Product Service → 3001
3. Order Service → 3002
4. Gateway Service → 3003
---
## Project Structure
```
skilltest/
├── submissions/
│   ├── user-service/Dockerfile
│   ├── product-service/Dockerfile
│   ├── order-service/Dockerfile
│   ├── gateway-service/Dockerfile
├── docker-compose.yml
└── README.md
└── .gitignore
```
---
## Tech Stack
1. Node.js
2. Docker
3. Docker Compose
4. Express.js
---
## Getting Started

**Prerequisites**
1. Docker
2. Docker Compose

**Check installation:**
```
docker --version
docker-compose --version
```
![Local Setup](https://raw.githubusercontent.com/sannnn1234/skilltest/main/screenshots/dockerversion.png)

---

## Run The Project
```
docker-compose up --build
```
![Local Setup](https://raw.githubusercontent.com/sannnn1234/skilltest/main/screenshots/servicebuild.png)

---

## Verify Running Containers
```
docker ps
```
![Local Setup](https://raw.githubusercontent.com/sannnn1234/skilltest/main/screenshots/ps.png)

---

## Service Endpoints
<div style="border:1px solid #ccc; padding:10px">
| Service Name | Description | Base URL |
|-------------|------------|----------|
| User Service | Manages user-related operations | http://localhost:3000/users |
| Product Service | Handles product data and catalog | http://localhost:3001/products |
| Order Service | Processes orders and transactions | http://localhost:3002/orders |
| Gateway Service | API Gateway & health check | http://localhost:3003/health |
</div>

---




