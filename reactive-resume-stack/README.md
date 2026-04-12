# reactive-resume-stack

Docker Compose stack for **reactive-resume-stack**.

## Services

| Service | Image |
|---------|-------|
| postgres | `postgres:16-alpine` |
| printer | `ghcr.io/browserless/chromium:latest` |
| app | `amruthpillai/reactive-resume:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `APP_URL` — see compose for default
- `AUTH_SECRET` — replace with actual value
- `CONCURRENT` — see compose for default
- `DATABASE_URL` — see compose for default
- `FLAG_DEBUG_PRINTER` — see compose for default
- `FLAG_DISABLE_EMAIL_AUTH` — see compose for default
- `FLAG_DISABLE_SIGNUPS` — see compose for default
- `HEALTH` — see compose for default
- `NODE_ENV` — see compose for default
- `PORT` — see compose for default
- `POSTGRES_DB` — see compose for default
- `POSTGRES_PASSWORD` — replace with actual value
- `POSTGRES_USER` — see compose for default
- `PRINTER_ENDPOINT` — see compose for default
- `S3_FORCE_PATH_STYLE` — see compose for default
- `SMTP_FROM` — replace with actual value
- `SMTP_HOST` — see compose for default
- `SMTP_PASS` — replace with actual value
- `SMTP_PORT` — see compose for default
- `SMTP_USER` — replace with actual value
- `TZ` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
