
# Containerized Calculator Project

This repository contains a simple calculator web application built with Node.js and HTML, and containerized using Docker.  
This is my first containerization project, through which I have strengthened my fundamentals of Docker and hands-on usage of core Docker commands.

## File Descriptions

- *server.js* – Main Node.js backend file that sets up the server and handles POST requests for calculator operations.
- *calculator.html* – The frontend HTML file providing the user interface for the calculator.
- *Dockerfile* – Instructions to build a Docker image and run the app using server.js.

## Essential Docker Commands used in the Project

| Command                                                      | Description                              |
|--------------------------------------------------------------|------------------------------------------|
| docker build -t <image_name> .                             | Build a Docker image from Dockerfile     |
| docker images                                              | List all Docker images                   |
| docker run -p 3000:3000 <image_name>                       | Run container and map port               |
| docker ps                                                  | List running containers                  |
| docker stop <container_name>                               | Stop a running container                 |
| docker rm <container_name>                                 | Remove a stopped container               |
| docker rmi <image_name>                                    | Remove a Docker image                    |
| docker volume create <volume_name>                         | Create a named Docker volume             |
| docker run -v <volume_name>:/data <image_name>             | Mount volume to /data in container     |
| docker run -v /host/path:/container/path <image_name>      | Bind mount host folder to container path |

***

Replace <image_name>, <container_name>, <volume_name>, /host/path, and /container/path with your specific names and paths. This covers the essential Docker commands for containerized calculator project.
