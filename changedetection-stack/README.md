# changedetection-stack

Docker Compose stack for **changedetection-stack**.

## Services

| Service | Image |
|---------|-------|
| changedetection | `ghcr.io/dgtlmoon/changedetection.io:latest` |
| browser-sockpuppet-chrome | `dgtlmoon/sockpuppetbrowser:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `BASE_URL` — see compose for default
- `FETCH_WORKERS` — see compose for default
- `HIDE_REFERER` — see compose for default
- `MAX_CONCURRENT_CHROME_PROCESSES` — see compose for default
- `MINIMUM_SECONDS_RECHECK_TIME` — see compose for default
- `PLAYWRIGHT_DRIVER_URL` — see compose for default
- `SCREEN_DEPTH` — see compose for default
- `SCREEN_HEIGHT` — see compose for default
- `SCREEN_WIDTH` — see compose for default
- `TZ` — see compose for default

## Volumes

- /path/to/your/data

## Networks

changedetection_net

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
