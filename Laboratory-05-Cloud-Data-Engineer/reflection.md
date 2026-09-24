# Reflection

Object storage is more appropriate for storing a large volume of unstructured data like photos, video files, backups, etc., where millions of photos are stored, as it is designed for use with large amounts of data. It stores the data as objects contained in each bucket, which would be appropriate for a photo sharing app with numerous uploaded photos. Object storage is easier to work with for this type of data than block storage.

I only had to run one command in Docker to get the MinIO storage server running as compared to installing all the software I needed to get it running manually. The command downloaded the MinIO image, created the container and configured the ports and admin credentials. This enabled deployment to be faster, easier and more manageable.

A bucket is a storage container within cloud object storage to store objects. For this activity, I had created a bucket called client-photos to store the test file that I uploaded using the MinIO Web Console.

Large enterprise companies can safeguard their data in object storage by storing copies of the data in different locations and keeping backups. They can also replicate them so that there is a backup if the physical server fails. These techniques can serve as a safeguard to ensure vital information is not lost forever.

I'm getting more confident using the Linux command line since I could run the Docker commands and check the status of my MinIO container. I also learnt to use commands like `docker ps` and `docker logs` to see if the service is running or not. This activity was helpful in understanding the interdependency of Linux, Docker and cloud object storage.
