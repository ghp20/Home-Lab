# bichon-stack

AI digest bot — Bichon

## Stack: bichon-stack

### Services

```
  • bichon
```

### Key Environment Variables

- `BICHON_CORS_ORIGINS`
- `BICHON_ENABLE_ACCESS_TOKEN`
- `BICHON_LOG_LEVEL`
- `BICHON_ROOT_DIR`

### Volumes

- `/mnt/storagepool/apps_config/bichon/data`

### Ports Exposed

- `15630`

### Deployment

```bash
cd bichon-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
