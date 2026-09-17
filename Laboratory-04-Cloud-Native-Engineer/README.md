# Laboratory 04 - The Cloud-Native Engineer

## Mission Overview

This lab is concerned with the understanding of the concept of the difference between Virtual Machines and Containers and about the basics of using Docker. I used the KillerCoda Playground for testing, to verify Docker, to download an Nginx image, to run an Nginx container, to run some test on the web server, and to practice some basic container lifecycle commands.

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

I have been introduced to the basic Docker commands, how to pull an image, create a container and start it, map a host port to a container port, test a containerized Web server, and manage the lifecycle of the container. I also got to know about how applications may be deployed in a lightweight environment using containers.

## Challenges Encountered

There was one tricky thing I had to get my head around that is understanding how to use Docker commands in conjunction with each other when creating and managing a container. Also, I wanted to know what port mapping is and what's the host port 8080 being mapped to in the Nginx container. It was obvious to me what was going on as I followed each of the terminal commands.
