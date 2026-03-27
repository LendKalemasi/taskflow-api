# Taskflow API

A lightweight REST API for managing tasks, built with FastAPI and SQLite. Supports full CRUD operations with automatic data validation and interactive API docs.

## Tech Stack

- Python
- FastAPI
- SQLAlchemy
- SQLite
- Uvicorn

## Getting Started

### 1. Clone the repository

git clone https://github.com/yourusername/taskflow-api.git
cd taskflow-api

### 2. Install dependencies

pip install -r requirements.txt

### 3. Run the server

python -m uvicorn main:app --reload

### 4. Open the interactive docs

http://127.0.0.1:8000/docs

## Endpoints

| Method | Route | Description |
|--------|-------|-------------|
| GET | /tasks/ | Get all tasks |
| GET | /tasks/{id} | Get a task by ID |
| POST | /tasks/ | Create a new task |
| PUT | /tasks/{id} | Update a task |
| DELETE | /tasks/{id} | Delete a task |

## Project Structure

taskflow-api/
├── main.py
├── database.py
├── models.py
├── schemas.py
├── crud.py
├── requirements.txt
├── README.md
└── routers/
    └── tasks.py