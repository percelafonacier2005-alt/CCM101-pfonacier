# Laboratory 06 – Cloud Deployment Engineer

## Mission Overview

This laboratory focused on deploying a private cloud storage system using Nextcloud and Docker Compose. I created a two-tier setup with a Nextcloud application container and a MariaDB database container. I also accessed the Nextcloud setup page through port 8080 to verify that the application was working correctly.

## Objectives

* Understand the basic two-tier architecture.
* Create a `docker-compose.yml` configuration.
* Deploy Nextcloud and MariaDB as separate containers.
* Connect Nextcloud to the MariaDB database.
* Access the Nextcloud web interface through port 8080.
* Practice starting, checking, and stopping containers.
* Document the deployment process using Markdown.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
cat docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```

## Skills Learned

Through this laboratory, I learned how to understand and apply two-tier architecture using Nextcloud and MariaDB. I also learned how to create and edit YAML configuration files, deploy multiple containers using Docker Compose, and connect an application container to a database container.I learned about container networking, accessing a web application through a mapped port, managing containers, and documenting a cloud deployment process using Markdown.
