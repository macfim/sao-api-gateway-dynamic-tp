# API Gateway with Kong

A simple demonstration of an API Gateway architecture using Kong to route traffic to multiple microservices.

## Project Structure

- `service-a`: Simple Node.js service exposing user data on port 3001
- `service-b`: Simple Node.js service exposing product data on port 3002
- `kong.yml`: Kong Gateway declarative configuration
- `docker-compose.yml`: Docker Compose configuration to orchestrate all services

## Prerequisites

- Docker
- Docker Compose

## Getting Started

```bash
# Start all services
docker-compose up -d
```

## Access Points

- Kong Gateway: http://localhost:8000
- Service A (Users): http://localhost:8000/users
- Service B (Products): http://localhost:8000/products
- Kong Admin API: http://localhost:8001
