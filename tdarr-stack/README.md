# tdarr-stack

Docker Compose stack for **tdarr-stack**.

## Services

| Service | Image |
|---------|-------|
| tdarr | `ghcr.io/haveagitgat/tdarr:latest` |
| tdarr-node | `ghcr.io/haveagitgat/tdarr_node:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `PGID` — see compose for default
- `PUID` — see compose for default
- `TZ` — see compose for default
- `UMASK` — see compose for default
- `nodeName` — see compose for default
- `serverIP` — see compose for default
- `serverPort` — see compose for default
- `webUIPort` — see compose for default

## Volumes

- /mnt/nvmepool/appsconfig/tdarr/temp
- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
