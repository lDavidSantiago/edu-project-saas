# edu-project-saas
Edu Project SaaS

Educational platform built as a SaaS application using React, FastAPI, and PostgreSQL.

Architecture

graph TD
    A[React Frontend] -->|HTTP / REST API| B[FastAPI Backend]
    B -->|SQL / ORM| C[(PostgreSQL Database)]
    B --> D[Authentication]
    B --> E[Business Logic]
    B --> F[API Routes]

Technology Stack

* Frontend: React
* Backend: FastAPI
* Database: PostgreSQL
* API: REST
* ORM: SQLAlchemy

Project Structure

edu-project-saas/
│
├── backend/
│   ├── app/
│   │   ├── api/
│   │   ├── core/
│   │   ├── models/
│   │   ├── schemas/
│   │   ├── services/
│   │   └── main.py
│   └── requirements.txt
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   └── App.jsx
│   └── package.json
│
└── README.md

Backend

The backend is built with FastAPI and provides the REST API used by the frontend.

Main responsibilities:

* Authentication and authorization
* User management
* Course management
* Educational content
* Enrollments
* Learning progress
* Evaluations

API documentation is available through FastAPI:

http://localhost:8000/docs

Frontend

The React frontend provides the user interface and communicates with the backend through the REST API.

React → FastAPI → PostgreSQL

Database

PostgreSQL stores the main application data, including users, courses, lessons, enrollments, evaluations, and learning progress.


License 

This project is intended for educational purposes.

