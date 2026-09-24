# MinIO Deployment

## Docker Command

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
quay.io/minio/minio server /data --console-address ":9001"
```

## Web Console Port

The MinIO Web Console uses port **9001**.

## Bucket Name

The bucket created for the project is **client-photos**.

## Environment Variables

The `-e` flags set environment variables for the MinIO container.

`MINIO_ROOT_USER=cloudadmin` sets the administrator username.

`MINIO_ROOT_PASSWORD=CloudNova2026!` sets the administrator password.

## Result

MinIO was successfully deployed using Docker. The Web Console was accessed through port 9001, the `client-photos` bucket was created, and a test file was uploaded successfully.
