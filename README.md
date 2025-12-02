# hello_flask

A simple **Flask** application running in a **Docker multi-stage build** environment with a MySQL database.

---

## Project Structure

hello_flask/
│
├── app.py                 # Flask application
├── Dockerfile             # Multi-stage Docker build
├── docker-compose.yml     # Docker Compose setup
├── aws/                   # Optional AWS CLI or scripts
│   ├── install
│   ├── wheel-0.45.1.dist-info/
│   └── awscliv2.zip
└── README.md              # Project documentation

---

## Features

- Flask application running in Docker.
- MySQL container for database integration.
- Multi-stage Docker build for smaller final image.
- Connects Flask to MySQL using `mysqlclient`.

---

## Requirements

- Docker
- Docker Compose

---

## How to Run

1. **Build the Docker images**:

    docker compose build --no-cache

2. **Start the containers**:

    docker compose up

3. **Access the Flask app**:

Open your browser at [http://localhost:5000](http://localhost:5000).  
You should see the message with the MySQL version.

---

## Notes

- MySQL container uses root password: `my-secret-pw`.
- Flask app connects to MySQL using container name `mydb`.

---

## License

MIT License

