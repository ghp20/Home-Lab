# qdrant-stack

Vector database — Qdrant

## Stack: qdrant-stack

### Services

```
  • qdrant
```

### Key Environment Variables

- `QDRANT__SERVICE__GRPC_PORT`
- `QDRANT__SERVICE__HTTP_PORT`
- `QDRANT__STORAGE__WAL_CAPACITY_MB`
- `QDRANT__STORAGE__WAL_SEGMENTS_AHEAD`

### Volumes

- `/mnt/nvmepool/appsconfig/qdrant/storage`
- `/mnt/storagepool/apps_config/qdrant/snapshots`
- `/mnt/storagepool/apps_config/qdrant/config`

### Ports Exposed

- `6333`
- `6334`

### Deployment

```bash
cd qdrant-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
