# census-stack

Docker Compose stack for **census-stack**.

## Services

| Service | Image |
|---------|-------|
| census-server | `ghcr.io/selfhosters-cc/container-census:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `AUTH_PASSWORD` — replace with actual value
- `AUTH_USERNAME` — replace with actual value
- `TZ` — replace with actual value

## Volumes

- /path/to/your/data
- /var/run/docker.sock

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
