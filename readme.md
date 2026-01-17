# CloudBook-Orchestrator 🚀
### Full-Stack Containerized Book Management System

CloudBook-Orchestrator is a robust, multi-tier web application designed for seamless book inventory management. This project serves as a showcase for **DevOps best practices**, featuring containerization, automated orchestration, and scalable cloud deployment strategies.

[![Tech Stack](https://img.shields.io/badge/Stack-React%20%7C%20Node%20%7C%20MySQL%20%7C%20Docker-blue)](https://github.com/heyrohhh/awsBms)

## 🛠️ Tech Stack & Architecture
- **Frontend:** React.js (Modern UI)
- **Backend:** Node.js / Express (RESTful API)
- **Database:** MySQL (Relational Data Persistence)
- **Orchestration:** Docker & Docker Compose
- **Cloud Ready:** AWS Optimized (EC2, ECS, RDS)

## 📁 Repository Structure
```plaintext
.
├── frontend/          # Client-side React application & Dockerfile
├── backend/           # Node.js API services & Dockerfile
├── database/          # SQL initialization scripts & schemas
└── docker-compose.yml # Service orchestration & network configuration
⚙️ Local Development (Docker-First)
This project is fully containerized. No local installation of Node or MySQL is required if you have Docker.

Clone the Repository:

Bash

git clone [https://github.com/heyrohhh/awsBms.git](https://github.com/heyrohhh/awsBms.git)
cd awsBms
Launch Services:

Bash

docker-compose up --build
Endpoints:

Frontend: http://localhost:3000

Backend API: http://localhost:5000

📝 Key Features
Full CRUD Operations: Seamlessly add, view, and delete book records.

Data Persistence: Integrated Docker Volumes to ensure MySQL data survives container restarts.

Environment Isolation: Microservices architecture with isolated network bridges for secure inter-service communication.

Production Ready: Optimized Dockerfiles for minimal image footprint.

☁️ Deployment Strategy (AWS Roadmap)
Currently optimized for the following AWS implementations:

Strategy A (Monolithic): Deploy via Docker Compose on a single Amazon EC2 (t2.micro).

Strategy B (Scalable): Decouple services using AWS ECS (Fargate) for compute and Amazon RDS for a managed database layer.

Maintained by: Rohit Neel Mishra

Repository Link: https://github.com/heyrohhh/CloudBook-Orchestrator-A-Containerized-Full-Stack-LMS.git

## 🏗️ Advanced DevOps Features
- **CI/CD Pipeline:** Automated build and deployment using **GitHub Actions**.
- **Security:** SSL/TLS certificate implementation using **Certbot** and **Nginx Reverse Proxy**.
- **Cloud Infrastructure:** Hosted on **AWS EC2** with custom Security Groups.
- **Service Orchestration:** Production-grade **Docker Compose** setup.

## 🚀 CI/CD Workflow (GitHub Actions)
Har `push` par pipeline ye steps perform karta hai:
1. Code linting aur security checks.
2. Docker images build karna.
3. EC2 instance par login karke containers ko auto-update/restart karna.

## 🔒 Nginx & SSL Configuration
- **Reverse Proxy:** Nginx backend API aur frontend traffic ko route karta hai.
- **SSL:** HTTPS enabled via Let's Encrypt for encrypted data transfer.
