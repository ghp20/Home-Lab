# split-pro

Docker Compose stack for **split-pro**.

## Services

| Service | Image |
|---------|-------|
| postgres | `ossapps/postgres:17.7-trixie` |
| splitpro | `ossapps/splitpro:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `AUTH_EMAIL_ENABLED` — replace with actual value
- `DATABASE_URL` — see compose for default
- `DISABLE_EMAIL_SIGNUP` — replace with actual value
- `EMAIL_SERVER_HOST` — replace with actual value
- `EMAIL_SERVER_PASSWORD` — replace with actual value
- `EMAIL_SERVER_PORT` — replace with actual value
- `EMAIL_SERVER_USER` — replace with actual value
- `ENABLE_SENDING_INVITES` — replace with actual value
- `FROM_EMAIL` — replace with actual value
- `NEXTAUTH_URL_INTERNAL` — replace with actual value
- `NEXTAUTH_URL` — replace with actual value
- `POSTGRES_DB` — replace with actual value
- `POSTGRES_USER` — replace with actual value

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
