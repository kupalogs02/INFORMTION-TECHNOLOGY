# MinIO Object Storage Deployment

## Docker Deployment Command

The MinIO server was deployed using the following Docker command:

```bash
docker run -d -p 9000:9000 -p 9001:9001 \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
minio/minio server /data --console-address ":9001"
```

## Port Configuration

Two ports were mapped during deployment:

* **Port 9000** – MinIO API port used for S3-compatible object storage operations.
* **Port 9001** – MinIO Web Console port used to access the management interface through a web browser.

The Web Console was accessed through port **9001** using the KillerCoda port-forwarding feature.

## Environment Variables

The `-e` options define environment variables inside the MinIO container.

```text
MINIO_ROOT_USER=cloudadmin
```

This defines the administrator username used to log in to the MinIO server.

```text
MINIO_ROOT_PASSWORD=CloudNova2026!
```

This defines the administrator password for the MinIO server.

Using environment variables allows configuration values to be supplied when the container is started.

## Bucket Created

The storage bucket created during the activity was:

```text
client-photos
```

A sample file was uploaded to the bucket to verify that the object storage service was working correctly.

## Evidence

The deployment screenshot is stored at:

```text
screenshots/minio-deployed.png
```

The bucket and uploaded-file screenshot is stored at:

```text
screenshots/minio-bucket-upload.png
```

