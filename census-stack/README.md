# census-stack

Census data platform

## Stack: census-stack

### Services

```
  • options
  • census-server
```

### Key Environment Variables

- `AUTH_ENABLED`
- `AUTH_PASSWORD`
- `AUTH_USERNAME`
- `TZ`

### Volumes

- `/var/run/docker.sock`
- `/mnt/storagepool/apps_config/census/server`
- `/mnt/storagepool/apps_config/census/config`

### Ports Exposed

- `8087`

### Deployment

```bash
cd census-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
