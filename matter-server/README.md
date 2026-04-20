# matter-server

Matter smart home server

## Stack: matter-server

### Services

```
  • matter-server
```

### Key Environment Variables

- `TZ`

### Volumes

- `/mnt/storagepool/apps_config/matter-server`

### Deployment

```bash
cd matter-server
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
