# DOCKER MULTI-CONTAINER COMMANDS

## 1. Check Docker

docker --version

# Checks Docker version

docker compose version

# Checks Docker Compose version

## 2. Create Project

mkdir multi-container-app

# Creates project folder

cd multi-container-app

# Enters project folder

## 3. Create Docker Compose File

nano docker-compose.yml

# Creates Docker Compose configuration file

## 4. Write docker-compose.yml

services:
  web:
    image: nginx:latest
    ports:
      - "8080:80"

  app:
    image: redis:latest

# Creates two services:
# web - Nginx container
# app - Redis container

## 5. Start Containers

docker compose up -d

# Builds (if needed) and starts all services in background

## 6. Check Containers

docker compose ps

# Lists containers created by Compose

docker ps

# Lists running containers

## 7. View Logs

docker compose logs

# Displays logs of all services

docker compose logs web

# Displays Nginx service logs

## 8. Stop Containers

docker compose stop

# Stops all services without removing containers

## 9. Stop and Remove Containers

docker compose down

# Stops and removes containers and network

## 10. Rebuild and Start

docker compose up -d --build

# Builds images and starts services in background
