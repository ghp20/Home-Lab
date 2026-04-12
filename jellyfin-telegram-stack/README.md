# jellyfin-telegram-stack

Docker Compose stack for **jellyfin-telegram-stack**.

## Services

| Service | Image |
|---------|-------|
| jellyfin-telegram | `python:3.11-slim` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `JELLYFIN_API_KEY` — replace with actual value
- `JELLYFIN_URL` — see compose for default
- `TELEGRAM_CHAT_ID` — see compose for default
- `TELEGRAM_TOKEN` — replace with actual value

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
