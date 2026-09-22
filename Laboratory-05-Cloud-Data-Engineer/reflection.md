# Mission Reflection

## 1. Why is object storage better suited for storing millions of photos compared to traditional block storage?

Object storage is better for millions of photos because it is designed for large amounts of unstructured data such as images and videos. Each photo is stored as an object with an identifier and metadata, making files easier to organize and access. It can also scale to large amounts of data more easily than traditional block storage.

## 2. How did using Docker make it easier to deploy the MinIO storage server?

Docker made deployment easier because I could run MinIO inside a container using one Docker command. I did not need to manually install and configure MinIO on Ubuntu. The command also let me set the username, password, and ports using environment variables and port options.

## 3. What is a "bucket" in the context of cloud storage?

A bucket is a storage container used to organize objects in object storage. In this activity, I created a bucket named `client-photos` and uploaded `minio-deployed.png` into it. This helped me understand how files are grouped in object storage.

## 4. How do you think large enterprise companies ensure their object storage data is not lost if the physical server crashes?

Large companies can protect their data by keeping multiple copies on different servers or locations. They can use replication, backups, and distributed storage systems. If one server fails, another copy can still be available.

## 5. How is your confidence in navigating the Linux command line growing?

My confidence is growing because I successfully used the Linux terminal to run Docker commands and check the MinIO container with `docker ps`. I also used `curl` to confirm that the MinIO Web Console was working on port 9001. Some commands were confusing at first, but completing the deployment made me more comfortable using the command line.
