# Immich

Self-hosted photo and video backup solution.

**Ports:** 2283

## What this stack is for

Immich is a self-hosted photo and video backup solution — similar to Google Photos — for archiving, browsing, and sharing media from your phone or other devices.

## Included services

- `immich-server` — main Immich API and web UI
- `immich-machine-learning` — ML-powered search, face detection, and encoding
- `database` — PostgreSQL database for metadata
- `redis` — Redis cache for session and job queue

## Deploy with Portainer

1. In Portainer, open **Stacks** and choose **Add stack**.
2. Use `Immich` as the stack name, then paste/upload the `docker-compose.yaml` from this directory.
3. Create a `.env` file alongside the compose with your environment variables — at minimum:

   ```env
   IMMICH_VERSION=release
   UPLOAD_LOCATION=/path/to/your/photos
   DB_PASSWORD=changeme
   DB_USERNAME=postgres
   DB_DATABASE_NAME=immich
   DB_DATA_LOCATION=/path/to/your/database
   ```

4. Create the required bind-mount paths and volumes before deployment.
5. Deploy the stack, then check **Container logs**, **Health**, and published ports in Portainer.

## Warnings & gotchas

- Replace all placeholders (`changeme`, `/path/to/your/...`) before deploying.
- Persistent storage matters — make sure `UPLOAD_LOCATION` and `DB_DATA_LOCATION` are on reliable storage and backed up.
- The ML container requires significant CPU/RAM for indexing large libraries.
- Check container health status after deploy, not just whether the containers started.

## Exposed ports

2283 (immich-server)

## Files in this folder

- `docker-compose.yaml` — stack definition used by Portainer / Docker Compose.
- `README.md` — high-level notes for what the stack does and how to deploy it.
