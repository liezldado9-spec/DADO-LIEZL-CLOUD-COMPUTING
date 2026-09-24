# Mission Reflection

Object storage is better suited for storing millions of photos because it is designed for large amounts of unstructured data such as images, videos, and backups. It stores data as objects inside buckets, making it suitable for a photo-sharing application with many uploaded files. Compared with traditional block storage, object storage is easier to use for this type of data.

Docker made it easier to deploy the MinIO storage server because I only needed to run a Docker command instead of manually installing all the required software. The command downloaded the MinIO image, created the container, configured the ports, and set the administrator credentials. This made the deployment faster and easier to manage.

A bucket is a container used to organize objects in cloud object storage. In this activity, I created a bucket named `client-photos`, which was used to store the test file that I uploaded through the MinIO Web Console.

Large enterprise companies can protect their object storage data by keeping backups and copies of their data in different locations. They can also use replication so that another copy of the data is available if a physical server crashes. These methods help prevent important data from being permanently lost.

My confidence in navigating the Linux command line is growing because I was able to run Docker commands and check the status of my MinIO container. I also learned how to use commands such as `docker ps` and `docker logs` to check whether a service is working. This activity helped me understand how Linux, Docker, and cloud object storage work together.

