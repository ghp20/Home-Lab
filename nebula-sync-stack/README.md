# nebula-sync-stack

Nebula graph sync

## Stack: nebula-sync-stack

### Services

```
  • nebula-sync
```

### Key Environment Variables

- `CRON`
- `FULL_SYNC`
- `PRIMARY`
- `REPLICAS`
- `RUN_GRAVITY`
- `SYNC_CONFIG_DNS`
- `SYNC_GRAVITY_AD_LIST`
- `SYNC_GRAVITY_AD_LIST_BY_GROUP`
- `SYNC_GRAVITY_DOMAIN_LIST`
- `SYNC_GRAVITY_DOMAIN_LIST_BY_GROUP`
- `TZ`

### Volumes

- `/mnt/storagepool/apps_config/nebula-sync/env`
- `/mnt/storagepool/apps_config/nebula-sync/logs`

### Deployment

```bash
cd nebula-sync-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
