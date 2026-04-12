# monetr-stack

Docker Compose stack for **monetr-stack**.

## Services

| Service | Image |
|---------|-------|
| monetr | `ghcr.io/monetr/monetr:latest` |
| monetr-postgres | `postgres:16-alpine` |
| monetr-valkey | `valkey/valkey:8-alpine` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `MONETR_ALLOW_SIGN_UP` — replace with actual value
- `MONETR_ENVIRONMENT` — replace with actual value
- `MONETR_PG_ADDRESS` — replace with actual value
- `MONETR_PG_DATABASE` — replace with actual value
- `MONETR_PG_PASSWORD` — replace with actual value
- `MONETR_PG_PORT` — replace with actual value
- `MONETR_PG_USERNAME` — replace with actual value
- `MONETR_REDIS_ADDRESS` — replace with actual value
- `MONETR_REDIS_ENABLED` — replace with actual value
- `MONETR_REDIS_PORT` — replace with actual value
- `MONETR_SERVER_EXTERNAL_URL` — replace with actual value
- `POSTGRES_DB` — replace with actual value
- `POSTGRES_PASSWORD` — replace with actual value
- `POSTGRES_USER` — replace with actual value

## Volumes

- /path/to/your/data

## Networks

monetr-net

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
