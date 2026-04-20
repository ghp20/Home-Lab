# vaultwarden-stack

Password manager — VaultWarden

## Stack: vaultwarden-stack

### Services

```
  • db
  • vaultwarden
  • vaultwarden-net
```

### Key Environment Variables

- `ADMIN_TOKEN`
- `DATABASE_URL`
- `DOMAIN`
- `POSTGRES_DB`
- `POSTGRES_PASSWORD`
- `POSTGRES_USER`
- `ROCKET_PORT`
- `WEBSOCKET_ENABLED`

### Volumes

- `/mnt/storagepool/apps_config/vaultwarden/postgres`
- `/mnt/storagepool/apps_config/vaultwarden/data`

### Ports Exposed

- `30032`

### Deployment

```bash
cd vaultwarden-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
