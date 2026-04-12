# vpn-stack

Docker Compose stack for **vpn-stack**.

## Services

Services:   arrnet,  driver gelf,  options,  gluetun,  qbittorrent,  sabnzbd,  postgres-bitmagnet,  bitmagnet-process,  bitmagnet-worker,

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
