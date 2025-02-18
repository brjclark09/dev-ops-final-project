---
title: "Containerization"
author: "Brandon Clark"
description: "A summary of what I've learned this semester for the topic of containerization."
published: "2024-2-14"
---
# Containerization

## Basic Docker Commands

### Adding Docker on linux based systems:
```sh
sudo dnf config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
```

### Install Docker and Dependancies:
```sh
sudo dnf install -y docker-ce docker-ce-cli containerd.io docker-compose-plug
```

### Start and Enable a Package:
```sh
sudo systemctl start [PACKAGE]
sudo systemctl enable [PACKAGE]
```

### Check Version of Docker:
```sh
docker --version
```

### Access a Container:
```sh
docker exec -it [CONTAINERNAME] bash
```

### Pull an Image
```sh
docker pull [IMAGE_NAME]
```
Example:
```sh
docker pull nginx
```

### Run a Container
```sh
docker run [IMAGE_NAME]
```

### List Running Containers
```sh
docker ps
```
List all containers, including stopped ones:
```sh
docker ps -a
```

### Stop a Container
```sh
docker stop [CONTAINER_ID]
```

### Remove a Container
```sh
docker rm [CONTAINER_ID]
```

### Remove an Image
```sh
docker rmi [IMAGE_NAME]
```

### List Images
```sh
docker images
```

## Docker Storage

### Create a Volume
```sh
docker volume create [VOLUME_NAME]
```

### List Volumes
```sh
docker volume ls
```

### Remove a Volume
```sh
docker volume rm [VOLUME_NAME]
```

## Networking in Docker

### List Networks
```sh
docker network ls
```

### Docker Networking
```sh
docker network create [NETWORK_NAME]
```

### Connect a Container to a Network
```sh
docker network connect [NETWORK_NAME] [CONTAINER_NAME]
```

### Disconnect a Container from a Network
```sh
docker network disconnect [NETWORK_NAME] [CONTAINER_NAME]
```

### Inspect a Network
```sh
docker network inspect [NETWORK_NAME]
```

### Remove a Network
```sh
docker network rm [NETWORK_NAME]
```

## Port Mapping

### Run a Container with Port Mapping
```sh
docker run -d -p [HOST_PORT]:[CONTAINER_PORT] [IMAGE_NAME]
```
Example:
```sh
docker run -d -p 8080:80 nginx
```

## Running Containers with Flags

### `-d` (Detached Mode)
```sh
docker run -d nginx
```

### `-p` (Port Mapping)
```sh
docker run -p 8080:80 nginx
```

### `-i` (Interactive Mode)
```sh
docker run -i nginx
```

### `-it` (Interactive Terminal)
```sh
docker run -it ubuntu bash
```

### `-v` (Volume Mounting)
```sh
docker run -v /home:/container/folder nginx
```