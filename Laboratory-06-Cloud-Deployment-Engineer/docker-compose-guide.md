# Docker Compose Guide

## The services: Block
The services block defines the containers that Docker Compose manages. In this laboratory, it contains the database service using MariaDB and the app service using Nextcloud.

## Database Service
The database service uses the mariadb:10.6 image. Environment variables configure the database name, username, and passwords.

## Nextcloud Application Service
The app service uses the nextcloud image and maps port 8080 on the host to port 80 in the container. MYSQL_HOST=database tells Nextcloud to connect to the database service named database.

## docker run vs docker-compose up -d
The docker run command is commonly used to start an individual container. The docker-compose up -d command reads a Compose configuration file and starts the services defined in it in detached mode.

## Commands Used
- mkdir nextcloud-deployment
- cd nextcloud-deployment
- nano docker-compose.yml
- docker-compose up -d
- docker-compose ps
- docker-compose down
