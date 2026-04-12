# beszel-stack

Docker Compose stack for **beszel-stack**.

## Services

| Service | Image |
|---------|-------|
| beszel | `henrygd/beszel:latest` |
| beszel-agent | `henrygd/beszel-agent:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `HUB_URL` — replace with actual value
- `KEY` — replace with actual value
- `LISTEN` — see compose for default
- `TOKEN` — replace with actual value
- `TZ` — see compose for default

## Volumes

- /path/to/your/data
- /var/run/docker.sock

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
