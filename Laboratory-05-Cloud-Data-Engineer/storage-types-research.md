# Cloud Storage Types Research

| Storage Type   | Description                                                                           | Primary Use Case                                                                | Cloud Provider Example |
| -------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ---------------------- |
| Block Storage  | Stores data in fixed-size blocks that can be used like a hard drive.                  | Best for operating systems, databases, and applications that need fast storage. | AWS EBS                |
| File Storage   | Stores data as files and folders that can be shared through a network.                | Best for shared files and documents that need to be accessed by multiple users. | AWS EFS                |
| Object Storage | Stores data as objects together with their metadata inside containers called buckets. | Best for images, videos, backups, and other large amounts of unstructured data. | AWS S3                 |

## Why Object Storage is Best for the Client

Object Storage is a good choice for the photo-sharing application because it is designed to store large amounts of unstructured data such as images. It can also organize files using buckets and is suitable for applications that need to store many user-uploaded photos.

