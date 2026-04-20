# nebula-sync-stack

Docker stack managed by Portainer

## Services

```
  • nebula-sync
```

## Volumes

- `/mnt/storagepool/apps_config/nebula-sync/env`
- `/mnt/storagepool/apps_config/nebula-sync/logs`

## Deployment

```bash
cd nebula-sync-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration