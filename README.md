# hello_flask

A simple Flask application containerized using Docker with a MySQL database.

---

## Description

This project demonstrates a Flask application running in a multi-stage Docker build with MySQL as the backend.  
It uses `mysqlclient` to connect to the database.

---

## Requirements

- Docker
- Docker Compose

---

## Docker & Docker Compose Commands

### Build the images
docker build -t my-flask-app:latest .

### Build using docker-compose
docker compose build

### Build with no cache
docker compose build --no-cache

### Start containers
docker compose up

### Start containers in detached mode
docker compose up -d

### Stop containers
docker compose down

### Stop and remove containers, networks, volumes, and images created by `up`
docker compose down --rmi all -v

### Restart containers
docker compose restart

### View logs
docker compose logs
docker compose logs -f   # follow logs in real-time

### List running containers
docker ps
docker compose ps

### Enter a running container
docker exec -it <container_name> bash

### Remove a container
docker rm <container_name>

### Remove an image
docker rmi <image_name>

---

## Access the Flask App

Open your browser at [http://localhost:5000](http://localhost:5000)  
You should see the message with the MySQL version.

---

## Notes

- MySQL root password: `my-secret-pw`
- Flask app connects to MySQL using container name `mydb`

