# Docker-All-Basic Commands & Explanations
## What is Docker..?
### Ans: Docker is a containerization platform that allows you to package applications and their dependencies into lightweight, portable containers.
These containers ensure that your app runs the same way on any system, regardless of environment differences.
### 🔹 Key points:
  * A container is like a small, isolated environment for your app.
  * It includes everything needed: code, libraries, configuration, and runtime.
  * Containers are faster and more efficient than virtual machines.
  * You can easily build, ship, and run applications anywhere (e.g., your laptop, server, or cloud).

## What is Docker-File...?
### Ans: A Dockerfile is a text file that contains instructions on how to build a Docker image.
   * Each instruction defines a step — like choosing a base image, copying files, installing dependencies, and running commands.
###🔹 Example Dockerfile:
### # Step 1: Use a base image
   * FROM python:3.10
### # Step 2: Set working directory
   * WORKDIR /app
### # Step 3: Copy project files
   * COPY . /app
### # Step 4: Install dependencies
   * RUN pip install -r requirements.txt
### # Step 5: Command to run the app
   * CMD ["python", "app.py"]


## What is Docker Compose file..?
### Ans:

## Basic Commands Of Docker And Docker-Compose With Explanations

