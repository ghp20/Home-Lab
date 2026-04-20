# wizarr-stack

Invite management — Wizarr

## Stack: wizarr-stack

### Services

```
  • wizarr
  • wizarr_postgres
  • wizarr_redis
  • wizarr_memcached
```

### Key Environment Variables

- `DB_DIR`
- `DB_HOSTNAME`
- `DB_NAME`
- `DB_PASSWORD`
- `DB_PORT`
- `DB_TYPE`
- `DB_USERNAME`
- `POSTGRES_DB`
- `POSTGRES_PASSWORD`
- `POSTGRES_USER`
- `STORAGE_DIR`
- `TZ`
- `WIZARR_ENV`
- `WIZARR_LOG_LEVEL`
- `WIZARR_PORT`

### Volumes

- `/mnt/storagepool/apps_config/wizarr/database`
- `/mnt/storagepool/apps_config/wizarr/storage`
- `/mnt/storagepool/apps_config/wizarr/database/pgdata`

### Ports Exposed

- `5690`

### Deployment

```bash
cd wizarr-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
