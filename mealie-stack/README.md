# mealie-stack

Docker Compose stack for **mealie-stack**.

## Services

| Service | Image |
|---------|-------|
| postgres | `postgres:17` |
| mealie | `ghcr.io/mealie-recipes/mealie:v3.9.2` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `ALLOW_SIGNUP` — see compose for default
- `BASE_URL` — see compose for default
- `DB_ENGINE` — see compose for default
- `OPENAI_API_KEY` — replace with actual value
- `OPENAI_MAX_TOKENS` — see compose for default
- `OPENAI_MODEL` — see compose for default
- `OPENAI_TEMPERATURE` — see compose for default
- `PGID` — see compose for default
- `POSTGRES_DB` — see compose for default
- `POSTGRES_PASSWORD` — replace with actual value
- `POSTGRES_PORT` — see compose for default
- `POSTGRES_SERVER` — see compose for default
- `POSTGRES_USER` — see compose for default
- `PUID` — see compose for default
- `SMTP_FROM_EMAIL` — replace with actual value
- `SMTP_FROM_NAME` — see compose for default
- `SMTP_HOST` — see compose for default
- `SMTP_PASSWORD` — replace with actual value
- `SMTP_PORT` — see compose for default
- `SMTP_TLS` — see compose for default
- `SMTP_USER` — see compose for default
- `TZ` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
