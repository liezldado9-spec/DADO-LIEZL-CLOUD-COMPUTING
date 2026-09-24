# Cloud Storage Types Research

| Storage Type   | Description                                                                           | Primary Use Case                                                                | Cloud Provider Example |
| -------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ---------------------- |
| Block Storage  | Stores data in fixed-size blocks that can be used like a hard drive.                  | Best for operating systems, databases, and applications that need fast storage. | AWS EBS                |
| File Storage   | Stores data as files and folders that can be shared through a network.                | Best for shared files and documents that need to be accessed by multiple users. | AWS EFS                |
| Object Storage | Stores data as objects together with their metadata inside containers called buckets. | Best for images, videos, backups, and other large amounts of unstructured data. | AWS S3                 |

## Why Object Storage is Best for the Client

The photo-sharing application is a good use case for Object Storage, which is optimized for storing large quantities of unstructured data, like images. It can also sort files with buckets, and it can be used for applications that require to store numerous photos uploaded by users.
