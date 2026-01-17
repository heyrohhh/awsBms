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

Maintained by: [Your Name]

Repository Link: https://github.com/heyrohhh/awsBms
