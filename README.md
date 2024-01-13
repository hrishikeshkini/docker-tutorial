# Docker-tutorial
This repository contains a simple Python application that can be containerized using Docker.

## Docker Setup

### Build Image

To build the Docker image, use the following command:

```bash
docker build -t welcome-app .
```

### View Docker Images

To see the list of Docker images on your system, run:

```bash
docker images
```

### Run Docker Image

To run the Docker image and expose it on port 5000, use:

```bash
docker run -p 5000:5000 welcome-app
```

### View Running Containers

To see the running Docker containers, run:

```bash
docker ps
```

### Stop Running Container

To stop a running Docker container, use the following command, replacing containerID with the actual container ID:

```bash
docker stop containerID
```

### Docker Login

Before pushing images to Docker Hub, make sure to log in using:

```bash
docker login
```

### Delete Image

To delete a Docker image, use:

```bash
docker image rm -f welcome-app
```

### Build and Push Image to Docker Hub

Always build and push the image in the following format:

```bash
docker build -t hrishikeshkini/welcome_app .
docker push hrishikeshkini/welcome_app:latest
```

### Rename Images

To rename a Docker image, use the docker tag command:

```bash
docker tag hrishikeshkini/welcome_app hrishikeshkini/welcome_app1
```

### Pull Image from Docker Hub

To pull the image from Docker Hub, use:

```bash
docker pull hrishikeshkini/welcome_app
```
### Run Image in Detached Mode

To run the Docker image in detached mode, use:

```bash
docker run -d -p 5000:5000 hrishikeshkini/welcome_app:latest
```