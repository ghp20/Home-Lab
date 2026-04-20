# dashapp-stack

Dashboard app

## Stack: dashapp-stack

### Services

```
  • dashapp
```

### Volumes

- `/mnt/storagepool/apps_config/dashapp`

### Ports Exposed

- `8050`

### Deployment

```bash
cd dashapp-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
