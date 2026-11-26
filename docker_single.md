# DOCKER SINGLE CONTAINER COMMANDS

## 1. Check Docker

docker --version

# Checks Docker version

sudo systemctl start docker

# Starts Docker service

sudo systemctl status docker

# Checks Docker service status

## 2. Create a Project

mkdir docker-app

# Creates project folder

cd docker-app

# Enters project folder

## 3. Create HTML File

nano index.html

# Creates HTML file

## 4. Write HTML Code

<html>
<head>
    <title>Docker Demo</title>
</head>
<body>
    <h1>Hello from Docker!</h1>
</body>
</html>

# Simple web page displayed by Nginx

## 5. Create Dockerfile

nano Dockerfile

# Creates Dockerfile

## 6. Write Dockerfile

FROM nginx:latest
COPY index.html /usr/share/nginx/html/index.html
EXPOSE 80

# Uses Nginx image
# Copies HTML file into Nginx web directory
# Exposes port 80

## 7. Build Docker Image

docker build -t my-nginx .

# Builds Docker image named my-nginx

## 8. Run Container

docker run -d -p 8080:80 --name my-container my-nginx

# Runs container in background
# Maps host port 8080 to container port 80

## 9. Check Container

docker ps

# Lists running containers

docker ps -a

# Lists all containers

## 10. Open Application

http://localhost:8080

# Opens the web application in browser

## 11. Stop and Remove Container

docker stop my-container

# Stops container

docker rm my-container

# Removes container

## 12. Remove Image

docker rmi my-nginx

# Removes Docker image
