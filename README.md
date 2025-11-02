**Opus Lab — DevOps Engineer Project (2025–2026)**


**Author Name**: Feten Rhamna 
Role: DevOps Engineer Candidate — Opus Lab Internship 
Email:fetenrhamna6@gmail.com

**Project Overview** :
This project was developed as part of the Opus Lab DevOps Engineer Technical

Screening. It demonstrates containerization, orchestration, CI/CD automation, and infrastructure as code

(IaC) principles.

**Objective:** 
Containerize a Spring Boot application, automate its build pipeline using GitHub Actions, and

validate a simple Terraform configuration for cloud resource management.

**Tech Stack Backend:** Java, Spring Boot 
**Containerization:** Docker, Docker Compose
 **CI/CD:** GitHub

**Actions Infrastructure as Code:** Terraform

**Project Structure:** 
OpusLAb-/

├── backend/                  # Spring Boot backend source

│   ├── src/

│   ├── pom.xml

│   ├── Dockerfile

│   └── target/

│

├── infra/

│   └── terraform/            # Terraform infrastructure code

│       ├── main.tf

│       └── variables.tf

│

├── docker-compose.yml         # Backend + Database services

└── .github/

&nbsp;   └── workflows/

&nbsp;       └── ci.yml 
 **Docker Setup Build the backend image:** docker build -t opuslab-backend ./backend

**Run the application:** docker run -p 8080:8080 opuslab-backend Then open: http://localhost:8080/hello

**Docker Compose Setup Launch backend and PostgreSQL together:** docker compose up --build 
Then

**open:** http://localhost:8080
 **Stop the services:** docker compose down

**Continuous Integration (GitHub Actions) File:** .github/workflows/ci.yml Triggered on every push or pull

request to main.

**Steps:** 
- Checkout repository
 - Set up JDK 17 
- Cache Maven dependencies 
- Build Spring Boot project 
-Lint Dockerfile 
- Build Docker image

**Infrastructure as Code (Terraform) Directory:** infra/terraform Terraform defines a Google Cloud Storage

bucket (demo purpose).

**Commands:** terraform init terraform validate

**Result:** Success! The configuration is valid.

**No real cloud deployment was performed. The goal was syntax validation only.**

**Results Summary Containerization:** Completed Orchestration: Completed CI/CD: Completed Infrastructure

as Code: Completed

**Deliverables** :
GitHub Repository: https://github.com/feten517/OpusLAb-
Project Type: DevOps Engineer
Opus Lab Internship Challenge Submission Deadline: November 3, 2025

**Notes:** This project demonstrates understanding of key DevOps concepts:
 - Containerization with Docker 
-Orchestration with Docker Compose 
- Continuous Integration using GitHub Actions
 - Infrastructure as Code validation using Terraform

**Status:** Ready for submission — Opus Lab DevOps Engineer Challenge (2025–2026)

