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
<div style="border:1px solid #ccc; padding:12px">

<table>
  <thead>
    <tr>
      <th>Service Name</th>
      <th>Description</th>
      <th>Base URL</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>User Service</td>
      <td>Manages user-related operations</td>
      <td>
        <a href="http://localhost:3000/users" target="_blank">
          http://localhost:3000/users
        </a>
      </td>
    </tr>
    <tr>
      <td>Product Service</td>
      <td>Handles product data and catalog</td>
      <td>
        <a href="http://localhost:3001/products" target="_blank">
          http://localhost:3001/products
        </a>
      </td>
    </tr>
    <tr>
      <td>Order Service</td>
      <td>Processes orders and transactions</td>
      <td>
        <a href="http://localhost:3002/orders" target="_blank">
          http://localhost:3002/orders
        </a>
      </td>
    </tr>
    <tr>
      <td>Gateway Service</td>
      <td>API Gateway &amp; health check</td>
      <td>
        <a href="http://localhost:3003/health" target="_blank">
          http://localhost:3003/health
        </a>
      </td>
    </tr>
  </tbody>
</table>

</div>

---
![Local Setup](https://raw.githubusercontent.com/sannnn1234/skilltest/main/screenshots/users.png)
![Local Setup](https://raw.githubusercontent.com/sannnn1234/skilltest/main/screenshots/product.png)
![Local Setup](https://raw.githubusercontent.com/sannnn1234/skilltest/main/screenshots/addorder.png)
![Local Setup](https://raw.githubusercontent.com/sannnn1234/skilltest/main/screenshots/order.png)
![Local Setup](https://raw.githubusercontent.com/sannnn1234/skilltest/main/screenshots/gateway.png)

---
## Docker Setup
**Dockerfile**
Each service:
1. Uses Node.js base image
2. Installs dependencies
3. Exposes port
4. Runs with node app.js

---

## Docker Compose YAML
**docker-compose.yml**
1. Multi-container orchestration
2. Shared bridge network
3. Service dependency handling
---
## Docker Compose Logs 
![Local Setup](https://raw.githubusercontent.com/sannnn1234/skilltest/main/screenshots/dockerlog.png)

---








