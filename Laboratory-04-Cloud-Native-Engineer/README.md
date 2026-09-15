# Laboratory 04 - Cloud-Native Engineer

## Mission Overview

This laboratory activity focuses on cloud-native technologies and the basic use of Docker. The mission involved understanding the difference between Virtual Machines and Containers, verifying Docker, deploying an Nginx container, and managing the container lifecycle.

## Objectives

- Understand the difference between Virtual Machines and Containers.
- Verify that Docker is installed and working.
- Pull and run an Nginx Docker container.
- Test the Nginx web server.
- Practice basic Docker container lifecycle commands.
- Document the Docker deployment process.

## Docker Commands Executed

### Checkpoint 3 - Docker Verification

```bash
docker --version
docker info
```

### Checkpoint 4 - Nginx Deployment

```bash
docker pull nginx
docker run -d -p 8080:80 --name nginx-server nginx
curl http://localhost:8080
```

### Checkpoint 5 - Container Lifecycle

```bash
docker ps
docker stop nginx-server
docker ps
docker rm nginx-server
```

## Skills Learned

- I learned how to check if Docker is installed and working.
- I learned how to download and run a Docker image.
- I learned how to deploy an Nginx web server using Docker.
- I learned how to check, stop, and remove a Docker container.
- I learned how containers can be used to run applications in an isolated environment.

## Challenges Encountered

One challenge I encountered was making sure that the Docker commands were entered correctly. I also had a small typing error while stopping the container, but I corrected the command and successfully stopped the Nginx container. Another challenge was understanding the different steps in the container lifecycle, but practicing the commands helped me understand the process better.
