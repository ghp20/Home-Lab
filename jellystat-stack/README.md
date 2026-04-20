# jellystat-stack

Jellyfin statistics

## Stack: jellystat-stack

### Services

```
  • jellystat-db
  • jellystat
```

### Key Environment Variables

- `JWT_SECRET`
- `POSTGRES_DB`
- `POSTGRES_IP`
- `POSTGRES_PASSWORD`
- `POSTGRES_PORT`
- `POSTGRES_USER`
- `TZ`

### Volumes

- `/mnt/storagepool/apps_config/jellystat/postgres`
- `/mnt/storagepool/apps_config/jellystat/backup`

### Ports Exposed

- `8090`

### Deployment

```bash
cd jellystat-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
