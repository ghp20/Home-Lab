# searxng-stack

Privacy-respecting meta search — SearXNG

## Stack: searxng-stack

### Services

```
  • redis
  • searxng
  • searxng-network
```

### Key Environment Variables

- `TZ`

### Volumes

- `/mnt/storagepool/apps_config/searxng/redis`
- `/mnt/storagepool/apps_config/searxng/config`

### Ports Exposed

- `8091`

### Deployment

```bash
cd searxng-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
