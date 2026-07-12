# FlyRank Internship — Assignment 1: Build Your First API Endpoint

The smallest possible backend: a Flask server with two JSON endpoints.

## Endpoints

| Method | Path              | Response                          |
|--------|-------------------|------------------------------------|
| GET    | `/health`         | `{"status": "ok"}`                 |
| GET    | `/hello?name=X`   | `{"message": "Hello, X!"}`         |

## Run locally

```bash
pip install -r requirements.txt
python app.py
```

Server starts at `http://127.0.0.1:5000`.

## Test it

**curl:**
```bash
curl http://127.0.0.1:5000/health
curl "http://127.0.0.1:5000/hello?name=Warid"
```

**Browser:**
Open `http://127.0.0.1:5000/health` or `http://127.0.0.1:5000/hello?name=Warid` directly.

## What this demonstrates

- A running server listening for HTTP requests
- Two GET routes returning JSON responses
- The request → response loop, made concrete: client sends a request, server parses it, server sends back structured data
