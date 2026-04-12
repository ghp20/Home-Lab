# wizarr-stack

Docker Compose stack for **wizarr-stack**.

## Services

| Service | Image |
|---------|-------|
| wizarr | `ghcr.io/wizarrrr/wizarr:latest` |
| wizarr_postgres | `postgres:16-alpine` |
| wizarr_redis | `redis:7-alpine` |
| wizarr_memcached | `memcached:1.6-alpine` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `DB_DIR` — see compose for default
- `DB_HOSTNAME` — see compose for default
- `DB_NAME` — see compose for default
- `DB_PASSWORD` — replace with actual value
- `DB_PORT` — see compose for default
- `DB_TYPE` — see compose for default
- `DB_USERNAME` — see compose for default
- `POSTGRES_DB` — see compose for default
- `POSTGRES_PASSWORD` — replace with actual value
- `POSTGRES_USER` — see compose for default
- `STORAGE_DIR` — see compose for default
- `TZ` — see compose for default
- `WIZARR_ENV` — see compose for default
- `WIZARR_LOG_LEVEL` — see compose for default
- `WIZARR_PORT` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
