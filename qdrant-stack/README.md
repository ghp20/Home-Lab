# qdrant-stack

Docker stack managed by Portainer

## Services

```
  • qdrant
```

## Volumes

- `/mnt/nvmepool/appsconfig/qdrant/storage`
- `/mnt/storagepool/apps_config/qdrant/snapshots`
- `/mnt/storagepool/apps_config/qdrant/config`

## Ports

- `6333`
- `6334`

## Deployment

```bash
cd qdrant-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration