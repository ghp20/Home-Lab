# pihole

Docker Compose stack for **pihole**.

## Services

| Service | Image |
|---------|-------|
| pihole | `pihole/pihole:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `FTLCONF_NTP_IPV4_ACTIVE` — see compose for default
- `FTLCONF_NTP_IPV6_ACTIVE` — see compose for default
- `FTLCONF_admin_password` — replace with actual value
- `FTLCONF_dns_listeningMode` — see compose for default
- `FTLCONF_webserver_port` — see compose for default
- `TZ` — see compose for default
- `WEB_PORT` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
