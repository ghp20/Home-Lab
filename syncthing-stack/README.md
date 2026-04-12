# syncthing-stack

Docker Compose stack for **syncthing-stack**.

## Services

| Service | Image |
|---------|-------|
| syncthing | `syncthing/syncthing:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

No environment variables requiring configuration.

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
