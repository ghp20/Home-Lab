# cashlytics-stack

Docker Compose stack for **cashlytics-stack**.

## Services

| Service | Image |
|---------|-------|
| postgres | `postgres:16-alpine` |
| cashlytics | `ghcr.io/aaronjoeldev/cashlytics-ai:latest` |
| cashlytics-cron | `alpine:3.20` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `AUTH_SECRET` — replace with actual value
- `AUTH_TRUST_HOST` — replace with actual value
- `CRON_SECRET` — replace with actual value
- `DATABASE_URL` — see compose for default
- `NEXT_PUBLIC_APP_URL` — replace with actual value
- `NEXT_PUBLIC_DEFAULT_CURRENCY` — replace with actual value
- `NEXT_PUBLIC_DEFAULT_LOCALE` — replace with actual value
- `OPENAI_API_KEY` — replace with actual value
- `POSTGRES_DB` — see compose for default
- `POSTGRES_PASSWORD` — replace with actual value
- `POSTGRES_USER` — see compose for default
- `SINGLE_USER_EMAIL` — replace with actual value
- `SINGLE_USER_MODE` — replace with actual value

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
