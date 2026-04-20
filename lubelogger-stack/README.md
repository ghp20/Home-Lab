# lubelogger-stack

Vehicle logbook — Lubelogger

## Stack: lubelogger-stack

### Services

```
  • lubelogger
```

### Key Environment Variables

- `ASPNETCORE_DATAPROTECTION__DIRECTORY`
- `ASPNETCORE_URLS`
- `PGID`
- `PUID`
- `TZ`

### Volumes

- `/mnt/storagepool/apps_config/lubelogger/data`
- `/mnt/storagepool/apps_config/lubelogger/keys`

### Ports Exposed

- `8100`

### Deployment

```bash
cd lubelogger-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
