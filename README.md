AI-TaskBoard

Task management SaaS built with Java + Spring Boot, PostgreSQL, Docker, and CI/CD pipeline.

🚀 Overview

AI-TaskBoard is a task management platform designed as a full-stack SaaS prototype.
The goal of the project is to demonstrate modern backend development practices, including:

REST API with Spring Boot

PostgreSQL relational schema with indexing & normalization

Dockerized deployment

GitHub Actions for CI/CD

AI-assisted development patterns for scaling

🛠 Tech Stack

Backend: Java 17, Spring Boot

Database: PostgreSQL (JPA/Hibernate, schema migrations)

DevOps: Docker, Docker Compose, GitHub Actions (CI/CD)

Testing: JUnit, Postman API tests

Other: Agile practices, REST APIs, Unit Testing, AI-assisted code generation

📂 Features

Create / Update / Delete tasks

Organize tasks by status (To Do, In Progress, Done)

Assign tasks to different users

Basic authentication & authorization

Persistent storage with PostgreSQL

Docker-ready for deployment

CI/CD pipeline for automated testing & deployment

📦 Project Structure (planned)
ai-taskboard/
├── src/main/java/com/romankafi/taskboard   # Backend source
├── src/test/java/com/romankafi/taskboard   # Unit & integration tests
├── docker/                                 # Dockerfile & configs
├── pom.xml                                 # Maven build config
└── README.md

🔧 Setup & Run

Clone repository:

git clone https://github.com/RomanKAFI/ai-taskboard.git
cd ai-taskboard


Build with Maven:

mvn clean install


Run locally:

mvn spring-boot:run


Run with Docker (coming soon).

✅ Roadmap

 Create project repository with README, license, gitignore

 Add base Spring Boot application

 Implement REST endpoints for tasks

 Add PostgreSQL schema & persistence

 Dockerize application

 Set up CI/CD with GitHub Actions

 Deploy demo instance

📜 License

MIT License — free to use and modify.
