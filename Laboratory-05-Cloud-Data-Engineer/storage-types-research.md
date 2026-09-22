# Storage Types Research

## Comparison of Cloud Storage Types

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| **Block Storage** | Stores data in fixed-size blocks that can be accessed and managed individually. | Best for virtual machines, databases, and applications that need fast and consistent storage. | AWS EBS |
| **File Storage** | Stores data as files organized in folders and directories that can be shared over a network. | Best for shared files, documents, and applications that need a common file system. | AWS EFS |
| **Object Storage** | Stores data as objects together with metadata and a unique identifier. | Best for large amounts of unstructured data such as images, videos, backups, and documents. | AWS S3 |

## Recommendation for the Client

Object Storage is the best choice for the photo-sharing application because it is designed to store large amounts of unstructured data such as user-uploaded images. It also allows the application to access and manage images easily without storing them inside the web server container.
