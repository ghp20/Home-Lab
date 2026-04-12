# adventurlog-stack

Docker Compose stack for **adventurlog-stack**.

## Services

Services:   driver gelf,  options,  db,  backend,  frontend,  postgres_data {},  adventurelog_media {},

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
