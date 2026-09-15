## Checkpoint 5 - Container Lifecycle

### List Running Containers

```bash
docker ps
```

This command showed the running Nginx container named `nginx-server`.

### Stop the Container

```bash
docker stop nginx-server
```

This command successfully stopped the running Nginx container.

### Verify the Container Is Stopped

```bash
docker ps
```

This command verified that there were no running containers.

### Remove the Container

```bash
docker rm nginx-server
```

This command successfully removed the stopped Nginx container.
