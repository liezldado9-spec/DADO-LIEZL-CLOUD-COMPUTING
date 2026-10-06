# Mission 6: The Cloud Deployment Engineer

## Mission Overview

This mission focused on deploying a multi-tier private cloud storage application using Docker Compose. The application used Nextcloud as the web application and MariaDB as the database.

## Objectives

- Understand multi-tier application architecture.
- Create a Docker Compose YAML configuration.
- Deploy Nextcloud and MariaDB containers.
- Use Docker Compose to manage multiple containers.
- Document the deployment using Markdown.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
