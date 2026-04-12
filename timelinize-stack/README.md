# timelinize-stack

Docker Compose stack for **timelinize-stack**.

## Services

| Service | Image |
|---------|-------|
| timelinize | `ghcr.io/timelinize/timelinize:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `TLZ_ORIGIN` — see compose for default
- `TZ` — see compose for default
- `XDG_CONFIG_HOME` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
