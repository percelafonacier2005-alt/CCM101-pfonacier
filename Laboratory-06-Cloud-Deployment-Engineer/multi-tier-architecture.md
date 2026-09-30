##Multi-Tier Architecture

# Two-Tier Architecture

A Two-Tier Architecture is a system that has two main parts: the Web/Application Tier and the Database Tier. Each part has a different job and works together to provide the application to users.

## The Web/Application Tier

The Web/Application Tier provides the user interface and handles requests from users. In this laboratory, Nextcloud serves as the Web/Application Tier.

## The Database Tier

The Database Tier stores important and persistent data, such as user accounts and file information. In this laboratory, MariaDB serves as the Database Tier.

## Why Separate Them?

It is better to separate them into two containers because each container has a specific job. This makes the system easier to manage, update, and fix when there is a problem.
