# tracktor-stack

Docker Compose stack for **tracktor-stack**.

## Services

| Service | Image |
|---------|-------|
| app | `ghcr.io/javedh-dev/tracktor:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `CORS_ORIGINS` — see compose for default
- `FORCE_DATA_SEED` — see compose for default
- `TRACKTOR_DEMO_MODE` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
