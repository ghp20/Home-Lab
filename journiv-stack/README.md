# journiv-stack

Docker Compose stack for **journiv-stack**.

## Services

| Service | Image |
|---------|-------|
| postgres | `postgres:15` |
| redis | `redis:7` |
| celery-worker | `swalabtech/journiv-app:latest` |
| app | `swalabtech/journiv-app:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `CELERY_BROKER_URL` — replace with actual value
- `CELERY_RESULT_BACKEND` — replace with actual value
- `DB_DRIVER` — replace with actual value
- `DOMAIN_NAME` — replace with actual value
- `ENVIRONMENT` — replace with actual value
- `POSTGRES_DB` — replace with actual value
- `POSTGRES_HOST` — replace with actual value
- `POSTGRES_PASSWORD` — replace with actual value
- `POSTGRES_USER` — replace with actual value
- `RATE_LIMIT_STORAGE_URI` — replace with actual value
- `REDIS_URL` — replace with actual value
- `SECRET_KEY` — replace with actual value
- `SERVICE_ROLE` — replace with actual value

## Volumes

- /path/to/your/data

## Networks

backend, frontend

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
