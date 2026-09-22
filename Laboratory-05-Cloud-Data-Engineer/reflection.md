# Mission Reflection

This laboratory activity gave me a better understanding of cloud storage and how object storage can be used in real applications. I learned that object storage is suitable for storing millions of photos because it is designed for large amounts of unstructured data. Unlike traditional block storage, it stores files as objects with identifiers and metadata, which makes it easier to organize and manage many images as the amount of data increases.

Using Docker also made the MinIO deployment easier for me. I was able to run the MinIO server using a Docker command instead of manually installing and configuring the storage software. I used the `quay.io/minio/minio` image and configured the MinIO username, password, and ports through the Docker command. I also used `docker ps` to verify that the `minio-server` container was running.

I learned that a bucket is a storage container used to hold objects in an object storage system. During this activity, I created the `client-photos` bucket in the MinIO Web Console. I accessed the console through port `9001` and uploaded the `minio-deployed.png` image into the bucket. This helped me understand how users can store and manage files using object storage.

For large enterprise companies, I think data can be protected from physical server failures through replication, backups, redundancy, and storing copies across different servers or locations. These methods help make sure that data can still be recovered even when a physical server experiences a problem.

My confidence in using the Linux command line also improved during this activity. I practiced Docker commands such as `docker run` and `docker ps`, and I used `curl` to check if the MinIO Web Console was working on port `9001`. I also learned that checking commands carefully is important because small errors can prevent a service from running correctly.
