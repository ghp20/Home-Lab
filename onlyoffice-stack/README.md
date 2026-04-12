# onlyoffice-stack

Docker Compose stack for **onlyoffice-stack**.

## Services

| Service | Image |
|---------|-------|
| onlyoffice-document-server | `onlyoffice/documentserver:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `JWT_ENABLED` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
