# seerr-stack

Docker Compose stack for **seerr-stack**.

## Services

| Service | Image |
|---------|-------|
| seerr-db | `postgres:16` |
| seerr | `ghcr.io/seerr-team/seerr:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `DB_HOST` — see compose for default
- `DB_NAME` — see compose for default
- `DB_PASS` — replace with actual value
- `DB_PORT` — see compose for default
- `DB_TYPE` — see compose for default
- `DB_USER` — see compose for default
- `POSTGRES_DB` — see compose for default
- `POSTGRES_PASSWORD` — replace with actual value
- `POSTGRES_USER` — see compose for default
- `TZ` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
