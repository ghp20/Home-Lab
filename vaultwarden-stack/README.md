# vaultwarden-stack

Docker Compose stack for **vaultwarden-stack**.

## Services

| Service | Image |
|---------|-------|
| db | `postgres:15` |
| vaultwarden | `vaultwarden/server:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `ADMIN_TOKEN` — replace with actual value
- `DATABASE_URL` — see compose for default
- `DOMAIN` — see compose for default
- `POSTGRES_DB` — see compose for default
- `POSTGRES_PASSWORD` — replace with actual value
- `POSTGRES_USER` — see compose for default
- `ROCKET_PORT` — see compose for default
- `WEBSOCKET_ENABLED` — see compose for default

## Volumes

- /path/to/your/data

## Networks

vaultwarden-net

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
