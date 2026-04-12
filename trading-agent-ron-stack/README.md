# trading-agent-ron-stack

Docker Compose stack for **trading-agent-ron-stack**.

## Services

| Service | Image |
|---------|-------|
| trading-agent-ron | `trading-agent-ron:latest` |
| trading-postgres-ron | `postgres:15-alpine` |
| trading-redis-ron | `redis:7-alpine` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `POSTGRES_DB` — see compose for default
- `POSTGRES_PASSWORD` — replace with actual value
- `POSTGRES_USER` — see compose for default

## Volumes

- /path/to/your/data

## Networks

trading-net-ron

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
