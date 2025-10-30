# Basic Commands Of Docker
## 1) Basic Docker Commands:-
* docker --version	     Check Docker version
* docker info	           Show system-wide Docker information
* docker images	         List all Docker images
* docker ps	             List running containers
* docker ps -a	         List all containers (including stopped)
* docker pull <image_name>	    Download an image from Docker Hub
* docker run <image_name>	      Run a container from an image
* docker run -d <image>	        Run container in detached (background) mode
* docker run -it <image> /bin/bash	   Run container interactively
* docker stop <container_id>	         Stop a running container
* docker start <container_id>	         Start a stopped container
* docker restart <container_id>	       Restart a container
* docker rm <container_id>	           Remove a container
* docker rmi <image_id>	               Remove an image
* docker exec -it <container_id>       bash	Enter a running container shell
* docker logs <container_id>	         View container logs
* docker build -t <image_name> .	     Build image from Dockerfile in current dir
* docker tag <source_image> <new_name>	   Rename/tag an image
* docker network ls	       List Docker networks
* docker volume ls	       List Docker volumes

## 2) Dockerfile Commands:-
### These are instructions used inside a Dockerfile (not CLI commands):
* FROM	>>>>> Set base image (e.g., FROM ubuntu:20.04)
* WORKDIR	>>>>> Set working directory inside container
* COPY	>>>>> Copy files from host to container
* ADD	 >>>>> Similar to COPY, but supports URLs and archives
* RUN	>>>>> Execute a command during build (e.g., RUN apt-get install)
* CMD	>>>>> Command that runs when container starts
* ENTRYPOINT >>>>>	Set main executable for the container
* EXPOSE	>>>>> Document the port the container listens on
* ENV	>>>>> Set environment variables
* VOLUME >>>>> Create mount point for volumes
* LABEL	>>>>> Add metadata (like maintainer info)






