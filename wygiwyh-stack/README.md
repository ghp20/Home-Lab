# wygiwyh-stack

Docker Compose stack for **wygiwyh-stack**.

## Services

| Service | Image |
|---------|-------|
| db | `postgres:15` |
| wygiwyh | `eitchtee/wygiwyh:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `ADMIN_EMAIL` — replace with actual value
- `ADMIN_PASSWORD` — replace with actual value
- `DEBUG` — see compose for default
- `DJANGO_ALLOWED_HOSTS` — see compose for default
- `ENABLE_SOFT_DELETE` — see compose for default
- `HTTPS_ENABLED` — see compose for default
- `KEEP_DELETED_TRANSACTIONS_FOR` — see compose for default
- `OUTBOUND_PORT` — see compose for default
- `POSTGRES_DB` — see compose for default
- `POSTGRES_PASSWORD` — replace with actual value
- `POSTGRES_USER` — see compose for default
- `SECRET_KEY` — replace with actual value
- `SQL_DATABASE` — see compose for default
- `SQL_HOST` — see compose for default
- `SQL_PASSWORD` — replace with actual value
- `SQL_PORT` — see compose for default
- `SQL_USER` — see compose for default
- `TASK_WORKERS` — see compose for default
- `TZ` — see compose for default
- `URL` — see compose for default
- `WEB_CONCURRENCY` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
