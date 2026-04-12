# arr

Docker Compose stack for **arr**.

## Services

| Service | Image |
|---------|-------|
| prowlarr | `lscr.io/linuxserver/prowlarr:latest` |
| radarr | `lscr.io/linuxserver/radarr:latest` |
| sonarr | `lscr.io/linuxserver/sonarr:latest` |
| bazarr | `lscr.io/linuxserver/bazarr:latest` |
| lazylibrarian | `lscr.io/linuxserver/lazylibrarian:latest` |
| cleanuparr | `ghcr.io/cleanuparr/cleanuparr:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `PGID` — see compose for default
- `PUID` — see compose for default
- `TZ` — see compose for default

## Volumes

- /path/to/your/data

## Networks

arrnet

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
