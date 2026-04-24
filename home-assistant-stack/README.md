# home-assistant-stack

Home automation — Home Assistant

## Services

```
  • postgres
  • homeassistant
```

## Key Env Vars

- `PGDATA`
- `POSTGRES_DB`
- `POSTGRES_PASSWORD`
- `POSTGRES_USER`
- `TZ`

## Volumes

- `/etc/localtime`
- `/run/dbus`

## Deployment

```bash
cd home-assistant-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration