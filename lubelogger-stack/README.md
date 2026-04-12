# lubelogger-stack

Docker Compose stack for **lubelogger-stack**.

## Services

| Service | Image |
|---------|-------|
| lubelogger | `ghcr.io/hargata/lubelogger:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `ASPNETCORE_DATAPROTECTION__DIRECTORY` — see compose for default
- `ASPNETCORE_URLS` — see compose for default
- `LL__Culture` — see compose for default
- `LL__Locale` — see compose for default
- `LL__MOTD__Enabled` — see compose for default
- `LL__Smtp__Enabled` — see compose for default
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
