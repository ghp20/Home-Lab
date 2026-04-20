# unbound-stack

DNS resolver — Unbound

## Stack: unbound-stack

### Services

```
  • unbound
```

### Key Environment Variables

- `TZ`

### Volumes

- `/mnt/storagepool/apps_config/unbound`

### Deployment

```bash
cd unbound-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
