# Docker Deployment

## Docker Environment

### Check Docker Version

```bash
docker --version
```

Output:

```text
Docker version 29.1.3, build 29.1.3-0ubuntu3~24.04.2
```

This command displays the installed Docker version in the KillerCoda environment.

### Check Docker Status

```bash
docker info
```

The Docker environment was running successfully on Ubuntu 24.04.4 LTS. The Docker Server Version was 29.1.3, with the overlay2 storage driver and 1 CPU available.

This command displays detailed information about the Docker environment, including the Docker server, containers, images, storage driver, operating system, and available resources.

## Deploying Nginx

### Pull the Nginx Image

```bash
docker pull nginx
```

Output:

```text
Using default tag: latest
latest: Pulling from library/nginx
6310eb16bf42: Pull complete
9302921ce9b3: Pull complete
ab606a349520: Pull complete
0478569e858c: Pull complete
76225461b7d3: Pull complete
c06193164a25: Pull complete
3fe5ab3f8614: Pull complete
Digest: sha256:d0d674272be3be36f9a13d79194fa0db5aa630ab3ede9bec459d12f67370aaef
Status: Downloaded newer image for nginx:latest
docker.io/library/nginx:latest
```

This command downloads the Nginx image from Docker Hub so it can be used to create a container.

### Run the Nginx Container

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

Output:

```text
a68be7d3c2dfdb0d853c567683c37103f44a3a296090aa8e33a71d262137f5f8
```

This command creates and starts the Nginx container in detached mode and maps port 8080 on the host to port 80 inside the container.

### Test the Web Server

```bash
curl http://localhost:8080
```

The command successfully returned the Nginx HTML page. The output included:

```text
<h1>Welcome to nginx!</h1>
```

This confirms that the Nginx web server was successfully deployed and accessible through port 8080.

## Container Lifecycle

### List Running Containers

```bash
docker ps
```

Output:

```text
CONTAINER ID   IMAGE     COMMAND                  CREATED         STATUS         PORTS                                     NAMES
a68be7d3c2df   nginx     "/docker-entrypoint.…"   5 minutes ago   Up 5 minutes   0.0.0.0:8080->80/tcp, [::]:8080->80/tcp   nginx-server
```

This command lists the Docker containers that are currently running. The output confirms that the `nginx-server` container was running and that port 8080 was mapped to port 80.

### Stop the Container

```bash
docker stop nginx-server
```

Output:

```text
nginx-server
```

This command successfully stops the running Nginx container.

### Verify the Container Is Stopped

```bash
docker ps
```

Output:

```text
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
```

The output shows no running containers, confirming that the `nginx-server` container was successfully stopped.

### Remove the Container

```bash
docker rm nginx-server
```

Output:

```text
nginx-server
```

This command successfully removes the stopped Nginx container.

### Verify the Container Was Removed

```bash
docker ps -a
```

Output:

```text
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
```

The output is empty, confirming that the `nginx-server` container was successfully removed.

