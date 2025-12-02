# hello_flask

A simple **Flask** application running in a **Docker multi-stage build** environment with a MySQL database.

---

## Description

This project demonstrates a Flask application containerized using Docker with a MySQL backend.  
It uses a multi-stage Docker build to produce a lightweight final image. The Flask app connects to MySQL using the `mysqlclient` library.

---

## Requirements

- Docker
- Docker Compose

---

## Common Commands

### Build Docker images
docker compose build --no-cache

### Start containers
docker compose up

### Stop containers
docker compose down

### Access Flask app
Open your browser at [http://localhost:5000](http://localhost:5000)  
You should see the message with the MySQL version.

---

## Notes

- MySQL container uses root password: `my-secret-pw`
- Flask app connects to MySQL using container name `mydb`

---

## License

MIT License
