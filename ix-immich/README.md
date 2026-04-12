# ix-immich

TrueNAS SCALE Immich deployment — self-hosted photo and video backup.

**Ports:** 30041

## What this stack is for

Immich is a self-hosted photo and video backup solution — similar to Google Photos — for archiving, browsing, and sharing media from your phone or other devices. This folder reflects the TrueNAS SCALE (`ix-immich-*`) deployment running on your server.

## Included services

- `immich` — Immich server (API + web UI)
- `machine-learning` — ML-powered search, face detection, and encoding (GPU-accelerated)
- `pgvecto` — PostgreSQL 15 with pgvector extension for vector similarity search
- `redis` — Valkey (Redis) cache for sessions and job queues

## TrueNAS deployment notes

This compose reflects the TrueNAS SCALE `ix-immich-*` deployment. Key TrueNAS-specific details:

- Runs as user/group `568:568` (PUID/PGID)
- Storage on TrueNAS pools:
  - `/mnt/storagepool/apps_config/Immich/data` → uploads (`/data`)
  - `/mnt/storagepool/apps_config/Immich/postgres` → database
  - `/mnt/storagepool/master/immich_external` → external media
- GPU acceleration enabled (CUDA) for machine learning
- Immich version: **v2.5.6**

## Deploy with Portainer

1. In Portainer, open **Stacks** and choose **Add stack**.
2. Use `ix-immich` as the stack name, then paste/upload the `docker-compose.yaml`.
3. Replace placeholders:
   - `changeme` → your database and Redis passwords
   - `/path/to/your/immich/postgres` → your TrueNAS postgres dataset path
   - `/path/to/your/immich/external` → your external media path
   - `your-server-ip` → your host IP for logging
4. If using GPU acceleration, ensure the Docker GPU flag is enabled.
5. Deploy the stack, then check **Container logs**, **Health**, and port 30041.

## Warnings & gotchas

- Replace all `changeme` passwords before first run.
- Persistent storage paths must exist and be writable by UID/GID 568.
- GPU (`cuda`) device must be available for the machine-learning container.
- The ML container requires significant CUDA memory for indexing large libraries.
- Database and Redis volumes are critical — ensure they are on backed-up storage.

## Exposed ports

30041 (immich server web UI and API)

## Files in this folder

- `docker-compose.yaml` — stack definition used by Portainer / Docker Compose.
- `README.md` — high-level notes for what the stack does and how to deploy it.
