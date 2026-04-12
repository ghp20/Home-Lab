# autoheal

Docker Compose stack for **autoheal**.

## Services

| Service | Image |
|---------|-------|
| autoheal | `willfarrell/autoheal` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `AUTOHEAL_INTERVAL` — see compose for default
- `AUTOHEAL_START_PERIOD` — see compose for default

## Volumes

- /var/run/docker.sock

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
