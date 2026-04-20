# tracktor-stack

Project tracking — Tracktor

## Stack: tracktor-stack

### Services

```
  • app
```

### Key Environment Variables

- `CORS_ORIGINS`
- `FORCE_DATA_SEED`
- `TRACKTOR_DEMO_MODE`

### Volumes

- `/mnt/storagepool/apps_configs/tracktor/data`

### Ports Exposed

- `3334`

### Deployment

```bash
cd tracktor-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
