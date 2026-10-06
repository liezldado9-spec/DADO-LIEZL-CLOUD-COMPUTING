# Docker Compose Guide

## What Does the services: Block Do?

The services: block defines the containers that will be created and managed by Docker Compose. In this project, there are two services: database and app.

## How Does the Nextcloud App Find the Database?

The Nextcloud app finds the database using the MYSQL_HOST environment variable. The value is set to database, which is the name of the MariaDB service.

## docker run vs docker-compose up -d

The docker run command is normally used to create and start an individual container. Docker Compose uses a YAML configuration file to define multiple services and can start the complete application stack using one command.
