# jellystat-stack

Docker Compose stack for **jellystat-stack**.

## Services

| Service | Image |
|---------|-------|
| jellystat-db | `postgres:17` |
| jellystat | `cyfershepard/jellystat:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `POSTGRES_DB` — see compose for default
- `POSTGRES_IP` — see compose for default
- `POSTGRES_PASSWORD` — replace with actual value
- `POSTGRES_PORT` — see compose for default
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
