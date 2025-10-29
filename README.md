# FastAPI-RESTful-API-System1
This project includes authentication and user management backend built using FastAPI, SQLAlchemy ORM, and PostgreSQL.
It provides secure APIs for user registration, login, verification, password reset, and password updates, along with basic CRUD for articles.

The project also includes JWT-based authentication, Alembic migrations, Docker containerization, and optional GitHub Actions CI/CD integration for deployment on AWS or any cloud provider..

Features

🔑 User Registration & Login with JWT Authentication

🔒 Password Reset & Update (Forgot / Reset APIs)

📧 Email Verification Flow

📰 Article Create & List APIs

🐘 PostgreSQL (Async with SQLAlchemy)

⚙️ Alembic Database Migrations

🐳 Dockerized Setup for Local/Cloud Environments

☁️ CI/CD Ready (GitHub Actions + Docker + AWS)





Tech Stack

FastAPI – High-performance Python web framework

PostgreSQL – Relational database

SQLAlchemy ORM (Async) – Database interaction layer

Alembic – Database migrations

JWT (PyJWT) – Secure token authentication

Docker – Containerized environment

GitHub Actions – Continuous Integration and Deployment




Installation & Setup
🐳 Run with Docker



Make sure you have Docker installed
 on your system.

Clone this repository:

git clone https://github.com/ayushkumarrocc1201/secureauth-api.git
cd secureauth-api


Copy environment variables file:

cp .env.example .env


Add your PostgreSQL credentials and JWT secret inside .env.

Build and start containers:

docker-compose up -d --build


or (new syntax)

docker compose up -d --build




App will be live at:
👉 http://localhost:8000

🧪 Run without Docker

If you want to run locally (not in Docker):

Add PostgreSQL credentials in:

alembic/env.py

src/core/config.py

Install dependencies:

pip install -r requirements.txt


Run migrations & start the app:

chmod 755 start.sh
sh start.sh



Installation & Setup
🐳 Run with Docker

Make sure you have Docker installed
 on your system.

Clone this repository:

git clone https://github.com/ayushkumarrocc1201/secureauth-api.git
cd secureauth-api


Copy environment variables file:

cp .env.example .env


Add your PostgreSQL credentials and JWT secret inside .env.

Build and start containers:

docker-compose up -d --build


or (new syntax)

docker compose up -d --build


App will be live at:
👉 http://localhost:8000

🧪 Run without Docker

If you want to run locally (not in Docker):

Add PostgreSQL credentials in:

alembic/env.py

src/core/config.py

Install dependencies:

pip install -r requirements.txt


Run migrations & start the app:

chmod 755 start.sh
sh start.sh



License

This project is open-source and developed by Ayush Kumar as part of learning and demonstrating secure backend development practices using FastAPI, Docker, and PostgreSQL.
