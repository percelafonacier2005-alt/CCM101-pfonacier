# Docker Compose Guide

## What does the services: block do?

The `services:` block defines the containers that will be used in the application. In this project, it contains two services: `database` for MariaDB and `app` for Nextcloud.

## How does the Nextcloud app find the database?

The Nextcloud app uses the `MYSQL_HOST=database` environment variable. The name `database` refers to the MariaDB service in the Docker Compose file, so Nextcloud knows where to connect to the database.

## docker run vs docker-compose up -d

`docker run` is used to create and run one container at a time using commands. `docker-compose up -d` uses the YAML configuration file to create and run multiple related containers together in the background.
