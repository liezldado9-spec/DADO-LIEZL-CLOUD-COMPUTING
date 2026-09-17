# Laboratory 04 - The Cloud-Native Engineer

## Mission Overview

This laboratory focuses on understanding the difference between Virtual Machines and Containers and learning the basic use of Docker. I used the KillerCoda Playground to verify Docker, download an Nginx image, run an Nginx container, test the web server, and practice basic container lifecycle commands.

## Objectives

* Differentiate Virtual Machines and Containers.
* Access a Docker-enabled cloud environment.
* Execute fundamental Docker CLI commands.
* Pull, run, manage, and terminate an Nginx container.
* Document container operations using Markdown.
* Continue developing my GitHub Cloud Computing portfolio.

## Docker Commands Executed

### Check Docker Version

```bash
docker --version
```

### Check Docker Information

```bash
docker info
```

### Pull Nginx

```bash
docker pull nginx
```

### Run Nginx

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

### Test Nginx

```bash
curl http://localhost:8080
```

### List Running Containers

```bash
docker ps
```

### Stop Nginx

```bash
docker stop nginx-server
```

### Verify Stopped Container

```bash
docker ps
```

### Remove Container

```bash
docker rm nginx-server
```

### Verify Removal

```bash
docker ps -a
```

## Skills Learned

I learned how to use basic Docker commands, pull an image, create and run a container, map a host port to a container port, test a containerized web server, and manage the container lifecycle. I also learned how containers can be used to deploy applications in a lightweight environment.

## Challenges Encountered

One challenge I encountered was understanding how Docker commands work together when creating and managing a container. I also needed to understand the purpose of port mapping and how port 8080 on the host connects to port 80 inside the Nginx container. Using the terminal commands step-by-step helped me understand the process better.
