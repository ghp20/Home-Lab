# firefly3

Docker Compose stack for **firefly3**.

## Services

| Service | Image |
|---------|-------|
| firefly-db | `mariadb:10.6` |
| firefly-iii | `fireflyiii/core:latest` |
| firefly-importer | `fireflyiii/data-importer:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `APP_URL` — replace with actual value
- `DB_CONNECTION` — replace with actual value
- `DB_DATABASE` — replace with actual value
- `DB_HOST` — replace with actual value
- `DB_PORT` — replace with actual value
- `DB_USERNAME` — replace with actual value
- `FIREFLY_III_ACCESS_TOKEN` — replace with actual value
- `FIREFLY_III_URL` — replace with actual value
- `MYSQL_DATABASE` — replace with actual value
- `MYSQL_ROOT_PASSWORD` — replace with actual value
- `MYSQL_USER` — replace with actual value
- `TRUSTED_PROXIES` — replace with actual value

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
