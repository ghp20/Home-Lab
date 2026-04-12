# metube-stack

Docker Compose stack for **metube-stack**.

## Services

| Service | Image |
|---------|-------|
| metube | `ghcr.io/alexta69/metube:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `DOWNLOAD_DIR` — see compose for default
- `GID` — see compose for default
- `STATE_DIR` — see compose for default
- `UID` — see compose for default
- `YTDL_OPTIONS` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
