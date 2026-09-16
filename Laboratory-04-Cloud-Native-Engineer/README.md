# Laboratory 04 – The Cloud-Native Engineer


## Mission Overview

This laboratory activity introduced the difference between traditional Virtual Machines and containers. It also provided hands-on experience using Docker in a KillerCoda environment to deploy and manage an Nginx web server.

## Objectives

- Differentiate Virtual Machines and Containers.
- Access a Docker-enabled cloud environment using KillerCoda.
- Execute fundamental Docker CLI commands.
- Pull, run, manage, and terminate an Nginx container.
- Document container operations using Markdown.

## Docker Commands Executed

```bash

docker --version
docker info
docker pull nginx
docker run -d -p 8080:80 --name mynginx nginx
docker ps
curl http://localhost:8080
docker stop mynginx
docker ps -a
docker rm mynginx


# Mission Reflection

## 1. Docker Container vs Virtual Machine

A Docker container can be started much faster than installing an operating system on a Virtual Machine. A VM requires a complete guest operating system and more resources, while a container shares the host operating system. In this activity, the Nginx container was created and started using a Docker command within a short time.

## 2. Purpose of Port Mapping

Port mapping using -p 8080:80 is necessary because the Nginx web server is running inside the container on port 80. The mapping connects port 8080 on the host to port 80 inside the container. This allows the web server to be accessed through localhost:8080.

## 3. Docker rm

The docker rm command removes the container. Any data stored only inside the removed container can be lost, while the Docker image used to create the container can remain available. This shows the difference between a container and its image.

## 4. Containers and DevOps

Containerization can make cooperation between developers and IT operations teams easier because applications can be packaged with their required environment. Developers can create and test containers while operations teams can deploy the same containerized application in another environment. This can make deployment more consistent.

## 5. GitHub Portfolio

My GitHub portfolio is becoming more organized as I add each laboratory activity. Lab 4 adds documentation about virtualization, containers, Docker commands, Nginx deployment, screenshots, and my reflection. The portfolio gives me a place to organize evidence of the cloud computing skills I practiced.
