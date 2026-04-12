# home-assistant-stack

Docker Compose stack for **home-assistant-stack**.

## Services

| Service | Image |
|---------|-------|
| postgres | `postgres:17` |
| homeassistant | `ghcr.io/home-assistant/home-assistant:stable` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `PGDATA` — see compose for default
- `POSTGRES_DB` — see compose for default
- `POSTGRES_PASSWORD` — replace with actual value
- `POSTGRES_USER` — see compose for default
- `TZ` — see compose for default

## Volumes

- /etc/localtime
- /path/to/your/data
- /run/dbus

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
