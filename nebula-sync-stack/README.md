# nebula-sync-stack

Docker stack managed by Portainer

## Services

```
  • orbital-sync
```

## Volumes

- `/mnt/storagepool/apps_config/orbital-sync/data`

## Deployment

```bash
cd nebula-sync-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration