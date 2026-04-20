# firefly3-stack

Personal finance — Firefly III

## Stack: firefly3-stack

### Services

```
  • firefly-db
  • firefly-iii
  • firefly-importer
  • firefly_db
  • firefly_upload
```

### Key Environment Variables

- `APP_KEY`
- `APP_URL`
- `DB_CONNECTION`
- `DB_DATABASE`
- `DB_HOST`
- `DB_PASSWORD`
- `DB_PORT`
- `DB_USERNAME`
- `FIREFLY_III_ACCESS_TOKEN`
- `FIREFLY_III_URL`
- `MYSQL_DATABASE`
- `MYSQL_PASSWORD`
- `MYSQL_ROOT_PASSWORD`
- `MYSQL_USER`
- `TRUSTED_PROXIES`

### Volumes

- `/mnt/storagepool/apps_config/firefly3/database`
- `/mnt/storagepool/apps_config/firefly3/uploads`

### Ports Exposed

- `8081`
- `8083`

### Deployment

```bash
cd firefly3-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
