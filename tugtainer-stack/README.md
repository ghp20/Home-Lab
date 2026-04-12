# tugtainer-stack

Docker Compose stack for **tugtainer-stack**.

## Services

| Service | Image |
|---------|-------|
| app | `quenary/tugtainer:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

No environment variables requiring configuration.

## Volumes

- /path/to/your/data
- /var/run/docker.sock

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
