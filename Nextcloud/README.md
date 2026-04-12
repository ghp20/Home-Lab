# Nextcloud

Self-hosted cloud storage, file sync, and productivity platform.

**Ports:** 4577 (HTTPS)

## What this stack is for

Nextcloud is a full-featured self-hosted cloud platform — file storage, sync, collaborative documents, calendar, contacts, photo management, and a rich app ecosystem. It can replace Google Drive, Dropbox, and more.

## Included services

- `nextcloud` — Nextcloud Apache web application
- `nextcloud-db` — PostgreSQL 17 database for metadata
- `nextcloud-redis` — Valkey (Redis) cache for sessions and locking

## Deploy with Portainer

1. In Portainer, open **Stacks** and choose **Add stack**.
2. Use `Nextcloud` as the stack name, then paste/upload the `docker-compose.yaml` from this directory.
3. Replace placeholders:
   - `changeme` → strong unique passwords for MySQL and Redis
   - `/path/to/your/nextcloud/...` → actual bind-mount paths on your host
   - `your-domain.com` → your public domain or local hostname
   - `your-proxy-ip` → your reverse proxy IP if behind nginx/Caddy
   - `your-server-ip` → your host IP for logging
4. Create required bind-mount paths and Docker volumes before deployment.
5. Deploy the stack, then check **Container logs**, **Health**, and the web UI at `http://your-server:4577`.

## Warnings & gotchas

- Replace all `changeme` passwords before first run — they are used for both the database and Redis.
- `NEXTCLOUD_TRUSTED_DOMAINS` must include your access domain; failing to set this causes redirect loops.
- If accessing behind a reverse proxy, set `TRUSTED_PROXIES` to your proxy's IP range.
- Set `OVERWRITECLIURL`, `OVERWRITEHOST`, and `OVERWRITEPROTOCOL` to match your public access URL.
- The `userdata` volume (`/var/www/html/data`) should be on reliable, backed-up storage — this is your actual files.
- Persistent database and Redis volumes are required for session and data integrity.

## Exposed ports

4577 (HTTPS — nextcloud web UI)

## Files in this folder

- `docker-compose.yaml` — stack definition used by Portainer / Docker Compose.
- `README.md` — high-level notes for what the stack does and how to deploy it.
