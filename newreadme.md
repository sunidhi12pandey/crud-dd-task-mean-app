# MEAN Stack CRUD Application

This repository contains a **full-stack CRUD application** built using the **MEAN stack** (MongoDB, Express, Angular 15, Node.js). The backend provides REST APIs with Node.js and Express connected to a MongoDB database, and the frontend is an Angular application communicating via HTTPClient.

As a DevOps engineer, I have implemented **Dockerfiles**, **Docker Compose**, and a **CI/CD pipeline** for automated building, testing, and deployment.

---

## Project Structure
.
├── backend/
│ └── Dockerfile # Dockerfile for Node.js backend
├── frontend/
│ └── Dockerfile # Dockerfile for Angular frontend
├── docker-compose.yml # Docker Compose file to orchestrate MongoDB, backend, frontend
└── .github/
└── workflows/
└── build_and_test.yml # GitHub Actions CI/CD pipeline


---

## Key Features

- Full-stack CRUD operations using MEAN stack.
- Backend and frontend containerized with Docker.
- Multi-container orchestration using Docker Compose.
- CI/CD automation using GitHub Actions.
- Integration testing during pipeline execution.

---

## How to Run Locally

1. Clone the repository:

```bash
git clone https://github.com/sunidhi12pandey/crud-dd-task-mean-app.git
cd crud-dd-task-mean-app
````

2. Start all services using Docker Compose:

```bash
docker-compose up --build
```

3. Access the application:

* Frontend: [http://localhost](http://localhost)
* Backend APIs: [http://localhost:8080](http://localhost:8080)

4. To stop the containers:

```bash
docker-compose down
```

---

## Author

**Sunidhi Pandey** – DevOps Engineer

* Developed Dockerfiles for backend and frontend.
* Created Docker Compose orchestration.
* Implemented GitHub Actions CI/CD pipeline for automated build, test, and deployment.

```
