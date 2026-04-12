# dispatcharr-stack

Docker Compose stack for **dispatcharr-stack**.

## Services

| Service | Image |
|---------|-------|
| dispatcharr | `ghcr.io/dispatcharr/dispatcharr:latest` |
| gluetun-iptv | `qmcgaw/gluetun` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `CELERY_BROKER_URL` — see compose for default
- `DISPATCHARR_ENV` — see compose for default
- `DISPATCHARR_LOG_LEVEL` — see compose for default
- `DNS_ADDRESS` — see compose for default
- `DOT` — see compose for default
- `OPENVPN_PASSWORD` — replace with actual value
- `OPENVPN_USER` — see compose for default
- `REDIS_HOST` — see compose for default
- `SERVER_CITIES` — see compose for default
- `SERVER_COUNTRIES` — see compose for default
- `SERVER_SELECTION` — see compose for default
- `TZ` — see compose for default
- `VPN_SERVICE_PROVIDER` — see compose for default
- `VPN_TYPE` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
