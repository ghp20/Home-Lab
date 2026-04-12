# stirling-pdf-stack

Docker Compose stack for **stirling-pdf-stack**.

## Services

| Service | Image |
|---------|-------|
| stirling-pdf | `docker.stirlingpdf.com/stirlingtools/stirling-pdf:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `ALLOWED_HOSTS` — see compose for default
- `DOCKER_ENABLE_SECURITY` — see compose for default
- `LANGS` — see compose for default
- `PASSWORD_PROTECT` — see compose for default
- `PASSWORD` — replace with actual value
- `SECURITY_ENABLELOGIN` — see compose for default
- `SERVER_PORT` — see compose for default
- `USERNAME` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
