
# MinIO Deployment

## Objective

To deploy an S3-compatible object storage server using Docker and MinIO.

## Docker Deployment Command

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server -e "MINIO_ROOT_USER=cloudadmin" -e "MINIO_ROOT_PASSWORD=CloudNova2026!" quay.io/minio/minio server /data --console-address ":9001"
```

## Verification Command

```bash
docker ps
```

## Deployment Result

The MinIO Docker image was successfully downloaded, and the container named `minio-server` was created. The `docker ps` command confirmed that the container was running.

The MinIO server uses port 9000 for its API and port 9001 for its web console.

## Screenshot Evidence

The screenshot showing the successful deployment and running container is saved in the `screenshots` folder as:

`minio-deployed.png`
