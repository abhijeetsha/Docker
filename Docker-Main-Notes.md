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
* ### #Start from a base image
* FROM python:3.10

* ### # Set working directory
* WORKDIR /app

* ### # Copy code into container
* COPY . .

* ### # Install dependencies
* RUN pip install -r requirements.txt

* # Command to run app
* CMD ["python", "app.py"]

