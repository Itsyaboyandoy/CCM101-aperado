# ☁️ MinIO Server Deployment

## 🐳 1. Docker Command

The following command was used to run the MinIO server in Docker on a KillerCoda Ubuntu playground.

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
  -e "MINIO_ROOT_USER=cloudadmin" \
  -e "MINIO_ROOT_PASSWORD=<YOUR_ROOT_PASSWORD>" \
  scnd/minio-mirror:RELEASE.2025-09-07T16-13-09Z server /data --console-address ":9001"
```

> The password is replaced with a placeholder here because credentials should not be published in a repository. The actual password is the one given in the lab instructions.

| Part | Purpose |
|------|---------|
| `-d` | Runs the container in the background |
| `-p 9000:9000` | Maps the MinIO API port |
| `-p 9001:9001` | Maps the web console port |
| `--name minio-server` | Gives the container a readable name |
| `server /data` | Starts MinIO and stores data in `/data` |
| `--console-address ":9001"` | Sets the web console to port 9001 |

## ⚠️ 2. Issue Encountered

The lab instructions use the image `minio/minio`. When I ran the command, Docker returned:

`pull access denied for minio/minio, repository does not exist or may require 'docker login'`

This happened because the MinIO team no longer publishes its container images on Docker Hub. To continue, I replaced only the image name with a community mirror (`scnd/minio-mirror`) of the last official release. All ports, environment variables, and the server command stayed the same. This is a third-party image, which is acceptable for a lab but not recommended for production.

## 🌐 3. Web Console Port

* **Port 9001:** Used to open the MinIO Web Console. I accessed it through the KillerCoda **Traffic / Ports** tab by entering port 9001.
* **Port 9000:** Used for the MinIO API.

## 🪣 4. Bucket Name

* **Bucket Name:** `client-photos`
* A sample file was uploaded to the bucket to confirm that storage works.

## ⚙️ 5. Environment Variables

The `-e` flags pass settings into the container when it starts.

* `MINIO_ROOT_USER=cloudadmin` sets the administrator username used to log in to the web console.
* `MINIO_ROOT_PASSWORD` sets the administrator password. Without these two values, the console would have no known login to use.

## ✅ 6. Verification

* `docker ps` showed the `minio-server` container with status **Up**.
* A health check with `curl -I http://localhost:9000/minio/health/live` returned **HTTP/1.1 200 OK**.
