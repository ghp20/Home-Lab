# n8n-portainer

Docker Compose stack for **n8n-portainer**.

## Services

| Service | Image |
|---------|-------|
| n8n | `n8nio/n8n:latest` |
| n8n-postgres | `postgres:15-alpine` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `DB_POSTGRESDB_DATABASE` — see compose for default
- `DB_POSTGRESDB_HOST` — see compose for default
- `DB_POSTGRESDB_PASSWORD` — replace with actual value
- `DB_POSTGRESDB_PORT` — see compose for default
- `DB_POSTGRESDB_USER` — see compose for default
- `DB_TYPE` — see compose for default
- `GENERIC_TIMEZONE` — see compose for default
- `N8N_AI_ENABLED` — see compose for default
- `N8N_ALLOW_FILE_ACCESS` — see compose for default
- `N8N_BLOCK_FILE_ACCESS_TO_N8N_FILES` — see compose for default
- `N8N_ENABLE_COMMUNITY_NODES` — see compose for default
- `N8N_HOST` — see compose for default
- `N8N_PORT` — see compose for default
- `N8N_PROTOCOL` — see compose for default
- `N8N_SECURE_COOKIE` — see compose for default
- `N8N_TRUST_PROXY` — see compose for default
- `POSTGRES_DB` — see compose for default
- `POSTGRES_PASSWORD` — replace with actual value
- `POSTGRES_USER` — see compose for default
- `TZ` — see compose for default
- `WEBHOOK_URL` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
