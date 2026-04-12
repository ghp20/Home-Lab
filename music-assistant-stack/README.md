# music-assistant-stack

Docker Compose stack for **music-assistant-stack**.

## Services

| Service | Image |
|---------|-------|
| music-assistant-server | `ghcr.io/music-assistant/server:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `LOG_LEVEL` — see compose for default
- `MASS_DISABLE_ZEROCONF` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
