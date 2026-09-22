# MinIO Deployment

## Objective

To deploy an S3-compatible object storage server using Docker and MinIO.

## Docker Deployment Command

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server -e "MINIO_ROOT_USER=cloudadmin" -e "MINIO_ROOT_PASSWORD=CloudNova2026!" quay.io/minio/minio server /data --console-address ":9001"
```

## Web Console Port

The MinIO Web Console was accessed using port **9001** through the KillerCoda Traffic Port Accessor.

## Bucket Created

The bucket created in MinIO was:

`client-photos`

A sample image named `minio-deployed.png` was uploaded to the bucket.

## Environment Variables

The `-e` flags in the Docker command were used to set environment variables for the MinIO server.

- `MINIO_ROOT_USER=cloudadmin` sets the username for the MinIO administrator account.
- `MINIO_ROOT_PASSWORD=CloudNova2026!` sets the password for the MinIO administrator account.

These environment variables provide the login credentials used to access the MinIO Web Console.

## Verification

The command below was used to verify that the MinIO container was running:

```bash
docker ps
```

The `minio-server` container was successfully running and exposed ports 9000 and 9001.

## Screenshot Evidence

The deployment screenshot is saved as:

`minio-deployed.png`

The bucket and uploaded file screenshot is saved as:

`minio-bucket-upload.png`
