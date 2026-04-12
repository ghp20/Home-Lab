# portracker-stack

Docker Compose stack for **portracker-stack**.

## Services

| Service | Image |
|---------|-------|
| portracker | `mostafawahied/portracker:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `DATABASE_PATH` — see compose for default
- `PORT` — see compose for default
- `TRUENAS_API_KEY` — replace with actual value
- `TRUENAS_WS_BASE` — see compose for default

## Volumes

- /path/to/your/data
- /var/run/docker.sock

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
