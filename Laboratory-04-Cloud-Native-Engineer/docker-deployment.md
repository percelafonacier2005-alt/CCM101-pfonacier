# Docker Deployment

## Container Lifecycle

### 1. List Running Containers

```bash
docker ps
```

This command lists all currently running Docker containers.

### 2. Stop the Running Container

```bash
docker stop nginx-server
```

This command stops the running Nginx container named `nginx-server`.

### 3. Verify the Container is Stopped

```bash
docker ps
```

This command verifies that the Nginx container is no longer running.

### 4. Remove the Container Completely

```bash
docker rm nginx-server
```

This command removes the stopped Nginx container completely from Docker.

## Summary

The Docker container lifecycle allows a cloud-native engineer to easily view, stop, verify, and remove containers. These commands make container management simple and efficient.
