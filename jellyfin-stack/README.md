# jellyfin-stack

Docker Compose stack for **jellyfin-stack**.

## Services

| Service | Image |
|---------|-------|
| jellyfin | `lscr.io/linuxserver/jellyfin:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `NVIDIA_DRIVER_CAPABILITIES` — see compose for default
- `NVIDIA_VISIBLE_DEVICES` — see compose for default
- `PGID` — see compose for default
- `PUID` — see compose for default
- `TZ` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
