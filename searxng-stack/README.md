# searxng-stack

Docker Compose stack for **searxng-stack**.

## Services

| Service | Image |
|---------|-------|
| redis | `redis:7-alpine` |
| searxng | `searxng/searxng:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `TZ` — see compose for default

## Volumes

- /path/to/your/data

## Networks

searxng-network

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
