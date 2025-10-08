AI-TaskBoard

AI-TaskBoard is a modern SaaS platform for task and team management, built with Java 17 + Spring Boot, PostgreSQL, Docker, and GitHub Actions.

It provides a clean, reliable, and scalable backend for small teams, startups, and freelancers who need an efficient project tracking system without enterprise-level complexity.

🚀 Key Features

Create, update, and delete tasks

Status workflow: To Do → In Progress → Done

Assign users and manage responsibilities

Priorities and due dates

JWT authentication and roles (coming soon)

PostgreSQL database with Flyway migrations

Docker & docker-compose support

Continuous Integration and Deployment via GitHub Actions

Unit and integration testing with JUnit 5

🧱 Project Architecture
ai-taskboard
├── src/main/java/com/romankafi/taskboard
│   ├── TaskboardApplication.java
│   ├── config/ controller/ dto/ entity/ repository/ service/
│   └── mapper/
├── src/main/resources/db/migration/
├── docker/Dockerfile
├── docker/docker-compose.yml
├── .github/workflows/ci.yml
├── .gitignore
├── pom.xml
└── README.md

🔌 REST API
Method	Endpoint	Description
GET	/api/v1/health	Health check
GET	/api/v1/tasks	Get all tasks with filters
GET	/api/v1/tasks/{id}	Get task by ID
POST	/api/v1/tasks	Create a new task
PUT	/api/v1/tasks/{id}	Update task
PATCH	/api/v1/tasks/{id}	Change status
DELETE	/api/v1/tasks/{id}	Delete task
GET	/api/v1/users	List users
⚙️ Quick Start
git clone https://github.com/RomanKAFI/ai-taskboard.git
cd ai-taskboard
./mvnw clean install
./mvnw spring-boot:run


Check: http://localhost:8080/api/v1/health

Swagger UI (if enabled): http://localhost:8080/swagger-ui

🐳 Run with Docker
docker compose up --build
docker compose down -v

🔐 Environment Variables
SPRING_PROFILES_ACTIVE=dev
SERVER_PORT=8080
DB_HOST=postgres
DB_PORT=5432
DB_NAME=taskboard
DB_USER=taskboard
DB_PASSWORD=taskboard
JWT_SECRET=change-me
JWT_TTL_MINUTES=60

💰 Monetization & Billing

AI-TaskBoard uses a subscription-based SaaS model powered by Stripe API.

Plan	Users	Features	Price
Free	1 project / up to 5 tasks	Core features	$0
Pro	up to 5 users	Unlimited tasks, priority support	$8 / month
Team	up to 20 users	SSO, backups	$29 / month
Enterprise	Unlimited	SLA, integrations, custom features	Custom pricing

Stripe integration supports Checkout Sessions, Webhooks, free trials (14 days), and automatic subscription renewals.

🤖 AI Features

Automatic task description generation (NLP)

Intelligent task prioritization and due-date prediction

Productivity analytics & team insights

Smart recommendations (under development)

🔁 CI/CD Pipeline

Automatic build & test on every push

Maven cache and dependency audit

Ready for production deployment via GitHub Actions + Docker Hub

🗺 Roadmap

 REST API + DB migrations

 Docker + CI/CD

 JWT authentication & roles

 Swagger / Postman collection

 Stripe integration

 AI-powered analytics

 Public demo deployment

⚙️ Requirements

Java 17+

Maven 3.9+

Docker Desktop

🤝 Contributing

Pull requests are welcome!
Follow conventional commits, include tests, and provide clear descriptions of changes.

📜 License

Proprietary License — All rights reserved © 2025 Roman Kafitulin.
This software is proprietary and may not be used, copied, modified, or distributed without prior written permission from the author.
