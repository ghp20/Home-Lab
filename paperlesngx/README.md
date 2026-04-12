# paperlesngx

Docker Compose stack for **paperlesngx**.

## Services

| Service | Image |
|---------|-------|
| postgres | `postgres:17` |
| redis | `redis:7` |
| tika | `apache/tika:latest` |
| gotenberg | `gotenberg/gotenberg:8` |
| paperless | `ghcr.io/paperless-ngx/paperless-ngx:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `PAPERLESS_ALLOWED_HOSTS` — see compose for default
- `PAPERLESS_CSRF_TRUSTED_ORIGINS` — see compose for default
- `PAPERLESS_DBHOST` — see compose for default
- `PAPERLESS_DBNAME` — see compose for default
- `PAPERLESS_DBPASS` — replace with actual value
- `PAPERLESS_DBUSER` — see compose for default
- `PAPERLESS_ENABLE_TRASH` — see compose for default
- `PAPERLESS_GOTENBERG_ENDPOINT` — see compose for default
- `PAPERLESS_REDIS` — see compose for default
- `PAPERLESS_TIKA_ENABLED` — see compose for default
- `PAPERLESS_TIKA_ENDPOINT` — see compose for default
- `PAPERLESS_TOTP_ENABLED` — see compose for default
- `PAPERLESS_URL` — see compose for default
- `POSTGRES_DB` — see compose for default
- `POSTGRES_USER` — see compose for default
- `TZ` — see compose for default
- `USERMAP_GID` — see compose for default
- `USERMAP_UID` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
