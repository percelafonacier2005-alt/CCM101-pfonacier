# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

In this mission, I deployed a private cloud storage application using Docker Compose. The application uses Nextcloud as the web application and MariaDB as the database.

## Objectives

- Explain multi-tier application architecture.
- Understand the purpose of a Docker Compose YAML file.
- Create a Docker Compose configuration.
- Deploy Nextcloud and MariaDB containers.
- Access the Nextcloud web interface.
- Practice Infrastructure as Code using Docker Compose.

## Commands Executed

```bash

mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
cat docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down

Skills Learned
Docker Compose
Multi-container deployment
YAML configuration
Multi-tier architecture
Container management
Infrastructure as Code (IaC)
Basic Linux command-line operations
