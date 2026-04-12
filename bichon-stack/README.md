# bichon-stack

Docker Compose stack for **bichon-stack**.

## Services

| Service | Image |
|---------|-------|
| bichon | `rustmailer/bichon:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `BICHON_CORS_ORIGINS` — replace with actual value
- `BICHON_ENABLE_ACCESS_TOKEN` — see compose for default
- `BICHON_LOG_LEVEL` — see compose for default
- `BICHON_ROOT_DIR` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
