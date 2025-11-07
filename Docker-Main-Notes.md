# Docker Main Notes:
## 🐳 1. What is Docker?
### Ans: Docker is a containerization platform that allows you to build, run, and manage applications in lightweight, portable containers.
* A container packages an application and all its dependencies (libraries, binaries, configuration files) so it runs consistently across environments.

## ✅ Key benefits:
* Consistency across development → production
* Lightweight and fast (uses host OS kernel)
* Easy scalability and deployment
* Version-controlled environments

## 📄 2. What is a Dockerfile?
### Ans: A Dockerfile is a text file that contains a series of instructions for building a Docker image.
* Each instruction defines how the image is built — for example, what base image to use, what dependencies to install, and what command to run.

## 🧩 Example:
* ### # Start from a base image
* FROM python:3.10

* ### # Set working directory
* WORKDIR /app

* ### # Copy code into container
* COPY . .

* ### # Install dependencies
* RUN pip install -r requirements.txt

* ### # Command to run app
* CMD ["python", "app.py"]

## 🧱 3. What is a Docker Image?
### Ans: A Docker Image is a read-only template used to create containers.
* It includes everything needed to run an application — code, runtime, libraries, environment variables, and configuration files.
### You can think of it as a blueprint for containers.
 * Built using a Dockerfile
 * Stored locally or on a Docker registry
 * Immutable (cannot be changed once built)

## 📦 4. What is a Docker Container?
### Ans: A Docker Container is a running instance of a Docker image.
* It’s an isolated environment that runs your application with its own file system, networking, and process space — but shares the host OS kernel.
## 🧩 Example commands:
### # Run a container
* docker run -d -p 8080:80 nginx

### # List running containers
* docker ps

### # Stop and remove a container
* docker stop <container_id>
* docker rm <container_id>

## 🌐 5. What is Docker Networking?
### Ans: 
