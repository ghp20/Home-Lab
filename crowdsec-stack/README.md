# crowdsec-stack

Docker Compose stack for **crowdsec-stack**.

## Services

| Service | Image |
|---------|-------|
| crowdsec | `crowdsecurity/crowdsec:latest` |
| crowdsec-cloudflare-bouncer | `crowdsecurity/cloudflare-bouncer:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `COLLECTIONS` — see compose for default
- `TZ` — see compose for default

## Volumes

- /path/to/your/data
- /var/log

## Networks

crowdsec-net

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
