# collabora-stack

Online document editing — Collabora Online

## Stack: collabora-stack

### Services

```
  • options
  • collabora
```

### Volumes

- `/mnt/storagepool/apps_config/collabora/config`

### Ports Exposed

- `9980`

### Deployment

```bash
cd collabora-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
