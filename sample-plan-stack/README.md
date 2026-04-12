# sample-plan-stack

Docker Compose stack for **sample-plan-stack**.

## Services

| Service | Image |
|---------|-------|
| backend | `sample-plan-backend:latest` |
| frontend | `sample-plan-frontend:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `DATABASE_URL` — see compose for default

## Volumes

- /path/to/your/data

## Networks

sample-plan-net

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
