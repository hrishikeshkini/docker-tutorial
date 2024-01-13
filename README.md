# docker-tutorial
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
