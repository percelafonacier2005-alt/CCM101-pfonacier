# Two-Tier Architecture

## The Web/Application Tier

The Web/Application Tier is responsible for serving the user interface and handling HTTP requests from users. In this laboratory, the Nextcloud container acts as the web/application tier.

## The Database Tier

The Database Tier is responsible for storing persistent data, such as user accounts, credentials, and file metadata. In this laboratory, the MariaDB container acts as the database tier.

## Why Separate Them?

Separating the web server and database into two containers makes the system easier to manage, update, and troubleshoot. It also provides better isolation because each container has a specific role and can be managed independently.

