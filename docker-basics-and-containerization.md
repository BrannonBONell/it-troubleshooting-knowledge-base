# Docker Basics and Containerization

# What is Docker?

Docker is a platform used to create and run containers.

Containers package:
- applications
- dependencies
- libraries
- configurations

into portable environments that run consistently across systems.

---

# What is a Container?

A container is an isolated environment used to run applications.

Benefits:
- lightweight
- portable
- consistent deployments
- fast startup times

Containers are commonly used in:
- cloud computing
- DevOps
- AI infrastructure
- web hosting
- software development

---

# Containers vs Virtual Machines

# Virtual Machines
- include full operating system
- larger resource usage
- slower startup

---

# Containers
- share host OS kernel
- lightweight
- faster startup
- lower resource usage

---

# Common Docker Use Cases

- web applications
- development environments
- databases
- APIs
- AI applications
- automation tools

---

# Docker Architecture

# Docker Engine
Main service that runs containers.

---

# Docker Image
Blueprint/template used to create containers.

Examples:
- Ubuntu
- Nginx
- Python

---

# Docker Container
Running instance of an image.

---

# Docker Hub
Public repository for Docker images.

Examples:
- nginx
- mysql
- ubuntu

---

# Installing Docker

# Windows
Install:
- Docker Desktop

Requirements:
- virtualization enabled
- WSL2 recommended

---

# Linux (Ubuntu Example)

```bash
sudo apt update
sudo apt install docker.io
```

Start Docker service:

```bash
sudo systemctl start docker
```

Enable Docker at boot:

```bash
sudo systemctl enable docker
```

---

# Basic Docker Commands

# Check Docker Version

```bash
docker --version
```

---

# Pull Image

```bash
docker pull ubuntu
```

Downloads image from Docker Hub.

---

# List Images

```bash
docker images
```

---

# Run Container

```bash
docker run ubuntu
```

---

# Interactive Shell

```bash
docker run -it ubuntu bash
```

Useful for:
- learning Linux
- troubleshooting
- testing commands

---

# List Running Containers

```bash
docker ps
```

---

# List All Containers

```bash
docker ps -a
```

---

# Stop Container

```bash
docker stop container-id
```

---

# Remove Container

```bash
docker rm container-id
```

---

# Remove Image

```bash
docker rmi image-name
```

---

# Running a Web Server Example

# Run Nginx Container

```bash
docker run -d -p 8080:80 nginx
```

Explanation:
- -d = detached/background mode
- -p = port mapping

Access in browser:

```text
http://localhost:8080
```

---

# Docker Networking Basics

Containers can communicate through virtual networks.

Common concepts:
- bridge networks
- port mapping
- container isolation

---

# Port Mapping Example

```bash
docker run -p 3000:3000 image-name
```

Maps:
host port → container port

---

# Docker Volumes

Volumes store persistent data outside containers.

Useful for:
- databases
- configuration files
- backups

Example:

```bash
docker volume create myvolume
```

---

# Dockerfile Basics

Dockerfiles automate image creation.

Example:

```Dockerfile
FROM ubuntu

RUN apt update

CMD ["echo", "Hello World"]
```

Build image:

```bash
docker build -t myimage .
```

---

# Common Docker Troubleshooting Scenarios

# Scenario 1
Container exits immediately.

Possible causes:
- application crash
- invalid command
- missing dependencies

Check logs:

```bash
docker logs container-id
```

---

# Scenario 2
Cannot access web application.

Possible causes:
- incorrect port mapping
- firewall issue
- container stopped

Check:
- docker ps
- port configuration

---

# Scenario 3
Docker daemon not running.

Linux check:

```bash
systemctl status docker
```

Start service:

```bash
sudo systemctl start docker
```

---

# Useful Docker Commands

# View Logs

```bash
docker logs container-id
```

---

# Enter Running Container

```bash
docker exec -it container-id bash
```

---

# Inspect Container

```bash
docker inspect container-id
```

---

# Resource Usage

```bash
docker stats
```

---

# Why Docker Matters

Docker is heavily used in:
- cloud environments
- DevOps
- CI/CD pipelines
- AI deployment
- microservices
- Kubernetes

Docker knowledge is valuable for:
- cloud support
- DevOps
- MLOps
- AI infrastructure
- system administration

---

# Beginner Docker Project Ideas

# Linux Practice Container
Run Ubuntu container and practice Linux commands.

---

# Nginx Web Server
Host simple webpage in Docker container.

---

# Python App Container
Containerize simple Python application.

---

# AI Chatbot Container
Run local AI application inside Docker.

---

# Key Troubleshooting Mindset

1. Check container status
2. Review logs first
3. Verify port mappings
4. Confirm networking
5. Test inside container
6. Isolate one issue at a time
