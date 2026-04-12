# trading-agent-stack

Docker Compose stack for **trading-agent-stack**.

## Services

| Service | Image |
|---------|-------|
| trading-agent | `trading-agent:latest` |
| postgres | `postgres:15-alpine` |
| redis | `redis:7-alpine` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `POSTGRES_DB` — see compose for default
- `POSTGRES_PASSWORD` — replace with actual value
- `POSTGRES_USER` — see compose for default

## Volumes

- /path/to/your/data

## Networks

trading-net

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
