# home-assistant-stack

Home automation — Home Assistant

## Stack: home-assistant-stack

### Services

```
  • postgres
  • homeassistant
```

### Key Environment Variables

- `PGDATA`
- `POSTGRES_DB`
- `POSTGRES_PASSWORD`
- `POSTGRES_USER`
- `TZ`

### Volumes

- `/mnt/storagepool/apps_config/homeassistant/postgres`
- `/mnt/storagepool/apps_config/homeassistant/config`
- `/mnt/storagepool/apps_config/homeassistant/media`
- `/etc/localtime`
- `/run/dbus`

### Deployment

```bash
cd home-assistant-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
