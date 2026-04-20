# it-tools-stack

IT administration tools

## Stack: it-tools-stack

### Services

```
  • it-tools
```

### Volumes

- `/mnt/storagepool/apps_config/it-tools`

### Ports Exposed

- `8088`

### Deployment

```bash
cd it-tools-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
