# Docker FastAPI

A lightweight **FastAPI REST API running inside Docker**.

## Features

* FastAPI REST API
* Dockerized application
* Health check endpoint
* Interactive API documentation

## Endpoints

| Method | Endpoint  | Response                           |
| ------ | --------- | ---------------------------------- |
| `GET`  | `/`       | `{"message": "Hello from Docker"}` |
| `GET`  | `/health` | `{"status": "healthy"}`            |

## Run with Docker

```bash
docker build -t docker-fastapi .
docker run -d -p 8000:8000 --name fastapi-app docker-fastapi
```

Open:

```text
http://localhost:8000
```

### API Docs

* Swagger: `http://localhost:8000/docs`
* ReDoc: `http://localhost:8000/redoc`

## Project Structure

```text
Docker-FastApi/
├── main.py
├── Dockerfile
├── requirements.txt
└── README.md
```

## Tech Stack

**Python · FastAPI · Uvicorn · Docker**

---

Built by **Arsalan Ali**
[GitHub](https://github.com/Arsalan5629)
