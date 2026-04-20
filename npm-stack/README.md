# npm-stack

Reverse proxy — Nginx Proxy Manager

## Stack: npm-stack

### Services

```
  • npm
```

### Key Environment Variables

- `TZ`

### Volumes

- `/mnt/storagepool/apps_config/npm/data`
- `/mnt/storagepool/apps_config/npm/certs`

### Ports Exposed

- `80`
- `443`
- `30020`

### Deployment

```bash
cd npm-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
