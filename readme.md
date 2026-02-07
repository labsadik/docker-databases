````markdown
# Docker Databases

This repository provides ready-to-use Docker Compose configurations for running popular databases locally using Docker.  
It is intended for **development and learning purposes**, so you don’t need to install databases directly on your system.

---

## What is this?

`docker-databases` helps you quickly start database servers in Docker containers.  
Each database has its own folder with a `docker-compose.yml` file.

You can run, stop, and remove databases easily using Docker Compose.

---

## Databases Included

- MySQL
- PostgreSQL
- MongoDB
- Redis

---

## Prerequisites

Before using this project, make sure you have:

- Docker installed  
- Docker Compose installed  

---

## How to Use

### 1. Clone the Repository

```bash
git clone https://github.com/labsadik/docker-databases.git
cd docker-databases
````

---

### 2. Start a Database

Go into the database folder you want and run Docker Compose.

**Example: MySQL**

```bash
cd mysql
docker compose up -d
```

Docker will download the image (if needed) and start the container.

---

### 3. Database Ports

| Database   | Port  |
| ---------- | ----- |
| MySQL      | 3306  |
| PostgreSQL | 5432  |
| MongoDB    | 27017 |
| Redis      | 6379  |

You can connect using any database client or from your application using `localhost`.

---

### 4. Stop the Database

To stop and remove the running container:

```bash
docker compose down
```

---

## Notes

* This project is **not recommended for production use**.
* You can modify environment variables in `docker-compose.yml` files if needed.
* Make sure the ports are free before starting containers.

---
