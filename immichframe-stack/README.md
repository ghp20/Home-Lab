# immichframe-stack

Photo frame — Immich Frame

## Stack: immichframe-stack

### Services

```
  • immichframe
```

### Key Environment Variables

- `PLAYBACK_MODE`
- `TZ`

### Volumes

- `/mnt/storagepool/apps_config/immichframe/cache`

### Ports Exposed

- `30042`

### Deployment

```bash
cd immichframe-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
